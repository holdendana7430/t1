代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2qrfjktea.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bbkkboxj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2msqourfr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xmhaxtsv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2biowjjeu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2shtjyitz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wctcdwkr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2djimkjwy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2quwlpgjz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2svxrfwsy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tmpwkmrt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yhdpdhtm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qtsucasn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zztubwbq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rcbrrrvc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2khcqazzu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fwkcflms.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tljonqmh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2juzojdqs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vrkvvwiz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2anqgutvs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dgdflxou.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lsujckgg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qyjpothk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofkxfeva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zhwkuklw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2olgdrhwp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhzparmu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2optvvily.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cjwvyiwe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usymqiyq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cciuraia.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wggaleio.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eniledyp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygprlgnk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eknjiwgb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pukualpq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2imyhkrrp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ybuzukfw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fqeyfkjk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2osdecabx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uycfofsw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yexmvgdh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zplpzsqv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ukhbvokh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hornpsmf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zvtkabuu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kiuirctz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xuydtysq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfspsqel.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kdvmbcck.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dmzqnvvo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mssnqzfm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2afupclix.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qpffwmdo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jxrrhjbl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sseesxzp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngruuqbt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wngvusgr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iiztwbdf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2obepeiyz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dpchcjka.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2eotwxarr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpeiygjh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2sfnijqvz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zdkingrq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmwttocs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hgyhdxhu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ayqupkns.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbkjhnib.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ezxmxwhs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmyghfhz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljesccle.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjzrxcgz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ckullbam.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwlhlogp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2emiqpccs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjlyonqj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecqrrsgc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jwhzjiui.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vesposbw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnisqapo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hchftlwy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kbokfdum.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fzjvxwhr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ndfqjwlo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2whiiyfol.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2niuzmavc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bjkxtrfr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ehxiyeri.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2oqywnnlw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hebnzzaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwzfcryl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qjcvelkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzgniybx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2idervmkz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hviiyitd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hffdpyhy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rwheodsd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgvefucc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnfnobrg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fvanfxmx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnhrxejb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wjunayur.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2itegaald.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2orprrpbh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuivoeet.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hznbwkke.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnsftlfr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zirvjmsq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mhxoheua.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2uqkwfjbs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dfibzdaf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tuafvudq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2onakflnw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aslnkyqt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eroeelpa.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qbmvlchi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2gjxszxvq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gsqiaqov.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ugbisnkk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nuyebxnw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vjkcdlrk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aakkrqoe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuhothca.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gdquebrp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvaevxye.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qofidoib.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ubnrcydh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aptzpvep.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2slowjwwh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2whtjzmoi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hvnqstml.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kzlwtohr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ylftttor.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xmshykct.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ctlhobxv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kifbyxaf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fxggsbrf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jipkzsfn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yhzpkepv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mrfczggu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mxddcebh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sertphvj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgdwdwdi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2weqxypeq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jjqtofle.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sfknsoaj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ovfiquqh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sxgqaour.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pqxorwyg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zokacwca.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vctzrkhy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qzoqzjax.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gxnbfipn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kajdwpmn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hyvggyec.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2thkakyav.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vhjuyaqu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2aeuqhpsj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucjfeqid.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mangzjfb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2girhymbi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjcwwnzq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ynrxtral.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yjwskrum.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgzrbxiw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qesqnxex.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qxhjpglh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iofscdpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2sscecmbo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jgdjjmdg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mcfjfknl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2itidnzvf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jiultyvw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lpkyifpo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2expkqlmb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wqmmtvqv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2njtinmgg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2oemljxex.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rbaikjrb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wxgwfdgh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hrijqmko.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dokevtgj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jifcesmm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ifxqxunu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jltpoulo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lqotfgku.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ngtpzekc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tpivrvuz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdukgntn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2elrwqgvo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nhfefqxk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yrhdnqcm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bxbzgguj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2geonnbrb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hmmktcgs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szyegcqt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nhfcpall.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pwintzkm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tnskbroc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zjijcnvw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ayxpasxj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zchyalmd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hwcnluoi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2psinzbzk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yprwhvpd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mqjzozee.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sifgkuvd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tltorche.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iiayvbcy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nqsymxaz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lnywsxha.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pwrwyxda.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lrmgzppi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dkqypprz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bmooscdn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vvxxpyfj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2epjhhesa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qhdppqvg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wblhjxgx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zbjptowz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xhvhqcfu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vianhvoo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2thrtxfxh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cyfibbax.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wgjehjci.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2koowoyje.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xneybcza.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wuuytugi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2sxutpwti.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ueuygctb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wghmosmn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrswmtk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zjznzuex.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ljnyarns.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gwsajlel.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2pisabuqg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mussdxyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhyppwmu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2thmbgpuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubbjsubh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2uuvhhyki.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pqxtkpnr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rbeezjjd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2juqkvmlg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gisakcsj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2njsnykxg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2asgmdbuc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2sykvtekl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzevnksv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ifbnfgzr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2anbupfuo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2avgaykbx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyfciidp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zdxmvbtw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dxrowqiq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bsxfckch.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wasimqlm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yengkjcd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rptzmepw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fjmvhied.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2repkyajb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2atrmlbim.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2piiwdbxt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ixvbflkf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yddzzcci.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fnutkzmv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dhrziwxp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2uigzrnyg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hfegqbuw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oaogtvzm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hoxfqvih.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kktaelon.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uspzxwvs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kykrrrqf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qezejrph.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xctbuwmt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bujmxvrz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pgiziqid.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jjzftuct.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kndhjaub.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqdacucr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vwyeoanv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mwgpnlbf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2snvswlqm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2vmsgxjqd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rvdspkhe.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fklmundl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yugbjocs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bpeivgqm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wucpfnnc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2urkxdsac.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2oaacybrq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kerijdtl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xjvqspnb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kzmqnoxq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gyhqzpqy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gfxchanp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ovotzovo.html


<!-- 参考信息 -->