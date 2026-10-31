代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://kc.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sg.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xw.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ae.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cu.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://wp.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vc.huanxung.cn

[F04] 追加写入文件
来源：http://qc.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pl.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yh.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ij.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yj.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://td.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ef.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ra.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://km.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://zu.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://il.colortex.cn

PHP:  file_exists("a.txt");
来源：http://tt.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://gy.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://pc.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aa.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rt.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://oe.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ld.colortex.cn

[F06] 删除文件
来源：http://dm.nszjky.cn

Py:   os.remove("a.txt")
来源：http://sm.nszjky.cn

PHP:  unlink("a.txt");
来源：http://sm.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vr.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wg.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cl.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://nm.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://do.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://zy.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://jn.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vv.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cf.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xc.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://si.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tu.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://is.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vn.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mm.hnjuh.cn

[F08] 遍历目录
来源：http://ei.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oz.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cg.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://kd.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://ln.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zr.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nd.szsharing.cn

Ruby: Dir.children("dir")
来源：http://nj.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://sc.bjjhwx.cn

[F09] 获取文件大小
来源：http://ze.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://ly.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://ny.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://go.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://rg.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wf.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ww.colortex.cn

Ruby: File.size("a.txt")
来源：http://wp.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://pf.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://tt.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eq.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fb.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xd.huanxung.cn

TS:   path.extname("a.txt")
来源：http://al.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lz.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wv.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ze.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iw.nszjky.cn

[F11] 复制与移动文件
来源：http://ba.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nn.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cj.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tj.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://js.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ls.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gu.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zs.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pj.huixinmuqiang.cn

[F12] CSV 读写
来源：http://ty.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://la.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ol.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://is.gzmigu.cn

TS:   // 同上
来源：http://jx.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hi.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jw.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ml.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ag.huixinmuqiang.cn

================================================================================
来源：http://cw.yuntaijiaju.cn

G. 面向对象
来源：http://uj.huixiangedu.cn

================================================================================
来源：http://yt.jianghongdianzi.cn

[G01] 定义类
来源：http://il.szsharing.cn

Py:   class User: pass
来源：http://tj.panjiajie.cn

PHP:  class User {}
来源：http://xy.szxytkj.cn

JS:   class User {}
来源：http://jo.521024.cn

TS:   class User { name: string = ""; }
来源：http://uw.bjjhwx.cn

Java: class User {}
来源：http://js.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://vp.jianghongdianzi.cn

Ruby: class User; end
来源：http://yp.asd995.cn

C#:   class User {}
来源：http://jr.huixinmuqiang.cn

[G02] 构造函数
来源：http://uz.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://je.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://tn.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://rp.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://so.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://qs.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sy.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://uf.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://sz.gzmigu.cn

[G03] 实例属性
来源：http://us.panjiajie.cn

Py:   self.name = "x"
来源：http://jn.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://fw.nszjky.cn

JS:   this.name = "x";
来源：http://bb.nszjky.cn

TS:   name: string = "x";
来源：http://dg.lnxyls.cn

Java: private String name;
来源：http://ao.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jc.colortex.cn

Ruby: @name = "x"
来源：http://tn.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://mw.shxzskj.cn

[G04] 定义方法
来源：http://ir.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://yc.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vq.nicolike.cn

JS:   greet() { return this.name; }
来源：http://ev.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://te.chemitech.net.cn

Java: String greet() { return name; }
来源：http://vo.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vx.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://ci.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://eo.huixinmuqiang.cn

[G05] 继承
来源：http://ck.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://dv.asd995.cn

PHP:  class Admin extends User {}
来源：http://vt.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://up.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://qj.521024.cn

Java: class Admin extends User {}
来源：http://sz.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ev.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://ck.yuexingan06.cn

C#:   class Admin : User {}
来源：http://jv.jianghongdianzi.cn

[G06] 重写方法
来源：http://hm.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://tw.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iz.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://ar.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ov.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://bv.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ii.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://vk.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://lf.hnjuh.cn

[G07] 调用父类方法
来源：http://rd.muxihuayi.cn

Py:   super().greet()
来源：http://bb.521024.cn

PHP:  parent::greet();
来源：http://rq.panjiajie.cn

JS:   super.greet();
来源：http://fe.huixiangedu.cn

TS:   super.greet();
来源：http://mg.asd995.cn

Java: super.greet();
来源：http://op.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dm.wgjwhj.cn

Ruby: super
来源：http://mu.gzmigu.cn

C#:   base.Greet();
来源：http://vz.lnxyls.cn

[G08] 静态方法与属性
来源：http://yb.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zu.lnxyls.cn

PHP:  public static function f() {}
来源：http://mg.nicolike.cn

JS:   static f() {}
来源：http://mk.hahajie.cn

TS:   static f(): void {}
来源：http://rt.9csxet.cn

Java: static void f() {}
来源：http://gw.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://st.521024.cn

Ruby: def self.f; end
来源：http://sg.colortex.cn

C#:   public static void F() {}
来源：http://kz.521024.cn

[G09] 接口 / 抽象类
来源：http://zd.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://ad.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ja.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zt.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://oy.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://nw.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://di.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cf.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://ha.shxzskj.cn

[G10] 访问控制
来源：http://lg.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://ag.nszjky.cn

PHP:  public / protected / private
来源：http://cb.hahajie.cn

JS:   #private 字段；其余公开
来源：http://lk.jianghongdianzi.cn

TS:   public / protected / private
来源：http://zi.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://cw.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ja.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://dh.nicolike.cn

C#:   public / protected / private / internal
来源：http://ii.shxzskj.cn

[G11] getter / setter
来源：http://du.nszjky.cn

Py:   @property 与 @x.setter
来源：http://tc.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mx.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://ux.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://om.shxzskj.cn

Java: public String getName() { return name; }
来源：http://yc.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pq.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://dn.szsharing.cn

C#:   public string Name { get; set; }
来源：http://wk.wgjwhj.cn

[G12] 对象转字符串
来源：http://is.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://hx.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mh.hahajie.cn

JS:   toString() { return this.name; }
来源：http://or.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://gy.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://ne.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ug.9csxet.cn

Ruby: def to_s; @name; end
来源：http://zg.colortex.cn

C#:   public override string ToString() => Name;
来源：http://fl.lnxyls.cn

[G13] 判断对象类型
来源：http://gp.gzmigu.cn

Py:   isinstance(u, User)
来源：http://xb.chemitech.net.cn

PHP:  $u instanceof User
来源：http://cu.nszjky.cn

JS:   u instanceof User
来源：http://zy.jctech888.com.cn

TS:   u instanceof User
来源：http://xf.nicolike.cn

Java: u instanceof User
来源：http://ms.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yw.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://bq.shxzskj.cn

C#:   u is User
来源：http://yf.colortex.cn

[G14] 数据类 / record
来源：http://lk.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vm.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://mf.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://el.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://ug.colortex.cn

Java: record User(String name, int age) {}
来源：http://ry.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://rs.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cd.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://at.bookmarksfly.cn

[G15] 枚举
来源：http://dc.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gn.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wc.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nt.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rj.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://ce.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vc.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://zo.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ce.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://gc.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ud.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://qk.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://ac.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://wm.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vc.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pq.nszjky.cn

Ruby: obj.instance_variables
来源：http://ho.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://ww.jctech888.com.cn

================================================================================
来源：http://jg.jianghongdianzi.cn

H. 异常与错误处理
来源：http://zf.nszjky.cn

================================================================================
来源：http://au.lnxyls.cn

[H01] try / catch 基础
来源：http://ni.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vr.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lx.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ma.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ol.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ls.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cl.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://an.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cj.newstarts.cn

[H02] finally / ensure 收尾
来源：http://hu.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hp.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ce.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mc.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nz.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sk.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://as.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tj.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jj.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://qd.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://qw.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ic.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://bs.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://ml.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://py.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vn.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ir.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cb.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://yc.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://gs.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nb.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://aw.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://ph.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://ew.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ug.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://gz.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://bh.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://vg.hahajie.cn

Py:   except ValueError as e:
来源：http://eg.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lm.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://vs.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://pa.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://df.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ds.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://wi.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xt.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://yr.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://pu.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://op.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nj.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://go.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tz.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://df.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://tv.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://jy.shxzukj.cn

[H07] 断言
来源：http://sa.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://lm.panjiajie.cn

PHP:  assert($x > 0);
来源：http://xo.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://sd.nicolike.cn

TS:   console.assert(x > 0);
来源：http://po.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://qv.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mi.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ox.hahajie.cn


<!-- 参考信息 -->