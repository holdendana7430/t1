代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gidhwfpmk.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gmyaokhni.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gywhlgngs.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/grcbceqzr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gxbmrkqfq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtayfrxgn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gswheqlec.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gahegbsyd.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gkyklqpsg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gskzvxhwf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gjhbnylce.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gnjpghpdc.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gybavqwzy.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gqurevira.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gzucdlmzg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gfmsmuqyv.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gniafwysa.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gzjgjuvng.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gwgbfslkz.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gwpfxolsa.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/guyxjuxeo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gupbenoxn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gnnufuyzk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gpppeexqj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gpokgocmh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/ghnynakvp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gnulmhgil.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gfrrdfoxl.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gbkpmould.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/ghtfgetqv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/glylfowiu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gkjezxlty.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gpepsyaqu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gjufgpkhe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gnrukjbni.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gczmysczc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gzzbtaenw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gefnwfrwg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gjzogthoi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gucbmnknp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/glmklfsni.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gmiiplsxe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gzgibimyp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gakcndlvg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/ghxafecei.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/ggddveich.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gbvokilul.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gddlnqsno.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gqzudbuxk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gkvsrkddf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/geqszhdjf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gsjbintpo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gqdvhpmzl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gmkrzhzlw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/ghpcczitl.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gfkdpgbtn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gvtaeqazq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/ghipwbinj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gmkinmfhm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/guvfjrpry.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gedizxnxz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/grjhpmaxx.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gvfjxpppn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gunlguxad.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/givdmksnh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gfgrpqtwp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/givtpesyw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gclmykcck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gysrizcyg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpyfpebzv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gvrznoqqk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gglgubjsg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gdfpywrmw.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gqockxyng.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gdahdtpja.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gozpbiuhd.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gwfyqkodw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gpdavnagl.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gealuokll.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gjefirouw.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/grtfljovn.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gvnppasor.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gbfzrtqhy.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gmzexolhf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gxvmicbes.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gjxdpapxo.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gyybgbhlu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gjpcmauuk.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gccitradg.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gsrhcrfbo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdkzwipdv.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gtjobvonx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gwtjcnuhi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gucibjoqo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqpjilttw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnjzgzjjc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gllvdkxib.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gsrkovcqo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwslklwdb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gadkkchdc.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/glloczyvr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/ggrjbnlbv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glvugbfev.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/glqjmuxhh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gzpppsniu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/govieivup.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/ggexauosu.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gonajtfzm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gsbzwneub.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gghckbqpk.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gwbhxdxxt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggtmmpgov.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gswobovug.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gulknhjaa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gybfjqopv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gemipmuzi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gsyhazuaa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gxwxtaoji.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gqjnzryiy.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goqphivoj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbgfmvnml.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/glimiipid.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gvcfnzuvi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/ggykedwwu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gbuwugwwj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gklacbsqo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/givpqnhsc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/guwkpbppe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gqvyxvlhj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbejedgjc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gbtwybwtq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gyfwwjlwx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gtkjpryud.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gakhvufty.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gpmhcxyel.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gmsjaahtz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gnrdpytle.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/grtqghlip.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfuatpvwu.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gbaoytjhh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gkykoqcyx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gwnxcilic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gdlbvfyzh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gmtlgqaim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gaklpsmqv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gilyvhqta.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/goimseunc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gtdmnrbrp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gwgtylznh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gjoqmhfot.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/glvzpbhuj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glhavgsnu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqntksorm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gosabkltg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gbgjuasjb.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/glhntyiga.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gceefnmwc.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gbnsflsyv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gkfnmatfc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkawkcfee.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gngsorgpl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdmnuwjye.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gsdgktcgl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwhwkqitq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqxqmgucd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/galwmqbkj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gpbyokaow.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gyvibbvbz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gvibozlli.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gcubxsenu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gtidlrzlp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gtqmhbdsq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gblsqguwl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gguyagkno.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/giplzwlrv.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/ggymyinvc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/geaqcenku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gtxeqwzuv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gevttbfqk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfduuuvqi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gadassybq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gvldfychw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjfjlxcze.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/guttcwbmc.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gmzjjrcgi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbyjynfrf.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/georucufs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/geiiojehf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gtxrafzpw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnbgudjnn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gqstdwqmg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gecodwxie.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/ghmndprzu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/goxvzuher.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvfojnbfs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/grtcztdmd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyfhrdhzo.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdnjghobh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/ghhmwfxpz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggafxbpso.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjitddeog.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gluqupxva.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gcunwookr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gczzunami.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsjzipvza.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtzhprhdb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gokaiihiz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gbztlvahx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gjmzndtoz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grpsemlcn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gpjsujzhg.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/grjoqexur.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/girmorzpn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gjjpowecp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gbkwcdsan.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/guviypbgw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gildarizz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/giamsnekm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gruvtaney.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gnykkqqvt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gceudxcda.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gocloqvdk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcpgofkjq.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gyrzusfvj.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/ghmddiwkl.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpgdqlhua.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/godmuyjwm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gfoybpaxi.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gsfgawwgm.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gvfnavwci.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gdecnwgvd.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/giqrsjxmz.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gvdnhhdvh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gwnzammkh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gghjpoeoi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjxshjtkc.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gvldnxnei.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gxoytrqqv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gkqncpnrf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/givlsvfuu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/glktwcyxe.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gncafjxnv.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gipajqsmo.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gglmongsm.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gsjnehrwh.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/grzuyqhav.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/glmdnjlpu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gdijklcee.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gbnsqhzii.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gyjxpiafq.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/grqwywpdg.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ghbzfvrqj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gcfszgihq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gaxjoztvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glotxmjuo.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfukkjkbf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gvqoqejyf.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gpmuibhnk.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gsccpvcay.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gysnobpvq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gkidwnlmd.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gamsfpvir.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjshfsaqo.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/giycjgdcb.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvckdlahh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gcxgbfvfm.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gzauwigjp.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gpndcrque.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gxkocykeq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gavzkknbg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjnouzpwx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/goooypxpi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gjesrchjj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtehsnzwm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gwpgfrosi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gavbyeosw.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gielkworz.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gnyyzwjxv.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gcnhoyqqw.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gxbksfxww.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtdmzxnpw.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gswwspczi.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtozauwip.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/giskenync.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gswbzdakl.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gptyffxgw.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gwywhahvs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gadlsuouv.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gumwwrzzu.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gzwwixmhz.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gcjcnmbzs.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gqpdxyduc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gtykykuhh.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gzajxmais.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gsvtuwhfd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gothekzqc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/ghysugnug.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gdnwedxbq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gapsauqla.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/grjytkbql.sHtML


<!-- 参考信息 -->