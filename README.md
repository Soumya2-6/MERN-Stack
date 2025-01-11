const mongoose = require("mongoose");

const transactionSchema = new mongoose.Schema({
  productTitle: String,
  productDescription: String,
  price: Number,
  category: String,
  dateOfSale: Date,
  sold: Boolean, // Boolean to indicate if the item is sold
});

const Transaction = mongoose.model("Transaction", transactionSchema);

module.exports = Transaction;
