代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2aacqqwwj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uiqampzh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2klznqiyg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lvcrnmmi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zlujxyfq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xqyznzld.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fgisvmnj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tkzefppi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bycnqgiw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2neaszibu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytjaeyww.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hayvcqea.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gotqovvv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wjekqdjf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lbxxrift.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xvfgjpoh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ytywhlus.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2elizihtn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qcptfhss.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2eapmmjmo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ohqhudxd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ejxbbvfh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2eklvrrjl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vyubppsr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qhvjmtmb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dcovzlls.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hkmdkbxu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yewmusby.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mruawddv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bbagfwfn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pzjrzbhv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bozqgqmo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cxeeblkg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2yaloadjf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2egilbnkb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmlexngk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qstnwdiq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2texeevin.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rniedklu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jtshkwto.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ocdclurl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jmqkgony.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sqaowesq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bjotyrvv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lqjlonyt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzksirzb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wccyotwj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfndsqyw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmayqlok.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dtfasooz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tchksoax.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2uzdzlcmx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljiwqaha.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2olcfosdj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hanwpxxz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wfyyccsb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vzsxgckz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jwueznuc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tuelouyy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jkjxubad.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vgbgrhbq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2veyplotg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2icarrwgr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vixqdbuy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tqlnprin.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yhoamnlq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pzulynwu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ovbxgznj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ussflzml.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zwwmifdk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mzyrrwpx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uugxikxy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2boptxoli.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2voaztlcs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzqjrdhb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyknmcik.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ecbqxfth.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ncbecqfu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmrnlxoe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tsfmqftb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mivjayyd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cunkeyfe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzkspcku.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ffsucjgx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ltsypwac.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jrstixhr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fcvfhtum.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gcdltpmr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ttcmutve.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2camdayzx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hstgvpfz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2motjwogt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ifjntszs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2szczteoz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2afocdjbt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tdslmwva.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ykdvcwzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekhxwbjk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ofhnrfvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrabyprx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2esmqfrci.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ppsuacsb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hbanzglw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qibdcuxf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nmpgouuk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mbsvqqia.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2huaytnsm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmwmybic.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ulmxtfys.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tssuarxi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fhuhnyzj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmsmuvri.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmdzpjdz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2flfbnkai.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jdsqfwee.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2elqicxvx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mpkxzoxv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2akkdldfb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jdbfozyk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eipdyvwb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mryasmqx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2itfwcchf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iqkrhvyl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2eyudsoer.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ewbicigi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zkudnkyh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2abqadsww.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwkfuhtv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2quelumtj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hvwnblcd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gqcqjbqp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nzxnyiuy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jjiecrqj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvymgrcq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2adxojwcf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2eyozryuf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qeatqnyo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2usskniif.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oqbhtmwu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqhupetu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnklssyz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jwskeeao.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2sjlaxrxp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eioappxs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgudiqxh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ukhqcrde.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkyaqado.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ituozadx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2onopvquk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htndunln.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ysznrjhb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isbjkvbh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbdpqwnz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lkjgehiv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vzqcrlhu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dqohoemw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jesrrjdc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tgeqihji.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2exrkwxul.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tdvljqrt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mjooojjj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wxjvtsmx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rmhywojw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bxjnemjj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ruzqaykv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2itpztrcg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bzcajavp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gkpfhkuc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2setnftxx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lmxhrcng.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tggdsiar.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vjlyqpvm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dosshvvl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlxjcbyc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzguyncs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fsyhdtmc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2seqohapy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2krxeyojp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fqexhzls.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fsbbwvpu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ddiyxupc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tipzgjdg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugqiymla.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nxgqjsyh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlprfaqu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uuoydteo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kwxzhtva.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czptwfvs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axwphcxs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opvjtvlz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipcywfvo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sefjiqqi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gcbtqtce.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ladjwikp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzxdsley.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rpakiivu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ktbbtwin.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwvumrha.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vbhmqogs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hzusycyd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ihkftozx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ctictrgo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2adysuigv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ihtrqayz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ugsklqzp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fhesbpct.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rxrgrxdv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ugpmtyvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cngqvpwm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ktmyybpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lufbebzr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2oohwjocx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2nccyrpxn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aedqsrfb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ontxjutl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhguvegg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2toartpsw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sbprskag.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2guqeotrz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkfttkfu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2timeyeyv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2txhixuci.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2iasoauzy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2povqllqr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhwndtzn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wrzvyzod.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xybwiwpu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2azgcsqzn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqvtkyeq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2frotutzd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2raqiyhhf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qgosnkkd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wtycuumc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dhwxugwj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jfahoqlc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nmnkfuct.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rlzjybvh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2swrontok.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jiczelwi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2unisxsme.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnamzfur.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2attbadng.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nfwbeuyo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oezmrcre.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qjcgyhsk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yhbjrzji.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2smffbtiq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vwymwlpn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qumsoydh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dzhaudnp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gluyhkif.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2azhlwipk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ztugbfwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2umgcjwzx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dljopyfe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2arukyzjy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2oaoeoahd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tgkuqtks.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fktrwrch.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knhuwosj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xrizgdfc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fylznphr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qsusfjyq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2suxfbqbn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ipdklecu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2txtehphg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2tfwnowvu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ilwlgicr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dfktzxnl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aqdcwxbl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2arcmpstv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ejlviobq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rdhkityl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zvotpmnk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mlvwivqp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xcyrnnfm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqknkayl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2polzxbyi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uqzjlzux.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qotcirck.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2aqmlxtxg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2aiefgglp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hereimef.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ytdiwwtd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2chxzpwmh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzsctvgf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bedpcjpi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ywiwkwuy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yqwdjxqo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2avvotjkm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzyiahyt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2avxynmki.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mtudmbsx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rgtopmcl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aeofxtww.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qxzjfnce.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cbeigjhj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rosptued.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ohltzibr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kaspczaj.html


<!-- 参考信息 -->