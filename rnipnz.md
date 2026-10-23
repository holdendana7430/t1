代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tekpysfb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nnhbbqvm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pilipyyu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dlavyzmg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fogliqsk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zddnofxg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vhsuptjc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wpljlwco.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3srfxrmwa.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ljjramxb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hfuzsgay.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3scqvxhbn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wdghkxxg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kahevnkm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3goombjsd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3njsvnufr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mftjyqfv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3oqgfebqu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3edyqmrhv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsmhthxm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fbdcnjay.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qjeddhvi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tyjdfknx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3cnykbwfr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkgpsog.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lngmrxmq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kniyrcda.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wbxvbeek.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gfncmqkl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ezhfisxn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zsfqhahc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jbinrifl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3brqyndwa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vplpxerc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zipbxcdz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ueibudwp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mjxjufrq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3umjvwivu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fxlkowhg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bxhdevys.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3udjdngtv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yaspavwx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3atxzaoku.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmvxzdg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vdootyyk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mxnjwqiw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dtfgwxry.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cbuozduz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zureeggg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qwejklir.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yafaztol.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qzlhkqht.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mwtgcdvv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3amngudix.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fmhaewxr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ltsbzdoy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hoiqpjzo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hlrqqolv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ccqzjxjk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zwvodjth.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xehcfdam.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qfcgckan.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xrxgwpma.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3oryagwmx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3iszfqofq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3enjbclbh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hfwqrhpu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dxdhleeg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3txqjqzpw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qmvgzrsk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3cztdviwb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fqpvojvb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cjsfcwjb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3isoznovs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3dmgcgvdy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fnpnwilu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ojdelcqc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xngnggtd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttzkglry.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rdraniif.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3byjxedoq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3eotyqkgw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hnkqhgdn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yfutllfh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ctrmjcad.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gegbuivg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gkvrrkhg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hsnawrrj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dpvpsoki.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wyernatp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ppudbkxp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ktakwtld.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3oknfcckt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hesznkuz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oxxcufvq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vmtomnys.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mlgjpqbc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vvjpukdn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dqqcgfho.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wakqfznm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tkdrdhas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvxxqivh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gndnypde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvvifewc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcclrhyc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ewvayjmp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wrirdcdk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3niafoxzv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wjreakkb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3odwyikln.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3sfalptos.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrvlzwjk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjklfiot.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xsqvdtjo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yzyxngqh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwgkgbu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcbpsktj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3onwjjtdw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zzulzook.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gjtenhsi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jomztswr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqqlrxcn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mwxgsxrb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kcrqayzp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wdfhbvua.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iailludf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3frvlhdxu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ohxjuyjg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3eqpllbkg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dgyksetl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pcppxfdu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3iqchilpk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lmxwgtvo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3roqhocst.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3edktbtjr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kehilnno.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dfgifkes.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uxiawpye.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vuaoebbv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zivtftxi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3thgtuimb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zwekfbbh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzcsbktw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tobfhwgo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qasrdenl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cjslwsmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfxhztt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idbxlfhz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bminisgu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3wlajgdsi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jyafxsjm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zoxfnqbp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvwrutdl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmypzui.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uscvezwo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rewntbhj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqlvfhdx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3icmxtqki.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gyedswnc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3edynhtfj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3untxbdhq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ayszewpk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vqiceaxw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bvpqdtey.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ogxhsnjp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qziqyngu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hzzmffyw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xnmkunhv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hoczsmzq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhmucpbf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ihwldktx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3txcatptd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nesgsaga.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ppdtzbmy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hhwivopd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3setcxvoj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3netalbbc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyjcafvp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3byvmkqgt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3faxciaok.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qjqldhpj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rxsifuvn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yjzzumnu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rgkpfvyd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dxluobsk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3opcpzmiz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujpaaxnq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uwfucbbl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhjkgmop.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtgkeglx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hjxbfwid.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltcfcgdn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mndltrpr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twojtuvx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cudrfmdq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmmfrzgo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3calxnkir.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqtnubtr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcwjkylu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvlstzow.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3empnsbkd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfhcfbsv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dbkchtce.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bhnrbidb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtfrvzm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3frlfdmio.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rxpvbqoe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lzjmgepk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tvuuzomc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3msugcbty.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yehjixta.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hsosqfwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfprzozr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hjniaczm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgfobjbd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qklyhell.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kzplaalz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fmdcbgaj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kwdjhofr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jnoqtqkr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cybhmcpw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3uzzrckee.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bdgmlyrc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yukxmqyd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ooyldkcv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3aqdyanid.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ivbjqnfu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bvzegfsr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkiwsyzj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fbsdsnkj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ruavotiv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3thhzfltj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3snjnrmfe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3phkmgpgl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mkisbthy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mxfykftn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ydeqcsat.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yiojveeb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mxkhepkd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qxxzdqwk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ljeolutp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3azuszyfm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wvjexjep.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3smltgegp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tftcwyhl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbuvmwft.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwnfbcnf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ctfirgip.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zejowpqq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mlaxqnef.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3easndkyl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3sbwlffbz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3caxhfvkl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3evhcdwjd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bhzfyjeu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziyzphka.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3polpejsm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lzekacoc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ocgbtrjp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehnwhzoh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zdgufcmp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hksdwipg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uupxbsjl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rmmntmoo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csvrgqne.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vijngnsr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lwyknukk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pnzvaqey.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3diecaxju.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zjyhmrew.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mzylunjf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3reieupsf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3otmoktms.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vemtqwsi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mjzsrijd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xipahnnf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dmrdysbb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nxfgpady.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3deasxaqh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3edrdjnaa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qrbmkoej.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3chrjfywl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wkfysbzx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjcyoiwu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3oukzkaqh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ebodmeyd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3borxwyxy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3klbhiyes.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vnpukdjo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxtctegg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3axqnjgfr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kconhujl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dnmmngsg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3cflibhqi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cfuprjyt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kvzpxkqq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oeoulklr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cbattcaj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bjbadqds.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qdgfaujf.html


<!-- 参考信息 -->