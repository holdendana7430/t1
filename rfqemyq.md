代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://em.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://qt.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kr.huixiangedu.cn

[F04] 追加写入文件
来源：http://kq.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eb.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ed.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zz.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jl.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wb.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mb.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fp.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ul.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://cx.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fh.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://jg.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://bw.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://dj.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ky.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sd.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://vx.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://fv.jianghongdianzi.cn

[F06] 删除文件
来源：http://pa.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://na.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://mf.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rj.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oa.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gy.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://xj.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://wq.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://gk.colortex.cn

[F07] 创建目录（含多级）
来源：http://gl.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://du.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jp.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xo.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xy.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nd.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sn.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ky.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gf.9csxet.cn

[F08] 遍历目录
来源：http://yx.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zz.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xz.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://ab.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://rs.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://up.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://he.9csxet.cn

Ruby: Dir.children("dir")
来源：http://vx.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://ut.lnxyls.cn

[F09] 获取文件大小
来源：http://ee.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://kg.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://es.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://ra.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://mv.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yf.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qz.newstarts.cn

Ruby: File.size("a.txt")
来源：http://kf.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://rg.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://bz.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vf.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ud.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gt.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://rb.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hf.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://li.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vi.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gv.chemitech.net.cn

[F11] 复制与移动文件
来源：http://tz.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mj.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cy.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yq.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ql.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iq.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ky.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bn.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qd.nszjky.cn

[F12] CSV 读写
来源：http://qs.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fn.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fi.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sg.521024.cn

TS:   // 同上
来源：http://qn.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cw.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ly.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ym.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gp.shxzukj.cn

================================================================================
来源：http://aq.huanxung.cn

G. 面向对象
来源：http://lg.521024.cn

================================================================================
来源：http://yg.huanxung.cn

[G01] 定义类
来源：http://ku.shxzukj.cn

Py:   class User: pass
来源：http://li.chemitech.net.cn

PHP:  class User {}
来源：http://sg.shxzukj.cn

JS:   class User {}
来源：http://et.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://lr.szxytkj.cn

Java: class User {}
来源：http://ia.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://il.haigaiapp.cn

Ruby: class User; end
来源：http://iy.huanxung.cn

C#:   class User {}
来源：http://nw.wgjwhj.cn

[G02] 构造函数
来源：http://cm.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://iz.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://ep.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ub.521024.cn

TS:   constructor(public name: string) {}
来源：http://no.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://oq.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bz.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ub.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://nb.nszjky.cn

[G03] 实例属性
来源：http://mr.wgjwhj.cn

Py:   self.name = "x"
来源：http://xo.gzmigu.cn

PHP:  public string $name = "x";
来源：http://yx.shxzskj.cn

JS:   this.name = "x";
来源：http://vg.nszjky.cn

TS:   name: string = "x";
来源：http://ig.colortex.cn

Java: private String name;
来源：http://qt.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zz.chemitech.net.cn

Ruby: @name = "x"
来源：http://lo.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://my.panjiajie.cn

[G04] 定义方法
来源：http://yi.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://oq.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://el.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://cg.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://xu.hnjuh.cn

Java: String greet() { return name; }
来源：http://ze.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lf.panjiajie.cn

Ruby: def greet; @name; end
来源：http://gf.9csxet.cn

C#:   public string Greet() => Name;
来源：http://hi.newstarts.cn

[G05] 继承
来源：http://rf.shxzukj.cn

Py:   class Admin(User): pass
来源：http://bk.hahajie.cn

PHP:  class Admin extends User {}
来源：http://nq.panjiajie.cn

JS:   class Admin extends User {}
来源：http://iz.asd995.cn

TS:   class Admin extends User {}
来源：http://dv.nicolike.cn

Java: class Admin extends User {}
来源：http://wj.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bl.shxzskj.cn

Ruby: class Admin < User; end
来源：http://js.hnjuh.cn

C#:   class Admin : User {}
来源：http://ps.lnxyls.cn

[G06] 重写方法
来源：http://fp.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://vd.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yc.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://iv.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://wg.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://oa.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xo.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://za.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://zb.521024.cn

[G07] 调用父类方法
来源：http://qr.yuexingan06.cn

Py:   super().greet()
来源：http://mm.lnxyls.cn

PHP:  parent::greet();
来源：http://wl.szxytkj.cn

JS:   super.greet();
来源：http://ax.szxytkj.cn

TS:   super.greet();
来源：http://ed.chemitech.net.cn

Java: super.greet();
来源：http://vi.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zo.nicolike.cn

Ruby: super
来源：http://tp.huanxung.cn

C#:   base.Greet();
来源：http://dd.gzmigu.cn

[G08] 静态方法与属性
来源：http://tb.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jt.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://qt.huixinmuqiang.cn

JS:   static f() {}
来源：http://xg.asd995.cn

TS:   static f(): void {}
来源：http://lw.yuntaijiaju.cn

Java: static void f() {}
来源：http://mb.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ii.haigaiapp.cn

Ruby: def self.f; end
来源：http://uw.huixiangedu.cn

C#:   public static void F() {}
来源：http://oa.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://or.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://rl.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sr.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nm.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://rf.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://zf.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://dn.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aq.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://ui.wgjwhj.cn

[G10] 访问控制
来源：http://ow.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://zk.nicolike.cn

PHP:  public / protected / private
来源：http://ys.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://mu.gzmigu.cn

TS:   public / protected / private
来源：http://jx.asd995.cn

Java: public / protected / private / 默认包级
来源：http://rr.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://at.lnxyls.cn

Ruby: public / protected / private
来源：http://fs.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://tp.lnxyls.cn

[G11] getter / setter
来源：http://nc.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://hi.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ep.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://lb.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://jv.panjiajie.cn

Java: public String getName() { return name; }
来源：http://du.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ax.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://yv.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://hc.yuexingan06.cn

[G12] 对象转字符串
来源：http://ev.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://qw.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mu.newstarts.cn

JS:   toString() { return this.name; }
来源：http://st.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://sp.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://sy.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nj.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ja.521024.cn

C#:   public override string ToString() => Name;
来源：http://bv.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://xe.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://el.colortex.cn

PHP:  $u instanceof User
来源：http://ns.jianghongdianzi.cn

JS:   u instanceof User
来源：http://hy.yuntaijiaju.cn

TS:   u instanceof User
来源：http://ox.szxytkj.cn

Java: u instanceof User
来源：http://ne.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kb.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://fi.szsharing.cn

C#:   u is User
来源：http://om.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://vh.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://do.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://hz.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kl.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://qm.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://co.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://xj.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ny.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://om.haigaiapp.cn

[G15] 枚举
来源：http://qf.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fy.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wq.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wm.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uq.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://au.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cp.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://xl.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wq.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://sg.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ot.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://sq.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://qq.newstarts.cn

TS:   Object.entries(obj)
来源：http://eq.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pn.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bf.szsharing.cn

Ruby: obj.instance_variables
来源：http://qw.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ci.nszjky.cn

================================================================================
来源：http://lp.yuexingan06.cn

H. 异常与错误处理
来源：http://nb.szxytkj.cn

================================================================================
来源：http://at.bookmarksfly.cn

[H01] try / catch 基础
来源：http://ss.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ge.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tu.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pi.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xd.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hf.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ls.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nt.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://is.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://pl.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fg.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hx.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://se.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ke.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://co.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ur.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jw.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://il.nszjky.cn

[H03] 主动抛出异常
来源：http://dh.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://cv.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vi.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://sf.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://lf.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://en.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ji.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ar.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sg.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://wg.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://qv.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ki.colortex.cn

JS:   class MyError extends Error {}
来源：http://iq.huanxung.cn

TS:   class MyError extends Error {}
来源：http://bd.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://jq.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yt.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://ak.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://zk.lnxyls.cn

[H05] 捕获特定类型
来源：http://iy.wgjwhj.cn

Py:   except ValueError as e:
来源：http://bn.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cp.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://dm.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://fb.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://sb.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qh.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://rq.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fb.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://kd.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://qe.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zx.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fh.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lx.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ac.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nc.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://pk.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://tw.shtwfgs.cn

[H07] 断言
来源：http://st.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://bq.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://pd.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://fy.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://xw.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://pf.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dw.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nt.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://fw.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://yl.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://yy.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xp.yuexingan06.cn


<!-- 参考信息 -->