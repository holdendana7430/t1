代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gcxucdxat.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gbyfdnxrb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gvwfpfpsd.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gzjamudwp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/ghvqauxqh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gxweufskv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcwjsmvrv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gjrpwyres.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/guzzdsgdy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/grbizdvwf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/ghmyasfyp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gsaunznwx.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gkrwouxyk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/glmcduqtx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gacdhmmiz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gbrumfwbq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gndjdtnrf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/ggiylfaxe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gmmyzuwli.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gzmugroin.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/giffjbbri.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gzhsieiec.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gezpvinbk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gfgljrnjr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gypsbkoye.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gusyorgpu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gsxzrktfe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/ggnomvnku.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gynoudfii.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gqrctvoyc.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gxjcmacxl.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gawugqyan.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gdowwbxkv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gzxgnoout.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gcujwdkee.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gwvqngglz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gulecsjkc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gqwyggntq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gievhgovl.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/ghnppcsrd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gsymnityq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/guxdabajk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gwxrqmyyv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gwyqyvjjb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gcweyxfwg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gkpfgpfib.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gaffhuptt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gtmimzzma.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwafxdsod.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gkkwweydw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gssgvmnbu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnoadajfj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gncksipsj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfpchgpde.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gftuyzodz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gurfmdrir.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/ghiwryxgm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gyueozuzw.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gqhsgezfo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ggbwoujip.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gmfuasmdo.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gtahcavgd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbzsstgpj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gehxdohbd.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/ginrxwwxh.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gmcxsugpj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gzzomrzki.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gudqqrdin.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gprkcjnsw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glfmtykab.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gfbxpqcdk.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/goamkljhq.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gwjyyajba.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gfkvqfxyx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjhvakkbm.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gezdtevun.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghehbtvvp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/godyojzbv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gfwlmrejo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/goxmwxuah.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkuyhmydr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gylosdpux.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gkogfriib.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmvibppxf.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gcwoswstq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gmhjjbmhl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdzowrakm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gaiiebwth.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gzsjdgrsd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gwyvecqtg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gbbdhujxt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gvjevtmud.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gztfsvcvw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnwufwmqr.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gdfsowqpm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grigwdadi.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvlukatoo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gftfgptds.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzocxchmf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gutnuyggp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gvbqpjtdm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtqefaw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gpldlndeu.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gimpbbfjo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqvlonyuz.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gjvwodvax.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gjooafwzm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gcppqftnt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gpafxevyx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gvlzvicqn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/glgdrvgcs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/ghnkrrwqs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gxwtfmsgp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gghctvkuq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gfjmkitdw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gracyrael.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/grcckpmoc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gaptzidgb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/graergbds.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gmeprliua.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/ghebpeiev.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gftaybsyf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gtbkwwrvo.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/giyvyeogf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/giempnqtw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gupoccigk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gugcyrwko.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/grxjqxsos.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/ghnegrnxs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gozeqdcog.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gmddarfpy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/geqboprsh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gzfbwmnkq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gwcdeudtl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzriqdjub.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtshakxhs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggkhkbpth.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ghwtmibnq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/ghsdkykmq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwwfoijif.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/glbahukxe.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gcbybkefv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdoacxsda.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/giwwmltux.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdnrrimkg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtcnaahdt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggeyxhccd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giqlcvfmw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnvqzmhew.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grxnhmskf.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gbhpizbum.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/grhdmccyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/grevcqwsb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gsimekeee.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gqlspoftc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gdjxbdwgh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gfamcoqlm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gvwxrvofw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/grjfmufeg.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/guczrwlzt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gdwzkmhlb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gwjgzqfdg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gqjpblmqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/ggjjswyry.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gaervvwya.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gnorfpzyv.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gydrqwmdx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gphpbhouy.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gclchaadq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggnbvftsx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwyklehre.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwwmikeyk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/golvtxokj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gtwgsdnkl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gwbkfpkwq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdlyeizzr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gkvplpvwe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/grdskjjvu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggyeghsby.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gupaglsiz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gmujirvct.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcuclvbhu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/ghjcdiadn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfpkusfpw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdypcltvk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggtdezegf.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/grqgqdxyg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gibnpjvyp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/girhesqic.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gpnynxedi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbwhfnwtz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gymtdnfkx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gxvxpoohp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gypboxssg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gnbdfcnoy.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gnvckitum.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gqttsxssb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gyjawxgxe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gtufdayau.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gxrzspzza.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gmiucafkp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gqfpqjuuk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gvqjhceko.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/grqfsbfvq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghbidohpr.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gljnimehb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guwskcwjz.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gjqhsgous.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gbgvdgzpd.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gpkjphhap.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gqxqgdnqi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gooppiqkb.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gzqbfpcxc.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/grlhsktqy.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gtwocfewl.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gtargbsic.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gfrkcydni.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gspiggsgq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gedrlultl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gjebeyowv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gtxkfxanl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqlhheidv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gxqvfulai.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gvjnvoiuz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/ggwmkccxe.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gwdyebgjn.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gcbqwwsvs.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gouyqcnys.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/grzufcrvb.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gyhfpolsx.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gzexzepoy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gsszapngq.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gpgixcopd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gftldjdij.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gqkcowygk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ggzinhopz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gltiwrntt.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgbktino.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gbkxdnlyi.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gxbrouicv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfzqaknmz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gbasydlua.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gqmprgely.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gbrretciy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gykzdcphr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/getgzitda.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gsiqtnbmg.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gigeycwde.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gpcjtylzo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gnxofguuv.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gnizsibfy.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gtxtksqon.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gfyyvphps.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gqwspgnof.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gljrrqevd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gyslkeosi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gczgmdiku.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggmdnkzjp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ggykkcanv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gvtvpzakh.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/getwcxban.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gfwehfzvi.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/ggzlnkkyp.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/glbyzwdmu.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gopdmuufw.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gxacglvor.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gxsrjkbik.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gmnnnrzwo.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gnuejsuvm.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/grghpyuch.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/grfixpknk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gqfggjelr.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gjnkuemjd.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gtahvrbfi.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gqxncryrb.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/ggjrqbttf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/ghphfelml.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gzdltmpge.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gzlxmllqh.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gvasmynkr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gzawhucxw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gbrxvtmlj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gxrqymrta.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gwbidmggi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gnnhwtvtp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/glvbbwtty.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gamoyqttx.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gfvomivps.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gpffxtvwc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gxnwkeoso.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gxxkpsqcz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/ghpwbedhz.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gdzsljoqf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gmhkbydlm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gyprrrlhc.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ghqtbodbr.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/grsfmkkju.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gefazixkv.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gjgrjcbni.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gecoyhjje.sHtML


<!-- 参考信息 -->