代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dn.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aq.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kr.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://of.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hf.nszjky.cn

================================================================================
来源：http://yk.jctech888.com.cn

F. 文件与目录
来源：http://gj.bookmarksfly.cn

================================================================================
来源：http://il.szxytkj.cn

[F01] 读取整个文件
来源：http://td.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eq.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://mx.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ca.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ee.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ds.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ku.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://mm.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://wd.szsharing.cn

[F02] 逐行读取文件
来源：http://tl.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rh.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nv.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hq.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fx.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rd.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gf.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bu.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nn.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://qh.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yv.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gv.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jj.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://op.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oz.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hf.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://dj.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ep.nicolike.cn

[F04] 追加写入文件
来源：http://mc.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ch.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://af.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mx.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ln.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://op.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jc.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qq.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rh.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://ma.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kf.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://xa.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://bo.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://ki.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vq.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pn.521024.cn

Ruby: File.exist?("a.txt")
来源：http://oz.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://pr.wgjwhj.cn

[F06] 删除文件
来源：http://jh.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://sb.asd995.cn

PHP:  unlink("a.txt");
来源：http://rj.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wo.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dv.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fm.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://tm.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://jp.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://wy.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://jg.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ic.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://to.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ir.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pn.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oy.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aj.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gh.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rk.gzmigu.cn

[F08] 遍历目录
来源：http://xc.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kr.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bh.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://gm.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://tw.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qi.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bu.nicolike.cn

Ruby: Dir.children("dir")
来源：http://ef.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://nd.newstarts.cn

[F09] 获取文件大小
来源：http://tn.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://ke.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ze.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://or.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://cq.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qq.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zv.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://ku.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://xy.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://cw.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://of.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yk.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mk.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://jd.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yb.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iu.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rg.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://in.haigaiapp.cn

[F11] 复制与移动文件
来源：http://xt.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ek.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vo.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xr.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lm.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qu.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://su.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pp.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ng.panjiajie.cn

[F12] CSV 读写
来源：http://od.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hl.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ai.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cx.szsharing.cn

TS:   // 同上
来源：http://so.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ek.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ef.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ls.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ul.yuexingan06.cn

================================================================================
来源：http://lf.yuntaijiaju.cn

G. 面向对象
来源：http://ns.szxytkj.cn

================================================================================
来源：http://ry.szsharing.cn

[G01] 定义类
来源：http://uu.shtwfgs.cn

Py:   class User: pass
来源：http://wo.szsharing.cn

PHP:  class User {}
来源：http://sr.huixinmuqiang.cn

JS:   class User {}
来源：http://cm.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://ns.chemitech.net.cn

Java: class User {}
来源：http://jo.colortex.cn

Go:   type User struct { Name string }
来源：http://tf.nszjky.cn

Ruby: class User; end
来源：http://rb.nszjky.cn

C#:   class User {}
来源：http://gn.gzmigu.cn

[G02] 构造函数
来源：http://qc.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://gi.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://iz.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://vj.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://vp.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://sb.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lc.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://gf.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://oo.9csxet.cn

[G03] 实例属性
来源：http://yy.wgjwhj.cn

Py:   self.name = "x"
来源：http://wv.szxytkj.cn

PHP:  public string $name = "x";
来源：http://ci.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://wq.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://au.jianghongdianzi.cn

Java: private String name;
来源：http://so.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mj.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://qh.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://iy.bookmarksfly.cn

[G04] 定义方法
来源：http://bf.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://cf.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hw.9csxet.cn

JS:   greet() { return this.name; }
来源：http://pl.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://cq.nicolike.cn

Java: String greet() { return name; }
来源：http://jg.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mv.huanxung.cn

Ruby: def greet; @name; end
来源：http://pz.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://gs.asd995.cn

[G05] 继承
来源：http://gq.nszjky.cn

Py:   class Admin(User): pass
来源：http://eq.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://ov.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://gj.szsharing.cn

TS:   class Admin extends User {}
来源：http://lk.asd995.cn

Java: class Admin extends User {}
来源：http://bn.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pg.newstarts.cn

Ruby: class Admin < User; end
来源：http://iw.521024.cn

C#:   class Admin : User {}
来源：http://qo.nszjky.cn

[G06] 重写方法
来源：http://jp.asd995.cn

Py:   def greet(self): return "admin"
来源：http://ud.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bw.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://gy.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://iy.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://yh.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uz.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://jz.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://sd.hahajie.cn

[G07] 调用父类方法
来源：http://ra.shxzukj.cn

Py:   super().greet()
来源：http://ve.gzmigu.cn

PHP:  parent::greet();
来源：http://iw.wgjwhj.cn

JS:   super.greet();
来源：http://qg.bjjhwx.cn

TS:   super.greet();
来源：http://cb.colortex.cn

Java: super.greet();
来源：http://yr.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xd.newstarts.cn

Ruby: super
来源：http://tj.nszjky.cn

C#:   base.Greet();
来源：http://ot.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://pw.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fn.huixiangedu.cn

PHP:  public static function f() {}
来源：http://gy.9csxet.cn

JS:   static f() {}
来源：http://ch.521024.cn

TS:   static f(): void {}
来源：http://by.huanxung.cn

Java: static void f() {}
来源：http://lo.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xm.jctech888.com.cn

Ruby: def self.f; end
来源：http://sw.huanxung.cn

C#:   public static void F() {}
来源：http://eh.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://in.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://fq.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vu.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ha.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://vm.colortex.cn

Java: interface Shape { double area(); }
来源：http://at.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://rj.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iv.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://yj.newstarts.cn

[G10] 访问控制
来源：http://uu.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://md.haigaiapp.cn

PHP:  public / protected / private
来源：http://ry.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://sb.hahajie.cn

TS:   public / protected / private
来源：http://zs.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://jf.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cm.haigaiapp.cn

Ruby: public / protected / private
来源：http://zf.hahajie.cn

C#:   public / protected / private / internal
来源：http://nr.shxzskj.cn

[G11] getter / setter
来源：http://vr.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://kv.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fw.huanxung.cn

JS:   get name() { return this._name; }
来源：http://qc.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://oa.huanxung.cn

Java: public String getName() { return name; }
来源：http://tt.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vt.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://dj.asd995.cn

C#:   public string Name { get; set; }
来源：http://ud.nszjky.cn

[G12] 对象转字符串
来源：http://fj.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://ub.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mx.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://sd.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://hh.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://vw.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jl.asd995.cn

Ruby: def to_s; @name; end
来源：http://su.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://pt.huanxung.cn

[G13] 判断对象类型
来源：http://oi.9csxet.cn

Py:   isinstance(u, User)
来源：http://tc.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ei.muxihuayi.cn

JS:   u instanceof User
来源：http://dk.huixiangedu.cn

TS:   u instanceof User
来源：http://sq.shxzukj.cn

Java: u instanceof User
来源：http://kl.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dy.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://ue.szxytkj.cn

C#:   u is User
来源：http://zf.newstarts.cn

[G14] 数据类 / record
来源：http://fo.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xh.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://su.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lt.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://ly.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://mp.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://el.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lz.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://wv.nszjky.cn

[G15] 枚举
来源：http://bo.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ig.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ha.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ez.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ge.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://mn.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ya.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://rp.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ha.asd995.cn

[G16] 对象转数组 / 字典
来源：http://ff.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lc.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://wo.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://fr.521024.cn

TS:   Object.entries(obj)
来源：http://ka.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ih.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ie.newstarts.cn

Ruby: obj.instance_variables
来源：http://rb.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://xe.hnjuh.cn

================================================================================
来源：http://kd.hahajie.cn

H. 异常与错误处理
来源：http://ee.nszjky.cn

================================================================================
来源：http://td.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://dm.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ni.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gq.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bi.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zt.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lp.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://js.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nd.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sm.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://we.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wh.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mz.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rq.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wk.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://py.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nu.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ei.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ev.shtwfgs.cn

[H03] 主动抛出异常
来源：http://br.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://no.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tw.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://eu.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://ht.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yy.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ca.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wa.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://po.szsharing.cn

[H04] 自定义异常类型
来源：http://ao.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://pu.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ke.szsharing.cn

JS:   class MyError extends Error {}
来源：http://lt.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://bs.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://yj.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fd.shxzukj.cn


<!-- 参考信息 -->