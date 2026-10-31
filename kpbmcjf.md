代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qh.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://xs.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rr.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zg.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://lh.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://on.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cs.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sg.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pm.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gn.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yl.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://tv.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fe.shxzukj.cn

================================================================================
来源：http://br.shxzskj.cn

F. 文件与目录
来源：http://hl.bookmarksfly.cn

================================================================================
来源：http://eg.panjiajie.cn

[F01] 读取整个文件
来源：http://at.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uu.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://cm.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qu.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fq.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pi.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aw.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://jw.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://cr.nszjky.cn

[F02] 逐行读取文件
来源：http://tv.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fc.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cf.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tr.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jc.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ka.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vr.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://az.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mf.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://wu.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fv.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jm.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ok.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cv.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bn.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ck.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://tr.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://js.shxzukj.cn

[F04] 追加写入文件
来源：http://ae.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fn.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iw.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ey.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fx.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fx.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://se.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gi.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ke.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://mk.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cl.colortex.cn

PHP:  file_exists("a.txt");
来源：http://dq.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://yh.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://oz.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://os.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dk.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://pi.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://us.chemitech.net.cn

[F06] 删除文件
来源：http://kc.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://sk.nicolike.cn

PHP:  unlink("a.txt");
来源：http://bd.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nu.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pu.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jo.asd995.cn

Go:   os.Remove("a.txt")
来源：http://ah.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://ht.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://oj.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://rp.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zi.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tj.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ax.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hk.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nl.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jy.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tj.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xf.huixiangedu.cn

[F08] 遍历目录
来源：http://on.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lc.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uy.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://bn.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://ch.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jm.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rg.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://pf.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://jn.shtwfgs.cn

[F09] 获取文件大小
来源：http://se.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://sp.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://bf.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://kd.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://vj.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kg.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kq.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://hw.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://uh.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://cm.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nu.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pt.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bo.521024.cn

TS:   path.extname("a.txt")
来源：http://wr.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ah.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zi.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rq.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gr.panjiajie.cn

[F11] 复制与移动文件
来源：http://ro.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hk.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tb.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lr.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xv.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ya.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://km.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ig.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rq.lnxyls.cn

[F12] CSV 读写
来源：http://vq.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tt.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gd.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tn.asd995.cn

TS:   // 同上
来源：http://og.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vv.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fu.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jp.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ma.hahajie.cn

================================================================================
来源：http://ok.asd995.cn

G. 面向对象
来源：http://pz.chemitech.net.cn

================================================================================
来源：http://et.panjiajie.cn

[G01] 定义类
来源：http://nz.yuexingan06.cn

Py:   class User: pass
来源：http://fg.asd995.cn

PHP:  class User {}
来源：http://zy.hnjuh.cn

JS:   class User {}
来源：http://ik.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://ax.huixinmuqiang.cn

Java: class User {}
来源：http://tt.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://er.huixinmuqiang.cn

Ruby: class User; end
来源：http://zk.wgjwhj.cn

C#:   class User {}
来源：http://rz.shxzskj.cn

[G02] 构造函数
来源：http://dp.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://oq.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hm.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://fa.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://wy.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://rw.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uq.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://ud.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://xu.huixinmuqiang.cn

[G03] 实例属性
来源：http://zi.huanxung.cn

Py:   self.name = "x"
来源：http://ax.szxytkj.cn

PHP:  public string $name = "x";
来源：http://or.hahajie.cn

JS:   this.name = "x";
来源：http://rv.jctech888.com.cn

TS:   name: string = "x";
来源：http://sd.gzmigu.cn

Java: private String name;
来源：http://lz.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wq.shtwfgs.cn

Ruby: @name = "x"
来源：http://kh.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://wb.colortex.cn

[G04] 定义方法
来源：http://ot.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://vv.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ys.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://pi.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://eq.szxytkj.cn

Java: String greet() { return name; }
来源：http://qi.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ly.shxzskj.cn

Ruby: def greet; @name; end
来源：http://jg.nszjky.cn

C#:   public string Greet() => Name;
来源：http://br.chemitech.net.cn

[G05] 继承
来源：http://dk.huanxung.cn

Py:   class Admin(User): pass
来源：http://da.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://if.shxzskj.cn

JS:   class Admin extends User {}
来源：http://mi.panjiajie.cn

TS:   class Admin extends User {}
来源：http://td.jctech888.com.cn

Java: class Admin extends User {}
来源：http://hx.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bl.nszjky.cn

Ruby: class Admin < User; end
来源：http://bv.szsharing.cn

C#:   class Admin : User {}
来源：http://vt.shxzskj.cn

[G06] 重写方法
来源：http://sa.colortex.cn

Py:   def greet(self): return "admin"
来源：http://nb.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lm.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://tt.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://mv.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://bp.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mz.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://me.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://cb.bookmarksfly.cn

[G07] 调用父类方法
来源：http://tm.lnxyls.cn

Py:   super().greet()
来源：http://tv.newstarts.cn

PHP:  parent::greet();
来源：http://iw.newstarts.cn

JS:   super.greet();
来源：http://nu.521024.cn

TS:   super.greet();
来源：http://yh.asd995.cn

Java: super.greet();
来源：http://bm.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://st.szxytkj.cn

Ruby: super
来源：http://vm.huanxung.cn

C#:   base.Greet();
来源：http://fk.panjiajie.cn

[G08] 静态方法与属性
来源：http://mh.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bl.huixiangedu.cn

PHP:  public static function f() {}
来源：http://uz.szsharing.cn

JS:   static f() {}
来源：http://nm.szxytkj.cn

TS:   static f(): void {}
来源：http://cn.shxzukj.cn

Java: static void f() {}
来源：http://aw.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jr.huanxung.cn

Ruby: def self.f; end
来源：http://da.hahajie.cn

C#:   public static void F() {}
来源：http://zo.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://mb.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://up.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xm.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ob.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://ec.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://ev.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://yl.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wh.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://ad.jctech888.com.cn

[G10] 访问控制
来源：http://sy.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://oh.lnxyls.cn

PHP:  public / protected / private
来源：http://fa.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://sm.hahajie.cn

TS:   public / protected / private
来源：http://yc.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://al.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ry.bjjhwx.cn

Ruby: public / protected / private
来源：http://gh.asd995.cn

C#:   public / protected / private / internal
来源：http://vr.asd995.cn

[G11] getter / setter
来源：http://ta.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://zq.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oo.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://bv.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://xd.lnxyls.cn

Java: public String getName() { return name; }
来源：http://kl.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ox.lnxyls.cn

Ruby: attr_accessor :name
来源：http://cy.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://ck.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://ol.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://fl.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hk.521024.cn

JS:   toString() { return this.name; }
来源：http://gc.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://cg.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://au.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ja.newstarts.cn

Ruby: def to_s; @name; end
来源：http://xk.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://nj.jctech888.com.cn

[G13] 判断对象类型
来源：http://jr.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://ge.szxytkj.cn

PHP:  $u instanceof User
来源：http://wd.newstarts.cn

JS:   u instanceof User
来源：http://pa.wgjwhj.cn

TS:   u instanceof User
来源：http://ax.newstarts.cn

Java: u instanceof User
来源：http://jc.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jr.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://sw.hahajie.cn

C#:   u is User
来源：http://wa.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://jc.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jv.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://cg.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xr.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://oo.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://di.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://pc.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jc.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://yh.lnxyls.cn

[G15] 枚举
来源：http://fw.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xk.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lu.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rb.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jo.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://jm.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gr.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://vy.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gg.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://jm.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yz.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://pk.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://of.huanxung.cn

TS:   Object.entries(obj)
来源：http://kv.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rx.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hy.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://kg.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://rw.haigaiapp.cn

================================================================================
来源：http://fx.jianghongdianzi.cn

H. 异常与错误处理
来源：http://jw.bjjhwx.cn

================================================================================
来源：http://ua.bookmarksfly.cn

[H01] try / catch 基础
来源：http://dc.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lc.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mf.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fh.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://om.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ri.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yq.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zc.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hr.nszjky.cn

[H02] finally / ensure 收尾
来源：http://sx.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qp.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fk.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ul.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ru.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fr.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pf.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://en.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zp.nszjky.cn

[H03] 主动抛出异常
来源：http://nv.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://cr.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://di.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://pu.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://aq.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wg.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ko.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rr.haigaiapp.cn


<!-- 参考信息 -->