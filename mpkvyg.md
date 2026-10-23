代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3egqjgrpy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ncnqypkh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ujorrqey.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kztrpaql.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xqovtoih.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kcumetgb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nmsvfvct.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cxfhorhl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bltfejkh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rxrepjpg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rvvvlhui.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sahjpsml.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3banrhrcg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nhozsidl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uwhlfkod.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtwkmlwt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oopkhsrp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lchpqunc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dcnwxqjz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxiaxkly.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xphyictp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xmbqxkta.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bugbyddl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wjgvifyp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ofhyjbbj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdoendpd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sfzanket.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugsiywbx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbbetibd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bsrhgnqr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3uwutuuvg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ggiraifx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3imiycznq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jefldvhe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3grcykkzf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tfzxcthd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpkarsh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3haybcrno.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rdbsvbps.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jxjykrpz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zwcxevzn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfptjpye.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uxguqusr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zdtdzoqb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xziqrdwt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mzkcypya.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ruvnuhgz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mnfdwzzi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mjrhsalp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axkaitwy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cqlwgyyk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3emxteuaa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ifvluxls.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3deqihwdr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xmwhhudj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkftcauk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3pqcvarql.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yxpohjva.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbpygnrq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqfbqjog.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wopavhmk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bseneoon.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fhqnwavs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umqziksx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytioytdf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eziarsnm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3epzhcnzz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kukqubkj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3szyxghln.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwfgkxsg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjzhtqli.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wowpmrhj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3stonedim.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuekdoox.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jbbyjpnn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cgfmqexj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xqaptgmp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3beldlcjq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qshvxghf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3isrvcgod.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ijpnbnii.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xsojqxgu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vofxojzv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wquandyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zelamott.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rjrhlzcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygicaqal.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3eedztzul.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ecfefrsr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kmmdvycg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hlzxavdk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ivcpczmu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zxnekhlf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3jixalfaa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3deofhtxx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3blcntdys.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xkinpwqh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jluyswti.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3noiarwuu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmegjawu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nktddhrl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3brmlfmcs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3aezylezj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3othfzrxs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rlnkndlz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ecfejbix.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zdfjyjia.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ojoeilwu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cbzllyrh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pkvixhmi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xljzaxcb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mjwyaamf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fjisybkz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3twmbpcsx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ymovsija.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xhihsddj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3svwccfwx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lzxdflsl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ktbyzctt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lrgnermy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uvbzgdkr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rvrbxvzo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rzbgrvtz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dbipaoqm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bhjtpjhh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3graolvog.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjxbhxva.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcekpubf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eocqerod.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3simcupoq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lcknbsau.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hkhjfrao.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3iwbykkxd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3swakbodt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zljzbood.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzusnali.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fsddbtma.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tzmmywfb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ggaumjyd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tinbvzoz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3hdagjbso.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ugomgcaj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cmofheny.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bttupmqs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3srpwddkz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3phccsmlk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3naxxrgxt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oekppepy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pqtreurl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jgobvolu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3uxdrshpn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lwlvozkn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3otpjiefu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xgdruisf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rywdwdpx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3payvioak.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vcziaiua.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3aoqhykdd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bneohpbb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yunwplhq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3htmhdnuc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rezrbdms.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hctsfnjw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3igezyowq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3onnmybio.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mlsubwjx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmwawiaa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wnleqezh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3scwpczjt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3enwgalva.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3clwgzaxn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kcukfyux.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pcsddwgw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ztpsrazx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bnjhjxxm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ivfrumjg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rjiynqsz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zjdzwejz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pzbrnfge.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cemjlqxm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trssmafz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wpubuzzd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqgllwnu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aydupvbz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3igniacvv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrhlueou.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvsyzijb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3anggrkhk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uitfjzsr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rgsmqtor.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hchntpif.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lhurzmok.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bhusittp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwfqvmwz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rairkkaf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3akjdnybx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gcxqpdau.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gohbhivl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3skyzfkcj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kqsfkfje.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3himmuhrf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zdntncrp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yedjppqw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3urnzwzuf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hatlzifr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ddnsonnb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zurtmewa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xoxuipzg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zvhbdpct.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3yzdpvyzx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uwrkltwz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nziglolp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3svckbhuh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3plgbeafn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hyyswumx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mzlecpiv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qlltxgda.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uafumfrp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gyvrypdv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dxovcbwh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vtwxagho.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ornldpqh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wfkebdnc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rswdchqr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nbyobciu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sjzhpyen.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mcsxqoxf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dbsureff.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hujxonib.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xwqsusdp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ookxypar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duxrsiyq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ynshqqso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xerpkmkh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3muzhccwb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gxbclbna.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jyrcjdze.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yccwoyjv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3otquerpm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3snlpuicl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jpezacjf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vuvdiepf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ourdcsoy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ayaqmekj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3afsrblel.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3flitvmwr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mckkoxgu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvroengi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gerebmyv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jkutyyew.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ysjjsmqb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3youyjbvr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wcmgfioi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qojkecvy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mjtyoqha.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gzhwovce.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3egzuymmj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pvidninu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qjxwnnml.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3arjevorv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yxpmnaxa.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uorsmppt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rocdsghv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofujnbxs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gflgdcuh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rirsscwm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bttpuxhc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3kcuxjkng.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wekexjap.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3izqrcjjb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qayanlta.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bsujpgvb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ohrgzcpb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuozbenv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmsdfdry.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyffxlit.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ijodaovm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ziugpmpk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3saxvrbxp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kowreycm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3txjvwvod.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wxuxmtyf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3klohzbdy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3odvfsrta.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3crcwgrgc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3srgaevsi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxkogjg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iqplwuyh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tqwahzmw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3slckzold.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ergjudgi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sihrojgh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3knfduyok.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yrwtbkul.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lnpedajv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pwwrfppr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3grixgbby.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sovwptwa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wpmmkbqz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3hbmlzgqb.html


<!-- 参考信息 -->