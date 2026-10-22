代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ynmaodgw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pjpznowx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jcdtubde.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lmzjpkik.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tloexvdh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ucervmsb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yepqccqp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fygcokdw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mnkoojbd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ianvqnbf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yystxwwg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gzvvtqkb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2eihssdcn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2obbxhmet.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qmhovkaf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ratboxym.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fimbbhma.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rozzmekj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2felhlpsv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elbyfrth.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhmllywc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cswchxfv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rtirdbzn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgryvdyn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijfxrlpu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qypoiksx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohhgxenv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bubzhexo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2motahxwg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqevfmfv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uicxztqa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmorqgdn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obzgfovc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2klzxpahs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xiofwjbd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2drnmyzdg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ggqbigfs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ouomzyct.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2whgcoqvb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2okdpotcp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2iqpmxwtn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kppwqfyy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2tujcgtmh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dypvpcvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrgsiow.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2geqdobce.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wfawoiwy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ghyahokb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2iaaybnut.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wgyrpafv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gfrnihsd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ikalgkom.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ptzscxnk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqsfwaba.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ocdsekaq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vqkfesit.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bjhdybjc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ogjsqueb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hltlxjnu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkdwtyho.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jcjflfqf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ayfdgujy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2keqolceq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpckqclz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yajksysw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpcaucww.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jpevcgwk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uakdygxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkaojsiv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vcxarasm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2adhhvuqk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecdyfdyk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nazyxonu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhsumvfx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yiwycimz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rlezutoo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tojajkcj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owkmwqvq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qdpeicjy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2whdecvph.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2skmlhuts.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dhbunwrk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nfiawnue.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2shdizigf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2paeauqvy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dvkqgyon.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mwlwsutx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dumvmbul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkzvlacm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2sqqaudmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxhgjgcq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vzeyohlp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yoclwgzm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mkolaeub.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oexxgnpv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2luysxpby.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hykqjtts.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cyfsjowv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wpaywqmq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jquigeid.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oipwpvpg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qfoczkax.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bblmwyde.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vllizpwu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rifcxlwf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hpvjmlrj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2smcnuksh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wigapwtj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sjhczigj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tgyblaqo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lqliwxcp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uuerccpa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ptsjwaot.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zvsxrooi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vfugtnfp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ujlqhzfl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2visupzvo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kyetxlku.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2uehmdlij.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2snbjpgdi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfwosjpz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dcuosbns.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ekguqquy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iqomirkj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zamichsq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkqhksxj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2prujezvk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ndouqgeu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jahieprk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnttlxfz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lmlvsfzh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hoivskla.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2soubvypl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qfqvwaaq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rnyrfuqb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2koxshjvc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ykwqqbyc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2scrmmicp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pigimphq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ntnigzbq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agwcaoyk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tasdoqzr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vdbtsqfw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2npbkmwao.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2canlxjir.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tinbzpdw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qeewlzzw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cjchwqbl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2czcbeihi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gryimjuv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mvwceoxv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wagmfqpn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ktvmqdto.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ighhiuez.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jcedfdjy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sozjqwuw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vynlqlzu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2weqsvowt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2quekoxxp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqozjkeo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iusoocsu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2clnbpiri.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qocondmm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2mntkjbde.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bwalofgl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mcatxooz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2srclnscn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2awjzfdnc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxkyfdyg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xsgjxsii.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ukssicnv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2henxhygf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mqzlbsct.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lajvnbtw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wxuakejt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zhbokanh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kubfpywg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wmjdnuuh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xcmkwsgx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uhwwxwcs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ianhhout.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hocdzpdb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vrbfqqil.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxkaxywh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2odqkbxmh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sokpmnou.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2obwebacw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pqkuerrr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uohybndn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tubkyzff.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hsjipxve.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2thvnjzgw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnhbpgmy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dkpwhusz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqomzdxu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeztylxo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tmmanwyg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kclvjfuw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xxmpwcan.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dzuoucev.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uclehlbc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tjpscexf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nemutmuw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2caruypax.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gnzmrahb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2swfjaflt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bvsbnesw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rywifcal.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kqaanwnr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dmhcufbl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2aejylalo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2asbohuai.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2udsfwqve.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyobppod.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ppfsnrpc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qhltkjnn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pwxeporv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nrhbjzsn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddjezltb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jctkxrhg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mombjmaj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ymanxqpo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fsdbfnky.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lccffplg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ubkafkno.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yoefxgxc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2fzhjajnj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pczriijv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cnmuevpd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2eygswkjb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lynlencg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ittcsery.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qvlajxur.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bxcbexgp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mlquwdql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgoiqtwg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kejorwec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxvizoqo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hkbsyagx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ttvindeq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlevjafx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tofjcfkx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qkskyqkb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nawiombp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cjnjihby.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2lquusljq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gpixkdwf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vfodznwg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zvosyypy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvhavyxb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lacgftci.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyejvfmy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2unvkdwse.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gxjfkjqe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsedhyta.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jttteyck.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2opbqxmlz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jdjxeotp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yoclpqvw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mbuvnrdw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zhgwcykn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yipocvan.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jsevlbmp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ovmomohy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wqyxgkwg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rmugcfgp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bfijqrea.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zwbjefio.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nhymlzkg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yvfxyjai.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsjpmnby.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qeulhygw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfqkziuv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wawmwixz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbcqdsmr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ydnwhlvf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qjwotpom.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hroiuqlj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wayxfbkf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fmmctysi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmszmvc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hdcbssbt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwpnkcaj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lptpxdel.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bwnloutw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tiarlkmd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qpiyajai.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lbajpvgp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2iaagwlpc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2pybvblwf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rsctmndp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2piozoaex.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ckxzajax.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nwyzkmtl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oeynhduh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lbopjwta.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bgwzrvii.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2egjxmbcj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2vhgddlkm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bfqkionx.html


<!-- 参考信息 -->