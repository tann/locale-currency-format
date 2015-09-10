[![Build Status](https://travis-ci.org/tann/locale-currency-format.svg?branch=master)](https://travis-ci.org/tann/locale-currency-format)

#### NAME
**Locale::Currency::Format** - Perl functions for formatting monetary values

#### SYNOPSIS
         use Locale::Currency::Format;
         $amt = currency_format('USD', 1000);             # => 1,000.00 USD
         $amt = currency_format('EUR', 1000, FMT_COMMON); # => EUR1.000,00
         $amt = currency_format('USD', 1000, FMT_SYMBOL); # => $1,000.00

         $sym = currency_symbol('USD');                   # => $
         $sym = currency_symbol('GBP', SYM_HTML);         # => &#163;

         $decimals = decimal_precision('USD');            # => 2
         $decimals = decimal_precision('BHD');            # => 3

         $thou_sep = thousands_separator('USD');          # => ,
         $thou_sep = thousands_separator('EUR');          # => .

