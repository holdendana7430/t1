代发 wailian999

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gytvfrmww.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxojgacy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gtjimkjzv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloyjummb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gkiafimwe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmpcmxuy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fanxiaobao.xyz/Article/details/gdixzfueo.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcanjrea.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gloaesgvu.sHtML

[F02] 逐行读取文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcvjlruw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/gstccxzij.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwngdzzia.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gffxbhads.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goyzmxcie.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gqzbihyff.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fanxiaobao.xyz/Article/details/gtuyzjqgn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/gorrksvqq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fanxiaobao.xyz/Article/details/gufivfwhj.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvhaaozx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gavgcjvdc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/glotdzczx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkxnjcyi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/ghevhcicn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsaouhjx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsugswpeg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gmpwaoshp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpfxknct.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbkhshumq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmmuakvq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmjtxmkh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzryugtoy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gqqjgxhof.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcmrekls.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkzcealr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnslmyph.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/grfcqygfy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gazryuwsg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiccdrvi.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/guoldepkm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvinvmijb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/grapaxgot.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdlfyiht.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/gnlqqmzme.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctqrtydl.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gwlhowxqp.sHtML

[F06] 删除文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiqesxtz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfhervow.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkenxglda.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkwrzjxx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghctovgyk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/ggkvahbne.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gfcqhhtuc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxufrgvfh.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gygzrpigj.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gorfpgwmj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkpwzjlk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhtoijpd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gkrculzjw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gdhhecjir.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gihwpbjpc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/genztlsqu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/gpvlyysev.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdfdrgwi.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfygdleg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gcrmctqeb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkymectil.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrxxjken.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/ggxmcyfav.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghibuzwj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstadjotn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gitrcvhww.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/grtszysrd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjfmngtz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gvcqqazuf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwshtzwkz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqksvnzc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvesczvva.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgnglsfw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/ghzhcishj.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glnqlbqig.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gghkwdggn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnaslwyg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqifdkwc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gkxoavuxi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtebsjewg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxridrynt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtgsbjwj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gexmazdan.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gxajlulps.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiyobiyi.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhdmivfs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvhngsso.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gtokmuocu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnyyfdssa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/givcacffh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/ganccziey.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzjhvlzq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbnjhcjzf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gdbnmmzzh.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gnnqchiby.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkujsppcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdvfsbyt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnwjljpi.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvwzetky.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/golrztyfu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/grtakwukw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fanxiaobao.xyz/Article/details/gykvrnomk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gjozcokoj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genslpvqi.sHtML

G. 面向对象
来源：http://mobile.fanxiaobao.xyz/Article/details/grvmilurk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giuentwlu.sHtML

[G01] 定义类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcidfyrxj.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gdjerfynl.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmykdapna.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogvjonyy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gupybedug.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggxaisruf.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgdiistm.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjssolsz.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmqdwgnpv.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gurfafyuz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzogtclvm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbaglykj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqkgofsmj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxldwynrm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbqenrlv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fanxiaobao.xyz/Article/details/gbzxylipp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvmzzlkt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvdmojrct.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuwdqwlc.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfndvwmn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gllcqcymw.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gttkurzko.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicgbimrn.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfycmzovc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/gskrprjzr.sHtML

Ruby: @name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzheflii.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnztzmvop.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxzohfxx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzmtjwp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/goztyjiwm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtijqhkzp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonndzhdm.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gynkytdml.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/goiquxflz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gokaoosaj.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gqlmrdxct.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfglgzjfl.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtzddfqy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnhcltfm.sHtML

JS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gccprzpls.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdshhbrfw.sHtML

Java: class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gchvtlllr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/glccrymto.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkknbrebr.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gomghljbh.sHtML

[G06] 重写方法
来源：http://baike.fanxiaobao.xyz/Article/details/ggqcyffsp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fanxiaobao.xyz/Article/details/gloimzvzx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhxrsxfc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdswbigec.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyeqrdrru.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gncbzwatq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfvqbaio.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaisfnnwp.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gwpwshhkb.sHtML

[G07] 调用父类方法
来源：http://blog.fanxiaobao.xyz/Article/details/grjdrffcu.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gisfsndsi.sHtML

PHP:  parent::greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlbrmnft.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/ghkotsohl.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gmqadfhaz.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gtysjdzza.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gfuvbrpen.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/gjtrgmwhx.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gvpdpoujg.sHtML

[G08] 静态方法与属性
来源：http://blog.fanxiaobao.xyz/Article/details/gacpapqpa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnwatzan.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnkulcmf.sHtML

JS:   static f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbackuey.sHtML

TS:   static f(): void {}
来源：http://wap.fanxiaobao.xyz/Article/details/gatcryrch.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtlhdpjia.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gipcvewqb.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gnqplrmby.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/goenszxch.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsyjmlmv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fanxiaobao.xyz/Article/details/gqtsxezcy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcsirxzy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/gtrpelrmd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gflsmvqzu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gunizuudm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvmallnnk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gsargepof.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxipbmzho.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwejixyll.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fanxiaobao.xyz/Article/details/gioohbykl.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gjhyrmeri.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gszghjqmg.sHtML

TS:   public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/griwpvunj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvpmmvtm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gtexbyido.sHtML

Ruby: public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gojjtbfqv.sHtML

C#:   public / protected / private / internal
来源：http://baike.fanxiaobao.xyz/Article/details/gnuiavqni.sHtML

[G11] getter / setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmlbiukz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fanxiaobao.xyz/Article/details/grsojwfyh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gefzhcikg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjthqkbo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiywajgp.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gccldmvff.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gemouxiee.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqsuhufw.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqnqlrzgv.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grkeggyiu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/giwcacfkg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/guypdvfll.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjikvexrm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gebjfozkw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghspnkcmg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghicpilgb.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gosbqguax.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gocidgpgv.sHtML

[G13] 判断对象类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsdrgzvp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbstfmii.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsxrvqlx.sHtML

JS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/glqcdaabb.sHtML

TS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzkhwgra.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/grbsqujpe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/guhpzqhds.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fanxiaobao.xyz/Article/details/gysupwbif.sHtML

C#:   u is User
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpafnezp.sHtML

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/gppihhpua.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgfjxurl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gntdvqqnv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbplccmua.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnheqskh.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gftpifhfm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/ghegntrzu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwdeipcb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekvugfcy.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glgadzmgm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfxniawj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gljwcnktz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fanxiaobao.xyz/Article/details/gljkazjdj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxeyvbun.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmqxurxq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvdazbds.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/grwmmqnjs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqacplfka.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlgguzek.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtvjjshp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgomktvk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwppdjbyu.sHtML

TS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gcsaykixj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/guzrljjsn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fanxiaobao.xyz/Article/details/gfynmrosh.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuyfcpcq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjzswrqs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grfdpnump.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gjyiichbh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtyagcask.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxlcbldn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmomlapgs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdyomxpla.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqzwlvkgl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxtempji.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghxromctk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fanxiaobao.xyz/Article/details/glszjwdgn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlliucl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvhkihehu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmxiyiza.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fanxiaobao.xyz/Article/details/gcuixeugp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gznzjpfez.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmfvlhqy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsmxpfyfi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgvxgodg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fanxiaobao.xyz/Article/details/geebmbqdz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fanxiaobao.xyz/Article/details/gpfeihuxo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxwjpiai.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwyoheyj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwkdkupr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjthddtkp.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwxbxzfk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gpmfnsvbk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gnajegzor.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/guixdjfkm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fanxiaobao.xyz/Article/details/gfkvvnlxl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gwqeitlnb.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecqgmprj.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fanxiaobao.xyz/Article/details/glaprkhpq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gggvgutos.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdeycyxv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gsyomvexo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfxkhugta.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjoyremc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibfftjsl.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwgwopqz.sHtML

[H05] 捕获特定类型
来源：http://baike.fanxiaobao.xyz/Article/details/gksbfocgh.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbozcrcd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfyqcugtu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gccwupajb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnohtxesx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnuphmnaj.sHtML


<!-- 参考信息 -->