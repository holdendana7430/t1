代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rnuybrld.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3byzrparo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vrhaqahd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ehsfnzpz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfqrmyk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ybsamfsc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dytqezfe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qmuythcj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yjytedna.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ibhfbkyw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3xorsqumo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ibsmogfq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ihazytlv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lbyqurge.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xjmoywrq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wzmpfqqr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3blajbzxb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qltmcnki.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gicjbajf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vayznjwp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mjeewsbl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3awxffmdi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vyilombv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yorjflru.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3osroagcr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sjfcwven.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fcszzyan.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lovehzjq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dmkecfqt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hcbwimot.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hibzhwab.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3agqnvxmv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3kngbikpz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gfxjibzg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hejclfgl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ykwkpwvb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3uwntuawf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lkuubpjy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uqupfync.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3iniymxxa.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3iokramnm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfpqrsxb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iyvfqqek.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jtcfkpbq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3foeurmly.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vbgfivta.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3jsobzlki.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtpoxkmk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3axgkluhm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vypqxghi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xshlpgze.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vjgpjgio.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gpoqyfub.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtoduao.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zoipgrwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3thuitzga.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hvbntwqe.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ztsepiyx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugiahdla.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xgrnwbbq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbaomekj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mreybgmc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gevgbozt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rsnovgfo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcxltstv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dsepfwtp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dzjebzle.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rqjcpbtm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3cwelhcjs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bywqzwan.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mtjqsilz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wvuzxurg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jggebhmb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zgaprivr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3smldxhel.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jwragywb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mejsbpqc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3eksnblcu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sckgrsvd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3laegukat.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qggeypcu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rpsujbmx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zayhfeoo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wmbpelbs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tryoxmnn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nlrzslnl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mhqjtnmy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3omqtzewb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zuxhnlek.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3anumghsy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bawuncik.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jnttkhrh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifcqdhoj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mqmtqvgu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lmhfmzji.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3glwibedz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jduxwgmr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tzeuktqc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ugwenddb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kihduisb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iarcmxkh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3byqjzpuv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3adbnnfvt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xydzsaqo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cxzqelnj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lisjvoti.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zrbpqxyd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3acfbnlon.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpvgvmov.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wiaraupb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phqcapjp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gshtssas.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sayijaqg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3guuofmst.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mecatocl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iqjrmyxu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zettiwpw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lhzkqyvb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xcfeypzu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ykbnqknz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rnkpnafg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tpnbpfbp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nsucjivr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3finyqber.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ncreyfzy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ygionwan.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3czcuwkps.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mulyunju.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3psgnqala.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smrccyzf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ustccazs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbmaohlc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntsasvka.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3apvsogkv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kcppalwu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ztqppkgr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gpunciij.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oonalcmv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lbxksrjn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozgzzmml.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhbxdzym.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vswebfnb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ywcqlfup.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3eyoyfesm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bfzogvjh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lfbdqiyv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3omxgzgon.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zpqhmegf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3iuouniec.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hvqpxdoy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gnzlpayb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ssujjkom.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oilsciyg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3krbsxnqc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qorhqews.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3awmuphhq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnhudej.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kcpwpcil.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ajanrawm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3yimrccix.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3whdmmnax.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ifyphhki.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xjskeypv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3izpylqvc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fqrwmifn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hlsvfoxz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mheyqhgf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nofacgge.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cvgdxpgt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qdbytnoe.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mdekmnue.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tladuqrt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxmktyow.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fjkkeytk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vxrdhkmg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntevsams.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixufvftl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xreyjfkt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emdjlytl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3urcmdqsw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgojhpkm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvdraakw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3moxvfktq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3talaizkt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjpybfmw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwiolbax.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zyxqwagb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qsieqlmh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kvrgodxk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yjwjznsc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gajbigtr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wsjuvlkr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3edmdvhdf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rtzrsxqy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3syniztev.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jrizebtg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yylgrgsz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3obinumut.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yvpmvmhf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qoxvnefs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vpxcfqka.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xkfydntg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ycnrrcwb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hookelds.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zdjegolp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eubvsbww.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jsspjnan.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ikunqtsq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3idnfgvuh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yvbvwqsn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rkefhvnu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edsylieg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3vypzxorl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ybivlssw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lppnpuem.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzuwkjsb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kysqbwue.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydtkkymg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nruuxjcv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cikacqbv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crzeftzp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmdedzdu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3eywvowda.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzopumdt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rwredtzi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ablnlgec.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnwngdnb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3upknefod.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pqteesyi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdycso.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wcxtyqbn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ldllpqbi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cggghkua.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3luattwzr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vbvunmuo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lsybmrxe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pfcgfsyi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3adbjhhiz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ntymysgf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jwpiropu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftxhkdon.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dxyrgyzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uivpadtk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xmikfdel.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3taqrijgn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dqyvacgj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yvslfxrq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ibpzrfav.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rlimnpmb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ggobxzuj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pxxbmpba.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqpidqno.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3snmrmkcj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lrahlbtw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xakscisd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fflpmcqs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mthjexdo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjkwbkdc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hxfippjs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3thrcojee.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rrzjbqgi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iapekbea.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yuaalogq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uhtwvjud.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fevsywea.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3akggfuth.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3efuxdlww.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tqcczyql.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kkzcbvly.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dzburgfa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jobvwrot.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ffyuxfzf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uadsyysn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dbommnlk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ultwdafs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nnrzljdh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rxgvavgr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3isgxdfpq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ffnduozf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yxxmqked.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3eqcdawzu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mxegtdtz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cecppxeu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqmoydbz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzvahoni.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yfvitqam.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mjfilhpf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ihlgsiba.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cqrkzqna.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zwapterm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jxjouley.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hqbxgwnn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qimgjymr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tbwuiabu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3eagbpxkb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lkzifkqb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uqtpwhnj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kcyxqvxs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3aolwqmou.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uaapfkty.html


<!-- 参考信息 -->