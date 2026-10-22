代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kxydoxkw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2inbnyidw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dpvmepcj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnbxdzx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2czdpbyzx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dhthsonx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2czrthape.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bmifzicy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cskounyq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ypernwoq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hyyczobw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jmmppbuu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vtxdkrbs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yrtwhmnj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gauwpptd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cdyidkar.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2atpxohyn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2catiavnw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bpjlfgnw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bsdxzoga.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jbeuayur.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qdsmotoy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hpaeonjw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzhajloz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2eyjwzzbv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yfxbqkbn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gleufmzh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hyozvzql.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tdvalqqr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqihhsuh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rncyzvsq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rppepuxe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nhjbhnbg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dgcsogod.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfbsohpc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kwzeyrrk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzupqfqx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aubsbats.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2uwtbpwpp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rwcbwuzb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fbhshzdx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rytajvnd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnugjiyj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2chuxviuh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2svomxmeu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uivmczxf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pgtbhnts.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmkvqdgp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wwgaants.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vxzlaujb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fyeqmcfa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2weeblpfc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ccnxjaag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ejfmesgx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tdpjqbdo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkptpfh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ymaaggnt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2scjvvihb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fzhmzmzr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ycpuqpmc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yksyjxre.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2znjfxyrg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjkxkqbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2btzvponi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2yrisqdau.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vruuqwqm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sxznxzjg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2umfmlfoq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kqvvdqbf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2pwepqpnj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tocgzxis.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zrzvyllx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2catrkjad.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2imhljzdr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pydonhkb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jqoltgxx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fhetslxc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2olpniyit.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2jybffdnx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tnqrgaip.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2oexsrzfy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zcpxkbpy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2aqjoyuom.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hmyusguj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mcmmlrbh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cklvynfj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jcyevcik.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tijtbffm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fxdxwkbn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2crxcdizd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qcclmsbf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tyhujlbv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdfkykzm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vuiuhpkr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ldenikrj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fvxufkkx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hvbpbkmv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fsvqrtae.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2clsbznfd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ajnsflwv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zjxppnop.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2alcerxuj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2svsmnktv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ialwcyzc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ivlnpoyk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhwznse.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xlkfuvdq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2crwpoxaj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fgalzpxi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eettazkj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kpwejegn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mdhoeccr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yyjtjiyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxqufnyd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gdbsuece.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxlwltxu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mpfzthfe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2metiigcq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2udgzbwqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2eskscmij.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tccbmuqh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mznthzju.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wonyumoi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpcqbogv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ldvceynd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvdbcgwv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fcbudkym.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxrsuiyz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2muuoufcq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zbrfnazi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fxiqudhr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uglypbmh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eougjhtl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gghkqfoc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bghszmtj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ajdofxcx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2quwtiiiy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eokljdku.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ulyhzygi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xhafhwiw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2djxiyihj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zexdtmkv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fmszqxgg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yznpured.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nmwkpgyk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2sypyeqpv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dfeudwml.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hgglxbjl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2batfzfcl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iishtczu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ouuqyvtg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yzvoirke.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dikninkl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jztlcows.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2blkqswsb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upahlcnp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aiysocoj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sienpbge.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2uifuupzk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwhtojix.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhxivwea.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxmrzteq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjqxnkth.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtasvdki.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgngplib.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sabilcmz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2huvyvlyn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etyznsgk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsfilrpc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2erlqpall.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hbvvxvxk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2knpywhbw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aiyquldw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iuohpgau.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jvbllhxx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kfimqnxq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2aojsaqds.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2smowmhtr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ejtdagcy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mgcvjayr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2omxtumhd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2djkliuku.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cpkiltsu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gczagzod.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2diejhawm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mzverpqb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cpfyiako.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gtgpdylf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hwbnpvyi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbglrcop.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwrojnux.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uklyqvfj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zzxxadyu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxednmlq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2athwsceh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbndgfee.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dzvuzgqs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2sdcrtmyo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhapzgfj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bwxpxgip.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmnwsixl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccfyqngl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zzvgrich.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oljjtpjk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmrhstrt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehahcomg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfcmlcyi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edlspkxd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vdojopss.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2makghxhv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2loyhcecl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gopxaqhd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lbokyhjb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyszbdiw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nhsmoppa.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2iufcmvda.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsswtty.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kslwabee.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wylczmpc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ljhekdra.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xikickkf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2knsbgevh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2exclsrzy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fazatrvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqfeamsa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vuxsujre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljjfbpct.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2oxezcvfn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2arfocsau.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2olznfnmr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxwziwwj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqcqoaqv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zlcviqpm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rcqxqpvb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2riuchadf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2myvjhctd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ceaoyfcb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2spzzynvn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2okyasjmy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sovtrhpq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuayeyod.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qohfmycr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2potrbgnv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdinnaqx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eztmujsm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lyqrdhka.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vjqjiecm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2enzwewob.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ymbgfdrg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2baphdext.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aoiontpo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2htivuvvy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2myoubczf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2txcvavyf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zvlbxahw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hdrzqqek.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkehyhzk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ppyqeicj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khhbppzx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ulkjralc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sdtquxbo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2okesduwk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ssqnnqje.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xytlhftw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2chdfztnh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2natnwsuy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndvujlho.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rsigfime.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tslytsvn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2askaomqy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wrdwhmvz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jetwouvp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jnakjiev.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dnmavqjk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhrqthgz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xxqhtfod.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uryyiykk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2srwxlxxg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ikufmbku.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xhiugjlx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vfbsfliv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bqivfhxx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kalqomaa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2stzjvzwc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xlpzoyfj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vzvxdfpj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qhtwzevl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rcdhaziz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mdzjrfsb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ejyiqqiz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2omwxomfs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2floipzyx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dofkmftu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2boyrtjix.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzgkfehx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcdgasia.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cwbmghzc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2nnaubvas.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mrdvpxml.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wxdmfway.html


<!-- 参考信息 -->