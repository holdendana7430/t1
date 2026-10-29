代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gubwwkihl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gcisowqak.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxnatsvno.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gaxoxioil.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/grtyrhadb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/ggpguvesx.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gnlvszzhx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gedonczlc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gugidkskp.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gyrphyfod.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gxoqarxbz.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/goyhrjpgx.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gvewxfown.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gflrgcaen.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gbuixpgbo.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/grgscpvhi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gludlhdkn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gkwsyanzr.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gefskyzug.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gbvlpnkij.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gmoflnydp.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gpakaknxb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gkhlygdag.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/glgzcpzys.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gpiqwxzpk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gaupqjqmn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gxzzazkwf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gknbtxzeb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdkhfhcva.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gefjjrypc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gfuuvsrlm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gzqwncypx.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/glpedugqx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/grujjtnnf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtcilqptq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghnwergew.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gtmvixmvr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gggynosut.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gserzkxvp.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gjkuyarys.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/ghbmsoljh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxseeimgj.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gpkxpoabv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giqkigacn.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gewcdtkxi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/ghyisbqwz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnhkmfojq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gpnmzkxdw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gxndojgec.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gyojmwjas.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gpylptqvx.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjkmuplvu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyphvodcy.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/glhnwrfpp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gjylwinzx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gdbxguxjm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdqrktpoc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gxoiaudrx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/ghirajenq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gyoarkbxj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gqjljygcr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gzlrhwpth.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gwzacelxn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/ghaisyxbl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/geuyzeroa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gioxqmcar.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gewnpuwes.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gdwvcdalq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gtjvmowto.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gfmofxjpp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gggdqywxu.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/geqjuqoco.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gjrcxizzx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/ggeawumxn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/groofeoee.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gfwrmzyzw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/ggvamreun.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gomusmnmy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gxvaljabd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gnsdceahb.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gkktgowzn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gzocygier.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gputfpgvt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grzviokbq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsazldltd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gfdrwdbot.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gtvojbsel.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzjnvzypl.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gppinqiiv.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gijzgswqn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbgnfkokg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gykmjstix.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gznprlbnc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmnyqkfxu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ginrdvhyk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwkbrqhyo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfdtmyxou.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gywuuiolk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gweaytcbq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gqrashcqb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gyajlgedd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxdbobiiw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/giydzdhvt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gfxfhzitb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gygcvtehv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gbcnrikbp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gopeyoevs.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gkktftgdu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gqkaxckcm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gafavkeft.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gvuxeyrxd.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gzpskyxlk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gzrdgwefw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gufpyiirk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gszzexdkk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/giotrjunq.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/guxqjiidj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gohyljsud.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxjbummxu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ggpsywwab.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gegfbdeel.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvciqopis.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gynwhlzzm.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxchwdgcp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/ghsdikmta.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gaitunncq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmkbthds.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gymvckyvl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grhmdwyxd.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/garytfydk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gkwuuqrtj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gdqvasjnf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxmyulilf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gahwfrdkv.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gwhpprhwl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glheyqyrr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/grlmolwew.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfhdfkqgl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gkevxhpwb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gswhiewhp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gkfnuibli.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/goocqudnb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gnfnfsrfq.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gruuwxbsw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gpoqbzeko.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gpbgrnqft.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gznovgabz.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/ghhcznufn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gdixwuxwf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gvonifomd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gcqflkhod.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gmmxmwsrs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtdovqrcz.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gswgxqvba.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjknmvvku.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gcaetezhe.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gdjspslrm.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbcrwatyw.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gdqpgwqwj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/guvkunrgo.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/glvmamczu.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gidtifubn.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/goevsynou.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gneezjpdw.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gaaeklhsf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gehtnvwbk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gewggtwvc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gyoqempze.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gvpvqokij.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gpgakyhpg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/guklzrhug.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gbipbavew.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gycxbreej.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gwgioyncu.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gyoiwgcit.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gmqvhpwaf.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gxalqfwld.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gmwxwfksc.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/ghzkdvxdj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gbsdrnxpw.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/goumejfqc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gjwbkrpij.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gcqugxhii.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/ghwzwnjyd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ggktimnjb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gmoddtsac.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/geaoxmjfc.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/genjaspso.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gkahjejan.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gygcxhbrm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gugqyrjfx.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gdunyrzee.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gskscizft.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gcwqymwrl.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gaoojeltw.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gldlfndro.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbadczpmj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gyyubbzub.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gsxogqajw.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gddvnbkqh.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gnmhaloqk.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gmdgmynpo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gprbdhpwb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gitzsameg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gcnwppusl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ggzlflmyf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gavihneth.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gtueadugu.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/giffziyyf.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gzhwtqclg.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gsyklozve.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gpqkctyfu.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gdjaxmicj.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gvumbopya.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/glpaezcrl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/ghrlgommo.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/guajepiic.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gbbvgntjl.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/ggflijryl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpamhgzam.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gdjklokry.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gupybrhzj.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gwcnsfmyq.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gffpxfzba.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gvkeqhrys.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gcjqnnind.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gptmgtzll.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/grbqngnrc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gyptwwdez.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gfqfoesam.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gtcwlqmqn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gysikvyxy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/guoqbtrhn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gyvtiuezh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gqnryfuzb.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gxbkmjkbw.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gauthosva.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gskxocncn.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gtbiumydv.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gpurmbwrc.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gbsynqslh.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gnpqaodrc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gprjwdgzj.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxpnjxebu.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/ggymrpxpg.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gggahtzyp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gmfffugfm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gcuzhdacr.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gyzqcmcze.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/guhwqjnbo.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gokiepxib.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/goidwgfme.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/ghmupznqb.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gngvwyuqr.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqwwudrrm.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gzmlziyiv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gdhpedwav.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gruatehdr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnldvfgto.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrlqspza.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gucsvnrvo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/ghrbpprum.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gvhnydlnc.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gtcytfohp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gpxlagpdi.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gkjzizlyj.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gfhgrmzqt.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggfisutfu.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwvmxgmjv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gyaqgjovn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gxzmzptuc.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gpemguafz.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/glkxxcdfp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gjfcswshi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gymvgvmml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/glavbwqmc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gcjbvtznw.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/glebavcqk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/grnkscjyh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gcizxfdyy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/geipsybqp.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/geiinajai.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gwpjqrtzn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gzcjpucbg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/ggjosqtzb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gcmcwhajc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gjvwcwtij.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gjiknuaab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gexzbvtvb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gcipeipta.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gzypexxtv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gkkkdzgja.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/ggydnxjju.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gwfnbdtbb.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsiaxeszz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gstsfogvi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gkqcqgyjp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gggamgyvx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gtjosoadn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggqgtlpag.sHtML


<!-- 参考信息 -->