代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hn.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gq.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rw.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jz.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oo.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mk.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ue.huixiangedu.cn

[F08] 遍历目录
来源：http://ey.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fd.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ae.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://ag.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://nf.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gp.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ry.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://bp.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://hu.hnjuh.cn

[F09] 获取文件大小
来源：http://cx.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://nw.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://nl.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://zk.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ds.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yk.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iv.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://dl.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://mt.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://ef.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cq.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://og.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cp.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://eu.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xq.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://on.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rk.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oh.shtwfgs.cn

[F11] 复制与移动文件
来源：http://xa.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kk.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lg.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://da.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zv.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pq.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ba.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gv.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://id.panjiajie.cn

[F12] CSV 读写
来源：http://sy.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yb.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zn.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://om.wgjwhj.cn

TS:   // 同上
来源：http://at.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rs.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://on.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qc.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iy.szsharing.cn

================================================================================
来源：http://vw.huanxung.cn

G. 面向对象
来源：http://nq.muxihuayi.cn

================================================================================
来源：http://ji.huanxung.cn

[G01] 定义类
来源：http://td.panjiajie.cn

Py:   class User: pass
来源：http://mt.chemitech.net.cn

PHP:  class User {}
来源：http://ed.haigaiapp.cn

JS:   class User {}
来源：http://js.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://xe.huanxung.cn

Java: class User {}
来源：http://gx.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://hi.asd995.cn

Ruby: class User; end
来源：http://ga.huixinmuqiang.cn

C#:   class User {}
来源：http://mg.haigaiapp.cn

[G02] 构造函数
来源：http://mi.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://ii.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://cu.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://na.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://tv.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://nh.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nr.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://sn.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://vh.newstarts.cn

[G03] 实例属性
来源：http://te.nicolike.cn

Py:   self.name = "x"
来源：http://qk.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://oo.bjjhwx.cn

JS:   this.name = "x";
来源：http://tw.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://tb.asd995.cn

Java: private String name;
来源：http://nx.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://if.bjjhwx.cn

Ruby: @name = "x"
来源：http://cm.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://mt.9csxet.cn

[G04] 定义方法
来源：http://lw.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://kt.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zk.521024.cn

JS:   greet() { return this.name; }
来源：http://bu.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://sf.bjjhwx.cn

Java: String greet() { return name; }
来源：http://xq.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xr.lnxyls.cn

Ruby: def greet; @name; end
来源：http://yy.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://iw.9csxet.cn

[G05] 继承
来源：http://rw.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://zs.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://wy.huanxung.cn

JS:   class Admin extends User {}
来源：http://vq.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://yl.szxytkj.cn

Java: class Admin extends User {}
来源：http://ju.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dp.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://yz.yuexingan06.cn

C#:   class Admin : User {}
来源：http://sm.hnjuh.cn

[G06] 重写方法
来源：http://ll.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://ll.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vn.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://yg.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://nl.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://gy.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lk.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://zi.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://as.9csxet.cn

[G07] 调用父类方法
来源：http://ap.huixiangedu.cn

Py:   super().greet()
来源：http://ka.shtwfgs.cn

PHP:  parent::greet();
来源：http://fq.muxihuayi.cn

JS:   super.greet();
来源：http://zc.gzmigu.cn

TS:   super.greet();
来源：http://gp.nicolike.cn

Java: super.greet();
来源：http://sx.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ag.9csxet.cn

Ruby: super
来源：http://vk.huanxung.cn

C#:   base.Greet();
来源：http://wy.yuexingan06.cn

[G08] 静态方法与属性
来源：http://kn.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rb.shxzskj.cn

PHP:  public static function f() {}
来源：http://db.nicolike.cn

JS:   static f() {}
来源：http://jd.nszjky.cn

TS:   static f(): void {}
来源：http://gi.szxytkj.cn

Java: static void f() {}
来源：http://wx.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jh.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://ds.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://is.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://jt.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://uv.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ch.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vt.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://rw.asd995.cn

Java: interface Shape { double area(); }
来源：http://zc.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://rb.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ry.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://ko.lnxyls.cn

[G10] 访问控制
来源：http://ua.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://wj.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://ig.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://xa.huanxung.cn

TS:   public / protected / private
来源：http://qo.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://wu.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pz.gzmigu.cn

Ruby: public / protected / private
来源：http://ln.szsharing.cn

C#:   public / protected / private / internal
来源：http://wi.bjjhwx.cn

[G11] getter / setter
来源：http://ai.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://dy.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://we.nicolike.cn

JS:   get name() { return this._name; }
来源：http://el.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://kf.hahajie.cn

Java: public String getName() { return name; }
来源：http://mo.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ao.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://ng.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ae.nszjky.cn

[G12] 对象转字符串
来源：http://tu.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://ms.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vs.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://js.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://mt.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://hv.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hi.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://ap.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://cs.yuexingan06.cn

[G13] 判断对象类型
来源：http://yh.colortex.cn

Py:   isinstance(u, User)
来源：http://vj.shtwfgs.cn

PHP:  $u instanceof User
来源：http://ei.gzmigu.cn

JS:   u instanceof User
来源：http://qp.chemitech.net.cn

TS:   u instanceof User
来源：http://xb.lnxyls.cn

Java: u instanceof User
来源：http://oj.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eg.newstarts.cn

Ruby: u.is_a?(User)
来源：http://mv.nszjky.cn

C#:   u is User
来源：http://aj.shxzukj.cn

[G14] 数据类 / record
来源：http://gz.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iy.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://qm.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mc.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://im.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://iv.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://hq.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ll.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://bo.huixinmuqiang.cn

[G15] 枚举
来源：http://xq.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://me.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pn.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ja.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yo.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://jm.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gg.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://hm.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rx.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://ks.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wi.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://ky.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://mx.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://fe.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eu.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sl.shxzukj.cn

Ruby: obj.instance_variables
来源：http://ag.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://uw.muxihuayi.cn

================================================================================
来源：http://kz.asd995.cn

H. 异常与错误处理
来源：http://fy.hnjuh.cn

================================================================================
来源：http://ga.gzmigu.cn

[H01] try / catch 基础
来源：http://uj.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gs.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hv.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cv.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vn.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cf.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xn.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ka.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://am.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://xn.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yb.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qj.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oh.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dq.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hw.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hn.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zq.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nl.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://ee.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://us.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vs.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://kb.colortex.cn

TS:   throw new Error("错误信息");
来源：http://yj.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jp.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://od.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ev.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sj.haigaiapp.cn

[H04] 自定义异常类型
来源：http://ae.colortex.cn

Py:   class MyError(Exception): pass
来源：http://zf.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gk.asd995.cn

JS:   class MyError extends Error {}
来源：http://bh.szsharing.cn

TS:   class MyError extends Error {}
来源：http://cc.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://ad.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lc.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://mw.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://zg.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://qo.nicolike.cn

Py:   except ValueError as e:
来源：http://jq.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oe.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://cm.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://bi.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://jj.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jq.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://iz.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fq.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://ud.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://lc.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cv.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wq.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ub.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hf.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tt.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://di.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://kq.jianghongdianzi.cn

[H07] 断言
来源：http://vo.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://gj.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://co.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://jf.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://nn.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://sh.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zb.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ip.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://dx.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://je.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://nl.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hy.shxzskj.cn

JS:   e.message;  e.stack
来源：http://sb.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pr.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kp.jianghongdianzi.cn

Go:   err.Error()
来源：http://vu.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://jf.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://ry.9csxet.cn

[H09] 带错误码的异常
来源：http://pi.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xv.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ix.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mv.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cj.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dz.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oo.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ms.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oe.bookmarksfly.cn

[H10] 资源自动释放
来源：http://bv.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xo.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xb.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://em.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fz.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rq.colortex.cn

Go:   defer f.Close()
来源：http://fy.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bd.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nl.9csxet.cn

================================================================================
来源：http://fp.asd995.cn

I. 正则表达式
来源：http://or.szsharing.cn

================================================================================
来源：http://nd.szxytkj.cn

[I01] 判断是否匹配
来源：http://ls.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ek.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gq.colortex.cn

JS:   /\d+/.test(s)
来源：http://gl.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://co.bjjhwx.cn


<!-- 参考信息 -->