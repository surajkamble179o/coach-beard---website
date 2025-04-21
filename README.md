# coach-beard---website
import { Button } from "@/components/ui/button"; import { Card, CardContent } from "@/components/ui/card"; import { CheckCircle, Mail, Phone } from "lucide-react"; import { motion } from "framer-motion";

export default function Home() { return ( <main className="min-h-screen bg-white px-4 py-6 text-center"> <motion.h1 initial={{ opacity: 0, y: -20 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.6 }} className="text-4xl font-bold text-gray-800 mb-4" > Coach Beard Strength & Conditioning </motion.h1> <p className="text-lg text-gray-600 mb-8"> Online Monsoon Fitness Classes for Housewives </p>

<motion.div
    initial={{ opacity: 0, scale: 0.95 }}
    animate={{ opacity: 1, scale: 1 }}
    transition={{ duration: 0.5 }}
    className="mx-auto max-w-md"
  >
    <Card className="rounded-2xl shadow-md p-6">
      <CardContent>
        <h2 className="text-2xl font-semibold mb-2 text-gray-700">
          Join the Batch
        </h2>
        <ul className="text-left text-gray-600 mb-4">
          <li className="flex items-center mb-1">
            <CheckCircle className="mr-2 text-green-500" size={18} />
            Easy Home Workouts
          </li>
          <li className="flex items-center mb-1">
            <CheckCircle className="mr-2 text-green-500" size={18} />
            No Equipment Needed
          </li>
          <li className="flex items-center">
            <CheckCircle className="mr-2 text-green-500" size={18} />
            Live + Recorded Options
          </li>
        </ul>
        <a
          href="https://buy.stripe.com/test_1234abcd5678" // Replace with your Stripe/Instamojo/Razorpay link
          target="_blank"
          rel="noopener noreferrer"
        >
          <Button className="w-full text-white bg-green-600 hover:bg-green-700">
            Join Now - Rs. 999/month
          </Button>
        </a>
      </CardContent>
    </Card>
  </motion.div>

  <div className="mt-8 text-gray-600">
    <p className="flex justify-center items-center mb-1">
      <Phone className="mr-2" size={16} /> +91 9172310220
    </p>
    <p className="flex justify-center items-center">
      <Mail className="mr-2" size={16} /> coachbeard.fit@gmail.com
    </p>
  </div>
</main>

); }

