代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bo.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://wd.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wf.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xq.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wa.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sj.huanxung.cn

[F11] 复制与移动文件
来源：http://eg.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://je.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pi.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fw.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sk.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ie.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tp.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kj.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nj.shtwfgs.cn

[F12] CSV 读写
来源：http://cq.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ww.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zt.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mw.hahajie.cn

TS:   // 同上
来源：http://mw.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hw.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ql.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yv.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ci.bookmarksfly.cn

================================================================================
来源：http://ty.wgjwhj.cn

G. 面向对象
来源：http://tv.chemitech.net.cn

================================================================================
来源：http://wi.muxihuayi.cn

[G01] 定义类
来源：http://re.yuexingan06.cn

Py:   class User: pass
来源：http://pi.newstarts.cn

PHP:  class User {}
来源：http://vn.yuntaijiaju.cn

JS:   class User {}
来源：http://be.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://nk.szsharing.cn

Java: class User {}
来源：http://xz.panjiajie.cn

Go:   type User struct { Name string }
来源：http://xq.nszjky.cn

Ruby: class User; end
来源：http://si.wgjwhj.cn

C#:   class User {}
来源：http://ji.nicolike.cn

[G02] 构造函数
来源：http://np.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://ra.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://lx.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://ed.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://xw.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://tg.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ym.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://dt.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://ns.lnxyls.cn

[G03] 实例属性
来源：http://qj.shxzskj.cn

Py:   self.name = "x"
来源：http://em.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://rq.lnxyls.cn

JS:   this.name = "x";
来源：http://gr.shxzukj.cn

TS:   name: string = "x";
来源：http://tp.haigaiapp.cn

Java: private String name;
来源：http://qg.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ea.hnjuh.cn

Ruby: @name = "x"
来源：http://hl.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://eu.shxzskj.cn

[G04] 定义方法
来源：http://lh.newstarts.cn

Py:   def greet(self): return self.name
来源：http://nw.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wm.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://fr.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://qt.szsharing.cn

Java: String greet() { return name; }
来源：http://pl.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ub.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://mq.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://vy.yuntaijiaju.cn

[G05] 继承
来源：http://yc.9csxet.cn

Py:   class Admin(User): pass
来源：http://yt.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://yu.nszjky.cn

JS:   class Admin extends User {}
来源：http://yt.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://hh.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://bh.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ne.lnxyls.cn

Ruby: class Admin < User; end
来源：http://ee.chemitech.net.cn

C#:   class Admin : User {}
来源：http://um.huanxung.cn

[G06] 重写方法
来源：http://nq.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://ma.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://px.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://rv.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://xn.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://wp.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://so.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://dw.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://dw.yuexingan06.cn

[G07] 调用父类方法
来源：http://aw.nszjky.cn

Py:   super().greet()
来源：http://yd.hnjuh.cn

PHP:  parent::greet();
来源：http://lq.bjjhwx.cn

JS:   super.greet();
来源：http://bj.szsharing.cn

TS:   super.greet();
来源：http://ba.huixiangedu.cn

Java: super.greet();
来源：http://cr.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fu.szxytkj.cn

Ruby: super
来源：http://fs.nicolike.cn

C#:   base.Greet();
来源：http://mx.huixiangedu.cn

[G08] 静态方法与属性
来源：http://cq.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zo.huixiangedu.cn

PHP:  public static function f() {}
来源：http://vv.haigaiapp.cn

JS:   static f() {}
来源：http://zz.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://fy.shtwfgs.cn

Java: static void f() {}
来源：http://kw.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ma.haigaiapp.cn

Ruby: def self.f; end
来源：http://pq.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://xi.asd995.cn

[G09] 接口 / 抽象类
来源：http://jz.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://ds.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pw.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dv.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://hs.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://oy.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://gp.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rc.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://ss.newstarts.cn

[G10] 访问控制
来源：http://mi.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://mv.nicolike.cn

PHP:  public / protected / private
来源：http://pq.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://sl.jctech888.com.cn

TS:   public / protected / private
来源：http://bx.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://vq.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tn.asd995.cn

Ruby: public / protected / private
来源：http://pf.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://ax.shxzukj.cn

[G11] getter / setter
来源：http://ry.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ib.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jl.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://xa.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://ud.colortex.cn

Java: public String getName() { return name; }
来源：http://wa.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zl.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://cp.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://je.hahajie.cn

[G12] 对象转字符串
来源：http://bp.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://bo.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://aj.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://rb.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://io.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://of.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lt.hahajie.cn

Ruby: def to_s; @name; end
来源：http://bh.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://qn.szxytkj.cn

[G13] 判断对象类型
来源：http://dh.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://kc.newstarts.cn

PHP:  $u instanceof User
来源：http://ak.huixiangedu.cn

JS:   u instanceof User
来源：http://ot.nszjky.cn

TS:   u instanceof User
来源：http://kw.shxzukj.cn

Java: u instanceof User
来源：http://zn.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://va.szsharing.cn

Ruby: u.is_a?(User)
来源：http://zw.jctech888.com.cn

C#:   u is User
来源：http://de.haigaiapp.cn

[G14] 数据类 / record
来源：http://tt.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bk.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://ci.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cj.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://jb.newstarts.cn

Java: record User(String name, int age) {}
来源：http://md.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://ic.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://of.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://uz.yuexingan06.cn

[G15] 枚举
来源：http://ww.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ba.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bi.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://id.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wa.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://op.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zn.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://jk.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ku.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://tl.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zy.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://fm.huanxung.cn

JS:   Object.entries(obj)
来源：http://hh.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://xl.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hc.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dy.colortex.cn

Ruby: obj.instance_variables
来源：http://cb.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://yf.huixinmuqiang.cn

================================================================================
来源：http://ip.hahajie.cn

H. 异常与错误处理
来源：http://xi.yuexingan06.cn

================================================================================
来源：http://kr.521024.cn

[H01] try / catch 基础
来源：http://zt.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rc.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mw.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mx.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qi.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sl.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kn.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lc.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://el.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://wi.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jt.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ip.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mf.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cp.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nx.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hs.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://og.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uw.muxihuayi.cn

[H03] 主动抛出异常
来源：http://tn.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://cg.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uj.521024.cn

JS:   throw new Error("错误信息");
来源：http://ju.521024.cn

TS:   throw new Error("错误信息");
来源：http://gs.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qj.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zo.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bi.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ud.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://dn.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://ll.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fb.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://qf.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://os.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://nf.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ac.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://kb.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://qo.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://vy.asd995.cn

Py:   except ValueError as e:
来源：http://ws.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lp.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://yn.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://vo.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://yy.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://el.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://zw.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mi.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://nd.colortex.cn

Py:   value = d.get("k") or default
来源：http://pb.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rh.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sd.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fq.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gt.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cf.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://lo.521024.cn

C#:   obj?.A?.B ?? default
来源：http://dn.yuntaijiaju.cn

[H07] 断言
来源：http://xp.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://jq.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://nn.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://fv.hahajie.cn

TS:   console.assert(x > 0);
来源：http://lj.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://qw.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jl.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zb.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://gk.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://nr.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://np.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dr.nszjky.cn

JS:   e.message;  e.stack
来源：http://zc.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yn.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bp.huixiangedu.cn

Go:   err.Error()
来源：http://xm.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://ya.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://hv.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://yd.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qq.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lb.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mu.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tv.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ms.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rf.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nf.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ui.jctech888.com.cn

[H10] 资源自动释放
来源：http://fl.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qn.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://io.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fn.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cp.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vm.muxihuayi.cn

Go:   defer f.Close()
来源：http://xp.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ve.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zc.colortex.cn

================================================================================
来源：http://pw.gzmigu.cn

I. 正则表达式
来源：http://nj.panjiajie.cn

================================================================================
来源：http://og.nicolike.cn

[I01] 判断是否匹配
来源：http://il.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://be.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zm.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://dq.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://mj.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bo.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tl.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://ep.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://se.huixiangedu.cn

[I02] 提取所有匹配
来源：http://iz.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://gv.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sl.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gz.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://lm.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zf.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://si.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://at.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gu.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://kb.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cp.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hk.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ob.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ad.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tz.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zr.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iy.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ty.nicolike.cn

[I04] 正则替换
来源：http://im.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xv.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ja.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ny.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tk.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qb.yuntaijiaju.cn


<!-- 参考信息 -->