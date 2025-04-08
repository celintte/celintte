// pages/index.js
import Image from "next/image";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Mail } from "lucide-react";

export default function HomePage() {
  return (
    <main className="flex flex-col gap-10 items-center p-6 md:p-10">
      {/* Hero Section */}
      <section className="text-center space-y-4">
        <h1 className="text-4xl md:text-6xl font-bold tracking-tight">Celintte</h1>
        <p className="text-lg md:text-xl text-gray-600 max-w-xl mx-auto">
          Timeless elegance for every silhouette.
        </p>
        <Button className="text-base px-6 py-3 rounded-2xl text-white bg-black hover:bg-gray-800">
          Shop New Arrivals
        </Button>
      </section>

      {/* Product Highlights */}
      <section className="grid md:grid-cols-2 gap-6 max-w-5xl w-full">
        <Card className="overflow-hidden">
          <Image
            src="/linen-white.jpg"
            alt="Linen White Dress"
            width={500}
            height={600}
            className="w-full h-auto object-cover"
          />
          <CardContent className="p-4">
            <h3 className="font-semibold text-lg">Linen White Dress</h3>
            <p className="text-sm text-gray-600">Soft, breathable and chic</p>
          </CardContent>
        </Card>

        <Card className="overflow-hidden">
          <Image
            src="/sweetheart-maxi.jpg"
            alt="Sweetheart Maxi Dress"
            width={500}
            height={600}
            className="w-full h-auto object-cover"
          />
          <CardContent className="p-4">
            <h3 className="font-semibold text-lg">Sweetheart Maxi Dress</h3>
            <p className="text-sm text-gray-600">Flowy fit with romantic details</p>
          </CardContent>
        </Card>
      </section>

      {/* About Section */}
      <section className="max-w-2xl text-center text-gray-700 space-y-4">
        <h2 className="text-2xl font-semibold">About Celintte</h2>
        <p>
          Celintte celebrates feminine charm through refined, versatile pieces. Our
          collections are inspired by simplicity, softness, and the confidence
          that comes with wearing what you love.
        </p>
      </section>

      {/* Newsletter Signup */}
      <section className="w-full max-w-xl text-center space-y-4">
        <h3 className="text-xl font-medium">Stay in the loop</h3>
        <div className="flex items-center gap-2 justify-center">
          <input
            type="email"
            placeholder="Your email"
            className="border rounded-xl px-4 py-2 w-2/3"
          />
          <Button variant="default" className="rounded-xl">
            <Mail className="w-4 h-4 mr-1" /> Subscribe
          </Button>
        </div>
      </section>

      {/* Footer */}
      <footer className="w-full text-center text-sm text-gray-500 mt-10">
        <p>&copy; 2025 Celintte. All rights reserved.</p>
        <p className="mt-2">Follow us on Instagram @celintte.co</p>
      </footer>
    </main>
  );
} 
