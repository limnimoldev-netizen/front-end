<template>
    <div class="min-h-screen flex flex-col">
        <AppHeader />
        <main class="flex-grow">
            <div class="container mx-auto px-4 py-8">
                <h1 class="text-3xl font-bold mb-6">Company Dashboard</h1>
                <p class="text-gray-700 mb-4">Welcome to your company dashboard! Here you can manage your job postings, view applications, and access important insights about your company’s performance on our platform.</p>
                <div class="bg-white shadow rounded-lg p-6 mb-6">
                    <h2 class="text-xl font-semibold mb-4">Job Postings</h2>
                    <p class="text-gray-600 mb-4">You currently have 5 active job postings. You can create new job postings or manage existing ones from this section.</p>
                    <button class="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700 transition-colors duration-200">Create New Job Posting</button>
                </div>
                <div class="bg-white shadow rounded-lg p-6 mb-6">
                    <h2 class="text-xl font-semibold mb-4">Applications</h2>
                    <p class="text-gray-600 mb-4">You have received 20 applications for your active job postings. You can review and manage these applications from this section.</p>
                    <button class="bg-green-600 text-white px-4 py-2 rounded hover:bg-green-700 transition-colors duration-200">View Applications</button>
                </div>
                <div class="bg-white shadow rounded-lg p-6">
                    <h2 class="text-xl font-semibold mb-4">Insights</h2>
                    <p class="text-gray-600 mb-4">Access important insights about your company’s performance on our platform, including metrics on job posting views, application rates, and more.</p>
                    <button class="bg-purple-600 text-white px-4 py-2 rounded hover:bg-purple-700 transition-colors duration-200">View Insights</button>
                </div>
            </div>
        </main>
        <AppFooter />
    </div>
</template>