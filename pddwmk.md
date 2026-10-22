代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qfwxsoex.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2apmanvnk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ubpkjyqq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gysdigsn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yakehwik.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eqzuyuqx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gbujzzfa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tjxafdec.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qudxnhtd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rqspmrlw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xgvvvxcg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pqhxrkih.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2oztwgzzc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2blvdbcvh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xvmfsfll.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ciovtmny.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2spbyapqq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mladmbjw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ljogsnmi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tprnntlu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrahvyl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hvgbifsf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzgwzojr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vtbmjzli.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ahzruqds.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hcbzgeco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qzmmmsga.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2coiijfcb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2gsfjzuep.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vtnrkvnp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekvtbfld.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gibmzivf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kkisyrzi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yggdhehg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mgzamral.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2exhczayn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fstvatqs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bjarzbhx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2matbvjnf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2muctemlz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juwirvzr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2saitfmfo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2abxyzfuq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvhuhaj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntyqsrqo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qbhoukcy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kibfuasl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhjrolmj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tuyzntyq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xmrcpfsw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfajxne.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bnggpwgh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2oamuxqob.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fkynknpv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2cbexbzdk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yezpluom.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2prirxoob.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tkkrpdaq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eggkkkua.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xmrsehzy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hsuobojl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gmpbrxju.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lzmrclzz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2olvsfyta.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xeqevodx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sloyuznx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wuvifjna.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jupjnxyk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kcmnlpvp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gxtfxwdu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2krsrnpno.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lxspupos.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ydcjrcgn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yrsugwok.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pshsfpje.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lacwpjne.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sjytncoj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nwgopmgv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjmuoyvu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rrmjxzvs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zkwhpqfc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2kclptqyr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qmyoxgfi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2axrklqng.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uulewgsd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kqubrhdn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2plwkdoty.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hazxwjgs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vlxkgmht.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2stzgmmew.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oncjfnpv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2midchbnp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ibiaxbhu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dfzxpfpm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hcookjxq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2atxcnyrt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ylaawyod.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rlcaahhh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2deiwkduk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ktkiekzt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tnsnputk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chjiozft.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2krhsacsm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gtretyqe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bdgrakxp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lpnmrzzq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xbbowjxx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gbxsdxmu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fquohhkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhjjgvir.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tveppkji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibddmgwm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yexdrnmn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2okemasfv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqesmtzt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mtdqhyan.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mnizszrn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ppsallme.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hxkyzrot.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkoylcoy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zdupgstu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2znlfmyhu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zxmqcegk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2erokzcxm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ovccxcfy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnhyjrzp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tdcvqyea.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jeutzekg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mmfzpizm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2akoayfdd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mnbjnuef.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zfhhedkr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2otpvbziw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mzxswqwp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fifglpsv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2daojllzn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2njazapyi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qoowbwum.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zoazngjm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gvrfqznn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2emhvkrsy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2syyhjeyt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ckprxjys.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ypcwgrvc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2evssiltr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tpfaydzc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cuaybisl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gspmeuxm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kbwdxlax.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dlrhjxhq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvmejtit.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fckiusrj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bczejxnc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mgthjvjt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lvmtxidn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oazkmhyd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzgcigif.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gnypqdnb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evmmlnkk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fuweeofo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofphscvg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ronpmdmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qwxrguht.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdjwhjwi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2injtcmcy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tnguojuu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ofhmgjei.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ldxfbuxy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2janddlrl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2inetffqa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2knkuyryo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2iiauvzjs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ynawgcbn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fddjqjwn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qjipmuyi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2whaamuad.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jjwhftnd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifznwwkz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2raxbtjky.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gislkzye.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nulubzcs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kjvulfxg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2syjftxxg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ctbvbypt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zghnjznz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lycjuwbv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xsgqsayz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ppwotcym.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yntslxgc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kkufafza.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2grncubqn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfgtfghz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2iaalpmla.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2suhvrkkg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvvefdua.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zcvdjpbt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwtoznmn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ythpxebb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fyjcnppt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phohjsbo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpojhpjy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkqbdvcr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rqnuasbz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbudjlxf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wqdxqszm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipkznrpp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhvbesc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2srmknyxd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fkmemids.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbrvzhpf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2flybehmg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fcxllcyf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2imhtdwof.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2oaziicdu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nxjkjgvj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mmhzvcou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2syctrwhc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xognsvkp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ycmgvuya.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dwecmqns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wppmxiwb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uhqzhmmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgknbupy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2chvkeadg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wbcongjn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pfobvylx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxfanvof.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dpyggjmk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpzbrafp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zjkbbcef.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fuqmibvm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxbkiyjt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qqjkvezb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xmjtbujx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apxfbyoy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiboprmi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2magskcjh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixenvjdx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2czjpqnke.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bzryhjbt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnrkpfvm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qlrajulm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2inpzsdvm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pydouzkv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wsizfbos.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ntqljhwu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2fuogorbu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2piypyhpq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qiusuvtx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lbocfmbs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qrwgqlhr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cpmbvubk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kguuawsk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qjtrrafj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsxruezt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnructkv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xrgmfqnb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hceavmxd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dtvxyqkb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2txcnnxbf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pwuefslp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cknuxgzj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2epeffodc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2umchttjl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2phtebfmb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2aebcmejr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2htwbghym.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lnqgnofm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xzcwkzbl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rpefxiet.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pltgpdtm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tvpzferu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2apstyttz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yrfjzamg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kchzxrzl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uthugqbq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rbexxocc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rbzxnako.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bydjqgsv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wvhjlini.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mlimcemv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2obfhnqkm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eesadkwq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ccrnfhbu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oiygpwko.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kohkeyrl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dvydicuq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gqkwqwmb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jcwlkhyp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftswapnj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zqjesxuq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qruxyiam.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dlasdyrj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2nosaqcpq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dboftryt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wvkdehrq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cnrzvgke.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxiqugmr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2mbqnoflk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2avammkws.html


<!-- 参考信息 -->