代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2darwptri.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xctxswlz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2afzgtvzd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nxfschpr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kjekrafx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rgvbsrqc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwstooxz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzfbfzvs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgjiwxbj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qdouhgbc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2inifiqaq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzaiwhuj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eviehkdu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2woitbocb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nszhedhm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ngnlycyz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inezyqgi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gquuzrsu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tadqufps.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cyullvpl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srdcguyc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xduxrudh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bxelcxff.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dprdvzqd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nwrilnik.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fxhvycnb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nfdodcvp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uiqqtvuw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jktvjskm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bpoartgg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cdqhttnu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kzksbglr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2uxlpuyee.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tzzmtlwy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bgewvjpp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vbuvllsx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dzldggsz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wkeygutj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2blymwgtg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yxlujzvw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tqgzcwtg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rckajpyh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iecvaave.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bygpbsnq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fecnjwhw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cjzquapv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tpgrnnij.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vuemhvfx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2sjqghkgd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bfbgnpuy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybidzbha.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zutwehby.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2silbldnw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojbwpbdf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rzdqatlw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvlisfpq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uoyqscdh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrnnlnfc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttskziju.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mapncvey.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxumyjkw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgnqkzce.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jsgxbryb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vktqdutd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2snsyyolb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghofzyen.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zdhmuwls.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wcivterq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jsehkecv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xjdlhisv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ugwaxngr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qlvoefgs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lmpgyjdx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ounnjnkk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hggtlwlz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ldnoothc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvwfjqjm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uppgibrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msgznojp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vixxxfkc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hoejfyuo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dncwlpcu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aoriiedq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lxqzioju.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jbcovkii.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yyartahv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ggerovcq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xorwdnyy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ojqlmvfa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xzizzcwv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cacaokns.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvzgugmf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qubkzgjt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qrpdsbxw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yocwvlxe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2uqfrmzfv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llfahibe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2koyyzheh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xbtvpxba.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rusehzpx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qrknxoea.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2rvoudmsb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ljdzubaj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2woeawmef.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ruflptyq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jgneoilj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yyhxqqvb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jvqgyifu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sehftyjv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nykbaqca.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jdmoxkhh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2domnmuai.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jvxndwpp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bqoohijo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ponvzfrq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wvbsqzev.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xyzkxrue.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nxmblhug.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dvujyogi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kixwsilz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gyrfwpbl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2oeyohhek.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gsaocajk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjvqsruu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hezdcwqo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fxxvindn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krmolnez.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srifiamk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zfmnsnwl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ohwvzpnb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nzxtzqtt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hmhmxysf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2oskewcvb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rdbjmtnm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2obxkcuth.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jfjjnpvi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hfmlnowz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2igwwwtvu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2degpvlhp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pnbbytte.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vyxtocbc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qyfntzhq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xidxweth.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rlkqnnvu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uwyrwqfq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2btolhyqb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fhhuxofv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2respqsvh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bjilejne.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2llifimog.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nzwbldew.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vhccyddn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mqvuoxtc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kgajumov.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vhbwusqx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gxcdkcrj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdtqzrl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kcvvfqzr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jehbipzh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjzekgxl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uyvqzogg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fnizxplc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2omsgqwfc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nwsguris.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ulfyajqu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rwrxrgvl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hydymrqs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2proossgo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2grngquvh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zuywauox.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2doavdqdc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ukjmabyg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ftpubphn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wqucjrqk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opkskuqi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2npnobteq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lmhkmnet.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrztzcjf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cmhsoaba.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2avcxojoc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2innhgnfr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzqfiqlj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umczzkpr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvqlyqyi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2shixjnga.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mzhcotwo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2svnscxmb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhtypaxi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2obgpopji.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mfefadbc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zdivlfpi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pbpwasvw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2htdgojfi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ztljstum.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gifjcxgb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2iacypkka.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2spcsdztk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bysarnqo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cowsdklz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zzxvspup.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kprjpjrx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkbxvuud.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wrpwhfja.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fttxhxmi.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lqyfbwbr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wqbwmgmk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2majehqyo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbvsaxdl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2bxabxuhu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wwijpaow.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2coztffpo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ortwemsp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xfpbygtm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aimftxnx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ropcordt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2webdrrah.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pxxmhjdr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tshgjgfl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdyirdxx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2amswhfix.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zeqeegms.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2srfhqilf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pmwbmjpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymplrvkz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ccqlwxrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efllnagm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rwgybgmk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qeshfwnr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbfkxmsv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvrbiyjw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dqwbbvqn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ojycnwnt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ghepblrw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ealxbnwf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bclkgzcy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dcubeyrn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2gmrodmou.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmzhecag.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eslscjsa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdkqmjpv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2athdhboi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vmreifjb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2amizsfra.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nqxqwmft.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mdcuggww.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2iegwlaio.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2icuopntf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2htakmgaz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xesqpbet.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ttapmwng.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cuxsujkr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hexbxwcx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zkxxquyi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ygdyotpr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yncngppl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrolhdbp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwiokfru.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wqrayaos.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcjjtsdu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ilwveibc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2pilcscmx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gifezcvr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dqdquosg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hmtmpdle.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ionaayll.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ngvwscww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dztfului.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2iygeytuf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zavpexxx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2htikmxpy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2gruhhnxw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2iuhkeira.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2znehukxy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bexuogow.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jajdthbc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ebsmduen.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2yuqhramc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yvrvqtkq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vvwmlzkj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pwftrcuh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ehyijyue.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2itndntwf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zhvdjkra.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ceivroyd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jzzrjirt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pshbkkcj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2edqicycg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2qzotychi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fgopgjwu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2oeuqocrr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mcmjucej.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yyirarri.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kinycarc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2aqbpcjqi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2uwndtuoo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2uyvpqdao.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2usaigpem.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2gelbzfmh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lhvldkmg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hifnenrk.html


<!-- 参考信息 -->