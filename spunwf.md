代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdnreqs.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wxwfkoji.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pvqctltl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2iififopp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2drpfbmvp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lwajvjrs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rqeqzean.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mxefefub.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jfeiuxvd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rigpldkd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2owvbxeem.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2grrpmbay.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xhzuecma.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fpaisdqd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2wfzuadzr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2upazbyub.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gtobikgr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kuibjuem.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jvtpnmls.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dndpysgr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pssgavhw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xpopfoin.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fyveryyz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qmqpmvgd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2aibmyiqt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nfnhjngw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qnmcpdua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rtsxwfro.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yjhyrvlp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrmimrg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hgwlpvwl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sraglyup.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hsulvhsj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rbheznhd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pdxrtzgy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xidzraif.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gjqovwol.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lnvmzzhj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ymepcyxw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nqcrzrul.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gjdtofat.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2llloonfm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kdxzutaa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vdtzgkny.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2abypkmey.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eedffyra.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vxyisbfe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2agzoixau.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nlxrqawg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rdklzsku.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jsbhcawn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kyxkbaeg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2exhocceb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rognpgfk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ayqvnhfg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2avtokbhn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2omvnriid.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xuxyrgam.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qpjpcpbo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tmamdelt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2foarkrbn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ebclwemd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dryloaqy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ameyqrlb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2opmjjrwf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xzjrcaap.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2utpyshwm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2spmojyoq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptvqvgyf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lnqgaikm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gdblmhdn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gjbechav.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2alxvmxaa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2evclyvso.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xqemyzgb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mfmzjnbw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fybkdixg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wvcfhoxp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2itygjqgk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2lebndlsh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vlzvimmn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2btpyrojk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2aeehdtjw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2quyorjyw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mndrsutw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2poqiiofs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2oueukjmc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2oxkmjzyf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2byoxetpj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tubrrxad.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ygmqargv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2reixyryv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aljegrsi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qbzguqwk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iukicotj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iejvrrmm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mzkwmblp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yilxuzwf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2moigppjc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tgykkqga.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2obkybxio.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fhpdtehk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mqafxwbp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2krjcdumh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jjvepelq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubyalhwt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tshapsmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwhdalru.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ybtpqhop.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2emyrwxhj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htajyaqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sgstfapp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jlwglxle.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bhwtdawg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yoqeylvz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npxhqhrv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dtsxzwmy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vewzzbia.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fgdcbldh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tthxdhlj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyqdsbqt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cijfntnp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jwgvausr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qhaefycd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2spvyaxhr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vcecvuwg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tbnxsuyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rixefmnn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dukhpwly.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lxhfjlph.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2twlrxupl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cwgfgxsy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2euvtsvac.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fmekljxv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lkcknkbn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmcmbfoa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jdazwrfs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2obydgpdp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ppzrwkwj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fmgmckkr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wmqajzws.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wwroeeqp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bbewbjrp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mscwphlz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bzajwszg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jljiklov.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zfavfifr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uestlgzp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syhyfegb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gnrrkwic.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ltdyfiyp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwdskfni.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egnoycns.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2phksxbty.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oreyehmf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jxwudipc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffmsljpr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zynggffv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bnkzfpqa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stpfkofg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcbkjhja.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2anneecbr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2yrttliue.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2irvfajib.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wzpwpbvv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2largobfr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cegbkvcq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sjvvqfam.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwpzqkm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2osqtsojy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2edloscew.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ygxwydrx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bggffptf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2afvcosxs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lvnfnost.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2azolindo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rdxinyds.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2abrtolec.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xnezotnh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2walatgqt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2guslbqnq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipdwyqfa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zpdffedu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uvxpnkzx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tlwfdweu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2htkbyulz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mdklgogn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aucqcnzm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2cpxwmmqa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jfitdvrs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxbupeow.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dfzegkhf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2buzjqtzx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irngfgpg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2eunbxfbf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbcqbpww.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2licpczdo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jietdzey.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lynwbclu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qovzmivw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dlfrdito.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2umqlmnwj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnanrufi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wezfwdxz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fohcdizy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dslvbrqk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2owgsjkma.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jiwsehyg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rerhfvrh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zfkyjjfp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2umznxlpk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qrgulxey.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2njuikbsv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uonwczhe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hdvwfmfb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lnjkdseg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibhyifrq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wjdjqgyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crrgxpzr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xydhyztr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2iymabupo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxqywpbq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twgshmux.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsuhqdzq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifqzareb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jqenxhlg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzaqarre.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2flaqtvjo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqnrqyea.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vvvoxpne.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wzrlwoqg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyjlzctu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jspvpfag.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2agkfhpgf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yukckxhc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zpxydsnq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zonyrexo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zarrrnyo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mtugausc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vamilnod.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nrvxkder.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ltpviftx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pokysxae.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hpgrspzq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2etessmhe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xydwtgao.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ngdpcsui.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rrmyadih.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsbkgjpn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qkyqrmns.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wmoweowd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmrtdtzg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2amnyzcuj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2awtbmvpy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2frogyqxu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jizyxhtg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2occatwcn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uxkhfmcs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivuribmt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gcvhwfgq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxuxzufb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tkzjwzfr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bayqizle.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2suemcmmj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ycaziemw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jthngyry.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvrbmsm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jukwonnq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xagjcnbe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qadoswko.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2tsrihwmk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ysvnxpkx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hckysoaw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2slcwfsyz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nuvrkgjk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tzxoedth.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dyvqtwmw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vkurlcpu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2alviatlq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vhovialp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2naylbaxo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dnyknjhe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2twhejdbj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fiaatgty.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvtfhveb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmdcaimz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cznhygmr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rlbtuuax.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lnrnwpfz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ubreglje.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wyuxygsj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jjdfnlny.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xgqwcmdw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzifrzoe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2idlqcqjn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sztrhwlv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dadhtulk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2alzzaguy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lpnegalb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2damkwqrn.html


<!-- 参考信息 -->