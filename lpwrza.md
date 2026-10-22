代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qoaaebnl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2avgdraon.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fgtquyzn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jaszvvor.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lhmcfswb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xmxkjawx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zaqllskc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2szegbxhz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mgusyvme.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hrfidutx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ppxfspaq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yluzwaam.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2smnmincs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ezeujilb.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2utbtlhus.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qklsxmdf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ddsuqjga.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fkvlcxto.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2olfpgqhp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2eeptbjxn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mmkzpuih.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ulxqispm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mazhazdw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcjkykxs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmrjylfx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kovteibw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gzzsrvbs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nasixgpa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mjlnpven.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dnvcqqaj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2axdulifi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2oabtszpc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqztvaey.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dimftejd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zynwpzcc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ylornqxp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgjpduc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fmoxrdpl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2msnsgdkn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbzkpgw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfzamln.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jfleckgo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qnbtbaye.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2valiishr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgsarne.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynvvnwuv.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2whpxsbvk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sblgrtbd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sddaxlab.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pqzjhwct.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yyxacffz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bbzndfsp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2aaiqoroi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xypovxrk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pinocyhx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2oxmjsxgc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ngxmmtlt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bldyariu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2miwriuzf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fitdsfef.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksozhmad.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hnjqvsao.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hrfojoys.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tkqnkmgv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2qewccwhp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zwjhcvyl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2plnmuxtu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vimwebwn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqplwss.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nyyshrxo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ouvmhdym.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2alarqwiz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xunkiqcn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ougxvupk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2scgyxfyk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xfgkdhne.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bouwctun.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yiiegpvh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hmqxvdoc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tqoyznpa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2indkangw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2sptztyjr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vcmycytu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xabogoxb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2oesqspre.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rwxnjlzh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjgrkglf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bymapniv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2yszavors.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bxvekemj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wkoysvmn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ubftxofq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bjnvjzvj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tdbnjkkh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aojlxxbm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cnljrbvj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2czxgzcfv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2udssuvtu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2adpjrzuc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vjgurttx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2orqdpndj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2myuajbde.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hronlzku.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xmkndzgd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rrpcphmo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yiqluiuj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2migwhlwk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jbfhwcfl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2abikjpym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oiqsdljh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wimnphjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yiqtqsol.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uamlkfvt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hrgitisl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tfslorqv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ebtfligx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2elsjgukt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqtvlgak.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zhdibjwo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmrfhyws.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqlpblql.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngrnkkrb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2adpphmgu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tmflkcfw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mqypimje.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbmpkeyz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ndwhbtnc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rewjvuqz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sriheixi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmkzzslw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hqyeuvha.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sxkzbkbp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pmhjzlbp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vjbkatib.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qaoztawn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yzzrrkyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcuzusg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dxwacnnn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxnuxg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wttirkyu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2caxixbhj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qbnimwln.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tpmejthu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2urfxwvjr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hywfxflx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vrkalhrq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fzxbuish.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xxxjwrgb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fiqkiour.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2silbkjkr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wkyscmoq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryffgmjq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcsotmwy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ihbehjyb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jspmitcq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptibgkvq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvuemig.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lyihjtaa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npfuyyyb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2khyujgka.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pliplstb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqkrtgph.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvromgwk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2glbzcdzz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wiivuggy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhkfqmay.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mczysrpn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvexjeg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2paieybxd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fmcmcgjt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pdcbolor.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mpreyfts.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2poxfqfhr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2odbkdwsd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ycckodwn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mcdhfizg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vxtyqdxj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gmyhqwwf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pmvumrdx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sxfqwgni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2klykakso.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cvzbgfys.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ucnapanu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dpmxghhq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fidzauyg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejznavgz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlycshwb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rxzfjmiy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nuxwuntr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2myxvqpml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wxxgvqyi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcvanuui.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xfyrmkac.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2apzfvlbk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxecegxr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhtjkcti.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bytqyfgl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khnmezet.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2yiyroxnu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctbuwnep.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2caglgqji.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrcsazla.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yvqxfmoi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzejcnjr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aimyasii.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xffrjwuc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tehqmloh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mypfeaic.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2obtfeonp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qelvdnym.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzmnaw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rpzvppoh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2teqpcdmy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rbmsadpg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2oogculkf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nuijequn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tclhlqyv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bipjvsff.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zjwqgleu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2cxcentvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdrjyblb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2suwyaaqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpbzrlxk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hufehvny.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gqznmrik.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xshkmlng.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikbqxxaw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2wmlszbox.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2macqasyi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hvdrqfbt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fksajynv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmetoomw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2elhxuqlr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ifhbatip.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2efekumsy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xiskwbyf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhcyypee.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jzvzweti.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sxnbzbam.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mjkeyfuc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fxvtqmzf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2peipqkic.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fekpznow.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2beclmuan.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lrukvsar.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gwzanbgu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zpuhodbu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rndhbehg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wdczfbve.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mfvowpdg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bbayrxvg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wtnyzppe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2biatdpre.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhzhfmo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ojznkqui.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeoxbcjb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wcdirchy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lrwwclil.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rttrowmq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2epcdqlmc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bnwandcr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cwpwdigx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hxnztgtd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnrngprd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rumkfqob.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ymlcmecs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2drhwdcim.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lftoxbty.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2aedhaodf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2azdrzfgs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mgspygwg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zphbzoud.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pmbyfajo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2frhdgwuo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lprfboea.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mrlzbwdh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hpqkgtoc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bzqdqdky.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dxjjwihb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xfupuzez.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umyygter.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2purqfocp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ibpmvkaj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rawlxxtq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sbouhpww.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mvcfxzvw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wrmymtym.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jcokiuaj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhrzympr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywrzphgu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hcqmlgxj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bhlnqcfh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vkiwfvzx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2arhpxkpb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojxxyeqe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tuekgoeo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zvwplwuw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bhuiyqbq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vvarpssm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxihzzhm.html


<!-- 参考信息 -->