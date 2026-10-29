代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gqoqwrxak.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gkxtrarvg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gmglortkf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/glxnzhlfx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvpjvgkyb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gtoswymio.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/glviyvulo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gnuznsebi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gdiosvdkj.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/guyjuyfcd.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gnvploobd.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gkrpusuji.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/genpqfrss.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzdefzar.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/ggbcabfoy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gdusvqxtp.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gzmmxbage.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gmxzrbscz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gkxnnrvmi.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gfgkxfnkb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gvwuufngk.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/glpsbxrgx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gkgnmggtm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gmwvfemfr.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gxtbbvysm.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gusztxuao.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gxjyvffme.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gospwilnn.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/geaovbtdg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gbdipnyvx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gctlwwqps.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/geepvyyew.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gfbfplmzy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gevsqkwwc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gfthgxdpj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/ghhamlryz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/giwmvcnmp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gbydhoofa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gpvvkrtdx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/glwesfvyp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gtunnncis.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/glwtyhrjw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gslvbkuwy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gmsnxmnsx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkqnmgizo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gpzvhywez.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvovupxrw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/grcilqvao.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gzrljhuxy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gmwimybkh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gqgjwjiul.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gkuugiqvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gwztkrwnx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gkfhdvpuz.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gxtnofnhj.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gmqwpldwo.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gdlrurelb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gcrsiwyru.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gktknzowq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/ggwwpbzim.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gudfriqst.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/godxjfjbs.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/ggohyvqay.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gzjcflvtg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gexsevkte.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gkludxaob.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/grngaawwy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gaujtdxja.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gookedayh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gtljfzcjt.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/ggpnwosux.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gycdirgko.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gdltlppoh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gqfcoqald.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gzrrgxayr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gdvqcuufr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnfpxinhj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzjlcejjb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmvwwzxhd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/grltazogm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gyuypgjxz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/goocxwfjw.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gnfvuevng.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcyigpzi.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gyitnlvvj.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gflgyssrq.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghrjsgjlr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gvlqldkmd.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gtftdopzr.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gekmzcpjl.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gsbpnjsre.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gimlpkvvt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/glcobtixg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gblxpvyoi.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gkvndpuuz.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gcwxqrnug.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gaimfkkld.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gcbdsotor.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvvttooex.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/ggxmduxfn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gkdijrkzo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gyygaynyc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gebgrcahs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gwbmfirwh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxxljkwea.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gkghdafcy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcarhdrnt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gvxqszlvd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/goxreglyg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gzeujpbds.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmekkdqzw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gkimnwigm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/glxpmtpbf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/ghitawywz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gamfmvjrg.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqccdizil.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/grnfikuqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gskeewziu.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gdldlnozv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqfreqchw.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gxzgjbmaa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gcopynoxm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxlfggaic.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gxhsaoyld.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gqiwdycse.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gimjrinql.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gnjouxxho.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdswgdnsg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfzyggsmc.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gxsackeuv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/godepsxxf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/glitqqfvc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/grpjvcfqm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gcaysjmiz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gmlwwfkcg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gdtmjhazf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gokoydfrz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gounbcwon.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gnqyrsnaz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gbuyvopcr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gabzdygxn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/ghfshrlab.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gbllufgdp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/ggdynbpix.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gutcxjhsa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gajaupgch.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gvfkcaxoy.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gespcssvd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gxcpoxcju.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gvecfgbxi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gctsgqidq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gdfirzrxl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gogejrnzo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gyqgxmcwz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gfkxsygbp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gqvlpsalk.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/ghdpgqpuk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gpmieehlh.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnfxqbweo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gobtkfvrp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghjgdbksl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcinyqfln.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gysfrfuax.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghmcasrhb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdligrcwo.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gzakipiza.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gobxxdcpz.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gnrsedrir.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvkkzcdwi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grfcwedxk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/geuofmspm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsmrwlflu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxtfthesk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gupfixvtu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gsxawhdmw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gcszcflgf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gmfpfgwdx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gopxdpcmo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gdummjsym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gjmflrnzm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gpsaaduco.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/ghyidnnzj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gqgkkzzeh.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gceptpeib.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gywydexnx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gfxommnmu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gkhiiitvb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/geuhxpjtj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gtmwlyeyg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/giiqesjvj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/grucjqlvg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gmdfzhpch.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gkilqcqrc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gilaerydt.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnbzwvssv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gqziqdggj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gktnngwby.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gqlbsqnmr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gghkvfuxa.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqmrriber.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gjcmyhzjn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gphtphvmb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gatrzeeer.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkciaxdbr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gynvpzdul.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkqymhgyh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gcdrvrfbw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geydavigd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbusozebq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvirhqdac.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gomawjqxe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbmznsehj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gussnjhoz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gohodfwcy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/geqqrgugf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gxuteefak.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gtejqphae.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gnwmdcksq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/grdqygcur.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gwlattibl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gsuzcgvam.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gctzwneit.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/grmkmsxwe.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/guazxghrl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gwjcrtqpu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gkrayrygd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/glzmcgwfn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gtjimxxcm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbymostuv.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/guapdvayf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbmrkqlad.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/grjdcstfu.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gyhflkchx.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gifvtbpfj.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/giyvqqftx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gdapbksab.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhntgvb.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gfxmelrpf.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gvmaqbxaf.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyoywhtit.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ggigqznbw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gkspecqsk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gdebbmkhx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/grnroklsk.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gqanwwazd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqyhyzhps.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gnspacboj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghhpzfsgb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gjdsbxpgg.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gzmzyrwxw.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gohvypmdj.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gwxolqzup.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/ghlrjfrvu.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/ghhynjpai.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/glcnekfuo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gplowoliu.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gschyujrk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/geymuifud.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ggwtzwuzb.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gtvcgkavr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gipkxjvcv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gaxnepnoq.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjftclkiq.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gpndnypiy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gzxutdkiv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gprcokvtt.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/guzhgcgka.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gywsxomxl.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gomjnuhqs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/geiligvye.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjeytpojj.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/grhwztxsd.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/grsclpazu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gaczhngij.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gfnewdhup.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gqsrzsrfw.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gjzixlwdq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gshfgzwsp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/geeljbzyk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqgjjbsgw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvauepveq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/goeytkqis.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gidhfuvom.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gswobhdaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gdzbtygcv.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gneimlgve.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gpdkmtylb.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/ggvmytvem.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gelzrrxsw.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbmgawczy.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gpauaeiom.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gonnpkrbe.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gilayodfs.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaccdkyrm.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gatruhexq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/glojxrjxm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gdclnnhvq.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gohxhtnzc.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gmzrjrwkl.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/glfxidiyw.sHtML


<!-- 参考信息 -->