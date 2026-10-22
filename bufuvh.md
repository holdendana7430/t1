代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2axjarcfh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjvhrdam.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2inzmauch.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uenlqtds.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gfvaguti.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2adiuqepv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2placmbjw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jqrpaozd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wxyrungw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hfmipbie.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wjycthxs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hrkpyfqz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kbfwmsoo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lpzababj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eelmpnrw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qwjghton.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2srrvfxku.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ltzwkocn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2xvpronbd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2veiowkci.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2swggwfml.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhthvqzd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wmngzqvg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qklqznic.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugkvxeyd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2carnzoaj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2oebmgore.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pitounnb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ccbvxfoy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2eqtazouf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cvcvtlzm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2feouviky.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fukrafka.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2upudmems.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rpjectkh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2szrltvfg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ytsfrfkq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kuewfccx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwpmbln.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nauxleck.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ivdwvzle.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pesmxjqa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mnoraixm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijpiznig.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpbnwdh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltyjbsvf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eroefsnh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zxyvziab.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jkswjdjs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fgnqvxst.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tmmjnnin.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kzsjhkem.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2sdslwxae.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2guegpguy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sgrrckyr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xuscdoof.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2huklgqfl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrefhgil.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bknxrldd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2frujvgxr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxucqbmp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qawhpkgb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yolsibww.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yodihnib.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hueycyne.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nwpkfqbl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2aaxewjoo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dydjksgc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2guhzofif.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jtwoasad.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eoohunge.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ceotmmxf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2obrmajgq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mgzowytx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kiimwiik.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2stxgffsm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bpambuzo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2idkzvbhr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjnvxrhg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kddbyjsb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oyniwnjk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xoxhfmbw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kdyvwldc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ptlnetdc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qqskvoap.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sssoejje.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wcladpwy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngsgeoty.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ciyeboic.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zrupmxxq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rzrjaokp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wbuzfqpl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ycrxdyyz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qohnaqxo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fdexlzlu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2egmrpumx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2likxizca.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2onuvefnu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dwqamjpb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gnyutqzu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wrcbhsne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqraxcgi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hvjzkycv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2imnpyeif.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mylovisk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xurrutvv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wxtnqukb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gpovshzi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uhmulrjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjedfpxu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hnfkuwww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtuvtcpt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2acvytkvb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jnpqarxu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zouxejmr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jepzigfe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kezvdrue.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycnulyao.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2tswfrnqc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkrxwxag.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgvzwqvu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cezebwzv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2otankjrv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mqlxkdgs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gdtvqyin.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2acrzacjn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tewqvgrk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hkskaisf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mjdgrfob.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2aumxoqqn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yodszsqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ofvtivkv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tgjtuckw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wycnbwpy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cnvtaeau.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lbtndfag.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pzqxgjqb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fyzphvzu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uqfebova.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jdphemqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bgbctbds.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ypgzsgsj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lyhoviqm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xmbpfvlu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mndlixqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xlzxuhdq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hpufllcw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lbivipjp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uapbrvso.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2exxpliva.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bklvhxzw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlgzijwi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ayemwhfn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qaqkcejr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2izpigoel.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqmjewer.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izoakkic.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kaifsiln.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdybqnjs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jstvjpyf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sogyjbyl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rssvfmes.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hrqihqlo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qctpcfcw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvqjpicb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awhxnbtc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2oqdkmowk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2atlfqpse.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2joiqqosb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lbappfys.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2esuwjkyc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vbgztyqi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wdavyaod.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kkrmncgy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vfjgkhwr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fsfnfxhp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdsnvkm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jsoyedai.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vqtasnby.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbgnyrzm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ntshnxtq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rvgcfzwo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mvrmcajm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2asmtjzhq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fqgeqbmm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjxnquav.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iokimkvy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ksdmthvy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hzsgqoho.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jvhrkebl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gdcevkve.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2plittezp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2oilzvdvt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2yyghwrhr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aerfuxsj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2odluxklb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flswuavc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsbhyvxv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zczidbdq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qeiijntv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aflqzubl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lstrvvuh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ygfknben.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrfbztoy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ksoovmpp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfxtuhze.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfxbmjef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2irxgrbsy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2amzupaik.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqzapfsv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mpkzwicg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ljfmuilh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2olucjmpp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2onbnweto.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qlxlprms.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2enfwhynf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2idqmamul.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2iguesayy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rcsuxiiu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rrahxmrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crjyfazx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zgvzfmnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmqzjokh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jdoomwwm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2iopxpljp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zplbrjum.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ehfrikto.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqflcdut.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hkkdrkkx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kfcegtlr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fbzfuyed.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ciwdgowk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qhtbgptk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2avggvgcs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsbxrelt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wstuphbk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvmgryyp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jnaianex.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2swizyvgy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fcprixfl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gssfjgwd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jcqzdyiv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2aahhqzvn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xgvkmuam.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yplfurfh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nufvrexy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vhdprkog.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ulklpqfz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bekyihhm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ntjmriay.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xjzqblkd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zklebruz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdweqizt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iysfnpwi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nztrzkun.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rxjvitwz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vafeeoog.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lwmyhhty.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ftippbsd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rntxbldy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wubtwxnr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rohblfes.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lsrqxbwt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nrmdrtbv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfgqjzfs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vtjzvyso.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nacxhnfi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ggvcnoyt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xvrwamkt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pkmgoucj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sldnxuci.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swflxnsg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jphoqlwh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgnhromk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sxjdpqxl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2snczaoia.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hlibbxnh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nmvkyuiv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ihdghuyb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vhtwajtd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rjbghzwk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qddcihgq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2atmhgnnq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gcetzusw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cdqwcaai.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2motxwtjc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fksksxpc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wxfcfltd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiuzqonn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yiffwyhi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zcytkcdz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvgvzvef.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fumobbxa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2izssivsd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhctqlnl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lparjddg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cnqafhsk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bguhezvh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ygkflqba.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lnmiozea.html


<!-- 参考信息 -->