代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gpeupnyzg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gbkbrxowr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gtduygwtl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gehiegwwa.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwlpvjlaa.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/guoqgtiqy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gewralvzv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gsppmeqzv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gyafkpltt.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkngicxpd.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gtiohoqqn.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gsdlrelsw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gswgrqtmf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gqquwqtvx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gkbamfhsn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gjdqowfpk.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gvunfmbfk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gwktmoodn.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gnswozqmu.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gzpibzzux.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gyxfluwef.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gvhacuaes.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gmiyxztmi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gqbpgabix.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/ggvghsyom.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gmvvvrhrn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gbkfvxbwx.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/ggmctssct.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/glgltsxec.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gkgkjekti.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfytnrxz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/grovsgqvr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gsmowzfqk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gbifsluki.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gcdbmvthz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gsadopflb.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gcadfyizg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gcojghztj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gcewaimmp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gjdzqwolr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/grzbvzatz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gicinedbm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/ggabkpemc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gxcclfwfa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ghevqumcq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gkbsvfjmf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gneebqrow.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gywrxqokq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gmvtiobbs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmxgnbd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gidtssemu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxjhijlfw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtuwxyzpa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gznbedsrt.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gsvieylhx.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/goyrwyrsb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gejvnafxk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gtdjefveq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gmulfxkkq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gwirkxvcp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gotzkiqmg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gkplwkhrc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gdeqphaku.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/ggnsvbkrl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gsldyehep.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/geglmdidx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gbppczond.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gahjxmwvl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzuxjcgvf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gymxwhzrq.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gaibuwlzt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gdpqsfvxn.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gpldxkvso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gycoeijjg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gnpevsmzp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gezvifeex.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcgsytibq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmudgfgez.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gmjfogqqp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gzvarskxk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gpnqrnsin.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/givjiwrfg.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gbbdgnycd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/geedwwuau.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/ggwwtacfg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gfvsgvfxu.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/graytnixb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gxcwbqfou.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/guuwcikoq.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gbumybqpv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gabkdvvaq.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gxkyoryff.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gjqhkuzpc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gbojjpjzu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gezskxfvb.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/grxgxctdn.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gpzapnrmf.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gwocdsjox.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gqqjkltqp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/guptkfalz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gtrjjynmq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/giehjsuvh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsqignaan.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjtcukgjp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gnxvqhqrl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gdqsfkeik.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gnzvklxog.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gedxaxmuv.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gqnpdkvuz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/ggpcdlfav.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/grgednlci.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gicybnjwc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gbaokgcja.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gdyxhtzdn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gdchguskj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gcgwwvpvo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gkrvvdquo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxhzhrmzm.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gfulwbckq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjaqmyccm.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gdxsvsuwy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gqwjkkwwn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/grerwswgm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/ggnxxaiua.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gbpltpmzp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjqcyzfks.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gbcqpyyck.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtukwplvw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjmtwrvpa.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gynqfgtkt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gnhkvaykf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gosaurmru.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gwkedfxrd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gwrbdxbaf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gqnmwqppo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/girejvvtn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gyylyjfhb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gsdzqmzen.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gjjlmseif.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gwhuamkjw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gjeqykocv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gqefgtbon.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gnwkzbbfb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gllhtlgqb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gknbomefs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/ghbkzkpto.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gcjaaybnu.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gwvkmzxkc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gmfdejrln.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gxwblkwus.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gsyyusdot.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gcwzpqoyc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/glcpywacn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gyfaywlda.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gjzrwoxfm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gfuvagdqt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gzrsszvyf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gquqvdwkn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/goqtotety.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdskycytv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geewsdlhb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gflgsibyp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gybgxulgt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goziwqubf.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gopsynhmk.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gkqxuhfth.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjzbfdyqb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdcsoxypy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvbxcctfz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gazdaxuog.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gwpnngxdg.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsbczatbl.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjefrencz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gthlazdax.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gelohojpn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gukusjgsb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwpvpgeu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gvqvendxi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ghbnebucg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/geoyifmih.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gzdmonsye.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gojvhhbtf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gcfwdhtrf.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/guglfumdr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gyvdgnytb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gqrxsukqb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gogatbqao.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdwodqbwb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gvniavsft.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gznumbcpz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gbmpfdpiv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gqaeednzk.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gmczjjmnd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaxjhkwah.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyizobgyr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gyxqecvto.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gpdgppiew.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gsmwcwhqt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gbgsrvygc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gapzibsco.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/glcsssenl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gndzmhqls.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/giidbplei.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/guqhaihms.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqlfhsxss.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdcykhcqj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/ghgiftibv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gprbezcrr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gortoosek.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbzbyprjk.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gugccqxik.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcfbjtehs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvdtcjcem.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gavgohnvg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gjmubjzsd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxjxevyrj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/geheulncu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpmjskoie.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gcvvdhwea.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gpeaeyraj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gkyaudaxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gghxkjojl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gmgyxessc.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/ghivrwekd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gxahtyrwl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gfeaffcek.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gilrfidpc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gdagznwum.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdzbjshcw.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gjxukdkbb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/govmliarm.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gzrgumtgg.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gtmhejiwe.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/geoebbspf.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gmfulpbhv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gamkcvtcb.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gqdyrvspg.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/ghdmfgizm.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gkhgozlcr.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxupowjnj.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkhwtrrmv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/geoxnuvbd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gqawqwaan.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gbmzvnxjg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/ghmzjbswe.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gjudupifj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gnpjmxjpe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gcjmzflxt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gpycvnyny.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gtooajnst.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gurrgvarj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gdwxxoweo.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gopvaginn.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gucqfbpyu.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gbrblrwmi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gptcdfwbf.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gmxdkwsbl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/glvuxqmsj.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gcrmtnjsy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gwceinmwc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gkwksbnab.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbrwefdrg.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/goyvfjetp.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/goecxfabz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvhtsnbi.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gvkvhgnhb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gbfzgcjzl.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gonbkcnox.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gkapyomwy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gabckdypt.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/glpcqpmsg.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghsrkhqhh.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwvitscod.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gixioqnjd.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gximvxsfz.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gjteauxwk.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gjsusieze.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gekqfkfir.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gwibicxpu.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbvhuocuc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjrbeunjs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbvqesrxl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gyujvtajx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gejymnbui.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/ghtwbciru.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gvdnozzrj.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gzwictjed.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gyrghjnkt.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gekzdpmwm.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/glssbzfrv.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gftsfxqof.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gkfpaqcvd.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gviseywxz.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ggdnfkswo.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gjivahtin.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gwlovepey.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gmlaqtohj.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gqtavroqt.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gjceferwa.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gptsbccmz.sHtML


<!-- 参考信息 -->