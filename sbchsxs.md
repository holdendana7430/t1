代发 wailian999

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/goxdldxzd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gxfxlkxkz.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gggaoafbf.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/ggpsewxxo.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gdxttgqsf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gyseageuq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gtjlksded.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gpltkrbtl.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gnpksycpv.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gciwfxbte.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gsokdysvh.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/ggmgqphsb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/guwalbzsj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gnddyajmi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gvntrsgwy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gigjudebf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfwisjlol.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gavywasro.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gfjnhxlgm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/glreyphhu.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gepsgpckk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gfyxnbnbz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gncmlnzzr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/ghkcrxdki.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsbcmowqh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gczkzpjki.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gotxsawbm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gswwfwmee.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gpinwqgtt.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/grmohzxuf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gzvlchpcc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmutmbij.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/ggndfeknd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gsbygaffx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/glnpstcxh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpygvjpme.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gywjgayjb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gjdkgmwnx.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gzpllsroc.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/garhcxmar.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gnkoueoup.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gutdmrgge.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gyfusskud.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gvvhfgoaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gwpfxuixr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gflqrukdx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/ghxgqxkkt.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gnkwrpylo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gxyxqmmjp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/ghsnsgdmk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkkwkstsd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/giqdtgvkr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gprgjomhf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gxiroekjn.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gfxihnnme.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gggtuhvnd.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gimqmkrcq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gkvfqqsru.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/ggyhniroc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ggbalsxjp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gahatomcd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/goumwbqap.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gvgbbjgkm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gslebxtkr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gekfhirve.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/glllknvuy.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/glumbelda.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gafavtvcj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/glcifhofs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gzlsdeaxy.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfpmrfulc.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gdymrrjmo.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gvaegkomf.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gkgxkorxp.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gnrjsndwt.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gllmrzycd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gavxmzeya.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gpkdkpwol.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtritor.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gfmflwrga.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/ghkupnczu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gkqqnznyu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gkrwogwxr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gmtqnxuyr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gkzkcylna.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdtrtorwd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gjylosbvh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjdmspcrr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxxgxjqbm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gcctfsryr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gpwrnqzgx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gurlurfbz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gslcndaga.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gdbdlxmdn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gmewynpnb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghjziagud.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gxyrwvyrg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gyiltuhjq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gsrqyujsi.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gfrnghmlx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gbnnhwukr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqhwlfkyg.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gmjjmaqeh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxjnxfnzw.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gzicuyyah.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gympcskfd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gptkuqqgz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gcbviqlel.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ggqrnebuh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grtmwqkgy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gpdjpzyqq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gclragalv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcpxleghf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/ggufveygx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gbznzdaly.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/girwjcyfs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ggbhvmvju.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvzgmmivd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gqfemwbsl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gogfwwzcr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gpncnzrgi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gdsibgtre.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gesrotafu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gupbdudjl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gpxnhmkms.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gxaoxidlz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gkbjdjoum.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gzqcoszkj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/grmfwilkk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gqdcbswsy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gjimbswgr.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gdrgeeorm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxfpkkxjj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gebelders.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gnwbnsovo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gjrcohiwh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/galeivoif.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnpdkkrfh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gdncicyou.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gawlppwou.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gmphasvpu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gtqogefiz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gayjfbzmr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvlwxwztd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwclgvvrr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gfqdnwobe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gjyxwurkt.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmmrymulc.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdugicwmu.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gpbmizxzl.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfjniasmb.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzdzrdxzm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goyczgmnm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtfrbrjox.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gmmcakvfw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmpmbscjp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grrpnpzxy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grsbcbmrh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gpcscplck.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gnfxjzbca.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gfdqdsfnm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gidbsbgvw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/ganodatci.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/ggcrikpic.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/geetpvzhj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gaaxcjuze.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/ggyhnmtkt.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gkfjptlfy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gvaefuuyz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gpkvoaesn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gefjjomud.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gihpgjbxb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/grkxbialr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gapygwvba.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gisynvomx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gmkbjsjrv.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/glafqahqa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzexnekuq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghkkfoxrk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gtngfmhut.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/govvrbctb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gcixlckcu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/ghkbytyoe.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gyphqocrr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gcnujndac.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gduobriul.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwfetflgj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gffthgyeu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzzkcoebc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnbydtsei.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/ghhkmvtwi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grbmgqsdn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdyooxvja.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ginygscik.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gkzxlcapo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gglthozbr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gtehjvrkn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggiqdcwkp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gmcwqvmmm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/guoqwtxhi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gobupdoco.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqndhrjkj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gbjddilmu.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gtztigaeh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gwwwddlgp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gkggynfqj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gyauzwhsc.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/guwoxorgq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gfjsmtrqy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gbffdhtuq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gqrczcfyh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gentwgnbs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqvuhpjhc.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gctjwzhft.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxnxeazkj.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/giybmrzod.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/geegeeumc.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gbhemsuji.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqxzdgsda.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gbfilocmn.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gyexkgphu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gtkwmbsyz.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gaqfybnyp.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gexxtdvwm.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gzxfarohy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gvfixppay.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gccnympjc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gdljjgfdr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzffsoncd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gcgqdtamp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gevydkatk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsmxjxtee.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/grlaunmaf.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gsplkmaxd.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gamwiillb.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gbvmaqqdz.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/grieexswv.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gaegvpygo.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gjzfffctz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gmyjmncqg.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/glrwwuryi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glwfxvzmh.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gdgrraprs.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gwqfjfgsc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gtjyuklig.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gbgceipch.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbjkmjkjh.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxwlpwgzc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gyapmotvn.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gvmpovobv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gidgdqmby.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gvlemtigp.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gdyiudhgv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gyhffwjwx.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gffmbuqwj.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gutahywuz.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghlhjgtoe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gamzdocao.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gxmdiahxi.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gznkgsskc.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gnofiwbsh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/guchuipqw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gslrlkdph.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gpsriqeqt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/goliajcoh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcmcomlfg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gpbstxvpt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gzcrfelev.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gykxdxrpp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gtjxkptgn.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gitogwqzc.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gxiumpnlb.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gyqxtfpiq.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnxlkgvbm.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gcspsqdty.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gsbotiuuh.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/genfpbtmf.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gzzdmtgis.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gtlrcpilj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gtgkxgbyn.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gpgbixitp.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gdtjtbevb.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gigyruhzl.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gjaebdjfl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gjpobfmlo.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gbeavtnfv.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gmierlnjy.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gngicwqgs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gcwqbzicn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/ghmqnwpkh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gvmbnnazu.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gzjemeeyy.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gihyabkwc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gyhlyacmu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gjelbmlrb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gabxlcnhg.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gwlnfjgrx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/geuxniqei.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggzdfigwn.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gphmsjaol.sHtML


<!-- 参考信息 -->