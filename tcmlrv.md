代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xrxzflmu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cmxtldwt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dhpssfvp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3letmunar.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dnybvgdw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ulpykkgx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3moxihwyh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3buhhzpwp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ubjxbmwo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nuhkggsg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rvrecghg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qlcusegc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nydwaanl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kjuduurq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jymoazad.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dhxxliec.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zwuvsyag.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbrebfun.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmnrahhj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wzznbddp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zjarumqp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3bubrsely.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wmzekedi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3srxvszid.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kaqashao.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cjswwloj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xhobnjzd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3pkftnjxe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbrzbak.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yelzdboc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pfnqehab.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3evkledwt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dszmpdon.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ebwxajra.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3atjucmum.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzgjdfmf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xqwyxmzf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3njuzxxci.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3geztlzut.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozusajlc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fwihldln.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ujgfzpze.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fawtcixk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bsklurvp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3inaayuep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xtarirfa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yzoxfpll.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kocyzaks.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3uxbsurqq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yjxcirpl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3grcczxjq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lhejrcag.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vbpamsug.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kqivgxxp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jqoyrnuk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eesbqjbh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lqvukzpw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3raggmnlu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mdqyrzpz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jjlcbmmz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qaenjvbo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qmncwamk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ttulmwon.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lhlkmvdz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pqegcquv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vhwmddmx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3chkgcmif.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hgshwtbz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wewgnifp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3inokrtwk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3kwsfskjm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rcyoyhnw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fccvslsr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lwvykqbl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ohssdfvc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dwfwffdy.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tpruyurp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tixrygmn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3fkujrjaj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3baqtiuzx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3darcisuu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwjawxih.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3aukflavq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zmnctdix.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qduzuffh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3vibsmqby.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdjmrrrd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xcceqbmw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3euxzebwm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gnglgjba.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wztwovbk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zjbqngwr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zfatwkhu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lawdjdbe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hdkgiyuv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uknbxkmd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3sogzrzjl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3igkfreuk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vhibmwad.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kdhpemaa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jygndqgy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aznambnl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tooecoae.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mhphpomk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rfxbljlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3moohayyi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3omunsnnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbrgoggz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zebinaoy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3drgutyaz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fzszdpzd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uxcqroxq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eqxsuakl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3npzsbhnz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ljxwdslg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idsyyndo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzpzxsjk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3spgbeozi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ejcnxsna.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaazugpv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3grtvyljz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlgvrevv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vhaekvoz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nspdinlt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nlerhoyd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqiibtaz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hkatwacc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mjlyubms.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qsjrigqh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ngntyvtc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ogldmiig.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gpfknfir.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qngxtybu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xdiklrrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nxuhbqst.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3veexinku.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xufhxluf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ndnbfyfj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdwkreq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3blbrxtbs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvmgarq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zttwjkyv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3cwycntom.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hxjbzayi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ncxzkmwu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lkiuftlb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oymqinir.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzlmkmur.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmgmbpwy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uniizpco.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nhkpqcbv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxgnvnvg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdxpylwq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kmohmrck.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnjxhlps.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pmrwoxol.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brgykenf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbuaocnv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bhnqnlme.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hgqymucs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtlgsxco.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ogcvgafu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nmrmhhsw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3esitvdfr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vbvutjom.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mrnanfzb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rwmwlcbg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3awcazkbd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jfdgwdrx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nozazgcq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3enbpodfr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ywfekebw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dlwysjnf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3msqcejrd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3aeoirvug.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lwrstmvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bahbrnxx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ekoskoyh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eudlzvow.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3cknuwfql.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nsvfajhq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chxscmbx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwsufdyx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fwmvatja.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dendcckb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cheshjsh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fuilklha.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilefaoyk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3uuuefalv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3oznslymz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwlhkdct.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fpqcsdzb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsrosxyr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pdcajrei.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yyrnfwtd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrttvjij.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxkxpuww.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfkzszcf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xlnhsybe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlzrdkzv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ualrsjep.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncanmzqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rzeicokt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gcfusegm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oxqkbqov.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sofqyrpk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3uinjhkxk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jaoofopg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mfexdbrt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rzwdfpyz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tuvwwmgs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oiupaknr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qkkruzec.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ejeqltsu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zmbenzpb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3urerortn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oewqrrse.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tmecssas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpehojuh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uqdlwtjt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lxdktxfk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpmlrkvv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hqbjmsfq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vgignqga.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3szboqhij.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nddbdeok.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wnlljtiq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlhwptjq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tmnteyrj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mxcrygfh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yyfgsnqh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuncjjbd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3trvjwubh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzmhrbi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3cqxsgxhs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pypwzwsx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pcsfyeix.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xsuwpmth.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rblomftv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tfqlbsuv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3affcuhvx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fjzzlllw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fsejczgc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fqhhnodm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sklbbgnq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nvqwijxm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ugouvsme.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cdvymxbw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3covrcjul.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vewvtehb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmoukfbi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ezgugfyw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kftcgnkn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xqdztlmh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wvhzslsn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3etcswzyu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nnefacop.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aiztdyxj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3newpzups.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljljbyda.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mugjcudg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rouabmyi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3sdqvmsqe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cdmqyqpl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zrtrphlh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3toyrgned.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynzrslwr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ttxtqhjv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyrhxpno.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chazmimh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qgccixvh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3efxyuepq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3obuwwpgy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3bzpvsymr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xyvolpsa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mjpcmory.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ombtgruv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ryvjhvow.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yrmlweqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qxnxepit.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tjduirab.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3psigyhll.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3aclfszoh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xbgykaaa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lcyugpon.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbvwmhcc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lwzcurza.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oemieihw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mvidjvqp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ipxammnc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jphaqtob.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3teknryhq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3firifmed.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zztgobjj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jwzipayg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vbbprxug.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3opujldpc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xvqhmbkl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iefeydti.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ofbxxigz.html


<!-- 参考信息 -->