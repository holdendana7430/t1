代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://ly.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hk.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hx.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pr.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ix.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://oo.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lf.panjiajie.cn

[F04] 追加写入文件
来源：http://qh.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sd.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aa.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ja.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ff.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lu.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kv.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vj.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hh.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://dh.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uq.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://jb.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://jh.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://df.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hg.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ov.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://pj.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://fq.szsharing.cn

[F06] 删除文件
来源：http://jt.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://zw.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://xx.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kx.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ak.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gi.asd995.cn

Go:   os.Remove("a.txt")
来源：http://na.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://xd.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://pi.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://el.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zx.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sr.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ae.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cv.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xn.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://as.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ck.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xv.newstarts.cn

[F08] 遍历目录
来源：http://ou.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dp.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sm.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://lx.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://we.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jf.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oh.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://xy.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://wz.colortex.cn

[F09] 获取文件大小
来源：http://fj.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://wf.hahajie.cn

PHP:  filesize("a.txt");
来源：http://xe.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://ql.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://fd.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zs.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ph.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://ft.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://rn.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://tr.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qz.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xe.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sr.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://js.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://me.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ux.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gv.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jt.nicolike.cn

[F11] 复制与移动文件
来源：http://mg.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gi.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vw.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vl.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rj.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vl.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://os.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sx.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yd.shxzukj.cn

[F12] CSV 读写
来源：http://xz.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nu.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wp.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eu.wgjwhj.cn

TS:   // 同上
来源：http://ng.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ze.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zh.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ow.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ej.yuexingan06.cn

================================================================================
来源：http://mt.bookmarksfly.cn

G. 面向对象
来源：http://ss.jctech888.com.cn

================================================================================
来源：http://nu.huixiangedu.cn

[G01] 定义类
来源：http://nv.yuexingan06.cn

Py:   class User: pass
来源：http://nw.szxytkj.cn

PHP:  class User {}
来源：http://qj.wgjwhj.cn

JS:   class User {}
来源：http://fz.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://sx.nicolike.cn

Java: class User {}
来源：http://fz.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://bc.hahajie.cn

Ruby: class User; end
来源：http://gl.lnxyls.cn

C#:   class User {}
来源：http://fb.szsharing.cn

[G02] 构造函数
来源：http://mv.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://qx.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://lp.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://yb.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://pk.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://wv.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dv.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://fj.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://vb.haigaiapp.cn

[G03] 实例属性
来源：http://de.muxihuayi.cn

Py:   self.name = "x"
来源：http://xv.szsharing.cn

PHP:  public string $name = "x";
来源：http://mu.shtwfgs.cn

JS:   this.name = "x";
来源：http://op.szxytkj.cn

TS:   name: string = "x";
来源：http://ok.shxzukj.cn

Java: private String name;
来源：http://py.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yo.521024.cn

Ruby: @name = "x"
来源：http://nx.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://tl.muxihuayi.cn

[G04] 定义方法
来源：http://xr.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://ft.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gp.asd995.cn

JS:   greet() { return this.name; }
来源：http://pu.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://nm.wgjwhj.cn

Java: String greet() { return name; }
来源：http://tt.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ek.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://ne.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://uj.newstarts.cn

[G05] 继承
来源：http://hz.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ei.huanxung.cn

PHP:  class Admin extends User {}
来源：http://xk.szxytkj.cn

JS:   class Admin extends User {}
来源：http://la.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://yq.muxihuayi.cn

Java: class Admin extends User {}
来源：http://qn.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vk.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://jf.bjjhwx.cn

C#:   class Admin : User {}
来源：http://ha.521024.cn

[G06] 重写方法
来源：http://gv.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://dt.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ha.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://dt.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://iy.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://cw.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xd.521024.cn

Ruby: def greet; "admin"; end
来源：http://vb.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://ic.shtwfgs.cn

[G07] 调用父类方法
来源：http://na.521024.cn

Py:   super().greet()
来源：http://lx.huixiangedu.cn

PHP:  parent::greet();
来源：http://xb.yuexingan06.cn

JS:   super.greet();
来源：http://ov.shxzskj.cn

TS:   super.greet();
来源：http://uk.bookmarksfly.cn

Java: super.greet();
来源：http://zt.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tf.jianghongdianzi.cn

Ruby: super
来源：http://no.panjiajie.cn

C#:   base.Greet();
来源：http://xy.bjjhwx.cn

[G08] 静态方法与属性
来源：http://tv.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fh.colortex.cn

PHP:  public static function f() {}
来源：http://cq.chemitech.net.cn

JS:   static f() {}
来源：http://lz.colortex.cn

TS:   static f(): void {}
来源：http://yk.bjjhwx.cn

Java: static void f() {}
来源：http://bp.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wf.jctech888.com.cn

Ruby: def self.f; end
来源：http://tt.huanxung.cn

C#:   public static void F() {}
来源：http://ky.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://vq.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://qb.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://op.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zj.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://kz.szsharing.cn

Java: interface Shape { double area(); }
来源：http://xw.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ti.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fm.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://pt.9csxet.cn

[G10] 访问控制
来源：http://tu.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://dh.lnxyls.cn

PHP:  public / protected / private
来源：http://ag.nszjky.cn

JS:   #private 字段；其余公开
来源：http://cw.gzmigu.cn

TS:   public / protected / private
来源：http://ym.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://yp.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vc.nicolike.cn

Ruby: public / protected / private
来源：http://eo.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://bv.9csxet.cn

[G11] getter / setter
来源：http://hs.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://ie.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://in.nicolike.cn

JS:   get name() { return this._name; }
来源：http://qg.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://jz.9csxet.cn

Java: public String getName() { return name; }
来源：http://al.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ez.lnxyls.cn

Ruby: attr_accessor :name
来源：http://xy.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://xm.lnxyls.cn

[G12] 对象转字符串
来源：http://ba.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://hl.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cs.nicolike.cn

JS:   toString() { return this.name; }
来源：http://rz.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://wb.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://dj.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iy.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://wx.colortex.cn

C#:   public override string ToString() => Name;
来源：http://py.521024.cn

[G13] 判断对象类型
来源：http://qp.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://he.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://ow.huixinmuqiang.cn

JS:   u instanceof User
来源：http://gw.haigaiapp.cn

TS:   u instanceof User
来源：http://cg.newstarts.cn

Java: u instanceof User
来源：http://zj.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fp.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://ho.szxytkj.cn

C#:   u is User
来源：http://td.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://qg.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pg.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://kc.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://by.521024.cn

TS:   type User = { name: string; age: number };
来源：http://jp.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://zb.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://bg.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fi.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://vq.yuexingan06.cn

[G15] 枚举
来源：http://wd.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ya.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cq.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ys.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pi.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://ok.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://al.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://ws.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gc.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://qk.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://id.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://ac.lnxyls.cn

JS:   Object.entries(obj)
来源：http://xs.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://jb.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hk.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cl.nicolike.cn

Ruby: obj.instance_variables
来源：http://qj.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://wt.9csxet.cn

================================================================================
来源：http://jm.haigaiapp.cn

H. 异常与错误处理
来源：http://bo.huixinmuqiang.cn

================================================================================
来源：http://er.haigaiapp.cn

[H01] try / catch 基础
来源：http://fl.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qi.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yg.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yx.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ts.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://it.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vr.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tl.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ra.hahajie.cn

[H02] finally / ensure 收尾
来源：http://qs.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pp.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ou.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qb.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sb.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fn.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qt.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ks.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oh.jctech888.com.cn

[H03] 主动抛出异常
来源：http://cw.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://zf.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dg.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ln.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://or.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fr.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://da.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yq.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tm.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://rf.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://if.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zo.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://pq.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://if.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://ub.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rs.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ii.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://wc.shxzukj.cn

[H05] 捕获特定类型
来源：http://jp.szsharing.cn

Py:   except ValueError as e:
来源：http://hy.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xo.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ib.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://da.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://bi.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ur.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://gv.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ne.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://hb.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://or.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qv.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sc.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cd.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kh.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gq.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://qn.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://xj.yuexingan06.cn

[H07] 断言
来源：http://xw.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://qq.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://gb.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://ba.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://dz.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://xm.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vy.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yo.9csxet.cn


<!-- 参考信息 -->