代发 wailian999

[F01] 读取整个文件
来源：http://eu.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pi.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://ch.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://us.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mt.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nv.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zv.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://cd.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://gn.lnxyls.cn

[F02] 逐行读取文件
来源：http://tw.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iz.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ow.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://of.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bb.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bd.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://na.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ed.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lk.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://rg.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://is.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uo.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kx.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vf.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xg.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://to.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://mr.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ql.hnjuh.cn

[F04] 追加写入文件
来源：http://ju.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gm.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ez.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mp.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jp.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zz.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hk.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nn.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qd.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://jx.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://is.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://ql.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://ux.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://pk.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nj.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mw.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://zp.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://hh.shxzskj.cn

[F06] 删除文件
来源：http://gd.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://wj.newstarts.cn

PHP:  unlink("a.txt");
来源：http://cm.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dn.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://if.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wg.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://by.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://hb.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://hk.colortex.cn

[F07] 创建目录（含多级）
来源：http://ge.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xy.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yp.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xp.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vm.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rj.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://se.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tp.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xp.jianghongdianzi.cn

[F08] 遍历目录
来源：http://yt.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://of.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jt.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://ub.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://lp.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ex.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kt.nszjky.cn

Ruby: Dir.children("dir")
来源：http://uf.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://yk.wgjwhj.cn

[F09] 获取文件大小
来源：http://cp.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://kj.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://bi.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://wk.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://dw.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nt.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lm.9csxet.cn

Ruby: File.size("a.txt")
来源：http://gu.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://gp.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ut.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://km.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ro.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://od.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://ur.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gb.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ui.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mb.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kb.hahajie.cn

[F11] 复制与移动文件
来源：http://gf.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bm.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qs.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://na.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yr.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dg.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ns.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nn.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zn.shxzskj.cn

[F12] CSV 读写
来源：http://kb.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://me.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mb.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vh.huixinmuqiang.cn

TS:   // 同上
来源：http://qb.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ll.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ua.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ds.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xc.nicolike.cn

================================================================================
来源：http://vv.gzmigu.cn

G. 面向对象
来源：http://zu.hnjuh.cn

================================================================================
来源：http://zg.9csxet.cn

[G01] 定义类
来源：http://xz.szsharing.cn

Py:   class User: pass
来源：http://xp.hnjuh.cn

PHP:  class User {}
来源：http://kx.nicolike.cn

JS:   class User {}
来源：http://yn.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://rh.szsharing.cn

Java: class User {}
来源：http://ds.hnjuh.cn

Go:   type User struct { Name string }
来源：http://jb.bjjhwx.cn

Ruby: class User; end
来源：http://xf.gzmigu.cn

C#:   class User {}
来源：http://dw.hahajie.cn

[G02] 构造函数
来源：http://rw.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://sl.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://tv.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://zn.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://us.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://gy.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fg.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://kg.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://ot.colortex.cn

[G03] 实例属性
来源：http://sw.chemitech.net.cn

Py:   self.name = "x"
来源：http://as.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://kb.bjjhwx.cn

JS:   this.name = "x";
来源：http://xv.asd995.cn

TS:   name: string = "x";
来源：http://gn.wgjwhj.cn

Java: private String name;
来源：http://fz.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zz.nicolike.cn

Ruby: @name = "x"
来源：http://mm.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://jg.9csxet.cn

[G04] 定义方法
来源：http://gg.9csxet.cn

Py:   def greet(self): return self.name
来源：http://dq.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xy.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://hn.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://gu.colortex.cn

Java: String greet() { return name; }
来源：http://fi.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vx.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://ye.newstarts.cn

C#:   public string Greet() => Name;
来源：http://vh.szxytkj.cn

[G05] 继承
来源：http://hr.nicolike.cn

Py:   class Admin(User): pass
来源：http://ww.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://hd.shxzskj.cn

JS:   class Admin extends User {}
来源：http://ea.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://ly.shtwfgs.cn

Java: class Admin extends User {}
来源：http://kb.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://or.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://nq.nszjky.cn

C#:   class Admin : User {}
来源：http://vr.nszjky.cn

[G06] 重写方法
来源：http://jm.521024.cn

Py:   def greet(self): return "admin"
来源：http://ct.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oj.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://sv.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://pm.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://dg.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jt.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://st.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://ak.jctech888.com.cn

[G07] 调用父类方法
来源：http://lu.huixinmuqiang.cn

Py:   super().greet()
来源：http://rh.bjjhwx.cn

PHP:  parent::greet();
来源：http://xw.jctech888.com.cn

JS:   super.greet();
来源：http://ic.yuntaijiaju.cn

TS:   super.greet();
来源：http://ps.colortex.cn

Java: super.greet();
来源：http://cg.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://is.nicolike.cn

Ruby: super
来源：http://ct.haigaiapp.cn

C#:   base.Greet();
来源：http://zx.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://cc.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sg.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://yx.szsharing.cn

JS:   static f() {}
来源：http://wz.panjiajie.cn

TS:   static f(): void {}
来源：http://av.huanxung.cn

Java: static void f() {}
来源：http://ni.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ln.haigaiapp.cn

Ruby: def self.f; end
来源：http://dg.newstarts.cn

C#:   public static void F() {}
来源：http://ep.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://yv.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://ui.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ar.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zg.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://es.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://ok.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://wn.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mq.521024.cn

C#:   interface IShape { double Area(); }
来源：http://lp.9csxet.cn

[G10] 访问控制
来源：http://lo.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://no.9csxet.cn

PHP:  public / protected / private
来源：http://yv.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://xz.9csxet.cn

TS:   public / protected / private
来源：http://op.asd995.cn

Java: public / protected / private / 默认包级
来源：http://oy.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ku.bjjhwx.cn

Ruby: public / protected / private
来源：http://sg.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://eh.newstarts.cn

[G11] getter / setter
来源：http://ow.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://tw.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wf.colortex.cn

JS:   get name() { return this._name; }
来源：http://rw.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://wt.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://um.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ja.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://tu.newstarts.cn

C#:   public string Name { get; set; }
来源：http://ld.bjjhwx.cn

[G12] 对象转字符串
来源：http://fv.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://ao.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ec.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://xv.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://fd.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://bo.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yy.colortex.cn

Ruby: def to_s; @name; end
来源：http://ry.asd995.cn

C#:   public override string ToString() => Name;
来源：http://lv.hahajie.cn

[G13] 判断对象类型
来源：http://br.9csxet.cn

Py:   isinstance(u, User)
来源：http://tl.nicolike.cn

PHP:  $u instanceof User
来源：http://qj.wgjwhj.cn

JS:   u instanceof User
来源：http://tf.panjiajie.cn

TS:   u instanceof User
来源：http://yp.yuexingan06.cn

Java: u instanceof User
来源：http://co.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://so.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://ma.haigaiapp.cn

C#:   u is User
来源：http://mu.bookmarksfly.cn

[G14] 数据类 / record
来源：http://td.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uu.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://wk.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dg.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://sx.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://gb.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://jy.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ve.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://xh.muxihuayi.cn

[G15] 枚举
来源：http://yu.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jp.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uy.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nf.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ka.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://dk.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ru.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://qx.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ci.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://ba.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ka.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://ys.panjiajie.cn

JS:   Object.entries(obj)
来源：http://ya.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://fh.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cw.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lt.gzmigu.cn

Ruby: obj.instance_variables
来源：http://ym.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://sg.bjjhwx.cn

================================================================================
来源：http://de.521024.cn

H. 异常与错误处理
来源：http://we.shtwfgs.cn

================================================================================
来源：http://lt.huixiangedu.cn

[H01] try / catch 基础
来源：http://am.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://we.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qo.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jf.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ei.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xh.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ps.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sz.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://db.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://ow.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dn.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pm.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://et.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mo.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fs.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bn.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nz.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hj.bjjhwx.cn

[H03] 主动抛出异常
来源：http://wp.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://rf.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gy.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://tw.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://th.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wu.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xv.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jt.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jt.521024.cn

[H04] 自定义异常类型
来源：http://vy.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://xo.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nl.9csxet.cn

JS:   class MyError extends Error {}
来源：http://ky.szsharing.cn

TS:   class MyError extends Error {}
来源：http://xi.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://eb.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bu.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://sd.hahajie.cn

C#:   class MyException : Exception {}
来源：http://fd.9csxet.cn

[H05] 捕获特定类型
来源：http://eg.yuexingan06.cn

Py:   except ValueError as e:
来源：http://hz.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vc.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://iy.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://ep.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://pn.muxihuayi.cn


<!-- 参考信息 -->