代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tdbbpddf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pmmfezeb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fmmnyabg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfkhorsa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qfhywcnb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hriejeej.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rrjitshw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wndikhra.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2arjztvev.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bmvjgywp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2yonfgwmy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2diorwypm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2umhvbtkp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ilvuailm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uciahbnb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2inxhboyk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lqowgpqd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wbklovdj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tcrkylsh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwcqnyn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyuqfbwl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ltoptorg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2whrxdyvy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tyslwews.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2evgcpvhv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wbkztnvm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ulbydbui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pipgzfwr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qujvmurc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pzvtmaea.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oxawmbet.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kaxxmaat.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yizmeadc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tneyvdui.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2owdfpvvk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ucgvvotx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhigtzx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pqolsufs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2harzvgiu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2aydvflny.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2elhmpsvp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jhdtzqul.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2svyfmigk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hrnfdbro.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hvtoikjt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uemmvkez.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qmzwdada.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nmoxbihs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tlvaobwu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gtoustvn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wbhmsjza.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nsdivtsl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpfugpt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ckpucpmp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gxbjxrbm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2utnbrlwm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2prfttkzj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hcdzcwld.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qkrimeab.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ryzvastj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2sdwzqepv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zydkgfww.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ilykcxgx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fldiyjyb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpvzjwsw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2euxqykan.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ovpdonod.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nubojrre.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hdggeigg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dzwojezk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2grbrwlmw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zboerpfg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gwipxsgk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ouxmhetg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qyqwffum.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2agrzsonr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pehypmoj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbhfjfk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ycsdkwtn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kevtiaie.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vhuteyip.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tvqlotqm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zqldpfet.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wpvjkubf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uyqfjmme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzzlaoqe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zmbrhzkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxiljery.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pycodcsv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nuywtfyg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fxuatkgk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2naaqkpey.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rsxcdnfh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aycpbqee.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2iyzjhnmz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fnerrxut.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qeuxbpbv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xoilafoy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qzapguhu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmzvscey.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2umchwujl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dntsnzcj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdbewty.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qbevtljc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wwlnunpy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vxhkhjio.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dvgjruse.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2svdygktl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iyhkdfmb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lnssuxql.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2drmpfoql.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tkygafvb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqehopc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2sujucssl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cbzsraxx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2incvtbre.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zfnrppop.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2uerlycsf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2obhsgtxw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rqnjxtxw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2auzkeykd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wimdqkpb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2sbstshwt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2plnshnva.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wwjihamb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cynhpgfa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cfxzvjvw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwgjkxdy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zawxfuyz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ypmldkna.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jsrbnzzw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpgheifx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2davuiwqd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vxmgslmw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oahfiuju.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gagzbgvt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhbbtdot.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgeckwhq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fhiodkmj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qaqvkqlv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eaqhmrnu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wglwgelb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2siudeuye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rbcbrxse.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vccymuel.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tixemxzz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iyxvbbpr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wptssjoj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2txmpfdgd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eljvdqve.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wbecbaqb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qvgmazin.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixxwaylw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dphtdpqr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hpitvjbu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qoruljrs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vbsfpyzt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jluacjil.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rythrvcd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zwteehcb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tdwjlitc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2caitjxlb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yaimmldw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ronusuvx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sdcxuyxj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wvjfdjdp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lpzxxfvn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aexcqjhd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2njqmaeox.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ydqokdth.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgoooutv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2alhhgmfz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qznricna.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nphlgaod.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bjrgasoo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trkwsunp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxiddfou.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdllckfq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2izvyyiig.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmnoywtd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wkayiaaq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsinndkq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxsaxrck.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mbnpfubg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qhpvpstu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yffmkskz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rpanygcl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zjqznyde.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnpwcgc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2cqvikwgg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jkhzxors.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bbfsokdt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2upxjuove.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kpfozqeh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tiwgvfqe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xcsuiaza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmzjphgj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ndqwprsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zllkyjkn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ygkinyay.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kytzidoy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rvtscslb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2feclkelw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nfavgbgn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zjeiaies.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uyqkexbe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rgioljzx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cqdyaene.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xusltrfa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2odvojsyl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gbsnatpz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eiwuaisg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krtptrqy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wprcxveh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nmhmisyo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vkpahelv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dsnutanz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rxorsnir.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ttczgfgh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2omtsnzuy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qktehoru.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qbwznfqz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zhgornoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vvjafiys.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ngozgnkw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gnfifhkh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vvtyoidg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hkkmoohk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2derfalnv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcyvfcna.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lruhmtba.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbbenfbw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hslfokga.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lcicdvir.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xeyrxahw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xliemvyd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2okmbllhe.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uuvmzrzw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dyldxrlu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfxliedn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jalgprhc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ooadwiit.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jryqdyrl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wvfzpyta.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2edtozsdc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rxskycko.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rommsuib.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ppinyvns.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pqlzdosc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbotxazt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xrspnljm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezfahobx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2apznihos.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ogslrkmv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hmqfavwe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tkcttpde.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tcxfsgzz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2drvibned.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2amixbxxg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ejnucfcs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2nsexypuk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yqmxudgn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cfknwmji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vbkivlrx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tdjiogrj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xevysufu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lwwyaosm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpoowusl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jhwzocgt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qsqaiqeh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tqcgchoq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wlaqyzxr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2esxczsmh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nbmfkrrw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mxuvnuzt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2batybewn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jyrwckij.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xuaggdkn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qspvldre.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxkegrcw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2aguravnk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2etfkvnim.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2olrypzuu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zxykkqhp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zztxcfck.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jqughjti.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wknfmpgt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ugxyncte.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hjiwnhgz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vychnggw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tszczinb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qkllwsbb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvyxnqou.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcaehsew.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2owranunl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2thjxybjv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tbgamnwo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuqzzyar.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lztbklqz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xuewxvdq.html


<!-- 参考信息 -->