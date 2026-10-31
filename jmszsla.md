代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kw.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zm.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://td.asd995.cn

[F08] 遍历目录
来源：http://fs.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bg.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dq.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://qm.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://cf.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qi.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vb.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://kz.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://qn.muxihuayi.cn

[F09] 获取文件大小
来源：http://nf.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://ub.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://tb.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://bt.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://ve.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vz.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cy.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://xj.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://ts.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://dx.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ta.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kw.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tl.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://yt.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vf.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gy.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wx.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pa.chemitech.net.cn

[F11] 复制与移动文件
来源：http://qn.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nj.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ip.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yi.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://os.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://no.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mn.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dw.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fh.shxzskj.cn

[F12] CSV 读写
来源：http://jb.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hk.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bv.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oe.szsharing.cn

TS:   // 同上
来源：http://bl.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zv.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://th.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ev.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vn.chemitech.net.cn

================================================================================
来源：http://ij.lnxyls.cn

G. 面向对象
来源：http://hj.9csxet.cn

================================================================================
来源：http://pv.yuntaijiaju.cn

[G01] 定义类
来源：http://cf.huanxung.cn

Py:   class User: pass
来源：http://jl.haigaiapp.cn

PHP:  class User {}
来源：http://rh.wgjwhj.cn

JS:   class User {}
来源：http://xn.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://fb.huanxung.cn

Java: class User {}
来源：http://av.gzmigu.cn

Go:   type User struct { Name string }
来源：http://ko.muxihuayi.cn

Ruby: class User; end
来源：http://uz.wgjwhj.cn

C#:   class User {}
来源：http://rs.newstarts.cn

[G02] 构造函数
来源：http://oh.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://wx.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://up.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://us.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://js.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://be.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wn.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://ht.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://gr.nicolike.cn

[G03] 实例属性
来源：http://dc.szxytkj.cn

Py:   self.name = "x"
来源：http://eq.panjiajie.cn

PHP:  public string $name = "x";
来源：http://ds.szsharing.cn

JS:   this.name = "x";
来源：http://jc.newstarts.cn

TS:   name: string = "x";
来源：http://sy.hnjuh.cn

Java: private String name;
来源：http://kp.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tk.colortex.cn

Ruby: @name = "x"
来源：http://zn.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://pd.hnjuh.cn

[G04] 定义方法
来源：http://ub.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://ge.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bx.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://pu.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://yl.huixiangedu.cn

Java: String greet() { return name; }
来源：http://br.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xh.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://sw.asd995.cn

C#:   public string Greet() => Name;
来源：http://ii.gzmigu.cn

[G05] 继承
来源：http://eb.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://xg.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://rz.panjiajie.cn

JS:   class Admin extends User {}
来源：http://zw.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://kw.nszjky.cn

Java: class Admin extends User {}
来源：http://jv.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uq.lnxyls.cn

Ruby: class Admin < User; end
来源：http://rr.huixiangedu.cn

C#:   class Admin : User {}
来源：http://dp.chemitech.net.cn

[G06] 重写方法
来源：http://ra.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://ay.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wp.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://gy.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://zb.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://ur.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mk.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://kw.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://zz.newstarts.cn

[G07] 调用父类方法
来源：http://xn.jianghongdianzi.cn

Py:   super().greet()
来源：http://oe.nszjky.cn

PHP:  parent::greet();
来源：http://fy.asd995.cn

JS:   super.greet();
来源：http://zi.hahajie.cn

TS:   super.greet();
来源：http://oo.gzmigu.cn

Java: super.greet();
来源：http://nm.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dc.shxzskj.cn

Ruby: super
来源：http://tz.yuntaijiaju.cn

C#:   base.Greet();
来源：http://wn.muxihuayi.cn

[G08] 静态方法与属性
来源：http://hw.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zh.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://jp.muxihuayi.cn

JS:   static f() {}
来源：http://hv.chemitech.net.cn

TS:   static f(): void {}
来源：http://uv.muxihuayi.cn

Java: static void f() {}
来源：http://vo.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://me.bookmarksfly.cn

Ruby: def self.f; end
来源：http://hn.szsharing.cn

C#:   public static void F() {}
来源：http://ey.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://ni.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://pu.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jy.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tp.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://bi.nicolike.cn

Java: interface Shape { double area(); }
来源：http://fm.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://lt.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ug.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://jb.szsharing.cn

[G10] 访问控制
来源：http://br.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://zu.colortex.cn

PHP:  public / protected / private
来源：http://tb.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://ll.chemitech.net.cn

TS:   public / protected / private
来源：http://fq.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://jw.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bw.jctech888.com.cn

Ruby: public / protected / private
来源：http://cb.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://nb.shtwfgs.cn

[G11] getter / setter
来源：http://sb.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://pa.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ya.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://fz.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://kd.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://lo.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yq.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://ga.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://lg.nszjky.cn

[G12] 对象转字符串
来源：http://pi.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://no.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ed.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://ew.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://mt.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://gt.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ck.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://qg.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://lb.huixiangedu.cn

[G13] 判断对象类型
来源：http://tx.hnjuh.cn

Py:   isinstance(u, User)
来源：http://na.muxihuayi.cn

PHP:  $u instanceof User
来源：http://wb.colortex.cn

JS:   u instanceof User
来源：http://ht.shxzskj.cn

TS:   u instanceof User
来源：http://fd.shtwfgs.cn

Java: u instanceof User
来源：http://lr.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eu.521024.cn

Ruby: u.is_a?(User)
来源：http://jg.shtwfgs.cn

C#:   u is User
来源：http://fd.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://pa.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wn.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://fp.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bg.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://af.asd995.cn

Java: record User(String name, int age) {}
来源：http://ns.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://nw.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yy.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://tn.huixiangedu.cn

[G15] 枚举
来源：http://df.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mb.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rm.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zj.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pd.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://dh.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sd.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://dc.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gx.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://hk.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sg.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://pq.9csxet.cn

JS:   Object.entries(obj)
来源：http://mr.asd995.cn

TS:   Object.entries(obj)
来源：http://pp.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ik.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hq.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://qx.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://te.szsharing.cn

================================================================================
来源：http://ue.huixiangedu.cn

H. 异常与错误处理
来源：http://ad.yuntaijiaju.cn

================================================================================
来源：http://mb.haigaiapp.cn

[H01] try / catch 基础
来源：http://zz.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fo.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://il.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ju.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yy.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ow.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uh.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gv.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fz.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://jc.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zm.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hw.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dr.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ya.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jc.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yx.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://az.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ln.hahajie.cn

[H03] 主动抛出异常
来源：http://px.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://xg.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fo.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://oe.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://sg.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ug.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ri.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uo.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://at.shtwfgs.cn

[H04] 自定义异常类型
来源：http://ml.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://dc.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iy.asd995.cn

JS:   class MyError extends Error {}
来源：http://ga.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://uj.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://hf.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ul.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://mn.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://ct.9csxet.cn

[H05] 捕获特定类型
来源：http://kf.gzmigu.cn

Py:   except ValueError as e:
来源：http://wz.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xh.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://mv.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://ka.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://lh.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sj.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://on.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fo.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://en.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://ba.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nw.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://no.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vs.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ux.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yv.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://nh.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://bl.muxihuayi.cn

[H07] 断言
来源：http://dh.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://zb.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://sk.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://dn.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://rx.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://gr.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://un.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://in.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://tv.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://dh.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://tl.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://su.newstarts.cn

JS:   e.message;  e.stack
来源：http://xq.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rx.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://es.huanxung.cn

Go:   err.Error()
来源：http://ae.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://no.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://tw.panjiajie.cn

[H09] 带错误码的异常
来源：http://rd.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bi.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vm.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pd.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cu.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hk.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ay.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fd.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lu.bjjhwx.cn

[H10] 资源自动释放
来源：http://jp.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nf.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ki.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tx.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://li.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dl.chemitech.net.cn

Go:   defer f.Close()
来源：http://be.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nh.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tl.hahajie.cn

================================================================================
来源：http://pf.wgjwhj.cn

I. 正则表达式
来源：http://ml.shxzukj.cn

================================================================================
来源：http://ga.haigaiapp.cn

[I01] 判断是否匹配
来源：http://ol.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rk.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sv.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://ai.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://ug.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dg.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zo.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://yb.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://st.asd995.cn


<!-- 参考信息 -->