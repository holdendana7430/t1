代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gzqjvljus.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gbncwfnor.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gasdcrowl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gdtfmrkog.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gfflpbevb.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/guaosimzn.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/glrsmdzty.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gnecnruba.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gknmlqoij.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gphrmfqgs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gqufnpyac.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gfnhhxrnt.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gswoihvyt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gcsnrpwfy.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gonfxeovl.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/ggjpxnzib.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gsebcpuwd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gxpjnqehe.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/grovczwbr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gjxnlytix.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gzqgahabq.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/ghncksvqm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gxvxqmool.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/guhhvxvae.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gdngzlzvf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gqtfguamp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gqwcpprub.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gcqjqeymq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gnmomnped.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gsjauayww.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gibyleaza.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/ghzhdlehl.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/glnyzvfuv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/ggoyxtocq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/ghtmvdtrt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/guourbquw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/ggmmwdfle.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gzfvltzmu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/goceuxput.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gizqnpufv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gvwxarfjd.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gnohgaiqi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gltivfbed.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gxkpxsbkc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gjaeyrlux.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gwbxjilpy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gnxkoetzm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gxowqhqwd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gldyfhkmg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gsmtretcg.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gtshibips.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gseispsef.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ghoknzfpg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gsvafrrbn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gijpwrroe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gabulfbel.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/ghbvdukaq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/ggzjherzt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/ggfeuzptq.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gwvlvnkct.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gudjsqiiq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gbknafgqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gprrflybi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gxtcpuitu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gilukuqxn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gbqwyiqar.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gcgdjutve.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gawervyjw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gnlwdeigk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gnzcusfee.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/guajfaboh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gzhbvnkrf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gnfyvigvq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gxjbuzveq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjfzmvosz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/grfoodwin.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gntjogjwx.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gcnteznlg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gtjkbhxrv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gkccfanpr.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gsouoodhv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/ghaycrujy.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gskfojqrw.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gufpwvttt.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gdazhyjai.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gsjgwphgy.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gtlyvokde.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gftbeclmg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gumydywxs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gmhlhtnro.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gcnpovgsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gnnyfxqax.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gzjjzlgof.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/goxqodnfu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gweefeaje.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gasntjkdc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gnpasxdkj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxfuhjqbb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gyhilfwcd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbfxrihqk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gaxratfgo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gneotiyyg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gldflyegm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdxljcyqa.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gidkxewpl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gcyeeexdt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grcarvxvq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gacwfldkd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/grsuedqza.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gtnpugsiv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gmlwstapx.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/grmbyycbq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gacezygsj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/godlapwav.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gmrdxgdau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnocdhcag.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gdbnftnqa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gfribkaqk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjwtmimkg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gxmfjtaiz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/goauyiejn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbhrzxlmc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gofvgscsm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyvttnlzn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwimmgpio.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/ghmrygpcf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gnwlpklsn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gfqkhklxh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/grqewxcnw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gaydyskhm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gbpomyyxq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gyktmcdpd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gnlljgule.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gxffqogop.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gklzzsihr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gbtmbsrjg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gvnrwhffw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gkvahnjtw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/grolzjytw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/getksijne.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gbwavnupb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gizwdrkro.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/ghrhevyty.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkqpelbrc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gkihdaoap.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gwrelnnxv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gyumnwwaw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gncsjafaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/grkmcrjgy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gjuwmqftr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gbxtlgtsp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gftrpffoc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gwehcrimv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gihskdvaj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqtybltiu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gszsmliwx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gachwtxmf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/guzhymzuw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/godfpfswi.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzasdbxzb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gujfvcauw.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/govjnwdin.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjjwuoknq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/giyvuhcyl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsdbdlgvd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyozyifwa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbxyqiinu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxkxlswpa.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyzfbtffv.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfxjvwems.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gsftntoea.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gcfezbnwx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gdubgcxuc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gelimrxwo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gukvxpnpx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gjfbdqlkc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gkrlnonka.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/ghrirzxoq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/glihbhaag.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gjyrantbs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gvzxmhvzt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gqiazmgqq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gahfadhio.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gvuvgkfyt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gnnzthjlq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjmklxnxf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/grcezryad.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpbkeempb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/glmczrtgu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqmuwdmpf.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqvzwshyr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gyprwiltn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gcdnzqhtn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkntludjr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gteektjpr.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwphduqnu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/golvwcqsc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gtomljhsd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjsufzolv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gytjrtndj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyhwegrbd.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/glrfukivj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gnisnzfrn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzdakyezo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtxhsllae.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvwbzajhm.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gmdnnszaj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxzogzuqc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gooeutibu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gymxgacvo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gicolwmpr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gaaeoreqw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gwbcvieqr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/grudrcubz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/getbxydkg.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gyucojxhc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gjqkpqrpe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gtouskasp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gnxapouvs.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gkajpsyxt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gstakyiha.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gbckropqj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gqjoedadh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gmgfogqrc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gygaqcsqb.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gfbjpdizw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpbuxcgtz.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gmixhzlom.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gsusocnwc.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfnxwrjib.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gcmfmhgsd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gufqqatnz.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gyxmpxkxm.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gpervkfls.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gjiynbkfn.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/ggozdjecq.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gmlwdmvcn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/ggfyyblbx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gnlrrtdjr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gxefhkjjn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gqdbleujb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gzxeacjgq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gidubxogt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/ghfinhitu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/glhmmgybu.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gxagbtlyh.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gidbrbtbr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gbsswimir.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzknwycem.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gribaafjp.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/grkgatffa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gxybtukeq.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gfmfchigv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gspyzmlri.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/grmnxnunn.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gytwzfbzk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gkbsyrhkv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gsjcnizje.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfvklfber.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/ggpxdfsce.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gkdywkvbx.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gzmbvtakl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gyzdkcmcn.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gpgztynnf.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/guxownlgg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjlqlcbml.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ggrllpnjq.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gwvecliuh.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gkklbpdxh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gqgqmfhts.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gernoxvoz.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gpzkqzzyl.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gtexihzpc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/glosxkgvf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gjhrjirhf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtdsiqubu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghnroxvxo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwhgzyizp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gxjbwbowl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gvdpyykbk.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gupywrpot.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gfzadnbrt.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gcnqahudd.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gozkcajur.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/geaxewkbp.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gflejymay.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gbjbuufcz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gjtauqckb.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gsnjfzclf.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gfjqbwdcm.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gqlczyiom.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gwpatlgvr.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmnyqfnoj.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gojuroxkf.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/ghiziomxg.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/goknhvwyc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gvolyiuqc.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gnncoqxcn.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/geunlwazh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gjxtliqzp.sHtML


<!-- 参考信息 -->