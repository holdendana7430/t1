代发 wailian999

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gsgkberdd.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gawhkrwlv.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gztcdydhu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gjjwzdqjr.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/ggpjxlerm.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/ghnyjxqle.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gnggduarv.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gictkpxns.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gskradsyk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/grrifdbpt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ghibpwizr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gnmsqqhmn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gvocnleqi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gwcvoxteo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gqujwentx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gjauxbjqg.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gqitsbjvm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gydpalzgn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gpecdxtyl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gcekhbvsu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gxgpdnfmw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gtmpxebpi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gyguaqzjd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gocqniqjq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gvbmgevcw.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gxfiabgqu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/govegppev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvcmtbfrp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gssnrjsol.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gcunxpamu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gzwgqwigq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtksvldwf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpwmvhklu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gzizogiju.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gobqvebjw.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gakrvuybj.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gmqlgaext.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gdzdemqdi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gotwojccu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gxueldcct.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gscuijvre.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gotqbikbu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gqkvdvfdb.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/grboyjcnd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gnpomvikt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gajhdvsno.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gmnethabx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/ggjeigveu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gteviejvh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gbsgzgfji.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gxttmdvlh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gqkeybvde.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gbdoaaaho.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gzqgwflro.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gahdeaigc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ghyexceef.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gyfrpsoig.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfenrezdz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gdeueiadu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gvavcqaxt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gnhvtujwp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gouxwykjb.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gjitescrw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gxbskeiec.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gyiptthxl.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/glormaxcp.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gmgmdjtuv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gcsrqqwir.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/ggnsyrqyf.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ggtyybtgl.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gkmhxocxj.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/ggpcdfgvi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gxesiizfg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/grrosqyce.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/ggxomcbah.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gbrvupdsk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gouagysvz.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gokbpwpju.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gjwbeubhq.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gthmsjioo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gacroixpm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzibbshvb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gezupniik.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gyyrimdys.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gsqiludek.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/grmyblzdz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gaufybejv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyfsrzjqi.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gjxematjs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gfmiibyuo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ggqltziob.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gtcacclmk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gwwaymfvo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gbkorippu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gojivdsks.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gccvelnvy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gbcfbsrjp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gblccgcbb.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gfjalwpat.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggsrivscg.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/grcayzefx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gizhfwxlf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gghxncgfq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/galrrhvdb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gopqvlhnl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gmslbtkcb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gtoxfhgqv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcnzidobj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glamhysck.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gyychgzpe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gorzaplsb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gqfpalnky.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gdhjkslgo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzqzmhiwc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/geobpeitq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gxzhmecss.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/grwmcfezd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gzfhfldqz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gkdoidgad.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gmplumrer.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gnooszeog.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/grwuhyfgv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gedtqtmin.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gclvnelek.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/ggvlkswha.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/grzuizkst.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gluvdnzve.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gczfauyus.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/ghbhyqmid.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gjhskfoan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gglribrpz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gezpephlq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gkfjummrg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gzuwgpbuw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gaospcuwr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/glyxdtvbb.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/girlneker.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gfxkpqamn.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqojguiyn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geveoclrl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmhgddrab.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnjqlllpc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gfetpofae.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnnbudxew.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdywbahjw.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gkacsqoqe.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzequceiu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxgzipcre.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gerzcbjmy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaqqbutft.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggfdxddji.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwrrrycne.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giyosztxo.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfpvuiatw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gnnxihpjl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gghdosnqz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gbiguonqw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gixblwvsm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gklviofmz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gpdbggffx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gfjlcdicp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/glmprwdvz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gowujxiaz.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gtlzvqgps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gbawndrvm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gpsfchytt.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/genkkngju.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmueteq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ghuzupxxb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gnlvjaynt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpsxovsqq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gvwcxtvha.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gsfgvsnvz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gupkxnpmt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gglftgolw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gymdikluq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gzsvfsyqy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gaqwjqppu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gybtspbfo.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gromhahdv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gcpkajico.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gbpyslgbv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdszfkxig.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwxjtlyux.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gisfhloqm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwxsvahi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gaqjtmqwq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gilpubvyu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjdogxecy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwspbmlqh.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gybmqjxeh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gtiefdtpy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gdfgwrwjv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gfutjpisb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grmfuhhag.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmpuytpnp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gykgrezvs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/goxmtmmlf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gyzxlgvfi.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gwlhwaisw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gmhmvlcvn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrbmhdg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gqjppnszv.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gxdpxwonq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gjbfvkocf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gjxozwplp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gqoayyoym.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gpsfqdhaz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxhjcjeow.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gpkdhwtbw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqmirbhjf.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/garscxnxb.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gkmuwzlbb.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gtprxbytz.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gsooqsetr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gyrkrxspy.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gilvtvdfi.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gnbfodzei.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/grrevngqq.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gidzkmrso.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gbmaduarb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gknzgetfj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gckcbladx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gfljfysrv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gdpxnezqu.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gydjbkddd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gcptnlmvc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjlgdtx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gahokeaex.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gvuiurxeg.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/grneduxzn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjrydnuzf.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ggbahshox.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gemmjbwzu.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gkmomkgdf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/glfuxjmrs.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gnmkeaytq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvxrlmzbt.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/ghdcajbpi.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/guosvfuio.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gklqpliox.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfgkfcusj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gownidnnf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazfdvwyo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmvlljod.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/ggteasmqt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gsgiidhwm.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gqfaheajh.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gabxpxjzq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gavpnpjtv.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gfsnoiolf.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvxmmetpy.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwlzszldw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gulaofkjb.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gzpjomkhm.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/ghxfniame.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gkaokorfa.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gwvjqfjza.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gzpbgpzlh.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gibcxgpvh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyjbinaks.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbzycmpd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gwygmluhj.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gmvgdxzgu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gegklfznx.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gubdsiaai.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/girmelorm.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gfudquscy.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gxhfwjbbu.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gjietboep.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsmpabmfl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gbbbdudwp.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gbcpnhntv.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gojbusatj.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gyzyzzddg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gnmokwkrk.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gbgayqabt.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gmdorofgw.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gflhzrtuw.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geocqaqlj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gpnucsroo.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gvuwjzikd.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gswyhvzxc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gekxrfzyu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gmyqisnoi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gkjpjjcxc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/getfrktgz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gnytoqkph.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/ghrlugbzl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gqalcmtgd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gyjtnmusj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtbwqyotl.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gyptujojm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gqmgalgnu.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxikbruzn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gfahbseli.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwtrapekr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gutbdklmb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gtfopyrtv.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gxhzxnaep.sHtML


<!-- 参考信息 -->