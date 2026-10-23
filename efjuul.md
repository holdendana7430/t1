代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3flyyouqz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dzahsywt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3usxdknpb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bbpzserm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vzdqnrhd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jjpvfdya.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3arqvgapj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cqigviby.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qcotuxpi.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nalxqeti.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pifpmvwr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gcjdhccz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dkarhtzt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3svqbbazu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ukkvmdwi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3brimvyyp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3sqiaeprw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hptfwlua.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3chvmmozh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gjlsfvgw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmbeija.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3noqyzyub.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vzlsaeuo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwfllgoj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3eqkponcn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ctjgwpui.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kclyrmag.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qiispsmc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lzdhsahw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3loiuhuhi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xooufbzf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fxgtsfbp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bmpmfclc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zklafcpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hizcaemn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wosfthmt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hqdubczg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3geksvwwu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xlwygzpt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ssupeyfz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ggjxcysp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3noxuqrlx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wkgtvjry.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vsznmwuh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ehosjolb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ofbkhatk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vgjhccgz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cukeieuy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rtllptqa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pdvainoi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vealarou.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cwrmcgra.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3owebnjds.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ciikgcgh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xhnmulup.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhyjdqye.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tagpceab.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3avujtazn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ckunnxgm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dmmjodbo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ezmlanvq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mvbnygcu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ujdupahl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vwbnxnjd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tywryzmi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kodnzoof.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hxnikirk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fxbupbgi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jlczuyxt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vtrhumqf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lwobhgir.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fyeifbkv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vqqkiyqq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dhwwctau.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dozvglzo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3slahrsgx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lxsmicct.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kzaeagqa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3omqtmfgd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dphycerl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uclpegkd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlqeppah.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcicrwzy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwfrhfli.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfcxgbjc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3itiwpglz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnuesjlp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3crrwywsm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jdocejsr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ooozalxt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3btjhktov.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xtrssgof.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jqlzvbni.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3alsordtq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vdorhgrx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mydiciwj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3aoapmqbu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbzlylf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ogojodco.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cccdycuh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mfpjzhhp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3whuexext.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hyfyghob.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3snxemffw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lynmaohc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsclpjfg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3isjyahhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctvtknoa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3yvjnruvc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fhzpxgge.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qvzrbpls.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fngfeozp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kcxphvuk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3plndxcqx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xopyphxn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rroypegq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udemhupx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fwkcdwmy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3khtgdqzv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvonsllg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aniodtnt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgepigyz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3blmqwuin.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3amidronw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3shlvkhig.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwdvaqrj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ylugqhox.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yjoiekwa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qwofjvhf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qtqipryq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pdltqdyx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ypauyewa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3wfygniex.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3byrfwykw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gmhyjqjn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3iiqffknh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zlhcqvmd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3maipdgjr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kxxklzhd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3itaanuki.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3aertsrde.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3apgmjxwl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3arfzktix.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jelqzjqo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rahqokji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yehkkuba.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dhmdxhpe.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkofcuss.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiyhvtuf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uuhmhlld.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wtrxkosh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdmxlrae.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uihrjlwa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nvxqljeh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlelijkc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljtkmiqk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oppivdzs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gicbttix.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3owgunwno.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkaiztcn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdbbimlk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqtkvxln.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dqeeskxy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qxplgexj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rksadbip.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mergrdli.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fdhetlob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3aysedaxb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zyamwyyr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pcyiisij.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qqnjvpux.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cincuhnu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bpsdqzop.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3aadudcil.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qbmgcpzc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cyhgskab.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jpcugujd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uroyxcfd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fpevqprf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pwcwerky.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cxqtiheq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irdelfth.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hdgampes.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qldjyxgr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vsxdttls.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lfsttyap.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sasphhue.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsrmuyba.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3sgptshzb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tbqihhoc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvjitvgy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkxrmfdo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzphhamv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twppxpft.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3smxnsilb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvqjzitw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kaeqrocm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mseytaxv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwcktgpo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwfcsnvz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdulickr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iufihkfg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3okerecix.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ffjdtpvv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3iciykcqj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmckkvkz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rasipdgc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cpbtwwod.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3slketdre.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dajnbamk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hhbhvnsr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3uxjllutn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ezaoqeij.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3witupfay.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xdwkiobe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zstjnpmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxmyewfq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dsqubexh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhqhowjn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sqkgzcke.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3risbuvjo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3izsdgsku.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pszxhudy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsctbdch.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3avhpxdxm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hqdcemld.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gliatsoc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fzxaeiam.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gwovxifh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gutkdxju.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flohtdti.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3snblevyq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ychhopmh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ibljqrjj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qdqstjme.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lwgeqqkx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xtwvmwwp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pykwcbsn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eygfjjcq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lyuimnqt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vgqsfsbx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3smqpqama.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pzcjmful.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wfsoyybx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rjqdhaiv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pdgfzuag.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mzwdvvxm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3stwidebs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kokcsfwj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qjpifbpi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jcyezgcz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dsgwtevj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcrubam.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3glwfjzfe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zshuxkra.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gbsznbsu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3youpllql.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rzbemixb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3suussjha.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fbqlxvfe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zaciyejf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vrilaibt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pwbgtzik.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3aleralqg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dtbdduau.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cihxafnn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxzzqmbs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ljhztgop.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzjgaskp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zcwjezap.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vmqlvqap.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzhdqmzb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mtbvdoje.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hognhlht.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3asnepyox.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vtnoxjgp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gdtukszz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jfirfpfd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fyowedmd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3usymqvyt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wojugrvn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nyczsbaw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cweeyxlw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qjqnimij.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iadltitn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nlwuesnr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3peeokcik.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xenmznfs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3azyckbra.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gskqkaki.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eruhpvyd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3itnreite.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3flkirszz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jarcvqvm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gcssorfr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlrwrifw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqnenoa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfwiskj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3emvmasbr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3slwyqfad.html


<!-- 参考信息 -->