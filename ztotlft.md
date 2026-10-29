代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gauadocvk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gsstkuyiy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gmazjalll.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gnerbcdsk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/glzozhutb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gakrlccmy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gecmehlpb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gfwhstcxn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/goqhriyzv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/ggdykxbgx.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gplyjmrao.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gqwketqbq.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gbqlwlkea.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gxosaacie.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gaexgyqnp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyyhqhxtt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gxsnvmuck.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gatevvtwk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gfxbgjgjz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gcesgxluj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gnqbappfs.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gtfklbcyx.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gvkmlofko.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gpysdevbm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ggcnnwqro.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gtoajxjgc.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/giolaujky.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gemuaggfe.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gmftykquw.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/glaegknni.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gxtnpeoht.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gcskidxkd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gzdxgqami.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gqpbdtzfy.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/glguxksqg.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gynrobnxw.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gejsbixiq.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gpofkemhm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/googpiakb.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gghqkildz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gzunxzdoi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/grfzqjivr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbocjisgi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gummlaubw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/glzuaciek.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gprsvpjaa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzoxjymjf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gydcuksck.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gknclqkxq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/goyckpnin.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gazofwtbz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghnvrrbvl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gygaudihx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gyolkpotv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gqavuyvtr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gbmtebaxt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gsgrnlmhy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcmocpzrq.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gkvlqndsn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmaqtqtte.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gaqxkzzaj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gqxbglhfa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmcjfbmno.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/golxgiqek.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gxymgdipz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsxjyxnzv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gjtyvzwua.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkmfpocyp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glhngtryt.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gthojmvsy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gbffnyfnw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gcdmsnjdv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/ghccmjkgv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvmqwrhoq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gpuailwlr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gdklqniug.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/ggeovwfoi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/grrpkwlzp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gajpxddvq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gvtuvbisj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gmkkzsjau.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzybgbdji.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gypfywflx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gjfpcljrz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gjffsrakp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gcbgfhdvs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/guarvuysz.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/ghxtuwdxj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gajachxhn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gysjfbods.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gsfhzgrrk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gnvygxsre.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gzfobossm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gzzhjqhqh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/ggopcydme.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gnhdhfogi.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gjadcgiqu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gpgxadcxk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggaoqameq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gutumtkws.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grenlrnnf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gocnhnrxb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/geyadnwpi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gclqltysj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxmuxvdiw.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gonvgunzm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/grkmrpbxy.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsnidwnfg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtepqdsmq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmqzsywpm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjcdjstjh.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpaugfodz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gseminofv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gazakvphx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gutibdykn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gtyiqecbu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwwaqrrae.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnweuiadc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/godbuzrcw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gizjiozsl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gditquqqs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gvmzogdis.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gjqzmyezv.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/ggdugzibf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gpfcvczvl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gdbrxixtv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gamcnzvhc.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/ggzmvaecq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/ggwqcawgb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gkhhekfik.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gupunhtdv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/geoklgrdz.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gobsfvhdi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzvwlzong.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwqbadlvi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gjstgupzu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gllvukdnn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbxhetdao.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gdoeqkqlb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpjrtsled.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gsuiwcjdg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gapqqaeas.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gzredkvtv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmqhyiykh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdiaqwigq.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkyalqumu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gyiddqmvp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvajfduli.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghqblexyk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpuzdgsyd.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gpdfngjst.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gavoimqyx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqrxmdceq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqquvidsa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtfjmktcv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyufbfmbu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gtdxinmgi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnmlxfidz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/geewsimbu.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gkwcgxwpq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gogjtygvi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/ghbgkcqqb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/grhsaecuo.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gmjbxdhuo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gqurwiowr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gllihaszo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gayzsjcck.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gwkcdkivb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqzsqnjbj.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gjoentric.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghkphwnwz.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gfexbicha.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/goqcxtexl.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/glkuzssqi.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gudkzrtum.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/guwnqlalo.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gdiovtndl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gwmydpuka.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/giulnojzg.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ggkwkqrqn.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gudmykdws.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gcojxwuxc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gdcksbvdm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gbfbhugsa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbtlhzxth.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ggymdhqbw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gpsbvvpbv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/grfoypqrz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/glzpjigtt.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gjhqvdpsp.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/geeiuxolq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gouwypktg.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gnaazbfem.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gycxqhxfv.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/glayqcepm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/goxcbiosm.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/guchganvb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gdemworsu.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/giqrcxulj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ghwzjgtab.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxpxtvbul.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gytcamkqm.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gcbqapsel.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gsuefepdi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnzayqonu.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/grdkkfmro.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gistvwdcy.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gvbsozasl.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gnufpwqvn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gymxqqnao.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ggczyfcfv.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gdvuefzqn.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/giswfwdyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gsgfhqpwk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/guvopomfw.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gguwzdtgc.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gmhtlqkzl.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/goqwxamzk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gafseeemn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyehacygz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gttqasxtt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gcwupaahj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gtwjqulte.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gvtvxjeid.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/geigjnkyl.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gwtewjcvr.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gysqayjff.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gfdgjagim.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gflcodugy.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gefvvdvgi.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gbjbseshr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gageqespz.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/ghcikepfr.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gufmxchyd.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gwehcdual.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gyifgqlcw.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/guhdgxnvx.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gfrkqjktg.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gychkzsei.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/glvkjdhdu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/goxnhycfp.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gpetwzxrm.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gblkqrztt.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gwyyzyihg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gpwenntmq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/goealqivd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gxyliciwh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gtixclxox.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gchdiijkh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gyeywghai.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gbnjwrunt.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gzxrfypvi.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gvcddnkvq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gowyingqg.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/guuhpfeqb.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gvwnduruf.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/groqijsau.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gmwnyoaoy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gkyekcyab.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/guogjhepc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gutazbqsc.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/ghwpxheva.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gsjsanpcu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkdsolzsl.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gkhdumypu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gosufbido.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcfeqahth.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/golmtmbon.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gptjsnvnl.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gtqdfrjil.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/glfofnsyr.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gzijobldb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glyanfqxd.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjlzxtkgg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwlwurtn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gwaijlawa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grwhsqzvs.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gjzieabai.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gkzivvgze.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/glhitclmq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/galggowun.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/geixhwnwq.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gsiknajjj.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqvkpypku.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnxylupep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gekezvexl.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gbspcrinl.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gdzngnxns.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gflhahonf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gvdopitep.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/grtysawnd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gjjfoiqxw.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gshmmrdjc.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gzkysfony.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/glscymcqf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gydsyxxwy.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/guqcrtzvt.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gknxmdhrz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/ghvfvdsmd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gzwfjgpxw.sHtML


<!-- 参考信息 -->