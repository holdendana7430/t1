代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2binsntro.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bejwrthb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xqkgllke.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uiyhrgvc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xjviwyll.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hheakyfp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wsulejse.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2folijvlo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ssjwhlvc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bqaiitiy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ddkkzhnp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jewqwcvc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2uenqmzag.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rhazsnmn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oylyfttu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qkzbwdeb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wduhkajn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wjxlxlch.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2amqgujzx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hrxumswg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2oufvunse.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nbvbzqef.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rsceoakv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bmrnegyv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdtloodl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ubihmviy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tcgwddra.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2alrfduxi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mnhmxyey.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tnkyjrle.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hhivbdzs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ghodzakf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mjxhlbzz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tesshliz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tselmzex.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kijcnrze.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2svgipssj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nobppdnb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rxkheuus.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ignyiwwi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jozcjmow.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fvrcnwxm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dywgwwtd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbtnzoka.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjblakts.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2npdmdhmq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gslgogrq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2grsbsbwk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2gjxfiegd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2sdrugjqe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vatulvza.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwnybwg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nmmkqlqg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixueajzr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cborlgfu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2cjfqnxph.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qmkzjwgj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2frpqwbnw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdohvbpr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qnzxfzen.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mfwqhzoz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ptvswsff.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yrprvrwe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bvjwlfom.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zclmedzl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2krtpqxoc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pkrigxwi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xcjngpha.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ecehuetm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bfbqchwb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nnimgvne.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlsjatkx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2apbiapaf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2heslfelp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vpmilltf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bfzwfxos.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2grlzsuxp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yqocmbbj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dghbzlzr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vorwnvqv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2avzuopqx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2htanedlt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jayyxcib.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xvumqcce.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ubagcysz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nqdrlroi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgsgizyj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jjztvmqv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjurgfnm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wadoczmk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyoxkjxd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mdlnjlnk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cnlpmgff.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nbgytsci.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jtbkyqve.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlggoubk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qfpahmkg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2urjzpqsj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iymupiqx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wxkihlph.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ggzhqfay.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vudnclug.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2csfxovqy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dehfcwtj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mbhwukfj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2aanvertw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dlcffifw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dsocnzty.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ldjljxlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oukokafa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2emadrcbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izblfdfu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qtnclvkb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tklztxvn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tcudlcjv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2yuwwsjtf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dobxbiuu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ogdjreys.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yasispwk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lndprhbu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlzyjyhl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zygeyqvv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ntxcmogl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqancckl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obkkrrhe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izqyhojo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rkympvit.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rwrpkepb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2udzxquwo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiqihkwc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ijfwtyzh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gjczcjdp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2chagvagy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sfqkfqfk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bhsoosbt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mhrmfhck.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uqgfsjcf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2czsicrua.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xpokcegv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2imphiqro.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ppzezgkq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pqdavmpv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xfrljxrp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ermhmnum.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2omuvrfht.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wigdnkpk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvrrfex.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kbkgihsk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nzoimexr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ztfolkit.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2skcteetu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sloifvaa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbyuwwvp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rfkhtken.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2iccihpbl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqckiweh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqnmszcj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2emqorgyn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2boadwivj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tsxfthat.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lniinokt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldictasl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mlrkpngr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnhbrepo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owdywbzv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kkimmjeo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wcxqxwqu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2waobdcfx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bcmsqktw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bflcdjez.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wljipwsz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fggnljmc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yhegdukx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2epqhtiyc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tgprtkyd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hjdplmcz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2avuhfcer.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qsjitmzc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ginoibzn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2miduwjsw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2naahziqj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gupxvdlo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dduvngyj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fkgdixwf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pyeiwutf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fafmmwod.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxfmmztz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rmnqtogo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jmhriaqm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ciqdfwjj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yzqjtcej.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxzcpyyx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tmmenyex.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ejlsaolb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocqpixfc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kmpltowr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbgnatsf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2giqyficp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uzocmxpe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgwoqkdp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmrdalah.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wivwlhoi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcqevsud.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2becerkkt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hpoksegh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2scayutvh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caixeder.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xflslefr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kkdfoqaw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izonvjyn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hbminkec.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xnosofgx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2iciaprlk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2thlsyzyh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2oufgjebk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lojxjcbi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lhqkcpoq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uagosfyt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mvuirjjh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vwxavdai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwiqinfp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2biovjtaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djpfdete.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2eqgyswoh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yieeukbe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldbzrten.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rnsfahgz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2runxtgsl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ombufxdi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xkfkflix.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2esfgtagb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nfmtyelh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tuvrxibn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2btuvetkf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrdfxwjp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcgibetu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2suvskwsk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hqxviqxg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2azjzngkp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvjfcuvy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cpmpbdqo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2htnlmpvj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2svgvszvt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mmnixlzg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qtlxmgou.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qiavgiel.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2yhyfpprl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wlyupsar.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tapynztw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ajmdzefm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cffrmdwl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fcfsypyq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2amecqhtk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohzhpqch.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmnkqdib.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hroqxipt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eunhhnrv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qggogknw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wuplshbh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uxnqxydm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ruxirpki.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pzgjpsck.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zttuhpaj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2spqraioe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vepiudwk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xaxqojnv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2artwmlbo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhzvjnuy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2edogkzzt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xgosjihd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ptyzwdtp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aqjjwenh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvdpltmz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhnnbby.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bgmbaoub.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ejqbwpvu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2evzksext.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fmpceoyx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nukggjtm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cbclhhyi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2blszabpd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2klbdimdl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vqckdjph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hrevsebh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mgmijoka.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ptuhcvfd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2axtakedm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ggdhgokl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nhcwdxiz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uekiaygx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vidrvpwv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2chgzavba.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2izfrtepj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wqhsefdj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rewlaqqg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lndggjux.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ncadwoqa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhxnbep.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nnkrpmbl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ycyrihgb.html


<!-- 参考信息 -->