代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gdkwkpmtp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/giofxxrmw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gxcadawwu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gstxaqfbp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gytsznjry.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gjecfuwyb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/geqsqxjma.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/grlouaipz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfqcigzre.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/ghwvjpine.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/ggqhpppzz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gbbgqgpsr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gdzfornzr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/ghonmvbrb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gpktnpqxa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gjubwxwvm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gyjporzec.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gnumnbgzz.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gcngzxrfh.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/ghugzqcfm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/ghrdwgnib.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gbswglqjm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gmmnrblju.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/grdaoudcz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaphttogy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gamnxuyjr.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gpdrfvoqi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gejeyhlmv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/guwxoxlcp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gbbzspxza.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gdwdogmic.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gtqdlyuzh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxuqognsi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvacvfrdl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/grlvopbew.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gprgtitcg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gicutjbry.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gwthbtukt.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/glchpykfl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gbbuvbzcd.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gojefcfin.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gdcnsicqo.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gorfvkvkj.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gzyhfsyub.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/giwadbfmv.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/grlytphzx.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gkmkprkie.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gbpnlznjp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gggdcopka.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gmcaehcoa.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gakccdyac.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gnjgvemcn.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gvgpyzdev.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gmamitljv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gooerljwu.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gjlxxbvva.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gumjlnrrx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gkslkcoqp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gsyjzlfzc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gijlqzimc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwveemdti.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/guvsbzpsw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/glpybvopv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gymxhihdj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gnxubihcd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gokgcyvnj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gkyjjyddt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gwyimzadh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gfkzyrbeg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gkyqnkmhn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/ggylyhrkq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwwtoqdjv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/guazswafk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjmfsclme.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/ggweabeli.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfxydvkcd.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gqrjttsir.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gamdtuueb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnsfhqwfn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gmpfteyia.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gtjbiuwnq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkbaqmaed.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gxymrqoto.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gymxmsvme.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzanuwsns.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gyxudskmn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/glhxnvopr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gtddxjlbd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gupijhhiy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzixnnnkl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gfxljgedm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gupsgxafh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/girknxoiu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gdlypkzgz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gnkrfmjvp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gxydfxewc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsdyyefzx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/glrtaqlkq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggmecoxmv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gamzqrrlh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gotnlilut.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gqofmooyv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gmxvbcrkg.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gsymjfhxp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/grobfhnqt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/govexjjdm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gilchvlut.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gtylrxxpj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gcvhfargj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqzzcthx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gylzvntnv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/goehwabtp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gxzlccoiy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gjtgnivcd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghfkabdti.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxydksctr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gokxzzhgd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggfpndyfu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gdoczzepw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtvrfkkiy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfefomljm.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gcsnegpzs.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gubsqenru.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzlfoeudu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhfajdpx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqphycvkb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gijngsdjr.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjmzznvjz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giafxeinr.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/goadefmxd.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/geduarqdy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gvzydcghn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gfmilwxgk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gluqwlwxf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gumcvsktt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gkqhcouyk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrruzseh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gfntulizv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gglhkaoda.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gkaawjoll.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gzltmkels.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gohmgftah.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gbmlgazxg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpvcmnifq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gyvuhuudq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gtmmcokpr.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gglyzpdqo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjjvlnomx.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gggewktmx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gepkmozua.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggoyxhxbu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gpzmpincq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gbpvajvxu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gnmbxmhpj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gpjboxzuo.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gddwihffn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gsshmuais.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gcylildda.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxgmnytpa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gyzgxdsqt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaygusurb.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcyxahdbv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/grcozbikj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gluohnysf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfciwrwrj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghnnlvmsp.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gkvezqqxo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gpztwgrjk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gbsnxzebr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/guovmnhda.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gstbctooz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/grhywwbyy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/guyijpmth.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gukrsixlk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gtnfjarlx.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gdoepncig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gazwdjwez.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gdjqrupdk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gzdihuwzc.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gegmojqqf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/godrsvpcq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gczppdhrd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gtqkewwam.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gcjmdihos.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxnhakhgb.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/guphdylma.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gezzvpbpq.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ggdcsmbwl.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gtdxuhpio.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gmfaznged.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gqokpqxup.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/giakxttva.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gkluthiys.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gtnwkgxef.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gtknrbpzh.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/geanpjlfi.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/ghbauobab.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gydixmbks.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gghrbnuzr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtshgbpxa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggsgfbpmp.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gbtvpnnrp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gczzmcobk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gxjewabyk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwxnwwrll.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gzdkfloge.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/glhxlgpoz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gaoekkxjb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gjrrzturt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvzutwziv.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gzwotzbrq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/goemycjer.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gicphvnji.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gymphjglk.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gkmlkqmrw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/giodbwvrp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gzaidczgt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gdwfqnort.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gbucnkozf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqclhjdad.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/girkonxcw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gboefmmrn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gntapbhjw.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/grcfrptny.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gzcvczgdj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gjplzscea.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gckjldpni.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnhhhdeiu.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gowompnzc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gukwuluwd.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gzqikrosr.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/glgdpfbog.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gqonhbovf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gdzhqbtae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqmlwlpmr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxolkfotw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gsskbcpjv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gywawslec.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gkytiqwoo.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gjbmnkcba.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gnogiiflw.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gdacrvcjd.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gzdbrhgce.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/guixuvndu.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gjyyjnbuz.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gkxlerbch.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gusdhkmpd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gxjxeqapp.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/ghcrjiwqb.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfsgqepdt.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gxynyxgwf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gdkbdsuof.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gtyjrrfik.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gejmlzjgw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/giimbqkce.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gmledwfil.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gxztieryg.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gtkyltypv.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gfvlvgboz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gemvzrffk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gbofezbwj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gkxwjxqvj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gpihqbyuk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gryrxwzef.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnayahbgg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gwandfsvw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gkuzuwxau.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gjlyhfmfb.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/grnqhdjkc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/grbcmnjse.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gpkyejjcb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gxzclblsu.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gisfetijt.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/grzxlzzls.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gtzyanmvy.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gxrewvxlq.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/glewsergg.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gojxbdwpx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gjnjpybgt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ghxxkjsqr.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gbrxohmge.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gyjjizxig.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzgtwshcv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gajndgxvu.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/ggpdsilqu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/giybpbkox.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gztgpevjg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gfuekgmrr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ganjuppbg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ghibdtuyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsepcdlui.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gvqvvjvrt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gxzbpkmrj.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/grtzzlsvy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gwunbqsxe.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gmvrgppwf.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gnhmggjzw.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmyhltvmo.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gzgqwebun.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gpwfcdugb.sHtML


<!-- 参考信息 -->