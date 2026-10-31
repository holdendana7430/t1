代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ld.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://ur.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jp.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fp.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ht.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nm.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://dv.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pa.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sq.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gs.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://no.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ju.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ky.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zy.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wr.szsharing.cn

[F12] CSV 读写
来源：http://tj.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ra.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dv.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dp.521024.cn

TS:   // 同上
来源：http://vj.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ab.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://af.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sc.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ve.szsharing.cn

================================================================================
来源：http://wr.muxihuayi.cn

G. 面向对象
来源：http://pt.yuexingan06.cn

================================================================================
来源：http://lh.asd995.cn

[G01] 定义类
来源：http://hw.yuexingan06.cn

Py:   class User: pass
来源：http://tc.yuexingan06.cn

PHP:  class User {}
来源：http://jj.bjjhwx.cn

JS:   class User {}
来源：http://om.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://zw.shxzskj.cn

Java: class User {}
来源：http://lp.panjiajie.cn

Go:   type User struct { Name string }
来源：http://qq.hnjuh.cn

Ruby: class User; end
来源：http://xy.gzmigu.cn

C#:   class User {}
来源：http://de.nicolike.cn

[G02] 构造函数
来源：http://pb.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://os.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://ul.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://vg.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://qn.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://be.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://er.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://zt.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://sc.lnxyls.cn

[G03] 实例属性
来源：http://xi.nicolike.cn

Py:   self.name = "x"
来源：http://hx.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://ap.huanxung.cn

JS:   this.name = "x";
来源：http://me.shtwfgs.cn

TS:   name: string = "x";
来源：http://cc.jctech888.com.cn

Java: private String name;
来源：http://bq.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yg.lnxyls.cn

Ruby: @name = "x"
来源：http://ji.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://ya.wgjwhj.cn

[G04] 定义方法
来源：http://nz.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://cm.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nc.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://sg.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://hp.gzmigu.cn

Java: String greet() { return name; }
来源：http://uw.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rx.gzmigu.cn

Ruby: def greet; @name; end
来源：http://me.szsharing.cn

C#:   public string Greet() => Name;
来源：http://dg.hahajie.cn

[G05] 继承
来源：http://wp.asd995.cn

Py:   class Admin(User): pass
来源：http://pc.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://ox.panjiajie.cn

JS:   class Admin extends User {}
来源：http://uq.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://ea.wgjwhj.cn

Java: class Admin extends User {}
来源：http://dh.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yn.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://oj.jctech888.com.cn

C#:   class Admin : User {}
来源：http://xx.9csxet.cn

[G06] 重写方法
来源：http://zr.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://be.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ik.521024.cn

JS:   greet() { return "admin"; }
来源：http://dy.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://cg.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://yj.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hr.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://ty.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://go.asd995.cn

[G07] 调用父类方法
来源：http://jr.huixiangedu.cn

Py:   super().greet()
来源：http://yx.chemitech.net.cn

PHP:  parent::greet();
来源：http://ei.nszjky.cn

JS:   super.greet();
来源：http://of.nszjky.cn

TS:   super.greet();
来源：http://xm.shxzukj.cn

Java: super.greet();
来源：http://vz.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ns.jianghongdianzi.cn

Ruby: super
来源：http://sn.521024.cn

C#:   base.Greet();
来源：http://fn.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://bc.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kk.9csxet.cn

PHP:  public static function f() {}
来源：http://zp.yuntaijiaju.cn

JS:   static f() {}
来源：http://qe.nicolike.cn

TS:   static f(): void {}
来源：http://fs.szxytkj.cn

Java: static void f() {}
来源：http://sc.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ab.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://ye.shxzukj.cn

C#:   public static void F() {}
来源：http://xo.asd995.cn

[G09] 接口 / 抽象类
来源：http://gi.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://jv.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fx.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jw.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://xt.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://gd.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://rs.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rn.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ug.9csxet.cn

[G10] 访问控制
来源：http://bq.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://bk.huixiangedu.cn

PHP:  public / protected / private
来源：http://gc.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://fr.bjjhwx.cn

TS:   public / protected / private
来源：http://db.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://em.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xw.hahajie.cn

Ruby: public / protected / private
来源：http://wc.hnjuh.cn

C#:   public / protected / private / internal
来源：http://ff.shxzskj.cn

[G11] getter / setter
来源：http://vl.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://dk.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ja.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://aq.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://jm.gzmigu.cn

Java: public String getName() { return name; }
来源：http://mm.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ew.szsharing.cn

Ruby: attr_accessor :name
来源：http://jv.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://qt.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://wl.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://ba.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nx.huanxung.cn

JS:   toString() { return this.name; }
来源：http://hi.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://ha.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://wh.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ur.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ws.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://kn.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://eb.lnxyls.cn

Py:   isinstance(u, User)
来源：http://lp.hahajie.cn

PHP:  $u instanceof User
来源：http://gw.yuntaijiaju.cn

JS:   u instanceof User
来源：http://eo.huixiangedu.cn

TS:   u instanceof User
来源：http://bi.szxytkj.cn

Java: u instanceof User
来源：http://ah.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yt.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://yw.shxzukj.cn

C#:   u is User
来源：http://hw.nszjky.cn

[G14] 数据类 / record
来源：http://py.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jc.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://od.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hx.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://ni.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://ll.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://ts.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://br.521024.cn

C#:   record User(string Name, int Age);
来源：http://dl.jctech888.com.cn

[G15] 枚举
来源：http://ps.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ei.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gh.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nk.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vr.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://ib.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://km.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ad.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sp.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://dd.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dh.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://kd.521024.cn

JS:   Object.entries(obj)
来源：http://gj.9csxet.cn

TS:   Object.entries(obj)
来源：http://vc.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fd.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hj.9csxet.cn

Ruby: obj.instance_variables
来源：http://cr.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://li.shxzskj.cn

================================================================================
来源：http://jd.haigaiapp.cn

H. 异常与错误处理
来源：http://ww.shxzukj.cn

================================================================================
来源：http://ev.asd995.cn

[H01] try / catch 基础
来源：http://xj.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oi.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rx.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wr.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kj.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://la.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://du.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qd.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iw.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://lc.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jl.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rk.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zr.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vb.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qw.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ts.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cc.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gu.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://jx.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://sl.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ms.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://cw.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://je.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wk.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ni.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ld.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uy.nszjky.cn

[H04] 自定义异常类型
来源：http://lj.colortex.cn

Py:   class MyError(Exception): pass
来源：http://ak.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pq.521024.cn

JS:   class MyError extends Error {}
来源：http://pk.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://bw.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://hw.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yt.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://zj.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://ti.huixiangedu.cn

[H05] 捕获特定类型
来源：http://vw.jctech888.com.cn

Py:   except ValueError as e:
来源：http://fb.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aa.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ng.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://hh.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://il.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://om.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://al.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dm.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://zn.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://fa.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ft.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gw.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kz.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jy.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iw.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://am.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://qg.wgjwhj.cn

[H07] 断言
来源：http://js.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://vl.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://qm.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://dx.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://kp.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://dp.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dl.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zm.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://gz.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://qy.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://yy.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tb.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://yh.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zd.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://az.521024.cn

Go:   err.Error()
来源：http://uj.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://bf.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ro.nicolike.cn

[H09] 带错误码的异常
来源：http://cv.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bp.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://od.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ha.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ce.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ti.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zv.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zy.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wz.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://gw.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ys.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qg.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://op.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yz.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://an.hahajie.cn

Go:   defer f.Close()
来源：http://up.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qg.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cd.huanxung.cn

================================================================================
来源：http://ol.gzmigu.cn

I. 正则表达式
来源：http://lr.yuexingan06.cn

================================================================================
来源：http://of.nicolike.cn

[I01] 判断是否匹配
来源：http://ae.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://av.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gr.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ip.521024.cn

TS:   /\d+/.test(s)
来源：http://kn.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ly.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ja.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://vl.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://od.jctech888.com.cn

[I02] 提取所有匹配
来源：http://yv.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://zw.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xs.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ww.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://ou.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ia.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rk.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://dg.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kt.huixiangedu.cn

[I03] 提取捕获分组
来源：http://xs.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qq.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kv.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wi.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nv.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mj.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://it.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pr.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cn.huixinmuqiang.cn

[I04] 正则替换
来源：http://oa.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ga.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iu.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tk.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sa.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://to.szxytkj.cn


<!-- 参考信息 -->