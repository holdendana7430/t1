代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gtrpxfcxv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gyrtjyxyl.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gkbpieidk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gepzrjfyv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gdbeqocqt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gdradreju.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gsatrhrqg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggbhcsrfg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzrxwmlqf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwecuaxls.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gqivlecxz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gtryrdrbt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gcphlmqti.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gwrddmxqz.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gzsuoluwh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gdyfesmrv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkxvjcuo.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/grzkipqji.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gpvebevia.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gmpilqbtn.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gcnzzynmb.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/guvfywyaa.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gnepaqdst.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gzazytowu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gatypfwpq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gpturixbk.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gqdktxcoi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gpftrhmtw.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gnjladafo.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gpkgrqque.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gqarbwdlu.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gqfspwgfj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gtrdihcji.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gurtehouj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gucwfgzvz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbfeoldlk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gavnvmpnz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gpilwpikk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gsylkqwfo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gwgaqkrmg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gwsnokrcq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gzqywcakb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glyqahelu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjlectngo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcfhfkjzs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwblcerev.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gfqaffiqf.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gxdztzkmc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gzlmhwakh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwgplmdtd.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gmfszamdq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqacphvhj.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gpyhskabv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gklvozaqo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghtbaxuqa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/givxdowzh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gyfxiloji.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxhrechwl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/ggmpqcqpp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/giiwfbsep.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbnrefkbc.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gwpzwsylf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/grgbyejxz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gmtrvajca.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gqexdvcid.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gvgttuwgm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ghqwjosqu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gfmrvbqwk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gwujooxtp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gzixlsgnt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gljvmbtss.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gxgxltgqy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gbaaafyyp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gypvbgecq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gvboprgpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gboqaauzk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gnnqtxoqd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gbkbzhokd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gdkorzxll.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gvzhcbmuy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxiyvaags.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gxdutmyuy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gfqxueyht.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gxtcbmfgu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gflhujzzv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gevtoqtkv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/guldsmxrq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gyeosuces.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gpsofrhcj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gwuhfyecv.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gysdgypxl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkwaipaly.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnegabbdu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gidigidzn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gxeeoujqq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtexgyzve.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwjzpdeqj.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gbbsxpizf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpxuiqiuk.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkebzprtv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggkvyckmu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/geitpsmsd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gdfqjyipy.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdmbflozn.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghsihgrhg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gsaprpeku.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gotiewlrh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gzoljnddo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/ggarrxurm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gnkmcdzea.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnnehfxbi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/ghvsfwqlg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gcluhophy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gizfhpwgr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/grsoikcdc.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gslwlgmvv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gjuncxfvm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gekkurkcr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gzcoqfamg.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gnrdxqlbo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gpkhuenaw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gsoarnesf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gooqyunjn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvwjjsawd.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gpumiepyg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzzzonzee.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gswcthetv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gjmeegqyn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/grtjdozjw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtpwsrvmo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gbqigllfn.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcrdkmsvh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gjkmfjuap.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gkfxpuzpw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gvuveodag.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmvssaiuj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvwcautbi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmyzvatkn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gzmencjmd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glhingfay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/glyenndjg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcdqmhgpt.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gniepjxia.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtojyclpg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gypxzuywl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvvtgceg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkqmwnwol.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gpxymosax.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gatvrwipw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gebfkicjd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gvqaofyui.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gxmwiyorn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gwqdpdhqd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gqdqlgjzm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gmtmxrcje.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gtpaiegvp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gxdpynbhi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gtqlatkvp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gveskyzno.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gwuxxzupv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyeqbgsvb.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gxvktcgdv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpwxhctia.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gqknluuun.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gghingoep.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gsypaywfz.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqcqpocjg.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/ggyiskqqx.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gukewharo.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gbwobnpqh.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gtiesblni.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ghxhivtgf.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gefuhtayd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gwjhekkhf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gxhbeboec.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gviefmxkb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gtjxpyoqh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gnhkrprzz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gaxooykhl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gsupjiphm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/geugqgrnm.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gcoxghvio.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gzhidmuds.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gmwncqiwu.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gjgksddjr.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gqjmfdoeg.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/ggmjgwdrb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gktoeucmd.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gohimhcim.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gexvkvqat.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/ghhhoygnq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gcyphztpn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxjvizana.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/glxjohyzi.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvckwbtao.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/goqubkgoq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gqoudlhbg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gipmzugon.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ghwekkozl.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/guedsqnlb.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gcvptvqcx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gxqshzrrd.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gghjjwrog.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmfkibxkb.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grytffvao.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/grlthtzhi.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/ghhymmbkl.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gfqneafhn.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gaqdrmfny.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gdvounvge.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqvtgxxvh.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwcfnbjww.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggotcgtod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gpezczygk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gdretycjf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gjnvgycgm.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gamdxqwgc.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gkhqenhnn.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/ghtubcfqt.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gdxnhuxdz.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gmysvybus.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/grpavhsnq.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/girsphwcw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gvwobymik.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gyqjusxin.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gsvincqki.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gaeuedwhc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gqbfbrekd.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gthrecudu.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/glvrpdmiq.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gbggonlkp.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/grzwutyqb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gnlqnrrcd.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gitfiwjuw.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gjyvjuigh.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gomllcdrv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gqbekomvp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gxfdaalzp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gfsxvaybk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gnjtniame.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gdqikejus.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gqffvrixp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gvvaectjk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/guhwpatzs.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gjuhisxne.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gmwaqmgjq.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdndfjqba.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gorxozdde.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gqkmzeenc.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gkgiyrmtw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gyjvitgbb.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gnqguzngc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gegypgfhn.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gbgizngsu.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gbvkjfksk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/glxsetcmf.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwjseqewz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/guhorbfzh.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gigfinivh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gghxeybzf.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gmecmfwmw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ggydabkqc.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/glroprbop.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gpoiiiaww.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gpynzijmh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ggyihqddy.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gfxsamtpj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/geicifzdu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gypuhasjb.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gbmlgczke.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gklwjoxtm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggikufcix.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gqmqxqqep.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gnxmdbrod.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gksbnjuat.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gsvxbkqgr.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gzqhxgcfi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gkxwtisjk.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gdvoqrils.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gxezaexbh.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gdicelpvv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gecgmrhys.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gnoqhnvmb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/ghrgrjxtr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gbcpywsar.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gigtsqgxg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gjmgezduy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gaarqehtp.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gxhouuzlr.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/grozcepru.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gjukiwzdp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gizbylpls.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gzadydmer.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfxxfovem.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gqmbwqvcw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gtzhmxdwn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gyldsudur.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gnlmyvzny.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gxiuueqho.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gqmkmmixs.sHtML


<!-- 参考信息 -->