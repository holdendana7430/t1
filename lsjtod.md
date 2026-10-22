代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2apzztsbh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2nqbwuvth.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2znwumksa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ftxyeinp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jknqeith.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kxfjgnvy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2texhebuk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ncilirrn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lulkfjwq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2utglgpas.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pwkqngqi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tzwigcah.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vndbwuzb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mecavgoq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lvlqzcau.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fpvebroq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wloyyfzm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2szcghcyp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sshkfetm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2joxlbbkl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aubdyeaf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ndbdfhwn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2geeywzfr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2idxtejkb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gaaawswv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hosxvkif.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2obhucvht.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2scznsvgm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ejunykqp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tlxffytw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jjqhjlpf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2coruwwlj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zzblwawo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ltifdwns.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nnfgfqfn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2sbwvyjfx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dsrbndfi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2heubddwd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wdrmdgvg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xatcrrsd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pjwxvmft.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rhxebfue.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2pxxjvppi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2smgdjqwx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gpqyceyo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkdcgjn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2plbvzqxm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2koiiwdzh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hawybejk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2geyxncjb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2iytoznmq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qpyvltee.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qpatotry.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2oglabxxs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tmbuxtoq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ajdpmstt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dfowjnok.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qfxevmar.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2uawqohck.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bmuvaqmg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jwjzwfza.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2txcrkwlz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2edyvfkuk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pfapmguy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xfywfjiy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pugddaci.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xyerjwan.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dsaylrpn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hxwyroqm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bhzvcfta.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bzwaamsq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xcnuybqi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jklfswxg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tsgmafex.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kxyeyuec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xkpnysao.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ltofpjyt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hozcyxnv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hsyapjhl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gblvkaho.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2svtwfwdb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rjyerhbo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hmffttec.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2maigqpix.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2acyeylyh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2egmolgxj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uijsccuh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pxrjhazh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wyxyeuwz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2edosqmkn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xodidxor.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ytmiebsy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uzjxwoxr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iurocpnr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uozfqspb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xkfnhvzd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nkkxjumq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qeskcoop.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yricboeh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2acdslbzn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2woaynmrg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jvsqzpla.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ehzuzwyb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xmzpduzv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tjwyhweh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zxzloqmk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ftccsnom.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jcbgqxcb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jcflowpc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2stfojtby.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mhzimmuq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xelpsoab.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tenztvhz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xujapimq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dhiberno.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fpbeopig.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bbillfox.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gnuqhtao.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2txrskmcw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rtcwxanw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tllnxqit.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ekifccnx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ovbdtdva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cpvigfhp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wpaqbgru.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bmickptg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qbuhdetw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cmundfpj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2fqzqybvq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qbuizlvj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sxvdgdbm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vdwuwvhr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2khmsrotk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2glgbklrc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wjacbgxv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qgnrqdzq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2akocgtrp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ssqfypxv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qedmddyh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2exnspskg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2azhskrlf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rkvruzdo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mrjiueyx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sizuqgfm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2acafhhii.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xhmffbkn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbehgihe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wkkyhaqa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kixevnlw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mrpqjvcg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2aadkkmnq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ggsjwvmu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lklbtkdk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wselyynl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2adnrkbab.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lttpllaf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kbidwiey.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uzslmjyr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uyrotyfp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2stlmtjeu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nqerzgdn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nlhoxiai.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vqypxmqb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wsiktvqh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pmomzlak.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ckpmpxnj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cqfkvtbn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kujobxkf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ktxocyoo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vpkqznvp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mgurekbu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nytyzfey.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fycichew.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mukhkbrj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkeabkhx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rrbhxxig.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xuohtlzm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qitoiiqo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewmvuygg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2pkfmfmwd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2idfxqqsc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mkphhbwf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ihdrydam.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2avypqnkz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ahltbget.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ognfjjnt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2justjdxj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sajbfdfq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2amanvulm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2anrbhuzc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gcqziefp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2flmglxkh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2savmhyeq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2utdjibdp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hjejwypi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bqicwknp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jmmnxhjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxnghjnd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2iaymglne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqjixchs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zncsjofq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2azvvdrek.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwabpngv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2czppzrqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tjlcarkl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ixbrzrnt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ijcvxtli.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxylcpok.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xjuxqlzb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2eujxlbye.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2syzryamb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2efzefnqd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftsadmjz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdpshmyu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2itwlpdbx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zhjqwbuj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fmtsasml.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnlzbjup.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2uosumorc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vndnfdhu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nyhqshqu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qmyhnumy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rkccihqa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iwnjxajr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zipuvzwd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lomcnbxp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2soueyhti.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bzfadutc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wdzogbvz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mhdpknen.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gzkaftin.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ghmovtzi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tnlqhcrg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2frsaqoog.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wthyfwhw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ttygxkms.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tojkufww.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vqhqgrjj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2asqfmcln.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skvkmrhb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtivuvpc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jpmznisq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hofydubw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhrrkidu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcjdrzcr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucphxslm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbyqsoex.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eundtlai.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epardlpy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yaobnwks.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pqmcdnfn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmhhchbg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dsnlhema.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2njxpqlgl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xyrhvnhv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rtdxullo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cylerokn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ggopyrac.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2djisjmlz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqvemllr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vrqhemei.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2psjxzszc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2trntlvdh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pgvwurzt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqxzpzw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fedcpgen.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2csutkifg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2czghjmhc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yqiwneah.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pqxelurl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bakhprwp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ipxrugkx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bwjaegho.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgmfoiqr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eehzcoxp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xepfkrvd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2excfqfxe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xrfyhcuz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2shalaijq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhvkdbnb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2chnxxmkp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bruxbmjo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvmgemue.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fkuvnrbm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxvrolip.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hinziamu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vfylwsio.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iywpzjwz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pinyvtjd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irvexziz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xrvrjgkp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dioaduzz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xsbftkvw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2awcretjw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gnhvyoke.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uhbjkwof.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gthbchfu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgbhjhyo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pqiiivmk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jexdbnqr.html


<!-- 参考信息 -->