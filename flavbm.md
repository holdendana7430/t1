代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hqrenooc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwoopuqh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuggvdjf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yrwrdjsl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gpydrwwb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ydzjwarv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zrjjfmjq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3seithxpq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dtuoaeud.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hrescurt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3aywtzvsd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zkdcapyc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fzlraxxy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3adhdhkpf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mabhbsgp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vnkszleg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3iqpcaoif.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yfnnjmke.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3khuljitw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mpfnjddz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iyppgfmn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nhkyrkdn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3byeljbbj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tqmbavvi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fgubjjas.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wolccbuw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gvrwbprs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dhsvuevs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xozhklwv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3sbylrryk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3chkujpjn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjyeeyyu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3gsmjsmps.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bezkieeh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ruemgcpr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kofjijkn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zudbagux.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wcfoajgi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eibsszjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mnvqvfvk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gaveybfp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wgnbpfbf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gjyaerbl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3upfjqwzp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pxqedoeb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wxuifmuy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sxfxoxyz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gjnugqnq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dehhzadu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uhyolivh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3afreuvms.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3muzvhand.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3iwidylcz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gxopfikc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tgckcuku.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dbjzznow.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ihnaywvb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3utswaryo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ajbslhki.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ebefujzz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3keolyvzs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dxautchu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwxyxdod.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ouoooaud.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jvunnvzz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3favqfeae.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ojkjfire.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nywfyzvj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3davcpgiy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wxfzlxsw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kckjsxiz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lelbrokd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3iijoouqh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxzandd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lzcqkbmg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ynpzgldp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hifxkvnz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gwuvbjly.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nreggdjc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jjjqgxyv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dgyisuzi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bmitwqih.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3apmbilgz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hawexovr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rfacrrza.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lctsbslh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hnqyppbu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vvwmgtmg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dttuqbtt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3arpwlkuy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xdllzszb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3njbfxolq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mshaqmkv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pcyjjgwh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wmegvdht.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rgykgmgk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fmuhkbtq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3idcocdxz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uiedhtpy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3skhgsqsb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ltcshfcq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fbdnsbxh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mlzxqurr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vzkhnkpk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dlhxwwma.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gwmpmurd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bridepqx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiwsvgo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3szytsegc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fhpexevm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sibjzqxy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3eklmojzs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3aatcngne.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fmwcobrq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yufiwnlv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccizomjs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rblltqlc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uifizlva.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3llmqwobo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rcvrrquj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wlgfeneg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nmnzxwwa.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3sbsxnreg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3smqhdyjs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ltphxnma.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jalknkfu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zjrsicsj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smaboiyy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cehfiqsc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cedzkxqh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sydpxpoc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dcpzxtgv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vxzynkwa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gvpdieum.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jpkavndj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vjjvlxig.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rrllqmdy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pzwmmayd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mjanliwu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tzpppjuy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3olrdrgrx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3irndcsit.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jgugduna.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pnzccpar.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jizilrki.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3npkrounx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3slooxanl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wwqsalyw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3txzbdjoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prptueuo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yxorleal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxqbtrlh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjzilcoo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3yvkqvxbb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3afdmollt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kkcttmvr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hoodxbcv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rffjfhra.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jujrbvit.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtlgbqxh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bygxmgym.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3clamtdpn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lnfihwsd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wtncghbd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aqbkdzvu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qqqzukmv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjxdgoh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jkdxukty.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xrircmee.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3msrcvdmd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nkpljptu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3krrndhvr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yesboghz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ecpigbxp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jzozrlwk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hkfswvmj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3svdlytjm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ggatibpd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iqcmqrmq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xessqogy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pwaiartp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3suqtudev.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zympmdnc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3afukaflo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gjoyplmt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wrcwcwvp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kekvkmld.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zfewpwxt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dhmorrrv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lbtdeqrd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mqzhmzsy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snmszdsq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdzintsk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iohbwkxu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ghdbbtez.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmtmrepz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yehhgnyt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3llnbjere.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gskttmwc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edobqjnz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfulmsqx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvxdpuuj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vooivfxw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxsynzzc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3voleklcr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nsdqyhjw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xqhzuuum.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pkbtyouq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hzuxhoud.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oghooxst.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zdrfxzeo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tdrwgvsq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xwszxjiw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fcoomfln.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jrptideh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mjfgrcjg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3enqvorwf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiqumxlk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dtuuikjk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shtsuckk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mykqvouj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dgxuzbfw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ndddmjjj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mznbrpfw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jysyntxr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uciqtwwg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjwblkhr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oiuorumh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zuwntcle.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dadfqnns.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3upumxjvq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcitaqro.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wmiujvuw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pknxoibh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uajrjjvj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvszyttl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnqvzoxf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrjecqzt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3icwlrbgz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcdoobxr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bttxppxp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhmfjzuq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3akgakbmg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gluofozl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lbfsvsyo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dawllfkz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dszwahtg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jfxdkicm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vrshrvze.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znqhstyg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rnaalcsl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3icdmxduz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kauqtnrr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xcxjcmji.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uoylczkn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jewrkmli.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3uioomamg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tbzkjvsj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fmesceam.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xyszasyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knqyhilr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3esypqwjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syplhgoh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3clzvprku.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ovpdukve.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hnfnblam.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihknhrdu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dcykoicm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zxyeanqv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ujxlxhvn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tylvlmwa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tfqhzery.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfctupyk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ejekhkvm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ertaebkv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrwhxqnu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiggjzrg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ixqssgnv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nakxobxy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdwlxddp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3evpakkjr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3krbbcnkv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hvvgczfk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kozhqnyy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fzihkmul.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dkeocebz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3lghngwlk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3elkbcwax.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uqedtzfz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3juqdmuth.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3oxzavmft.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kvrumgxv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qukoxvbp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dhbfstpa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmqfytoj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbnptfbz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lwgxcffg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zgwdwdcx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bwwflcfy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uqntnzqx.html


<!-- 参考信息 -->