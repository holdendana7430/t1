代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ptzgdpjd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qvxfmlqz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vplhuyqe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nbqumadk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fycxpmaj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tyuucorw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2frildohq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tcknpuqo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rkcudngg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2prjwllhm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cpzctmtj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lomdrhaw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jcbjcekc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vqbtvaed.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vfecbxvz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2roldufxw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2srditvtn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pvlihgan.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uugkkgzr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qneyfugx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2seclxiwe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gydebomm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ykpmruur.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jlwcbmcd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rdxjlvwp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lyatwrtw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nbbrxazp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2blyqlsok.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2olfjimhb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dyypqmqb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dtuhiqdb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvodxewv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2wpdvvplg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2teguzqmn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hsulsbce.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bglxyxxg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhhivuoz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bfsfbibh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nqfnrgkv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjeiumwg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wzknnanu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qkjfpdxw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qadbkmpz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2szteeiqw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mfarrodr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2opcxoxoh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uevckzlu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjamljc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kmhrlplp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pvytvuaa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qeobwfmu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqqxwfhl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2edhpenhn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vyuihvkc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2oynclbfz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2buklmocf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2aienkfsm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ykcrxjyg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2buorayra.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lljgehhv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nzbiatbo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndtmixza.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qefhxzco.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gymqjuae.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tscveoyc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wbexsoyz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ywvurtsw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2xrcrpdus.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnuigpeq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zvlsehmr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ywngqlzy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tfayocdd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ojmyiudz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vpcqsocj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2miwqyqef.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ymnnyonv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fvjfkxec.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vrrghhfm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2clncfhwx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dekvgvzz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lhguroih.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xujpqjqb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dsklkgwy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bcbzrhrr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ttascrmf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gtyozwnc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2geivzbko.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qleytddq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tapptnmc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfhkxvdx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2msakbgbp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nusxbsjt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijwmcjwv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fswapwlw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdbtdlge.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bxcehwpo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dehkxlik.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uneryvef.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rkzmqfmy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ztgqmpkg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dctoyefx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kamskibm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2arenswgt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ebgjipix.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2labnuthi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lfmgkgnj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ofgrmyck.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zezdspjz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dyrixyev.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nslthuas.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vdrkusjh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uvhmzntz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yzedxdvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcmhewht.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2saugrpqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2guaegfzi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2oypfhqav.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2avqyuepm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ckqnkprr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2onnsdybs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xitjzifu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xpspoirz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2okbbbbmz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fofdjafx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gzlpzaws.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2nalrhbyn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pmvcepft.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsmntrui.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oauwqytx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lesxogow.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2crwwygcu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ffoudhfy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jcengnac.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkolvnek.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gxtbthfk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zdfmgaoq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bthwymqj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ovnarsal.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cdtewytm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zfuyjefl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2swbgreln.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ocpudqeq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ywqyiltp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltmnrphy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2shxlozbt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ixaldzwu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2clxrzggv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kgugxbnx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nkybkzqj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2edfkylqg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2siwzjczx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jmgtyiho.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lfrqtkxc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2oozqvqdt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqaaydfs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksnhbwbs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mftswiko.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2javijhfu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gxekmckp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aoimqbph.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlvnkgez.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzhkessx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nycriwzi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iatprlzw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ultgygjs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aameknkj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jakusuex.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnlriprt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrjpnxzl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkflvcen.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wwhgiiju.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jjcidxgl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gvrqfduw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xwangrps.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wwfyzzhf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2etfgwilk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jcfjkyuy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lgadmxoj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2adzykrak.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2agbmrsss.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2krimmhby.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lmvzxbhb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zemwkuzs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lhqmdogm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wwtfsynl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tctvrjfa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2inigjudo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2orbspsyb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2cenrdrtj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clpbldnw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufsykjur.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yvyilgdq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2knwqddcx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqlamyzn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2eosiflkp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffkqciqs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rhjdyszt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lhfbvtug.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngmvzypv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tljtfvxx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnyyhgsh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwyuulsh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jhtelbol.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnuoxkie.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skjwndob.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dichictn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyzictfu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtkuhztm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kqzrpekd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrkcfthj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwiamgxl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gwshbvvj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ftwxhfuy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkwowvyk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xlbxtufj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xklsomra.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lbbxhurd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jrdowdbo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zahweaxt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qqkuhutr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tmnevmms.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cblxqyuy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tbfkzkpw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rqbvplio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkenrzqs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vdnuifzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smdkgaeu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fpjwjyyb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ghujqtho.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pwcxypgx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fctdfxij.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdearnsy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hmrgrnro.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2epxeyfka.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xruxtbni.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pchswaew.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffyqmlzj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tljweoue.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhwkohuc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xnzrhttx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghitedxh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyjsyaal.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2binxaqhm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vupipbst.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fdozurjo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qfwicqlh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ahwwhpvf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2llyrmcgo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pjfsrrkq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wonptnrz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pvpfviwe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nsahqbdj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2budszfrj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2syegfkfr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xavimijo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ddcqcrsk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aeeqjjza.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzppkofw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tecigvvp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nipdjwhb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uihnmhiz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2woucqyfy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iwalhkxu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2oviqgphl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ofriosmj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybaapckr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ckzifqgl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnhjbqod.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltmmdoat.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mnawnotx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qzupomzg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yurukhqp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2keezcrpz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ppcxhwen.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuhpvbso.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wotxsxrf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2upyycyqx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eigsupgg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fwpixjxh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2usrryhqa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2prhtvqmf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gpkprglj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yowcwqzh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qnxkadlg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mhsyfpnl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xoznvxxf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nhixftos.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zxponmls.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2babrasfk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2knfguojs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lpmycmvb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2umzkvexq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cnqhfuqc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zhkkotff.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofobhvwv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxfqujgw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ahatvknn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mjjqlyhq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlujvbcz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dnyzjayc.html


<!-- 参考信息 -->