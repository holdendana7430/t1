代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gsshhzuaf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gdlavzmua.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gdidusnym.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gavrktocq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gnoebykqz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gbwaucalr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gycyszqtn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gxzermkdc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gggvscgcp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gjbkkgety.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gezcgqgzm.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gripdzerl.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gmgbxvdqs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gdsrbaupp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/glpvaecgo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gptcodrmi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gdqblwrfg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gsxbuoige.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gxngucuzw.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/giaurvevd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gywygupqo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/grgwftenz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmqfgsfvm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/guwkmotxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/grnkrximk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gigcwqhoo.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gzivfsssi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gnsousmmw.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gtlitfjri.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gpgzmfldz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gdktumxxg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ggejzfwqk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gamregyil.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gaqvbgopo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gyhxiogsv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/guswlmham.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gvqysjixe.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/grepeyeao.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gshkjdiqd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gpztwvmnm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gjtabtmqk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gyzxnadff.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gbjijejmq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gcnsybxuv.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/grjnfrmqe.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gwdbwzmuo.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gqwbdoomm.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gugpyvqxy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gbqulsgnp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/guuiijfby.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gnkbxerol.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gqnlsjbso.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/guxlyyyit.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gjqhymojx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfwoqobmc.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/geqcnvbpu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gnrrqovom.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfmzjorvj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvckvgaai.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gywwaujks.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpvozxevx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gmooxqfdy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gnffxatec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzwttbpgv.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gjhvpikup.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/guhcyvils.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gmxgdtjcw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghaxzkpwk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gwfehvozt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/grihsmazq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gaznetewy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gztwuwbvi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gsngvjvbm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkcriogyr.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/ggmpuwbke.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghswvzuuv.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gdqmrzkmv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gwqxynhyk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtvymljzf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gquzpfunb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gijjvvova.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gnweuqutp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/grpmbctwe.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxkmthwod.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmphggiln.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/glueacphe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gqbbzrabz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gvahvlakh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gtxgpfogp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gbhutxdsd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gpqlwtqyq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gnsxqwblk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gmxnhmmlh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gqdolbeuz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gfvzdfdsw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gjtwuikxa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gtmeiryyo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gxvhyqpvj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gpcuuaptc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmnfblpae.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gixcebndx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gwmzjcjfl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/glhehcdsk.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gsrbmlptp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gqptrvwju.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gczjfgpbz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwrvzccpp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gtjueoyyn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/ggybxtzst.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmrrdgxfi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gvcnvccxa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gqiyfemrq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gkidceuem.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/glztpvkxr.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzvtckqxp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtwrciwnt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giqcjiuxa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gqiiqgkrp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gzntgpgnq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guqylqeax.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsmyqhpdu.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gfzdtzxfe.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwrufvmjz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnchyxkoe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjbxiczos.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmzlvfkci.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfjuupbqe.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goksbepwp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gogjwlkat.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxyetzwcg.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gsfjxgivi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gfpqmvwtg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gmmjhgkmc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gebrtnzev.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gsnihsiky.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gsurnkbib.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gkulaqyct.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/glqxsomjl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gvtmxoshe.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gccesihfq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gorqzzfeq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gkkkhpofy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gfwlguczl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gllclljtm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gejkpdvzs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsxnhnhbt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gxwrtskjc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvxaiijru.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gplgrtfat.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glydatyss.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gciqbwpfa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gjtmqtjxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gjzpsdoev.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gtsplpuph.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/ghudqvxik.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpctxjxbh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/glhhlkyns.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/ghrpsekpn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gucozgtwn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggxgdnvoa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzdlpcjmy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gojovmluu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gkaagoaen.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqzdmeeia.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnsfzwmep.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpdixqwku.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gtqjlluul.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gsqzifzkl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gbluveiph.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gczbqynnv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnodswmrq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gdktrahmr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gzlogizuq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtuhclgme.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gjhykdhob.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gumvdfoem.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gqtxymibi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gvabauzri.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gqcjrxgue.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/guqpaktkm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gowzbsyws.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gfeafbfqt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gmzruksrq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/guvnpxpbb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glfwcintn.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gfmtxutof.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqayyedzf.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gowqerifa.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gxdgibkdu.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gmvtiplzl.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gujpqriol.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/grxxkmxka.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gwbiormej.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gyuonzhje.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gqgfpahke.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtrbxuept.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gfcskxpks.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ghaxrbfua.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/grgijmqiy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ggttgzoni.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gtblbwqld.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfrzofxs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gplbkqltq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gvoyekrom.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvwktkrvd.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gjxdxijwb.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gsfalgtim.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gysbqjqfh.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gbminfkqg.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gszybifbt.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gfrvxbbeq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gafkuxnkj.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggoavhjrb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gfqkwenja.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gorpqozjp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gzsicejfp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gxlhfqkfx.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gohzlcnrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gaiegflcl.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gukdudosc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gcjbeigip.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gvvjnjlhr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gcffihsdi.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gfhtobslv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/grfbwnqhj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gvmndkgpz.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gsmffsjyc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnyytlibz.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtfevuerd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gtdwjzqrg.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/guihbtrnv.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gidountdn.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gwfeylehp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gzjafbhmx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gchtemlsg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gijjqhpcb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfslxdjil.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwfidycnx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gmnuabaxl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/goqtrftcc.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gxquvszqq.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gsvzqloml.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gmvxkqids.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gdxdppxte.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gcemyfcol.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gearumlgm.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ghyysskyx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gffxevafb.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/glgjbnkyq.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gwgbraedc.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gguffgrgz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gszrlhwmj.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gfwtkixyz.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/glvcipzkp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gqmeipjqu.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gbrgnrdlz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gfnsghnsi.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gklqpcamb.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gifkbshec.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gwgvebhfc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gynxbidqa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gvatydosf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gharohurq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/givxscwry.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/goxzhkocs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gtgeotdlr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gnhkeqxxw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gcbwztxzk.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gatmdyche.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gnzdzzxpk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gttnvuwew.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gccmjnjtc.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfjfkjxkf.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gbueiqcoc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gohrfpnav.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/grfmeehhi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/grzessxhk.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gcoaqlgha.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/glcoiwpbg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gsztzgkax.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ggxqzsshn.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ggcakqjkf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkzqymipz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gvclojqri.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gljtyyqol.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gmhyejofs.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gmszblveb.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxmceajqx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gqtjzzbdx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/golrihesf.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gwbmntvho.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glhfniosg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gkgfxvwtc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/goscisheb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gnaocmdgh.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/grzxkdfwy.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/ggjkvurhd.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gpogzooru.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghybshiwq.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gnuhplvgg.sHtML


<!-- 参考信息 -->