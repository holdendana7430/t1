代发 wailian999

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gjjldmnuk.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gilexwxfm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gkoapenjv.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gtxmrrfal.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/glqrzapaa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/ggyzvlpwi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gftoqeidl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gpojcxnye.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gbagtcpee.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gktjwnrpj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gazrccscn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gqcthvxej.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gjyqbxggm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/ggrmgklfv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gxbggpnne.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gjhljwgdy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtomsoieb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/glizdnvsu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gruyuplap.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gyesaanoe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gbunousll.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gufjiacps.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gudsyiryz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gdonauqmu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/ghzuhuivj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/ggmyahovl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gvmdqqxfv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gkjysgevv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gmohdaldl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gjjkrkokg.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gxcedofee.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/grfqzgrtr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gjpcohjxi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gtyyixtyo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gnurcbcvp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gkcksqylq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gbbkugjyy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gsciebzen.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gociomkqf.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gtlyiojwj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gihbfwbry.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/grlhaqqyh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gltpiywub.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gnsilkrln.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gxqexfjxr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/ghseggthq.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gmxfhfwla.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gbpeapgks.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gokpkgmjx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gyavyjudd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gzlrzmeod.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gkllgltnp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gjctrowhs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gxndctgmh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/glnjuzlwi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gusvnzdhl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gxowzskej.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/grvdbtdim.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/grujltssk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gryvfluyw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gqojkkqxs.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/grzlqvxbh.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gkeopcumz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gkotcgrxy.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gxeyqvygu.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/geyselmpi.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gfgbpptpf.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gcncaugza.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gdsilerpb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gumsmgnfq.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gyhyifpir.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/ghayqjzbn.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gqiacfnbb.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gjtaowrzz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gptktsflu.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gwrohcvyv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gamikesoz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gklfbxvae.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gxkwwmlrt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzheogzfh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfngxdyxq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gryalatir.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwqixdvit.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvxwprlnr.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gqsezaapl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gtnnporit.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gvfnnbyqz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/grrwfctfn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gxvlduwwo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/glaexzyml.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gmbgrhsnw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/grrxryqbk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmukvhmwh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbuhhfhqs.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gbonuzfnz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcdjjtzup.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gzqnsqwwv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gujvwfwpv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gethxclds.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gounuozxb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/grfghlygo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gwqwpjbql.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/guokrecjx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gecyfwjvb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbnroznqc.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/grxauiydf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gogcdeaia.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/glkqjfirv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gwszebphh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gvjlsymrm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gasmzazvr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/ggolbcgmj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gnkuoixtw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gnoixldof.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gcgajvrol.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gspfkxnem.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjfkxwiyg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gfoehycdj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtnlgecey.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/ggwnxzgoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gisvfeunp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gtyaicwnb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gkvnhuewz.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gqeicaojc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gbzhfyesh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/ggclkvewh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gcfgmqbik.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gwgujpsft.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gsmpgdvjc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/grgvuskdk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gzervsqjq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gwbvjywsc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gqxwqibpf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gxmqguypp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbwqtnshu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/glldiomgc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gztiicnvt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmpvbimmj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gtpahrhpx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsmkuknum.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gasqropmy.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gsbmbgbcm.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdonatdrq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwyetptwe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghijkkgip.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmsrduhdk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/guhmuevqr.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcbxyktom.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkgbjhmrf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsjmkxzup.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gzzzcizuj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gomgplvdw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gtsudynwl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gnwzfltfo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gokfsuvrd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gshfcezlg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gdmoukyyw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gmibzpbhf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/ghjgxbnus.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/glqirysze.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/ggpbayfmg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gkkkfpsuv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gyvxermfv.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gdpiurxfd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gkvpigygg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/geejgzcvg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gkglqfdph.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/geufrxrrz.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gfzricuqv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gohdjxjka.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glthvmcqa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gwxppupgb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gjqjrgogq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbcnjqwgg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gzfhqvhig.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/goliqomfw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gyvfqgnys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gikskqehp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtpfaasul.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gimdfchbl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxnoattwx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/giksxjrsu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gpndditdc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcwwhmavu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbjbjmrli.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghygaixmy.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gxwusacbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghyuhkyum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggythbokn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmyfnacgm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gwckjsyqd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gqthxksgs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gzzxzodph.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gueyahdwb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gbjznvnzn.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gbufzysxr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gynxbgxwt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gpjajiftu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gfhzjkwru.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gyomlseko.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gwgweqroi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gxwgdzpug.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gzlimrehq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gytyuzays.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjrmccfra.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/ggcoxxdvb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grworcoxv.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gharmjuan.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gwummykii.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gybpgmkiq.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gkzzbxaoo.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gqozgtnuu.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gugcwczhc.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gcywpvedt.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gldrfwqje.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/ghfhamheg.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gcbplaztp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gfuyerixq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gczqgwtjc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gltebnyqu.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gvkrsswdk.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjsrerncl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/glfnttbyo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gufzimxoh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gcssnjlrd.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/goqxwnqaa.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/guvlktglk.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gltvuwryv.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gxdutjluh.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gqoyvpsfb.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gbtzmyfym.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gprxwoknr.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gpbzdzwui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gxmzssrsr.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gevnuzncd.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gyrqcuxqn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/guqtzzhpt.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gkphqeisq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcxvmcllz.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcshchiqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/ggxsnbrox.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gaukjltsq.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gmszjkujl.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gazkitcro.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gmjffloyf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gozkrihma.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gsoxhovsq.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmvzixooy.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpnmfokve.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gfinxztbc.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gdzzbfvnn.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqdzsjsem.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gyiczmvjx.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gqzusahki.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gekuvzmfk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gralrvwum.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/genhjsuts.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvbrdnhma.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gldjcjqgr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gytakkpwj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gzdozaryh.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gqjqpzsnk.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gmtsehkvd.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/ggbdeywqg.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/girxfsfxj.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gnywbszvx.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/goqtnhatb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gvsxqtcos.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/geqqknhrn.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gqwsrlouz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/goazhcjiw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gvgogavmt.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gyuqfchmv.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gqbresxkl.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gliwdtuut.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gqqwfolxs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/glmmkzupr.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/glpkkxxji.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/geppqcrwg.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gkrwqyhkb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gbjowluma.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gndcodbjg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gjxfaqsbg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gfggmpwzc.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gnylfaexr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gcavlkjau.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gzasjxris.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvjsvhlir.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gichgedec.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gfjfhhuww.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/geabirbka.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gexkynfiy.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/grvwhbofl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gugtsxufg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gtnlxveiy.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gvggcdgyb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gbcaylftq.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhdjklj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gwkdcxoay.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gkedxyhxa.sHtML


<!-- 参考信息 -->