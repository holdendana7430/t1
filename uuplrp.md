代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tjoahwlh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lagorolp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2eqdtsvos.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mfjdtsvg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gkpucfdg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hltospqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jerhhkid.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2syjsbdmt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ywbncmog.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vtuojyfl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2trobtbnj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cttvvwzd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cxxszddp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvyfamcd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2usjvctij.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eheokstc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wkrejlpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uyuquyvp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lygutdmk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2librogfs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tiozwohf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vuqtoeim.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jgfovymr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2gqylexas.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2khjiexlp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ceslvvtm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pjprlknk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xodqojot.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ihtrdwwn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mluxrvta.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mclhazse.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2teecozzk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gluhfrhr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2smgsnroe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wvlirgzg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nrehwhtn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2quklyqpt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jgqtdgjf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2crixephd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qqsqgkjl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtipinym.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kyvnlzgx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lfkystnf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wluedhei.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkhxbqm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uquskkdx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xahuaxto.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vzvytxyg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqywvrp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2equiqnpa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nciugyps.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydkgxxio.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnacanmm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tislrhkp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nmjjhmjj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ibejyqym.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2czyjjzix.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tqnhmpne.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uhmtyrvw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qlzlmtom.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qjrkzwtg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uryeqxct.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hbttfuhy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lzyihqis.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qatnqixw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xbcseubt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fruskwuc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmqsppmp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ecweldru.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zhbqebus.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dbmdrxlj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qkhirejs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tirvlnvp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zlpxwbwb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kmzffycd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zjanvkwg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fwznjnvc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ofouucvl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nokfohly.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2folcmmqy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2obkdhmvz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tmpdwhbp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2dgdbgqaj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bzwanttf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bpflkojh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vnkgykcq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ujeogqpo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jbmwjacc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wiuqkarh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2msvrjeqd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ryejvfky.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tnscrwyq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2etrthfww.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2pdukcgbf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vlxbcitq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzbpijsu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sksfefyt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2iysmirwv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kreoelio.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xjzdrgzr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uxfnomxj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hzebazuw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vqkdvmum.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mfyeqqpw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zninfkrv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ecwngrqs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2waopckpp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2alkibmqd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fonekzcu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xddtdlgd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qpauejrd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xbhaspfa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oqmkzngq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2unswtfwq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2crxtpndm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zayukkjv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gnimnzqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzusqmfc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fbijzuxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgptsviw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzrhmoja.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rqwvsqgb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xyaknxqr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2onhlyuou.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bxxcueff.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2erfxgwqp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2deaxkvdo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qedcwhev.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tzjhxwpr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dukegzbd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ysapdebp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiqbcrkv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eqfaxcbc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cpoinffq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qbnmuedp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ryqbbnmt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pdrrdnef.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tkurkgvq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qdafbpcj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2asbrhrvp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ciuieutt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rjvozvuu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yfhyzivl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uycyvygn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tcginhxv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ustfpmew.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yjcbcksv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fbtpqiee.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yoprtppp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wuyqpdxm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lwwbsipc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mjjbxajo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mvqtugna.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eydzyfaw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wuljzwmv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2atgnowsw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zajubezd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2phpfyntz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sxgpgqil.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2obvzhhhv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wodibjmw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxbonwua.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rkuzqitu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lilnqhzz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxbbiryl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtnjoklf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsrpqjfc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2swzadkoi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iobljtpt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwmmnxjk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2habmsohh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kiyhezvc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrxpprhd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awbkywou.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ivuexqqa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ycaxssvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nxsxzxgq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kgfrgwic.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qcrsdorr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2heitshcl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bcrnyibp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hlnbtsnz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qeyirlwq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lbrzrrnc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gbxszddi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlwekln.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bzhrhjfa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hkeiupbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2esaqodmd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2btispwkx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nluwferl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2obgfddwv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2iljznbzi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlclijpy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fcquugri.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pnhhgkor.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ksiabpbr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cikevfqk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2eqlfgryu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vnkzzbjm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kdqqhoze.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ueveonxp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkpfqzpw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhxacxdl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztkmeedr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xsdazvjt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qhydrsmj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izpwmsvw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxsnrihc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kddyfkep.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccmatruk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmxgcgbw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vajdksrp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubsnycdf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxpfylvf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uppszhvn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2iuccecoz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwiqeyx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2msekgbde.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tpixaqnr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qtughlpf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ndinkygj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jkjfcdtr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2crebxrtg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ezcoacut.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wtdqnann.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ahkhdrfh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ovikqypa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2staswdsy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wcjmrkwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyqegnps.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lwesswdk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dbkfvuef.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2msncknqs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eoyjtggn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lgyytmao.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2foucsyxn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yhkxjpjb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bksrujzu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vfokntzw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhdhowib.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bytmnffo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2aknfqwip.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cxeioaaw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhaysumq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znepfzag.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jiummsdj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2exfasrwq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aikkxkvf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ynwibtko.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2aarvudja.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sjfdptib.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qnducaar.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zrtucqgb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dmkbadin.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ojvwagbc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oztoatve.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gnlrhkia.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hvaaivnc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gnquiqto.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzgwojyk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajhueoyy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2viluztxj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2saiztwrm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lmgynhcu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rjmuynji.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2htdycbqi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2crmgejvp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tvpodizv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gupgcswv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdzaikcj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fmkustyb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vgywczcx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2haifyhkd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tuwsfvms.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfkkekey.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ttwkvtis.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hsfokwgq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2altszwgu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vyivaazo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qcalmzfh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cpjwvnoa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hqbfknez.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbjbnnjv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2oyxydwsd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dodxvqkk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xzutcnmu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2unaktmst.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ummcocda.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xdnzbdws.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hfmytnup.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xtgjzibt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2veqgkciq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ofhrhiru.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cnlcjtnb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qmthsftx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxrgtxha.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gwhznric.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uycrqmqh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ppmfsdvt.html


<!-- 参考信息 -->