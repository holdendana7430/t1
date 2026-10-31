代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://st.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dk.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ui.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tg.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://di.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hc.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ob.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tu.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://rv.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tt.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://ol.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://dz.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://tg.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zo.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://nn.asd995.cn

C#:   File.Exists("a.txt")
来源：http://cp.hahajie.cn

[F06] 删除文件
来源：http://no.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://in.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://tr.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ph.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://py.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bn.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://yg.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://to.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://qf.colortex.cn

[F07] 创建目录（含多级）
来源：http://jg.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bv.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pk.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mw.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qv.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zy.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fr.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://si.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ob.shtwfgs.cn

[F08] 遍历目录
来源：http://hv.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ao.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pg.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://hj.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://zx.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://st.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yi.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://qd.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://bi.shtwfgs.cn

[F09] 获取文件大小
来源：http://gu.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://ax.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://ya.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://aj.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://pg.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://if.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fi.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://hu.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://iz.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://hw.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ab.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fx.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lm.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://ro.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://to.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dp.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ba.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ws.szsharing.cn

[F11] 复制与移动文件
来源：http://hh.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bt.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ie.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ef.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cb.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fu.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://th.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ik.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bs.lnxyls.cn

[F12] CSV 读写
来源：http://qv.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gm.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cj.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zd.hahajie.cn

TS:   // 同上
来源：http://kt.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jm.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ki.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wy.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ip.yuexingan06.cn

================================================================================
来源：http://so.szsharing.cn

G. 面向对象
来源：http://hg.nicolike.cn

================================================================================
来源：http://rw.521024.cn

[G01] 定义类
来源：http://ta.521024.cn

Py:   class User: pass
来源：http://wg.lnxyls.cn

PHP:  class User {}
来源：http://ig.huixiangedu.cn

JS:   class User {}
来源：http://rb.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ce.szsharing.cn

Java: class User {}
来源：http://cu.shxzukj.cn

Go:   type User struct { Name string }
来源：http://ar.521024.cn

Ruby: class User; end
来源：http://bq.shxzskj.cn

C#:   class User {}
来源：http://an.shtwfgs.cn

[G02] 构造函数
来源：http://lw.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://pm.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://vd.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://qj.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://of.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://lm.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xq.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://wl.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://wa.huanxung.cn

[G03] 实例属性
来源：http://wv.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://od.newstarts.cn

PHP:  public string $name = "x";
来源：http://ad.bookmarksfly.cn

JS:   this.name = "x";
来源：http://yi.bookmarksfly.cn

TS:   name: string = "x";
来源：http://yt.shxzukj.cn

Java: private String name;
来源：http://wq.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cy.szxytkj.cn

Ruby: @name = "x"
来源：http://je.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ky.gzmigu.cn

[G04] 定义方法
来源：http://so.nszjky.cn

Py:   def greet(self): return self.name
来源：http://le.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oc.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://uy.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://qp.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ka.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sg.lnxyls.cn

Ruby: def greet; @name; end
来源：http://dt.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://aj.yuexingan06.cn

[G05] 继承
来源：http://gm.9csxet.cn

Py:   class Admin(User): pass
来源：http://vi.asd995.cn

PHP:  class Admin extends User {}
来源：http://dp.colortex.cn

JS:   class Admin extends User {}
来源：http://ts.hahajie.cn

TS:   class Admin extends User {}
来源：http://xp.huanxung.cn

Java: class Admin extends User {}
来源：http://nm.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tl.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://ko.huixiangedu.cn

C#:   class Admin : User {}
来源：http://pe.jianghongdianzi.cn

[G06] 重写方法
来源：http://yr.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://mu.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://am.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ek.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://av.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://hr.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eh.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://bd.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ch.bookmarksfly.cn

[G07] 调用父类方法
来源：http://az.bjjhwx.cn

Py:   super().greet()
来源：http://kb.jctech888.com.cn

PHP:  parent::greet();
来源：http://ru.haigaiapp.cn

JS:   super.greet();
来源：http://ej.newstarts.cn

TS:   super.greet();
来源：http://nj.shxzskj.cn

Java: super.greet();
来源：http://sb.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ef.yuexingan06.cn

Ruby: super
来源：http://fp.huixiangedu.cn

C#:   base.Greet();
来源：http://wf.huanxung.cn

[G08] 静态方法与属性
来源：http://ep.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://in.jctech888.com.cn

PHP:  public static function f() {}
来源：http://kj.szsharing.cn

JS:   static f() {}
来源：http://kr.shxzskj.cn

TS:   static f(): void {}
来源：http://mu.shxzukj.cn

Java: static void f() {}
来源：http://ws.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jo.newstarts.cn

Ruby: def self.f; end
来源：http://au.nicolike.cn

C#:   public static void F() {}
来源：http://gh.9csxet.cn

[G09] 接口 / 抽象类
来源：http://vq.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://nt.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://el.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yp.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://if.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://ie.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://to.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nx.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://tj.nicolike.cn

[G10] 访问控制
来源：http://gg.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hq.9csxet.cn

PHP:  public / protected / private
来源：http://ad.521024.cn

JS:   #private 字段；其余公开
来源：http://xj.huixinmuqiang.cn

TS:   public / protected / private
来源：http://xd.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://vn.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tz.bookmarksfly.cn

Ruby: public / protected / private
来源：http://cr.nicolike.cn

C#:   public / protected / private / internal
来源：http://kk.colortex.cn

[G11] getter / setter
来源：http://lx.huanxung.cn

Py:   @property 与 @x.setter
来源：http://av.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xo.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://gi.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://mk.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://uu.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sm.nicolike.cn

Ruby: attr_accessor :name
来源：http://ze.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://xx.newstarts.cn

[G12] 对象转字符串
来源：http://ss.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://qk.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lu.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://yn.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://fx.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://zj.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://em.521024.cn

Ruby: def to_s; @name; end
来源：http://xl.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://xn.panjiajie.cn

[G13] 判断对象类型
来源：http://vn.asd995.cn

Py:   isinstance(u, User)
来源：http://bp.huanxung.cn

PHP:  $u instanceof User
来源：http://dj.chemitech.net.cn

JS:   u instanceof User
来源：http://mg.521024.cn

TS:   u instanceof User
来源：http://nm.newstarts.cn

Java: u instanceof User
来源：http://eq.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zk.nszjky.cn

Ruby: u.is_a?(User)
来源：http://ul.nicolike.cn

C#:   u is User
来源：http://td.bjjhwx.cn

[G14] 数据类 / record
来源：http://nt.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xa.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://yl.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qg.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://ea.nicolike.cn

Java: record User(String name, int age) {}
来源：http://es.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://xe.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lu.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://og.bjjhwx.cn

[G15] 枚举
来源：http://ab.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lw.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kg.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oy.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ta.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://zh.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pi.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://xk.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cw.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://hd.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jy.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://qx.huanxung.cn

JS:   Object.entries(obj)
来源：http://il.asd995.cn

TS:   Object.entries(obj)
来源：http://gx.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jd.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ek.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://lu.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://tm.huixiangedu.cn

================================================================================
来源：http://pq.yuexingan06.cn

H. 异常与错误处理
来源：http://ib.szsharing.cn

================================================================================
来源：http://zm.newstarts.cn

[H01] try / catch 基础
来源：http://xc.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ib.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://al.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pw.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mu.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gw.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dg.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yp.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qn.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://au.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bi.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zx.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dv.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oe.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bh.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oe.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ji.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wx.gzmigu.cn

[H03] 主动抛出异常
来源：http://wm.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://gz.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wp.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://re.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://nx.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uq.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bp.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://om.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://it.chemitech.net.cn

[H04] 自定义异常类型
来源：http://ln.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://vy.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sx.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://px.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://ky.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://bh.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ar.521024.cn

Ruby: class MyError < StandardError; end
来源：http://qz.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://xi.panjiajie.cn

[H05] 捕获特定类型
来源：http://wg.wgjwhj.cn

Py:   except ValueError as e:
来源：http://sz.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ri.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://qm.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://ul.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://pg.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tq.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://ot.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mh.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://th.huanxung.cn

Py:   value = d.get("k") or default
来源：http://jo.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mw.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wc.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://la.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://to.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oo.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://nm.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://bq.huixinmuqiang.cn

[H07] 断言
来源：http://ro.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://vf.szsharing.cn

PHP:  assert($x > 0);
来源：http://fh.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://xl.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://bk.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://gq.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uh.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://er.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://tu.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://bp.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ed.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ra.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://rr.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sl.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rc.wgjwhj.cn

Go:   err.Error()
来源：http://ba.newstarts.cn


<!-- 参考信息 -->