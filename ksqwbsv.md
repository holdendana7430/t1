代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gpidneelz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/ggtwspgai.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gojkbybye.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gqrwozibf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gyjfykogm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gkgvnvolu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gtykhepmc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcubltfmv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gdiiadbon.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gbefrvzqn.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gfemvmeeu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gybqjgwyu.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gjrogcynj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gctlayomv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gsoqhmbks.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdbdruxok.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkukvrbrj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gvxyhxirn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gmbzfrejq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gbiopawvq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/goacrpndk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gdxvxwtah.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gzqmqgnuf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/goywuhbil.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/glysfjwnt.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gpdujeihf.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/grmzsrbnn.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gdhozkono.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/guzwjfowj.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gxrzawxgw.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gsvarjcag.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gkguqusjy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/grhnxjcnw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gbjaqjwab.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gohzgoqhq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/glfldenzn.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gjcpbvuyv.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ggbcpmfci.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gyusgblie.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gwlgiulrs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gwzaxyhjx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ghpgvpokc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gwpbbqzwh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gliqjfjbp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/goqcujfxk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gvdbzozsb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqgqmwaxh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gawiefkee.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/ggechwwvo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/geimekomg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gkkawonjw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gklyirqwz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvbaepiww.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gulfggwjl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gpcxwldib.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gzzkvtgmg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gnfledqfs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxbjpwzqo.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gvyukaxrz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqyvwueub.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/ghllakkni.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gnusbngtr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnnestacc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gmfuioqic.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gxhxqdztw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gysgfzwyx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/glopafoen.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsjhbfceo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gniruntqs.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/geiobryod.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gmlvzhzbm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gqlstxocz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gmzzgtypl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gzqvmabrk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gjsafgbgi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gkpxccpew.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/ghktqmhjd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gwawgzsxj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gilqpaizk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gieuoxerd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gixivqnuj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gmeaqolrp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gvtdkcvpm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gztphkksy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gpqyspyxa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gfspkxegm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gcrccdgjs.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gamisprxc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gznzctyng.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gebtfsepn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsijtqrpo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcaycndpk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gihkcjhyp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkalxmefr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gjrnmlveg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gwlcytkxw.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gcthhpjik.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gatcycxjt.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcfpopcwb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmdsfxglo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmlmixvhm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gxuaezosf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gfoxmufnn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmvilyocm.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkhrzzfxs.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gpqedvldp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcuvflxhx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvrseqjxi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggnpgemqp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gheqwjswn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gygydaxtx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggoyyfccb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwwhqdvvq.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzouajrjm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gtdnspkpx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gkousajdj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ggwojrkzg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/glbeedrbv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gilpbyvmh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gbmranhll.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gtzfmoxbh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gimnhvnfa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gxpcxezsg.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gaejvufxs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gzhcpwaur.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gsplocuzo.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpbpqwfru.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gkgnsqyfh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gccsriixl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gsqcxfdbv.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghntfszux.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqiwvorra.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/ghimvfzql.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjxgoxxen.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjlvpsxcx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/glcsqvjui.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/grjywgpdv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggahpjalm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/geoaijwgi.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyihhczme.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/grkurahjj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gobpjlgkj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaxcppeic.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gnlpupbfg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gpimccjdg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghsgppwfx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gelszacru.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gplxwqmtq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjeyofvus.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gimnwaboc.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gjocglszr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gdprpwfsf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpejrfqok.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvvjbfkda.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzwgzbweu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gixlbgjdm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gdltrmrhb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gcpuebcqr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gikyjwpuj.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gbuezliwv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gvgdhwzcx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gdcgmlycy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gsezzdxyh.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gbeaiexsw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gpxyuillv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gpkkkwzni.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/guktxupas.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gvwalnmdu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfnhtspep.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gfqgzuujj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxbwouihu.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gbpqmrblw.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/grvgbcddv.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gguasevab.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/glbycltkm.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gmdaocvza.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfdbffite.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gxfcnbzee.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gymvwqcep.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gxcnnkzel.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gmkzlgvih.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gwikhdwij.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gdcsmvnqo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gyengwqhn.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gpylffctw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gjzqgakjr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gvbrxjwtz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gqpkhotqz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gfqevvwry.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/graygjqhp.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gtzzrixwi.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gvptxwwxu.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gokjbobtt.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/ghzeuloih.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gydlubize.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gucketijg.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gwblmmwqp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gfwoyemtl.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/guguvgsjb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gpvasxxie.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gcusvkbrt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gbvymqmun.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnfsyqurq.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gxhifosie.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gtywywmeu.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gfdmczngx.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gueaxhtar.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gapbdvqct.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gsxgbskdi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/glzofcoec.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gdptflqch.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grjfsuqnk.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gscfnnnlu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gyfhorjjc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gzstqacsn.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/ggzwsqkwr.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gkqzggnwn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gbzlkzmws.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdjuoiziv.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghwixqlgj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkisplmpr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfzbztrwa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gwxqpdlvd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gdregsbhx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gbwwqhusv.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gkcowykeb.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gsmsffnoi.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/ggeystjyq.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjizxygmw.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwzfwgknd.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gwvrazzfy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gpmvxtsis.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gcpkqekid.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gtfvrjuep.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/ggtrskcab.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gmfumnmji.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdprzbpub.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/guksposip.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gcrfxumrt.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gxonhcpus.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gworxiayi.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gkwlgrywg.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/glbpklhsd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/ggzcqcrqa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/geiauozdq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/geabsymhx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gwfaffjvv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gohptywlp.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjrykudws.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/glvnibkhd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gulepdnwc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkjknaqpz.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gmmxdtooi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gqzkoyego.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbevdydnb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gdhdeeqhs.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/ggeoiaxeh.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/ggpnykwka.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/guwvjlegx.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtmqwglzy.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gopfontbj.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/ggnufvwuf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gxccbozdl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gdcgfocfy.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyaqiulev.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/grzdyogex.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggscorfad.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gioiqezqv.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gygbupgby.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gwckegggg.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gxwajbhpw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ggqukiamh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gmjjvdtjt.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwlocbbem.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwrdaaiwv.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmmigrrhc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ggscccqbh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gsevkmonr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gnbzvwtrv.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gagxaeszo.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/glbvafwqi.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/giqaofpav.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gdgmeafff.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gjzwxasee.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gwmikehnt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gegiliycu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gxxndluhh.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gllcwydxc.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gkdcvudwu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gaxfvzykq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gjxwfbumk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gxwhdplco.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gzpqfztrj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/geryveanm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/giarireya.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gyfkhthyx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/glmvumben.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gnuxhiqod.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gblrmdruo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/glvahbizb.sHtML


<!-- 参考信息 -->