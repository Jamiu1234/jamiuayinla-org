# jamiuayinla-org
We Keep learning everyday 
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Twitter, Send } from "lucide-react";
import { motion } from "framer-motion";

export default function JamiuayinlaOrg() {
  return (
    <main className="min-h-screen bg-gradient-to-br from-gray-900 to-black text-white p-6 flex flex-col items-center justify-center">
      <motion.div
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.8 }}
        className="text-center mb-12"
      >
        <h1 className="text-5xl font-bold mb-4">Jamiuayinla Organization</h1>
        <p className="text-xl text-gray-300">Reliable Node Operator</p>
      </motion.div>

      <motion.div
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 0.3, duration: 0.8 }}
        className="grid gap-6 md:grid-cols-2 w-full max-w-4xl"
      >
        <Card className="bg-gray-800 border-none">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">Who We Are</h2>
            <p className="text-gray-400">
              Jamiuayinla Organization is a trusted node operator focused on delivering secure, consistent, and scalable blockchain node operations across decentralized networks.
            </p>
          </CardContent>
        </Card>

        <Card className="bg-gray-800 border-none">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-2">Connect With Us</h2>
            <div className="flex flex-col gap-3">
              <Button variant="secondary" className="w-full justify-start gap-2">
                <Twitter size={18} /> <a href="https://twitter.com/jamiuayinla9" target="_blank" rel="noopener noreferrer">@jamiuayinla9</a>
              </Button>
              <Button variant="secondary" className="w-full justify-start gap-2">
                <Send size={18} /> <a href="https://t.me/Rama4418" target="_blank" rel="noopener noreferrer">@Rama4418</a>
              </Button>
            </div>
          </CardContent>
        </Card>
      </motion.div>
    </main>
  );
}
