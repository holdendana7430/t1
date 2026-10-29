代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gogyxihss.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gacgtwlve.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gusoheoav.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gvlbjfhuz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gawpdpnvm.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/goahvlexk.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/ggrfvyzty.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gnwpvnhnt.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gvbdwheok.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghtpusgde.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gksxtjbno.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gyflijjsy.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ggexsncpt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gekgwybss.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gvyzshlpj.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gjklwulxe.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/giutdtrzc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gsgnijxnu.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gerrppsev.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gvgnvnnup.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gbnuzwrgf.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghszhzlzf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gjafhazjg.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gugvkwprg.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gtwuuimbf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/ghrraqgdd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/ggaahoivc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gussialln.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gcpmbpkmf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gjcunjril.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gcxalfmbd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gijtywvyh.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gotrbbryb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gjnjicths.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/ggwfefxte.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/geyaxdshk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/grpzzixwn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gdlucpdih.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gddyzdjyj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gyxmyzect.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzjbdrmbg.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/ggzolmvxs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gcedwyvda.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/glmnnojpa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gzjhiblyv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gkxwjcrwh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gemtxqndq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gcireybxy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gnqbzdjap.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gkxjmqyzg.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gjgxoksuk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gnibvcqlv.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gnrpgmwug.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gjxurbxwc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gdhgawqla.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/ghpbxpojm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gbzgfbjer.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/ggcvbrsgs.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gqhxgoyat.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gptbpwehg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gicruablu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gylmqadkq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gedjtvphi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghhdhuhau.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gxesdxcxb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/geuranqqi.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gavvgjaoy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gycyvmtuj.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gpckjfqqf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gfpbsxcsx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/guekgrtin.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/goiazjgga.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gegwndjqi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gpnwokiye.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghmnbtjkk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gcdanqbvl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gonxzthxg.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gkcrpnfda.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/ghhuiptzi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gthfdvswi.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gskskymux.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gvxamdtvl.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gmuxrvqxo.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/goexzgusp.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gotibqmij.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gswrnpvdn.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gyjsrihmo.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/ghiqrymlk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gjviobvtz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gdlsgiffl.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gasrzifzg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/grjicddtf.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gjgxwrzzh.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gvmwhctmm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gqpowqweg.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gvhklfyxj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gyswxddmj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/guefwauwq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbmyxjmfc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqmimvden.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/glvjrzjnj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gvggpoxpq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/greqhlocy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grenprajg.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gfzjuqtmb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/garzojtkb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gejhrfudq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ghqwkjyru.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcmfdqaak.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gcnzererc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/grrxmrwte.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gmbcclulv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gqyvxpetm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjjzxaidz.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gnpaeeycw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glzaihwii.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gersupvgq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/grlbaiktu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/garpjifyz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gmcldqzte.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gxrchmupy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gsfqofehh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gpcdeorpn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqdfmctkg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfazamciq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gpvlmsxcf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gmamhnajf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gtfdzrqvi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gwszstopj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gogtsdcjc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gtedkgypw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gsdnjowlh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gvehljwvk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gqjiqfaxj.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gjlzpycup.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gdhyikqmy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gdeasdtym.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnyfafrnl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/giaklisfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gulkbrorv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gwgshtjbo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gbdwjleio.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/geyxsizhe.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gthobitob.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gqikjhfld.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gnbstpqll.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gwysdxjdj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gpmazrxkm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gviywthad.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gfwvlawsj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gulgtyavh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gwlowjdwy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gemrshrls.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gzhctkcpy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gopudhacl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwwbmlrwi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gikswehbu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkvjwlkjk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/glbvriixv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwtygcmmo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbueekysm.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gvydoblnx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guwcmiybq.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gixytgggw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grwylxkhs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gydlufsdm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsmencnkj.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gasrkoxsk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvzsywqyn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gegupwljm.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/ghwdfkuqx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/grruuigzv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/guafxyvwf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ghvqgnenl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gfigkaftk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gesuyzdsc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gqffrntxw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/grnzkztsx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gqgugzawb.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gpwmdnzjr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gdmjutqiz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gazarndvl.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsyhifdki.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghopyvzfs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gelhckzwg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gaagkruuf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsjvmbqyy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzploxzmr.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gcrtueyxo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfyizwlwu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gufhuklqg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gbuvlmjjf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gsiqqsjsi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwjbvsqly.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gpepnidbf.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjqihudmu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gixhimfpy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/grorrpcgi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gipxtlgsd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtdcvyaqa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqxmmmbgm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grvsrdttt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gommqddpb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcfymiczl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/goarevdnc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grxcjaggm.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/goxycuqmm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grchsepjx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gsmixddda.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/grgxvsyzh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gdfyguooc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gonlshjku.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/glhawofok.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzudqiskc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gnxfcqbav.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gjflzujzf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gfscyosgo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gjefrawka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gbljirfiz.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/goywlrwxw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gdwtygsjq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/ggswvhexz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gswztvjli.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gghqcjwhb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gasdgmtqe.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gyvcbpjnu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzyudjchi.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gspcetlpp.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gvpwqffxg.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ginzunxom.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gedahxecx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gdutdjuhn.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/guysrifrd.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/ggctplvef.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gltgucidd.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkdywzq.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gdosdjnve.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/ghfpebdac.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gczolvnxh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghoktqtfq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gjbdvxhjq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggtxjdotb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gozrvaqpr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gtpgjxhtq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/grmruigbl.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gihqiynuf.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggaztaqoh.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gvznxozyq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbpmcylxy.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/grlrinmyp.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gxabzasyj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gydyvwotu.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gkqcntwwx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gmexjfwdp.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gvrvqhhdr.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gohmtlsgi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbfbiachc.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbxchgfhg.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxlvatfkq.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/grryojsem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gxykhnanw.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gdaxmoiqw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gwcfycvea.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gsuooswkj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gdiqvutrh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gevifyehl.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjioasyxa.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gsiozixpy.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/glgjppkgt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gwymlyjxj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gbqcniijw.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gjoutjury.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gwnxmxxyp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gunbfzaka.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gxibczbyc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfancewia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjatzprjl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gznletpmc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gmjamttif.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gbeboxhse.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gndvpexwd.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gqflaaqmh.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpdnwou.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gqznggnhy.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzthrsvqi.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/giqgykukb.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gkllmoygl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gfyzkigoq.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gfkxoovau.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/geeavssdr.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gvardtyhz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gnzvhttik.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gdijdqowt.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gudntukyi.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/ghtsfsetk.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gtktintnj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gbeqczpda.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gmfwllvph.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gjwwwehix.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gcaokqvpv.sHtML


<!-- 参考信息 -->