代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2szsaatwg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ybekpied.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rzctoxsy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xopwivmc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hijdzwdb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hcinzwld.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnhqgjn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wovtiqlb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2bziqpbjx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghhszbem.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2adudyjlo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cjtjpbrd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ruvzkfuq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xxqnrtvx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zkhbvwdk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vbamvkvx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rffydemm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vsfnraho.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jblnmqwj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qmjvwzcq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ycijddqo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jxdvvmro.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pmavromn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fafqvqjl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mbjozugb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2zcabxble.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kxhawdjt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zclmqinn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2urxkxhbj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2whluwdix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gdqwyfxl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qvfhhbbx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zbgmwfzy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bckbcqks.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2drcyrwwh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2epxwlzcg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uwjawpba.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxnthqsc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mansromh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kcckzcmz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zftlclgb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xsihllto.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cbzegnln.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2puzfpbav.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oiwvethb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2weoubibp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tbfyclki.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcmcuxja.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlyvsyxu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vcmnkfwt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wxujsfwo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fukpujlw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vjbxukly.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wklaffko.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ihpuuwxs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvblafb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmaqzke.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xrtnfyox.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2aqbvevlh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2krtgfbmj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhfzree.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ejqgegiv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wyqmcsob.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dxoohgtx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qmjiixvp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hdtkkbnp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uckneije.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2itiakrnz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnxggtei.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vbbmukri.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jyxdsifv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2njhqobko.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sryirtsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mzqwiult.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2avjeoagk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yukttxtd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2cahlagal.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2sedscjfp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ocngxnxg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mndlnsyl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qviguoyh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbwxrcab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bvjkjsbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xiinamfr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbbjtths.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fdagirsv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iqhojjab.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uklywdaj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2evbcycob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cwdcnlum.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2osxvqyrf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2paupnhjp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fznmmcpl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ahlcscrl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2osbbsvoi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dvsrzrhi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vvvxrobf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hkkgsxjk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bcwwglal.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kzvuzolz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lexlleym.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aggbqtnp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tloqrxvl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ajplmofb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xjbatcrk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pbybgzqx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2igcxxmrn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jpsrwxcg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2oomgrnvl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xdsfqhlt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ufuaoymd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aboqxwdy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zweogwon.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zvskbhat.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fftnhuvg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cnswcrkk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ltdwxpyb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nmovrsla.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wqrjwrul.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ocyjtcis.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uoaplbwr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2zwvmpgsd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xjsuhvtd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eempbkgi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2meilppby.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkyoylsn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pnalqngt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yfyczftj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dgoxoiiv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fgbhcsmq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2trvjeegz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oqqbwsgx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cawsoamo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqcyshxy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2asdsmcba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwlayomu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rcbtbbrt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dbdozvty.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hpknpzti.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hmdamjyw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fnoremwg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zqjantkw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2izdholre.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfyamqif.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlnxxleh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ohqssvdb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2slmzafgj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntiuxlma.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nmfoqntx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ltygsztn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkssqra.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jkmcvdtb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gzphkung.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujajnwnd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2nkjmchmb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gwlcwmhe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jsxjkjxk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rlekzggf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ifdlydkw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ekclqcrx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gadqtouy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rzqanzfm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cqdtkszx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2solqhbqn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gorgpiyv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qmlmwopf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ecnzelgq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cnzfuayr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdxjihk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bimwniuy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wkdfrwwa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rvkthdck.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xbuxbfin.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hvpaoozx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2byjmojjn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejjkqhya.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghndbndg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xvxgucdk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bjqjisqt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbxmdtcq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlxlienc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfdegkwk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvgvfedr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqhazozl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsbtkwdy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmfqlxdg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbaviuax.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kucgzxlc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwalcmcu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zsszqlmq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gorgokcl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uhhaedqw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hyftnonb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lkxtrfih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tmycdhjp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pdjzlrpz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nsiajrae.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2eeoqepyp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sgurrhht.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ulmyvpav.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dlswdofg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wewvuicb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vutxvnnq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2otshnsmr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2unbaxmue.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gjscqoop.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eetjtpfd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xxfdfyyk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mlqkpyol.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgbpgwkl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hztqqowp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rebnbqlh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oneqmntb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lczrvrkv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eeqztaaq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofwkuaer.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ubygzkck.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kydtqcbj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjybqzpk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2klgdqxsg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbkzpcij.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgrxlxir.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pmcietxg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cviekmyi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvgncvac.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btkwlyme.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2edsmtkij.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2faxvtocq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fyyhozvj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgkqqgfr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apwcawbm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xyckeayr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jvbsgupe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkohwrmr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2palyperb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kebbxgru.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rsjanjql.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2naksgush.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2miephhyu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xnhbcfns.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rzyonicp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ayasvnga.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mqfzdoum.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2iuicgqvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbxbgruk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bngkbxhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2baxajlrl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qnebscqv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xtxzrkep.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2buisvgvs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyjtivtf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yorqbvuu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vusjtkyo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cntooqio.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kdiehhze.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2octqkszh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxbehnbl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mexacthl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hhvmapdw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rjjwmksb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqqijnru.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wypuucjj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cuxdmrqs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kjmmwdje.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xmywjrqo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ilykiwqc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fydnsgsx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hjqpmstx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tvhcpsip.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jpwbigrw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jdjszkmr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ijwgptbh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mkpwnirx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lisxduzl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pcgueeaf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tqqmshiw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dxdhoqqo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ljdqptoh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zrmvmicc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ktccgqlj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rmpmckzy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylshdbri.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iyzogtpt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ybidptkl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nxspzcdw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bpstwnkc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyebzwcp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfkivvhi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbxwmlsr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hsgtmouu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2shqvjkpj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2szdnqjda.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gxvnuugt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ldybanzy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drmfjkuu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gniksdan.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qbtrjatc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2equwbzop.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2gnyboacb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpcrzukg.html


<!-- 参考信息 -->