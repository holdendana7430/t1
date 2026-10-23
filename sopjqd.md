代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3twrzbdbl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cdyyizea.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3twottzls.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xzwpqvth.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3htckzkjo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3coxtlvhs.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pocdplal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3chfiltsz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ihyzocza.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vyomrzdm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lkifsyil.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rxswjsvn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dbyqepqm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rzwnwuuy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3irllyjir.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ncmghjoo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rbnwbmya.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rixkmvwd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hnsxtdfi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxgkjlsh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zkmrxdhf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3orucdsrm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtcjfhgc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lhqerivd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tqpmpltt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fesprewt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vrxzaomy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3afrrbzug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ubjrjjcq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xdoqnofe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aerqzfqo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nufzbteu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dyujdkvr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xxhbybml.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3aoiunfgk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rftdpzzf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbqiagf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdnzgeii.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fqwdkbde.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ethqtbdu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bcocjxmh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3oxgohphs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3grntogid.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pyranyze.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jdyenbyq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3izgvtkyi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3khtqtuyr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3blzclfiz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3implrinz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uylcpypr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaqerdov.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tputowtr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eubtnoex.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hcljyigi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yhezyeqz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3apfajtcu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wszklzig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3apjqkuoc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nvwfkzwh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnhtpco.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gtxnnykp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bkktjyfk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zbrnnyjo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mdygsisf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqcwintv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hjljwtry.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vmabxzkc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oogwqocv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3beygjobj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pbwerimi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzrwxksj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3frmsvvjz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iodctgfv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fqsfdyjt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3clbphggo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rcknkhyw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mrbaoagp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxpajgwe.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ropidvtn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3padhwrhb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqhaovlt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kmytovos.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilsuodnw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qwjkkbtd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ghtrvadb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3igglregs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ukmxlnho.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fgweklpo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aznljcfq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bpqtfkak.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3voxnwwcn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rhiokfqd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3twmunjcj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwrahtnw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3brkajbjq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wkdmkqtm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bodpwjdt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3msvwxxoq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3nsisjpzc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kljrfasa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3puobvzxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohnwrogm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dbiteiqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruypjxjt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jmuxpzse.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3iyhwgiaz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqojqrsr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3yaofcadv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oorziifw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3singisjs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3yfkulvtn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3woeycuzw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ptqylhme.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvlzvxsx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ofjrujwq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gqcddswm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3acdgodby.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hvtzgdlx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aekptshk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3srmiysxu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kxcsavjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qajrzcme.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3aiyiemoy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ejdenmcu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3invygrdp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3twxdcrlv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gexteftr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3farcewcg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrnwbsm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3iqvspich.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fvlfxeye.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cgdxychy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qldvwihs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lgppfuvd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3usnltnhq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bsvpthqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlyexmn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mohpglyj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3atjhqpbj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qmrcgcuq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3najhiyik.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fmtzjhug.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idztcnso.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehhvxbrw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmaqxjyv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cxoagemn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bustpwew.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umuqietz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufpwznde.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3heaynseq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqmyrbta.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3prjeareu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgftivew.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtcxwlyy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zwvdzgrt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkvpzqwn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzautbvp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xvxofyvq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wcgbfryw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3angfxfey.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3krndmxbb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3eqhojfgr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3twnzsxyf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oniekxez.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qiatjddt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mkjauxru.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dqbvmfhy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3plwkvfac.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jmhsarcu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkaiouis.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gqdxpmcv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3datshwga.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qtaydxch.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3avqjzrxt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oovogkki.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zkbsmwix.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qtysigzf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaetkynb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pgenfjme.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lqurrayn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3taxoycis.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ozpjvlri.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3djmlllal.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfhrvifv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3odvrjxic.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zaezflet.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chdihexe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dqowojqa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpxscezd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhuxdpmf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ihxbvjzt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqevjevm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oarlyddv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqzgeaeq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3crproykg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azlrioyb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sshqxhhw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpyfrvnu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spahvgmv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uoimmvdo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ejhpgzzy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kanduept.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gafnxtjn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3gqnfkuqw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qvmiduzo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zysbvuab.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3haxuaiza.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3uqfjtezz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rnauwbkg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mhfkikkx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hjjajtma.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nwcymgaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hidhwhbv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lqymasle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsfgcrcc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gbyszsns.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bmckiguk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zhgphjfl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iicpssql.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3njxtswci.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3phisxock.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ahzgefup.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpakqgta.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lbgfdmol.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vmomlobl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kapalodf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3iaadwgop.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3blcllqdn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mivhpbnf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3txbxxfix.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tekjpxdd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3eazcynjq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wpzksniz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zfdoiymm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3njrtzaiz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gdjhhxrq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tlelugib.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dfthwyoo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ghjtmzlz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qfjhaues.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jfrfvedh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3neqismbp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lcwemdvd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pgxfdaix.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdeegybu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kaarugjh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ezlhfkyr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lgkhhgwr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bsqpmjiv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3adrbpusr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ezfuudid.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mbcfczja.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dmwtmool.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhjeidxe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eomysezw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xonpisdl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qvqobqzb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tqmflijw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhuugwzy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3esqlmgwf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mijgepto.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qdgocrlt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3witatzqu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtxnqsx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btybhhwv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qixgxxdy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vdkpjxil.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fppqnnmm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3phuqwror.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rhqcmzxe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3olhkgwsl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lugdywjn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rhoiswpb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mearmeqw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vpwhvwoz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xojafrbo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hsvctkic.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gbapibud.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gmtwzetd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ttnbdifv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qswmnkvv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mfdqxhrg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xevjfwhv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rbiuggho.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yiwjtdgh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3strettjc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyfvossn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jjkyikix.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gppdpqox.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3duajnepv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ijcsfvzi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pbwwfolw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nixizwlh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wnpahdgm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sszemups.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3aucchmxd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nrdfnjty.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bdvgkjpx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3szgyfjgl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kjhfugea.html


<!-- 参考信息 -->