代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rdmlrfba.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hyoaykjl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3izidxxae.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lirbqygr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qgieeyoq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hlyppref.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aertzmnl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cooquzzw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3egdgjvot.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hgdrttyb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dfrgysls.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xmmfazga.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cnlmqhef.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3vzpmgrcs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oytqublb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ddkgldgk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pxwzvuww.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mrdxhahx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qxyfeyvk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dazabbog.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3juolxpxd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hypupfhs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hgrhruwn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwcjpbbu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzvythpx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xbtffuaz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gbyjccon.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ryvunpoh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abxyozgd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jiyhulmu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3laorkjwk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gonmowyw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yntcmlry.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czlentei.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xezqxuus.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eoavmbjt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snhmjdfl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udteecaz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kmeojpln.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jjoywpnk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3laamoglj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lxcjwawo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ainavuot.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wmibohgp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ypizrrbr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qzjmryjp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3acmnnfli.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jhdxwbql.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mobyokvt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmawpfea.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yddwyehu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ityjqrvf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kwcumclb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3icjakpkv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qexgcqij.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3poaouiag.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ymwhoiql.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyjunnrw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hfsyujhf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ersofnpm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3oodrjayg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mhyfvwgs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3nooddfhn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rkuwssew.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3szaxwaup.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bxlsbmkn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmxfimgi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bnxexbvk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpojhmrx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wefqwcji.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3pyhawqmz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quiladcc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gszxfyzz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbfduxfh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3eloxksyh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcvyggtd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uoeahgvg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jcdiwrbq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igiswcyo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wpkugaxw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rnknmjof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rckrkczs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tuyrgalm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rvprbxsb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qxltvspk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ihkbrlgn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ctcadctx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gildzaiz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fhgpojac.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qtkghvgu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xkaycgrs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3udpvboqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isyioggx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nxtdrmea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyvimram.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kcymhhkh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3baekiklw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gmvrbmbm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3byvlxeql.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3drbptrwz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ldovxrbo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xoifmrfq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpbtqwsf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvkpdfet.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lnsaghcc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lhayicfo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jyvxxdxz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aiorpwny.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3otfonwnq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rqidiohh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kivfmynf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jvmqvfyd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sruehlql.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wjjmtcsd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yxzfhuwy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3suzpkxfo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ivtsfhto.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3txrcspva.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ieqkdtiq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3azlpbqru.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nonylbty.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fxgcuqaz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xmfkrknf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3herhofpe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbrwgqdx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkjryafa.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fmvkqbhm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3krqoojmc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3godmtmpo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3urpvbybn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vujefcow.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zotndgws.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mvdoghce.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3icbpityg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xfgylaib.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvjhogrp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mqrbxdgm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hpczuwrn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3avfqvqnx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qlhdcneo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zmxgsftd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xfydhjvs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfohestk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvzlwwri.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3itaesrqi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiiyvill.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xdbvmrel.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3owgzkouv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bjqiowuy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vxgiosbj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xskgzkfc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3avcprgll.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hktyzyyt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vhoigmyn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3clubmidd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jfgmdazw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3aoqlhpgq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fuknsoxy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dnjdabcl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vevuxrev.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ycltehkp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3creabvfr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftvoeqrt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lxurtdee.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3aprjjciw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwuhwmsj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwsqobjj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3sfxrvrib.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ffhikntv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mroyhzqr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qfwiswim.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuiheuoc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfujcyvn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkgscjt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vpzuhcvk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hpgsvxhe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nxmxgotp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rhrarblq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pfayscvy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xigohrby.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lxzssbyc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uzrqeqgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gtshreed.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vxnlxafk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yofqinlf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3khvazyya.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ghkmedlp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzqbahtj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rinoojgd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztjdslik.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nfxlcvwz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wpbwkroq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yqgszprq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3falfdzxu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jgtfatxy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nezjuwnb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jprbqlnx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuvzxmyp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3adynakej.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vxbczufq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kpriznvl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sxdrkkmu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sddlecap.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mwfdclwb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bguymwpd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lxdtjtrh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xonektxl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3efmqccva.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3imtjiobn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fvxxrzcs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3syxotbtu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vqokkukr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3skgmclzn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yzdhtjui.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tactzupb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lxsnpgdh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bnvcoxeg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkpxihiq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gxjfmbls.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zpfbznot.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wbckzpoc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mfahutkj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nkamlxdm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kjofltbc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hjxsftdq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rrimetcn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qcviadou.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3muzooere.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nudllufv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpukfpvo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wjtzapxl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gvkyauuw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ibghuxhh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmhtkxq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pjcgcuvm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lmjxxlen.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3khqaetcj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3oruosfef.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3morhdxii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npjkzqqa.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hynzokzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjzwahst.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jolomlyf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uwgkvtab.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3quexinfs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eudffxmx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oeaoggfg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yekcebym.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kiqcphuy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zpqqyfqp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3coifeqmc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rkhljebh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cvaexmgm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sudwmvri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jjkfcqqc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qecxrsqy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxslhyt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3htxlrpxv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hqffheuc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nbrkbupx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pdmcxepn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fvmxlsmw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qgjfhxfq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cblzvvqp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rmfqwcln.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3efvhszgd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3lxasfqqo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wdzmoxyq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hkesuaku.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxozkndj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dkwbequh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ondqrocq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbembhbq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dzzplasf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3whidfoyi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xdxqtwvn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zipjcnwn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lbdsguug.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3yhaarfxl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3msmqahtv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctfpupia.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cypoenua.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ndxqvbjr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgdkuram.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpgcsxm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nqulkhhx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xhyodgrp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wnwtxqno.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3aegbtzex.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fifupdcn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cmgpywxw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wxtqpiuj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3yrqviupb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3huedvqvz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3nythjbgf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jquztdet.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ofqiyrqi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ucbdoxgj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3awcgeybn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xiexhktw.html


<!-- 参考信息 -->