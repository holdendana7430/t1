代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wxxyqwpd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xtetllih.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2svhgqmcd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhabsvdr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2nouvjesb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rdpwhodf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gihlfbic.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bqbwokjh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2afztvxrn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nedbchcs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qefpwrhf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2icrrkbdp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hpagabas.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qtxtvwva.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmbgivc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bbcgfsmi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2huulnooi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ivxaizgu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ztmpdaog.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2urpiyqoc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ekgvkogo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gogmhfcl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mbthlcqd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2olebiqsx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hvptrvoc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2riktuhsl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vszqyphj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gfapmcja.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qiyjpmso.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2djgncyvj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ueukiuio.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cvtkmsyv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2zhnxgqiz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ojsdrdbx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fczibrye.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ovaknfbe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ruyzrqjv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2noueujkr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2uggxejeg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rqsjfyho.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xmwemqpd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2golnpwcm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2atjuoedk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fnlbuldq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mojdpjrx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmodfxwo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2abyeyqux.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ygzdprmv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mhvekhpp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rktzmjlr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vgdcvpuu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lhqfsmpp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2hzaaeecr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tmxqbrzg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yhuxewvv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2naexhces.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgvhkac.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zihhsgci.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lbrurnuw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oqdtwatk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ozeeenvg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yrflbira.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fcbxvnxn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2clhpjdpu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2aeilubkp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hgjjopui.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uohbiujl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ohykcjaa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bulnkoio.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2yxtukvln.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qfmbllqv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2iwgeqsae.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2izvqjrxm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pwvditng.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ulynplsh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gzkgevsk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2amnuzvhb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nppgtygw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2puzhvtxw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2desqlizq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dlrbamht.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qjjrfmxv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2johdevsv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kaqrtynq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xqfxynsg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2exjvyuul.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mssdmbjc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2trvnltwn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ezqqlsew.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2eohgyowf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zszxgiii.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2oibjtcuh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2yuigakut.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2senkvqhj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zbcgyfwq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vyyyepfk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kuuadcdj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2btepfvlq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lqikmjci.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wbddlnkb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgymrgn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fspxyscq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tgjqspxq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wuzyfgbk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lexnsmmi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vvpattmp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2udzsvkjg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gcptivch.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qorozhem.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jhoyuwcg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2inxndolp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fqnhgibw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ojpvqkft.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wggidblc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vkbvywxh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dlvetkgw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kqupbvmw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edmwetet.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fghhqdbp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsuoznvf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bywirdsa.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jjlygqtz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2phngyihq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zogvmdoc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2erzasnzi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zesslnzr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eitmwkuk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2swukdxmn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2riwrpogo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xprapwni.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yjboloet.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tydyaxps.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2uuugjkfx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bshxayir.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lfvjeqoc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hyhgrrug.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2niqgvykb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xvpmvwep.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ujjkgcho.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mmkvydyj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rtdpvkpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghbsnymh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2guitfjii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cymckels.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qtwjncgh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pujmnrtv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aztyawmk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2irgghchq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kvsuionx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nzujyujd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qiyvzmit.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rinqwcst.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zssoeybu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcaoghbc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sgxhakqu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2snudledp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2houwihol.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2josnhbfw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2iohfkguh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2yaqmtyvj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dierzqhj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruuibaaf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sviqrjps.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fbmhdyla.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hyemkcrf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fphixrbj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mpueiijy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fsniqlyk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uszxunkx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2temfsnmz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aydjelct.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ctcjfsbf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fewuzsnw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ipavctxi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2whnotjoo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hrniugcj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tlamslyj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mutkbtre.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mbjqqxoz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2osamtaae.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rnifaxst.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lecpsbnw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jbhpdyij.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pboqdgtj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ivqdnnul.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tppdzuwa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fsmjbnsv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxifqbvy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzujuuvd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2obkwlkcs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2relqakit.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2atfiheej.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tpkdorge.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgdbikmp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yqfxyuuj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpgvsxqu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ienjivtd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fllvdehl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jvsikcxb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kbvhlcvq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wtmycfty.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tejgyrdd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wfnunpfa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdspqvmi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2sohagfhm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qpqozpkm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2siwkkvju.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lienmhjt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ndlbsjcl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2akpopdnr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qkhvgnmy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2msyfohla.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2awdwhqyf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2uzgihhhy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qgdewnau.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2aooknwii.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2phejivib.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byfrmfeg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hfmdtyni.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2esogmvcn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ymkzfuuj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bfaujhea.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ssrhdgbg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzseuqaw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2sqbebncz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gyngsxvm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzrorppj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sbfphlwr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efgyusil.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stikfrez.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2orwsgbbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhugmoeo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umokxncd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agvrokiy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pvzmzggo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2brbzzxcw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zonpnwpc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdhgjusc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2elywcyrt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uewwyrrc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ydgfyhmr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mporbuqr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ebudwcao.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nrgxawii.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gyhzbxxq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hwqawjhm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kstfilur.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qrevxozl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dfsojxfz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rgyplnvc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pjmjikpy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vqpkldil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szkpeffz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lnjgfmgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajxefdst.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hrcedawh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ecvinrns.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2snysfwai.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2znbyyafu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovuqtzxk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggeaurho.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hslxhaom.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yevtcreq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2akpqhjui.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnfybddh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pvzptxal.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fbtubxjc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqejvmsz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zsjgghje.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gyybddrg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mihbhvmj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xqrbrqgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2catvrawn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gijevyti.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jkufwkfi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rkpwyztz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2thbrzemi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2luasapcq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qjlllgan.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fxsprfjd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2raqfaxju.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ksshuexa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vhyaaieb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tnsskale.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jidsqiof.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2joxpqqyt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wtmodozp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epzwmook.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nmusbhtv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wfdcbgqd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fmgzafex.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kvvfgazc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ykclbsiq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gsdotmuy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxzikawz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbewwhem.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbxgdvqd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jfqwvsir.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vxiuzxsq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukundsfa.html


<!-- 参考信息 -->