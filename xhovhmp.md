代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pz.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://ug.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vh.9csxet.cn

[F04] 追加写入文件
来源：http://oy.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xb.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bj.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tf.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fj.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://au.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ug.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ww.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dx.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://mv.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yn.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://rl.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://pj.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://gi.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kb.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mp.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://me.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://ch.shtwfgs.cn

[F06] 删除文件
来源：http://fk.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://rt.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://ri.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lk.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nx.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ts.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://os.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://um.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://cb.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://mf.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cw.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xy.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bp.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ne.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ws.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vs.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tb.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nv.nszjky.cn

[F08] 遍历目录
来源：http://xg.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ur.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nt.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://bp.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://ar.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://po.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zs.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://yh.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://vk.szxytkj.cn

[F09] 获取文件大小
来源：http://pm.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://fi.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://fi.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://dk.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://jv.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://da.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yd.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://vp.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://er.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://dc.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ni.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tp.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ts.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://ka.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sd.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ch.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xu.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mu.chemitech.net.cn

[F11] 复制与移动文件
来源：http://yl.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rd.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bl.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://db.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://du.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fc.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ue.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jp.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tu.yuntaijiaju.cn

[F12] CSV 读写
来源：http://fa.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ej.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zt.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zy.hahajie.cn

TS:   // 同上
来源：http://jh.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rh.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pz.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ap.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kl.shxzskj.cn

================================================================================
来源：http://nz.nicolike.cn

G. 面向对象
来源：http://ly.bjjhwx.cn

================================================================================
来源：http://ym.chemitech.net.cn

[G01] 定义类
来源：http://kc.huixinmuqiang.cn

Py:   class User: pass
来源：http://jv.asd995.cn

PHP:  class User {}
来源：http://df.gzmigu.cn

JS:   class User {}
来源：http://ns.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://pa.szxytkj.cn

Java: class User {}
来源：http://fo.shxzukj.cn

Go:   type User struct { Name string }
来源：http://nm.nicolike.cn

Ruby: class User; end
来源：http://mh.hnjuh.cn

C#:   class User {}
来源：http://co.bookmarksfly.cn

[G02] 构造函数
来源：http://hi.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://xb.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://wy.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://ek.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://nt.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://vk.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tk.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://wj.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://mt.gzmigu.cn

[G03] 实例属性
来源：http://tb.newstarts.cn

Py:   self.name = "x"
来源：http://wa.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ud.colortex.cn

JS:   this.name = "x";
来源：http://kx.521024.cn

TS:   name: string = "x";
来源：http://op.yuntaijiaju.cn

Java: private String name;
来源：http://nt.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jq.yuexingan06.cn

Ruby: @name = "x"
来源：http://xv.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://rn.lnxyls.cn

[G04] 定义方法
来源：http://jg.szsharing.cn

Py:   def greet(self): return self.name
来源：http://nt.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ma.nicolike.cn

JS:   greet() { return this.name; }
来源：http://ma.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://jf.asd995.cn

Java: String greet() { return name; }
来源：http://zl.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hh.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://jw.hahajie.cn

C#:   public string Greet() => Name;
来源：http://wj.bookmarksfly.cn

[G05] 继承
来源：http://kj.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://fh.nszjky.cn

PHP:  class Admin extends User {}
来源：http://fh.hnjuh.cn

JS:   class Admin extends User {}
来源：http://sz.shxzukj.cn

TS:   class Admin extends User {}
来源：http://cd.shxzskj.cn

Java: class Admin extends User {}
来源：http://za.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pw.shxzukj.cn

Ruby: class Admin < User; end
来源：http://vi.521024.cn

C#:   class Admin : User {}
来源：http://za.huixiangedu.cn

[G06] 重写方法
来源：http://gg.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://zu.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lp.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://qk.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://vd.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://oz.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qa.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://gm.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://ah.gzmigu.cn

[G07] 调用父类方法
来源：http://jd.lnxyls.cn

Py:   super().greet()
来源：http://ho.chemitech.net.cn

PHP:  parent::greet();
来源：http://ol.gzmigu.cn

JS:   super.greet();
来源：http://dm.huanxung.cn

TS:   super.greet();
来源：http://ja.nicolike.cn

Java: super.greet();
来源：http://ax.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rt.szxytkj.cn

Ruby: super
来源：http://wv.shxzukj.cn

C#:   base.Greet();
来源：http://jw.lnxyls.cn

[G08] 静态方法与属性
来源：http://qp.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xm.nszjky.cn

PHP:  public static function f() {}
来源：http://hr.asd995.cn

JS:   static f() {}
来源：http://yx.nicolike.cn

TS:   static f(): void {}
来源：http://nv.9csxet.cn

Java: static void f() {}
来源：http://lo.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yo.huanxung.cn

Ruby: def self.f; end
来源：http://bb.hahajie.cn

C#:   public static void F() {}
来源：http://lg.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://bi.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://zj.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pv.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://su.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://hi.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://hd.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://dz.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://de.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://mt.hahajie.cn

[G10] 访问控制
来源：http://fi.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://sc.wgjwhj.cn

PHP:  public / protected / private
来源：http://gs.hahajie.cn

JS:   #private 字段；其余公开
来源：http://zh.521024.cn

TS:   public / protected / private
来源：http://xd.521024.cn

Java: public / protected / private / 默认包级
来源：http://yi.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wy.wgjwhj.cn

Ruby: public / protected / private
来源：http://tr.szsharing.cn

C#:   public / protected / private / internal
来源：http://ny.jctech888.com.cn

[G11] getter / setter
来源：http://ea.9csxet.cn

Py:   @property 与 @x.setter
来源：http://qm.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oi.colortex.cn

JS:   get name() { return this._name; }
来源：http://cx.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://ax.lnxyls.cn

Java: public String getName() { return name; }
来源：http://ex.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ki.szxytkj.cn

Ruby: attr_accessor :name
来源：http://vz.9csxet.cn

C#:   public string Name { get; set; }
来源：http://bf.newstarts.cn

[G12] 对象转字符串
来源：http://cn.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://en.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ny.nszjky.cn

JS:   toString() { return this.name; }
来源：http://eg.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://sn.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://ho.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lf.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://im.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://ya.nszjky.cn

[G13] 判断对象类型
来源：http://uo.gzmigu.cn

Py:   isinstance(u, User)
来源：http://pp.chemitech.net.cn

PHP:  $u instanceof User
来源：http://xk.nszjky.cn

JS:   u instanceof User
来源：http://hw.shxzskj.cn

TS:   u instanceof User
来源：http://em.nszjky.cn

Java: u instanceof User
来源：http://je.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rb.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://rg.shtwfgs.cn

C#:   u is User
来源：http://gu.szsharing.cn

[G14] 数据类 / record
来源：http://xw.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ow.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://zb.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mm.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://zm.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://yx.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://fe.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fc.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://uq.gzmigu.cn

[G15] 枚举
来源：http://ax.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gx.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pv.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vq.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qz.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://zl.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fc.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://um.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fq.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://kl.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://am.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://pf.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://lh.szsharing.cn

TS:   Object.entries(obj)
来源：http://lv.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cl.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://au.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://zr.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://yt.hnjuh.cn

================================================================================
来源：http://im.lnxyls.cn

H. 异常与错误处理
来源：http://tr.chemitech.net.cn

================================================================================
来源：http://ek.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://uf.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pi.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ta.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fq.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pr.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ui.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://um.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tt.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wp.9csxet.cn

[H02] finally / ensure 收尾
来源：http://rv.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qp.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rc.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fh.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dl.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jl.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uu.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ma.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tz.asd995.cn

[H03] 主动抛出异常
来源：http://mj.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://mg.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://su.colortex.cn

JS:   throw new Error("错误信息");
来源：http://ek.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://to.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wh.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ky.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qx.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zf.bjjhwx.cn

[H04] 自定义异常类型
来源：http://xy.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://lz.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pe.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://mv.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://ax.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://ck.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kr.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://pq.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://eu.asd995.cn

[H05] 捕获特定类型
来源：http://sn.colortex.cn

Py:   except ValueError as e:
来源：http://nt.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kq.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://ls.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://up.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://px.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yw.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://ga.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yu.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://bx.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://vg.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nf.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tn.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vr.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ss.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ds.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://ad.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://lh.shxzskj.cn

[H07] 断言
来源：http://lj.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://hz.nszjky.cn

PHP:  assert($x > 0);
来源：http://sf.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://xx.huanxung.cn

TS:   console.assert(x > 0);
来源：http://np.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://ok.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tr.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ns.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://sd.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://vp.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://ap.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yw.asd995.cn


<!-- 参考信息 -->