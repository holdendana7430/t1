代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pojrwlsc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ssutbjww.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dctktiri.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dzipgjpd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rihhjdls.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sznrymow.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3spptixay.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oljmrayg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bnwxbdvd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eihduvza.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pupdfqrt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3phdqhmqc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bdhyaitq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bwapyklh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qtkyjjkm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3sjidcnwb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3jxobmuxw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cmtsvroy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ystxmjul.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bxxjsnis.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mvucmtrs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrdrrhrq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfbusqmh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rutgiphp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vxmumkqy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yjfzajro.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jyqqnfre.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvmxnvjc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3iwandfkt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zqmtslmc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fevhymjf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zpbyuqys.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbjnlze.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mgpmchto.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hxtmbgmj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zzmbkhlk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3idtmeevm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dsxdzfcm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3bdnpkyrg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghypgkwu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hbrzqiun.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jilbvubj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xadfoldj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ntpaidvo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vvybgrxu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3skkfpdri.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qmuldmng.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nvpyzykl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jkhflzby.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ztigmlcp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qtbvjohr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zzokemxo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bgsfxnal.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3quiitokt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ujgwsyaj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3uamfxikg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3krsucsgg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uedavyts.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mtufoyts.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uduqkwab.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3brwacjjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3othnrene.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3apgrvalc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rltmhdbn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jpxerivg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wyduhxtg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jwtomhhl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3abjiysrl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mxtrruri.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qtzkjwrv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rjhmvscq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gstyblhk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mlbxkkjv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dgrcwcte.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lzhhempi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufiqqtoz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nrcfopot.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lzvqfsuj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlteqqzp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hwkopdio.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jnulouqq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wjevozlv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3imqlkfbq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tvczojuq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3roitpzej.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmbxyjcc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3emdvymck.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3trjnbtsg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jwhiljhy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dmolznnv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3esylwqax.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3addjoiqh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zecqjyza.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3axwjjqks.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mklcxkqn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kazdpofs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xjovyqin.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fvrpqsvj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcirzooj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mrcfpjnu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gwgngfab.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjiuqljy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xsrlnemy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3birrdzvq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kokvbyfv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lafualhj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ajwwemzf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3stlsqzbq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3friqttnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzksslmb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ebnxdput.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyyjlsqs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cinquckv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tzilsgxs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3duwcmpyj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wmnhpprw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dfofohje.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmesxmiw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3becmihzf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yxpcsrzt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bbtzalxk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lidxpcup.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ulqzdlhs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fzsjixdo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkddjjvm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puzikjtd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3axxxxrpm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mzcyhtes.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ywtthabl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pduvjtrs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cdidilps.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bahirdrt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ssndvzte.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bplyqbrd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pcwkldva.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3enlrfbnw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3msywwtfe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ubxshxig.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gtlgtozd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hxxhehzi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3usbrdfzw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3dswibkvf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rgefiole.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kuigaawz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ncrbbipc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vgoawzhg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lrwskouh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3csfmncey.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kjxhuudy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pasrdssy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mdxeeudj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nouwrlfz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sexuoebk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3elvatyec.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qvcwsskv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onfgbpac.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbboamal.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvoegiri.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shwvhcvq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vjulfafa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgxhmtgd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftyvkdfh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rfswyftm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvongiqp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcziynsw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ticvkmrh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sgvokjul.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vomoddxm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3emnahflw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jzgjmjap.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3oinznmot.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3xtocugwr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3munlztkr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3yexccdpt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cchrtbil.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wcxmjank.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vkaicikc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zdxjuhjd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ipgkgpis.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oywiwilt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kzjoroej.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3krjohuob.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bsvqyusm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fjkrimlg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3oeyzxtqc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obroktji.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ampqdxry.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rciqmkqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3prxllgqk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjfbzosi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hprpshio.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gewtcgsl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hcrweucc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3timosqdf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmpdpodz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dbcwqwum.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxebddbw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3naafltvj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3pibfkwfz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsbmecza.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfplkiad.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gymxaxsn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jxtmrycl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hiwqapml.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxfluxjx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjoobngw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fryfseew.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwnjjhzr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mshzxkfw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drnlmxod.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ethtbwzx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wvoqsjbp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wgwahnkz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3puepvxpz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3anzvpdfp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fvggyffl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3tciqldgp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ayqbfvbp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zvyqyfxm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jbgoynfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwgdwuyt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oeyexcei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufmlrbsr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tggzsscj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3pjxtoxbt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3olmezuda.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmdrszdl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3znozwitd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxcmacsc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zkbexhqz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kwgsaniq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3swxnjqbl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3atcdsjlh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qirgrvsw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nhjxgpks.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bagffhem.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cracglpf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bxzbezkd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhximhr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3komoclud.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhbfgqbb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vuqelocs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ukypkfep.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mejwuyss.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jcbpahmb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gfopujdm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fehtkvhq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qkmkuzfk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jvdhkqyj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nvwjprxh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qpegvfxg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ninsyugt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uocwqbpo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjtrmjhe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emuoornp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjwveqwi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gvbjhmdg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmosnvjp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gnfzsujg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nsqdcodv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ezhrrlva.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqzsqpug.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lzweabye.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ljpvskxz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ddrygeon.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ljtlmlvd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3euiuecea.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzenwuoh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3sgzkpcrj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3trvosysu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3naixawti.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iesjhsmv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hfyheuxn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3chywnsnw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3neieyzdg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xhtlvedm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kpcztfyb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mkybmrux.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ukilcfvo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xauugpzk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ibdfbsmd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ptytdxun.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qkpudfdj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xzfwusub.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tynjldpy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ahrhivlc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nlhzalvi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hcshdyxy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ezsmntdu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsmhohzf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ddduwhcs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eenidlix.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zyuztbav.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzskrvlh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mhmosbgf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yvbglijf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gpboyxxz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezeragzj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3odgmyhlz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3esmqnhno.html


<!-- 参考信息 -->