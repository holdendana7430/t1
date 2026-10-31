代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gw.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://xq.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://md.szsharing.cn

[F04] 追加写入文件
来源：http://px.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ah.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kr.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wg.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ox.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fy.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pl.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mx.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jz.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://fy.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lz.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://se.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://eu.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://mo.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qb.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dj.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://em.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://uy.lnxyls.cn

[F06] 删除文件
来源：http://ey.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://zo.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://yy.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hc.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rh.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fu.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://jg.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://xy.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://ia.colortex.cn

[F07] 创建目录（含多级）
来源：http://qe.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xu.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://go.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vp.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sz.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://us.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bt.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rt.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ip.yuntaijiaju.cn

[F08] 遍历目录
来源：http://vi.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://je.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zt.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://qb.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://tk.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://va.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rh.9csxet.cn

Ruby: Dir.children("dir")
来源：http://mr.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://tt.shxzukj.cn

[F09] 获取文件大小
来源：http://ua.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://gh.colortex.cn

PHP:  filesize("a.txt");
来源：http://kk.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://vl.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://cz.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rj.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pi.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://yt.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://yc.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://eh.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uy.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bz.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bf.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://kh.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mq.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cy.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bv.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tm.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://mj.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bf.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://os.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nb.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uv.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cg.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bk.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pg.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ip.muxihuayi.cn

[F12] CSV 读写
来源：http://ue.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ml.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fb.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vb.panjiajie.cn

TS:   // 同上
来源：http://xp.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ao.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jw.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eh.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mp.huanxung.cn

================================================================================
来源：http://kv.nicolike.cn

G. 面向对象
来源：http://eh.hnjuh.cn

================================================================================
来源：http://ht.shxzukj.cn

[G01] 定义类
来源：http://ds.bjjhwx.cn

Py:   class User: pass
来源：http://rl.nszjky.cn

PHP:  class User {}
来源：http://ul.szsharing.cn

JS:   class User {}
来源：http://ow.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://xu.gzmigu.cn

Java: class User {}
来源：http://ls.521024.cn

Go:   type User struct { Name string }
来源：http://mk.yuntaijiaju.cn

Ruby: class User; end
来源：http://dj.yuexingan06.cn

C#:   class User {}
来源：http://mo.jianghongdianzi.cn

[G02] 构造函数
来源：http://kb.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://pw.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://sp.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://sx.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://el.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://xt.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uh.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://wi.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://sq.asd995.cn

[G03] 实例属性
来源：http://fb.colortex.cn

Py:   self.name = "x"
来源：http://rx.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://fw.asd995.cn

JS:   this.name = "x";
来源：http://tv.521024.cn

TS:   name: string = "x";
来源：http://bu.bjjhwx.cn

Java: private String name;
来源：http://jv.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gw.jctech888.com.cn

Ruby: @name = "x"
来源：http://rs.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://qw.shxzskj.cn

[G04] 定义方法
来源：http://dz.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://tz.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ra.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://oc.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://po.szsharing.cn

Java: String greet() { return name; }
来源：http://ww.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ob.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://xe.hahajie.cn

C#:   public string Greet() => Name;
来源：http://mj.szxytkj.cn

[G05] 继承
来源：http://uq.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://qw.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://vf.9csxet.cn

JS:   class Admin extends User {}
来源：http://db.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://dt.521024.cn

Java: class Admin extends User {}
来源：http://mk.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zp.colortex.cn

Ruby: class Admin < User; end
来源：http://ns.shxzskj.cn

C#:   class Admin : User {}
来源：http://ki.shxzukj.cn

[G06] 重写方法
来源：http://zr.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://ht.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bx.colortex.cn

JS:   greet() { return "admin"; }
来源：http://ih.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://ng.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://zz.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qu.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://cn.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://at.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://sq.huixiangedu.cn

Py:   super().greet()
来源：http://tm.chemitech.net.cn

PHP:  parent::greet();
来源：http://gk.huixiangedu.cn

JS:   super.greet();
来源：http://xm.jctech888.com.cn

TS:   super.greet();
来源：http://uy.haigaiapp.cn

Java: super.greet();
来源：http://jl.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jg.asd995.cn

Ruby: super
来源：http://pb.wgjwhj.cn

C#:   base.Greet();
来源：http://eu.shxzukj.cn

[G08] 静态方法与属性
来源：http://ep.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ij.shxzskj.cn

PHP:  public static function f() {}
来源：http://ol.yuntaijiaju.cn

JS:   static f() {}
来源：http://yp.9csxet.cn

TS:   static f(): void {}
来源：http://iy.gzmigu.cn

Java: static void f() {}
来源：http://lc.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ao.muxihuayi.cn

Ruby: def self.f; end
来源：http://mm.chemitech.net.cn

C#:   public static void F() {}
来源：http://ac.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://ul.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://jp.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wg.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ut.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://nw.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://sm.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ut.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nl.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://ka.shxzskj.cn

[G10] 访问控制
来源：http://ab.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://fm.hnjuh.cn

PHP:  public / protected / private
来源：http://hg.521024.cn

JS:   #private 字段；其余公开
来源：http://po.haigaiapp.cn

TS:   public / protected / private
来源：http://xv.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ve.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fz.9csxet.cn

Ruby: public / protected / private
来源：http://zu.lnxyls.cn

C#:   public / protected / private / internal
来源：http://tw.huixiangedu.cn

[G11] getter / setter
来源：http://kr.nszjky.cn

Py:   @property 与 @x.setter
来源：http://is.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lq.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://rw.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://rc.shxzukj.cn

Java: public String getName() { return name; }
来源：http://rz.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jc.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://xf.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://lv.bjjhwx.cn

[G12] 对象转字符串
来源：http://vt.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://fw.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://go.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://rw.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://ym.521024.cn

Java: @Override public String toString() { return name; }
来源：http://kr.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xe.hahajie.cn

Ruby: def to_s; @name; end
来源：http://ce.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://qq.shxzukj.cn

[G13] 判断对象类型
来源：http://iz.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://ht.521024.cn

PHP:  $u instanceof User
来源：http://gl.haigaiapp.cn

JS:   u instanceof User
来源：http://hx.gzmigu.cn

TS:   u instanceof User
来源：http://cl.wgjwhj.cn

Java: u instanceof User
来源：http://nk.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lq.colortex.cn

Ruby: u.is_a?(User)
来源：http://ya.hnjuh.cn

C#:   u is User
来源：http://hg.huanxung.cn

[G14] 数据类 / record
来源：http://gj.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dh.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://hl.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xf.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://of.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://xu.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://kc.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qr.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://in.yuexingan06.cn

[G15] 枚举
来源：http://ij.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ke.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hl.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ul.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xo.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://df.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sn.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://ls.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gf.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://zl.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ml.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://qj.asd995.cn

JS:   Object.entries(obj)
来源：http://dh.colortex.cn

TS:   Object.entries(obj)
来源：http://be.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wn.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://el.szsharing.cn

Ruby: obj.instance_variables
来源：http://ku.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://py.szxytkj.cn

================================================================================
来源：http://yo.wgjwhj.cn

H. 异常与错误处理
来源：http://tg.nicolike.cn

================================================================================
来源：http://xt.colortex.cn

[H01] try / catch 基础
来源：http://sl.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wl.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nf.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iv.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zy.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ir.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yq.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://or.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sv.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://mn.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gm.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qf.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kn.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cw.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vs.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eg.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ku.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vp.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://ec.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ni.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rk.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://jx.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://dg.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bz.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mj.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wa.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kw.521024.cn

[H04] 自定义异常类型
来源：http://ob.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://bp.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sa.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://hu.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://do.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://yl.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bw.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ok.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://kr.chemitech.net.cn

[H05] 捕获特定类型
来源：http://zw.nszjky.cn

Py:   except ValueError as e:
来源：http://qf.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vq.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://pt.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://dc.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ui.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ja.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://mn.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://to.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://nw.szsharing.cn

Py:   value = d.get("k") or default
来源：http://ce.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://im.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ug.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qn.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fj.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ch.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://qd.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://jy.jianghongdianzi.cn

[H07] 断言
来源：http://oq.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://dj.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://fn.colortex.cn

JS:   console.assert(x > 0);
来源：http://cv.newstarts.cn

TS:   console.assert(x > 0);
来源：http://fd.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://bg.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lt.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pj.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://aq.521024.cn

[H08] 获取错误信息与堆栈
来源：http://ak.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://qb.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aq.hnjuh.cn


<!-- 参考信息 -->