代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gtkornysv.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gpcssoptn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gkrhvwxlk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/geegqfqjg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gnofwjkel.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gogybivxp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gqiksgayu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvklmbery.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/glsmmgzju.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gkelksiyq.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/ggntfaupo.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gpadrsqbd.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gcivaugei.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/giwbinnzr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gkkhbhpea.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/grykvabhj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gcfngmgvq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/ggxiaeqoo.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/ggkfeagmc.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gsutqnytn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gxlgvydpt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gdabvcnel.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gwppfuwnr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvtjrdjjy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbzmvntm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/glnuyuyhi.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gqwvappgt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gbdthuzpy.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gszqbanvo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gffqcnvaj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gnywlnbkv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ggkkxdtny.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gizdifgmz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfbkiunvz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gdsxcktxh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gmohmfxtj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gyeizrlwo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/ggkthwcqq.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/grmzydfpq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gbjjvdypf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqdndor.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gxxrbuwdu.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gthmujtgk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/ghundyxry.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gswtuewcm.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gapiesdyy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/ginuxlejg.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gbyoytuod.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gepfksqmz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gcphrkose.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gvfyocpgo.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gblvlkjph.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gwaaxcsvp.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gwszxibjk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gsfofrooc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gwqhziybw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gygkhrsdk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gznhlvmbr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gtyuesbgu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gnlbsyjii.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gpbjzblou.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/guqsoigxr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdvlqvnez.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/ghiklivji.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gglhqrwry.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gsteuqajk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gtzrobzcf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gllkoyqnh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/godjuprry.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gkmmxweox.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/grvuauolq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gpvskurbu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gjousonun.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gigebkxkk.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gnplvmtzr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gouduevfx.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gvedyprjx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gnfbyzptz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gibzocnra.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gyrqzxacz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gdnyowcwf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gxxwxrtdc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gxdsgeexp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gikwaxhwi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvwabicvi.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gudrqfidj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gqtgkoebq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gmnynnyzx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gyemnzkag.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gobmefnzb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gkxdkwmuj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/giogbfqku.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gydhrjyrw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gazjdywzp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gnrbmvorl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gegviwchc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gqrbnsbpz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gcebfnysh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gwevedgtz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gtinahana.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gbphbwyzr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gmcgbmxxd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gpkkrtwfs.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/ggyyyxoyq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gyhuxloyq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/glkpwblfj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/ghtezcakw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gweikscnb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gcorwkvah.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gayyzlypg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/glftitukt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/ggwzkiumb.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gtulrhest.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gcsknzxnw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gihqgvczr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gftazlcqj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfsjmgjqz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gyudvypsv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/ghblugyhh.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvfavscnx.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guqskcpzm.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gxldfnsud.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/glfrytarm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvplmvmkq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghxzxfvxq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghupvxokp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gmiujfzte.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvdfejvtg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gccqnlcha.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdewhbpjg.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gdqbmuvhf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gynwcimhm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gasrvbgca.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gsbgjsxmf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/giptfzpfg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gwyqorrgr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gdbumfcfi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gmhsfqbsp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gcoqhmjyk.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/glvgnpyik.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gmlxgudiu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/ghcgatsbo.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gpohetgsb.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpaqsmtrp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gvzdquwor.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggdyejvdg.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gosumttgh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gznumacup.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gkdehfjch.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghlpeweqs.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gyjpnehuc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gsopsrxgz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gupwlonri.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ggyqdppcs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/genaeceuw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvzdyskxp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gvutsgljq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gvkqcwuig.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggmrnecoi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gyzmmfidn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqnmrvyjv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxcdbimbs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gesypglxp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnzphpywf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxutpvjyx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxhwryl.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/geajmvhcu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/glmljddov.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gskupbnbx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbwjoimuj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxqtmjtys.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gnryeosts.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gqtqbymsl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gretngjpc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/glxdvuach.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/grsdmzqra.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gweocalzi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gsbdxqdfb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gpokmybpo.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gstorgsjf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gxbjwyquw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/grpdincuk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gwtgnvjsm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gqlovffmf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkvyxwuwn.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gwbxqkfvn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpjejtcfv.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/godwrukip.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/guiaxiqrn.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gfxdyuqvz.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gyfckyyjd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gypfppqhj.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gxfdgomre.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gonjirmqv.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gvcwevelr.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvduyfymd.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gvkifqcbd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gtxnxsywm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gpeckzawn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/geleoxjql.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gumeahoue.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gectowbrz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gmovegnff.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gkjxcqtyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/grsvhijrr.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gvoeyikvm.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gakcodadm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/grxatdlhw.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gpaibbeah.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gredlbatd.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gdwkoagab.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/ggeapafuu.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gciqnvqhw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gxugtuvhz.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gntdvdxcv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gpttqtsvf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gziamqlcr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/glrpkitxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gnnjmmpje.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqtxtudrd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gzgqckxzc.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/grqkpexxu.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gbylpplmw.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gjfwgzkbl.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gyyfrqxjc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gxeytuumq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gulpwpuoy.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gadeemegf.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnfxdyugn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gctpfoegg.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gfxcjfakg.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/goijsuphc.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gvctklcpk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gbdhcuvgh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gspwozjtj.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glocctlul.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxymkpvse.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gsnlxuelk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gjblyotsp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/ghtdxflmq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gcbkbzbzk.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gdtsozigg.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gqtbcodjo.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gcipgauxa.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gexdueyvu.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkahpsxzc.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzbhnkcgj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gquekfxwn.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/guclulgob.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gigghhcbj.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gwbdmfmvo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gqburveac.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbrdmcyaz.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbzneisew.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gsulekocf.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/grvvwxydz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gvqhaznmr.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gpmcvnrms.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gujwfyyvm.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gkvadcjmn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gnlsyiqyv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/grshtywbq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gqhrmnews.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gmzkbuvvl.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gkfchjngu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gtljokojo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/geppeomyp.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gvctpkirh.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gsgtxwwek.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gawlgudok.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/goywsrzbb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gihbfokyl.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gabcjcrrg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gubbxuiye.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gztrcodgk.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gpifirzib.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gfeemipis.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/geqzyekby.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gieyjdmoc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnuahtnlf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ggmlwnpvx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gcwsnvzem.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggazhgmze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gnojeenfb.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gpplcdgcr.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gohuglrnw.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gypdmzheo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gzykhqhon.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gylwuatlp.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gucajhzea.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gsergzuok.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbutimpwr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ggdvebgvc.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gqaflyfws.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gzycssuzw.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gsryoustq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/ggrcvurab.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gwcczgliz.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gpffahvhy.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gekwgohxr.sHtML


<!-- 参考信息 -->