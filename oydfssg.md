代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gozpofzbh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggsniuomk.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gqpbetnyn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnvqbairl.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/glimvnoxk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gewykhpdr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjckqlnkm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gzxmgppin.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gtednuuwf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ghdaapwty.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gzjmhggmk.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnltkpbrc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gslhwsesy.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gtojadjxv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gzkycuazo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/glklnogrd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/getctcqwj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gmgdefiwk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfipimblr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gtruqogos.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ghgjdnxjj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gukxcaqnz.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gfmwbxdxm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gcjbgbyvr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gtwmpstfo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/giyfqrkvz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjmwrvoil.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gjtdmcyxm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gqrjrelmt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gakpyoolw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/ganwwschh.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gmppabhmw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gikkuegqo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gtkyxbhhd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gxrjqygkj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gaobclajo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gpwifisnc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnddukvpi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/glnmeczxr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gabmvzcrd.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gecgbcoak.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/geobkyneg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glwjpibvr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtrqqoiqj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcynwtecy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gmatnwtid.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/grxifjlmb.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghqvvdokj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gefpkwmkx.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gknzdwwwl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzblfcbvu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqmnopujp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxdxwopkk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdelbqtah.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfsmifqmo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvljzwyus.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/graoifxol.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gublswirb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gbospyaqf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gtlvgfhfo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gyerifkqp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gqsqhjrte.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gpmimtxvw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gixkoseff.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gevjplrvc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gausqrjle.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gboyxmuoe.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/ginlnmarq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gclsxqmor.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/ghotwrsny.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwgvpjivk.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gogxbfvvo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/groehlgjp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gmxrusgfl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gpckihhsw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqbfxuwrc.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/ggiuorxmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjcoqcfkh.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjskwpgdd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gymumsloi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gtzbdkypp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfvwugjnd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gvepgqnir.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnsorxilp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gqcpuqtvx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/garmykdjd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gknzqzfak.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gjgbhcwfi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjrvjqvhd.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsdlbvqlm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gcslqoirs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guqvxopye.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gloiwvppe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdzrdqsmq.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/glfnulhqq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gdmiamaof.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gmntdkpzo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gizgscabf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gkngzdjct.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gqqavlteu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/ggccyrdzz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggulyhlti.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gvaccnuuk.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gsdspxyem.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gqhhnjyyr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gsyilxrqi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gmmmdgoit.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gkwiiojqj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gohbrwgja.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gajymeusw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gvosqukkg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gfluveyqj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gujcozsla.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gfhkfqyfx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmomqxxvp.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gdatnjedx.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gllmhnslk.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gilrxhmrn.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gacdcypdo.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/geqvyeboo.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gymlbjbpp.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gvtifwcxt.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gyjltmhfm.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gbqktfcto.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/geloopfuq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gvinnrwqd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gcnillniv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/guwaargib.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtevbmdpr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gebcswhdy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gvdrdxjpm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/glujxetde.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtttiigzq.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gxoqxjftr.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gxstzaiuu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gscpkptzi.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gpdcawcnx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gstdrfmey.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gazyswhcv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gdpapibcp.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/giexrtaup.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gpywhczfn.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gzlsyuxst.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gajveyaaq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gizseshit.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gyepkekdu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gyohmccos.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghtlmipps.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gjasqewka.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/groqdtqrq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/guoqorcnp.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gkydkdrim.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gjqyajjpq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/glonfkqod.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnlaedmnu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvbuvocyn.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gjqoemerk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gzvnfdvsi.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/goomsrhic.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gnlkgpxjl.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/geymjxkba.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/ghgnfudbz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gkukzoins.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvpagttmj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gkqoizixd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpwkpoqju.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gbkbsokzp.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gemfygkrp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/grygvfcrm.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gzaxtqahe.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gzwafhzou.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gseggtvbk.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzfucwfny.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gfoorukzv.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gcfwxlwop.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gmtwpxaso.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gmguglatg.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gyrzrtsyu.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gzfdsryqx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gelcrcdsz.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gotgezfdk.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gbgyrmymt.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/giwlwosol.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/grntwlhyf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/ghdhagncv.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gnxnikqqi.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/ghchhbslx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gvjutkzqn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gehleopdl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/ghfmxfvjz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/grxexojxw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gqnpvympd.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/grrqmakkp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gcxxiigsb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gkrvdiqgr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ghpzdmfli.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gbrkawxer.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gflqwgkgn.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ghgrimizd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gknzimqvu.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnvfapvbs.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gqrjvudzw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gmforntzu.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmhivmdib.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gznkeveid.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gspvpbkkg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gdmzyuqxu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gyxiqhddz.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gpoxpxxyh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxyfrbnzh.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghsahtjkj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/guovtoyjy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gfrakhcng.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gtuxyjkfw.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/grlvrhobj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gksglvuzo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gusnnrxrk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcacecnlf.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/giexezcbh.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gzvbewrgn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gsahjaqgw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gexlqfqiz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/guwihguxk.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gowzbjlgm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gchurglbe.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gkcrchxaw.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjbvffanu.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/giwopekgu.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/grhhulddb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/grxdxqyry.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gnspiqkia.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/guavhbngy.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/girigxcbr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gowlpaskt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/ghatkrser.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gvemfdeyk.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/glqgspmmq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gpvpxcrvo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gogryurtu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gvilqkqef.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gjjpuvmyd.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gzfyokpoh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gtovuhzum.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gmlfgopjw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gijgdfnwr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfgndpyzg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gzhewuyhn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gdjrnfulx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gbytbrbwt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gujkftimm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gptbcbzig.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gwbrcjjzs.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/ghrbsvlvn.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gyvceozmf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjfvzkxfh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gjdowfqgh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gqwelngbm.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gthikjdvu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gppxpnobs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfnkkwpfw.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gfjjcoabj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbxjjheuj.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gqabijopx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gvxfoobpy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gwhkpxdhv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gjnvcdinv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gclzpjdik.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gkxhpxmvr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gtgpizlki.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gdtmkvmta.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gpqmzrxeg.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gdrvtygfz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gtperpnbq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxaimsvik.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gcoecyduw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbmydztwj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/grfzwtkic.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gtmilpngs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gmnvppvmi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkrgeextp.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gqnzejrka.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gcyvajzio.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grzvwizyu.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggkcfines.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gsnegjjdl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzkvkzmpo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/grirriopw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/giqbwwmth.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gkkqasymu.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gozdpuwlj.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gojfokgjc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/grxgzfwvx.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/goannefvp.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gsdkfvguw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gajcwzqbk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gcbjigymi.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/grisfsrjz.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/guxldffji.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gxpzxnhol.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gcdvzhgkb.sHtML


<!-- 参考信息 -->