代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gdegomqgl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/groqscdsc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gurnbspze.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gqmttieom.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gqmqdeltx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gaptcmbcd.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/ghsoeybdy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gxtlsvnka.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gurxenhkd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqzihelis.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqifwpnq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gpbkctkjs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gedsqvplv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gqkobpgwa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gnzllqjod.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/ghmdxqshm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gueqxkbto.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gttyyoxbs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gxbdebaln.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gdftnhiau.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gezmtuskp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gvtnbrvaa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gmwdvltqf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/ggoptsiew.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/ghzcpxwkj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gkghssyco.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gpfzrlgsz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goskgsomo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbdjkcfvn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcrccnrss.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gzqehffwf.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvkwlhlvw.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gatbggqed.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gbjlmaevy.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvmthfxcq.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjyjsjnmb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gaavwauyl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glyicoycu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ghkswgacw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwnvanbfu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpcwiqhzw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghrcpuihs.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gtvymjuwm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/glgaukclv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gyafiiwqd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxuzbtubt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gtmkuqixu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ggnwelkyp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gltshchcj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gptnagann.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/grlrqacjs.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gpdffyeft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/ggogpifql.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gyrysyjtt.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/grdmmqpzz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gfubljuxu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ghbedogbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gfsafvzyq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gfnrnmshn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gwvgazfxw.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gslrmldal.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/girhqdnrf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gndmsvbpe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gmkyxjhdi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/geukzusui.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gwhwebqga.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gzsorsglh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gklvnikfv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/goodagnbf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/glrenlory.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grfxipnrr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvaevgcla.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ghnqdbmny.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfqhesyat.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/goqcljghd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxhujtpig.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvstuytcf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gafeenlab.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gktdjtbdw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbfzbtkzr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gmmgrjikf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghpodxpck.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gxpjiusdg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gtoknlwwo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gmobhlqpz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggitsadtz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gpfikodmu.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gnifzsbqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/grhdrtatq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gaiqrgykj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gimkysztd.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/guixrcgmb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/ggtsvnwfm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gtdjthxal.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gfusnogbl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gyttjpsvl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghrbsyolb.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gqzmtzunm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggbwwrfvi.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/ggrrgkptq.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/glvohfifi.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gtzjuooem.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gebbgsixw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/grxocnjfl.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/grflczexu.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghezanidv.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gucykxuzv.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gbehejbfq.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gmzaipbpg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gfrhstceh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gwnhrexmt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gdmyjarqb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gadlftgmv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcxgkthn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gkgrqjvqs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gxruflule.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/grcsipwvl.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gwjzhxbll.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gygzztdyq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gqzhiepwq.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxdqcncvb.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/ggwdygstj.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gltjakrar.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gkwksrxhl.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gxdomemoo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gnfezuxvz.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gybubjjfs.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gznghzdwy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/glaekugnq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gdzfrguhg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqgccaayo.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gnfwaxwmo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwkqvxjun.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gyrrlncpz.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gqpvqavig.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gaqmabald.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gfgvatiad.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/govrqscgk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwsroyzzb.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gihmqmvjk.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqfkgphry.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/ggtdwmauu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gkkjmvzci.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/ggmwulrny.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/goyzridqk.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/grqbzglkl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkqtkwrrc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvxoxtcpa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gclqrqljl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/glhsvjmvz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gdynktrnd.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gldwxppgy.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gtqiomtuy.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gurodiyyc.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gcxcxgxei.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gzkcxwcto.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gowgqnhdy.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gwqwzipyd.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/ghemveeaj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gzhwsvymn.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gzastimxj.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gnrmejfws.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gprshnlnh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gmnesaudi.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/giiyfeifm.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gixfgmvpy.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gtbefiomm.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gvrbtwzum.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gedoifyqi.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/ghcwajvbc.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/grlmzmdli.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gnunzvzuq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/grfjiqenq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gunzwwvur.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gdohgkiic.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/ghezpeezr.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gpoeobzuq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gbaqdymnk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gdismonqg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gjikkanfz.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gmimyrixa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/glzajgasc.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/ghggrkvxo.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/grfdckxts.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gtyorvdbj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gvgukvxqm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gjnquemgu.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gumnvfecn.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gvwbzmien.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gyrykuvsa.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gkzvexxel.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gbmeldzkf.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gflznapna.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gyzjvwnhw.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gbglxyome.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gixpdvrrx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gzdmwetpn.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gqhvrpcvu.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gkmvkpueh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gjkmhubjn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gjkgrdgmk.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gheorluza.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdwjygqj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwaurskfe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/grokwvyda.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glugsvhls.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gnymizyvl.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/geeqfpdud.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gbmzloqns.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gxbjvisfx.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gqtodijpq.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxeswibvf.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggtnoegnd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gcjmunwwv.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gfxttcufu.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gbwcjtzum.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gyolzswlr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gjtbsrzjw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gybxntdcu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gxvdydman.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gwoainsjp.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/graddghni.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gjgliqzrr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gvgzxninl.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/ghnqvbrfe.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gwauprhhe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gyraiilwv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gesgbdhsu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/ghigthexr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxszijaqa.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/ghfmvuqex.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gookgarrs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gptbmitgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gvvuupbyf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/ghdnqpght.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gujncrcdz.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gzdjxleus.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gevatddjx.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gbymtnmzi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/goqiokbkg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gcgoexzzf.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gvrsrctlx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gqgsyjilz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghvubudtk.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gdbsjhkbl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbihatwdx.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/glketgqhw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gcbamnzum.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gabqzelps.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/geoxppujk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ggvoxvpae.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gictcmdty.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/groheyhue.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gfnfxegok.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gocpftnzi.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gfwvqlkss.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gxhyhvriz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/glfycirtf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gncaajwui.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gpglxedcc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/guqnqufsi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gconlhjmd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/glhfpxfrc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpgaakzsl.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gwstrkwdz.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gdrjnsmka.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/guhoyokon.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gkuaeipqi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvrfhdxwi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gmyruotxx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/grldrcdol.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/glfgxevrt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnyyetvwo.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gaiqvkdxo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gjzypdfui.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gwkeevlyi.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gqwwyajtm.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/geptqtdvc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ggjmfdjwo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gcxpvvzhv.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gbfvjlwjb.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gifjxxwvz.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gjpsjoonb.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gwejavbqq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gcymiqdgx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gltxittio.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gcrqapuuh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gslrrnkls.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gpjujodbj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/geyobvmyo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwnbngh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gqvlcpjvf.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gobnfpcjq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjabprxft.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gxnkxejor.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gbbymgwcp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gfzzqobjz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/ghelnbamk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gnofklwjw.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gcaxtkeet.sHtML


<!-- 参考信息 -->