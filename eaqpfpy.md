代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ih.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://sm.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xw.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ve.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dy.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cm.9csxet.cn

[F11] 复制与移动文件
来源：http://vk.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sf.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uf.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qk.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dz.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rg.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gh.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cr.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://at.chemitech.net.cn

[F12] CSV 读写
来源：http://bi.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ne.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sr.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fw.bjjhwx.cn

TS:   // 同上
来源：http://fx.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bx.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vi.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lq.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nl.szsharing.cn

================================================================================
来源：http://ue.nicolike.cn

G. 面向对象
来源：http://xo.jianghongdianzi.cn

================================================================================
来源：http://ir.chemitech.net.cn

[G01] 定义类
来源：http://qp.asd995.cn

Py:   class User: pass
来源：http://gp.colortex.cn

PHP:  class User {}
来源：http://os.9csxet.cn

JS:   class User {}
来源：http://pk.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://mh.lnxyls.cn

Java: class User {}
来源：http://sf.nszjky.cn

Go:   type User struct { Name string }
来源：http://ps.yuntaijiaju.cn

Ruby: class User; end
来源：http://qe.shxzskj.cn

C#:   class User {}
来源：http://oz.9csxet.cn

[G02] 构造函数
来源：http://ew.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://pr.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://ic.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://xk.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://nk.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://gg.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gk.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://ti.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://pv.jctech888.com.cn

[G03] 实例属性
来源：http://in.szxytkj.cn

Py:   self.name = "x"
来源：http://gx.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://qp.chemitech.net.cn

JS:   this.name = "x";
来源：http://zg.shxzukj.cn

TS:   name: string = "x";
来源：http://ve.yuntaijiaju.cn

Java: private String name;
来源：http://rk.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vu.huixiangedu.cn

Ruby: @name = "x"
来源：http://vt.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://zm.wgjwhj.cn

[G04] 定义方法
来源：http://rk.asd995.cn

Py:   def greet(self): return self.name
来源：http://uh.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dm.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://xj.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://hg.yuexingan06.cn

Java: String greet() { return name; }
来源：http://la.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://co.szsharing.cn

Ruby: def greet; @name; end
来源：http://ji.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://qs.muxihuayi.cn

[G05] 继承
来源：http://cl.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://ch.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://jw.lnxyls.cn

JS:   class Admin extends User {}
来源：http://zc.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://sn.wgjwhj.cn

Java: class Admin extends User {}
来源：http://ys.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gc.newstarts.cn

Ruby: class Admin < User; end
来源：http://zb.yuexingan06.cn

C#:   class Admin : User {}
来源：http://sz.muxihuayi.cn

[G06] 重写方法
来源：http://dw.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://ww.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fr.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://an.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://ra.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ab.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cv.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://li.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ey.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://ct.nszjky.cn

Py:   super().greet()
来源：http://sb.shxzskj.cn

PHP:  parent::greet();
来源：http://yi.shtwfgs.cn

JS:   super.greet();
来源：http://tc.wgjwhj.cn

TS:   super.greet();
来源：http://rl.shxzukj.cn

Java: super.greet();
来源：http://lf.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://do.lnxyls.cn

Ruby: super
来源：http://hd.lnxyls.cn

C#:   base.Greet();
来源：http://dg.szxytkj.cn

[G08] 静态方法与属性
来源：http://be.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ri.shxzskj.cn

PHP:  public static function f() {}
来源：http://xq.szxytkj.cn

JS:   static f() {}
来源：http://io.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://xo.lnxyls.cn

Java: static void f() {}
来源：http://si.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ad.jctech888.com.cn

Ruby: def self.f; end
来源：http://bh.panjiajie.cn

C#:   public static void F() {}
来源：http://gf.9csxet.cn

[G09] 接口 / 抽象类
来源：http://yh.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://ck.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uf.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jz.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://aq.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://oh.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://tv.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eo.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://sn.hnjuh.cn

[G10] 访问控制
来源：http://yb.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://qb.huixiangedu.cn

PHP:  public / protected / private
来源：http://ap.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://lp.panjiajie.cn

TS:   public / protected / private
来源：http://on.521024.cn

Java: public / protected / private / 默认包级
来源：http://ck.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cn.chemitech.net.cn

Ruby: public / protected / private
来源：http://qw.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ql.huixiangedu.cn

[G11] getter / setter
来源：http://yi.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://sl.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vy.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://sj.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://sq.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://as.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lg.shxzukj.cn

Ruby: attr_accessor :name
来源：http://dw.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://xo.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://qh.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://zs.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yh.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://as.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://bv.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://cf.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oc.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://hd.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://xg.yuexingan06.cn

[G13] 判断对象类型
来源：http://sq.szxytkj.cn

Py:   isinstance(u, User)
来源：http://jn.wgjwhj.cn

PHP:  $u instanceof User
来源：http://xp.yuntaijiaju.cn

JS:   u instanceof User
来源：http://jm.wgjwhj.cn

TS:   u instanceof User
来源：http://vs.haigaiapp.cn

Java: u instanceof User
来源：http://yo.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://us.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://tq.jianghongdianzi.cn

C#:   u is User
来源：http://cz.shtwfgs.cn

[G14] 数据类 / record
来源：http://lf.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kp.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://wm.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cr.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://uo.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://ik.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://hn.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yk.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://pp.haigaiapp.cn

[G15] 枚举
来源：http://og.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vn.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ne.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://le.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cy.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://aj.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mg.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://cx.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hp.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://hn.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://op.asd995.cn

PHP:  get_object_vars($obj);
来源：http://sm.newstarts.cn

JS:   Object.entries(obj)
来源：http://wz.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://qz.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tt.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pq.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://zv.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://fu.nicolike.cn

================================================================================
来源：http://cb.szsharing.cn

H. 异常与错误处理
来源：http://up.wgjwhj.cn

================================================================================
来源：http://lo.chemitech.net.cn

[H01] try / catch 基础
来源：http://in.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xh.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jq.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kr.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ae.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hw.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gs.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nr.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sa.szsharing.cn

[H02] finally / ensure 收尾
来源：http://fg.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ui.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wk.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rz.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gp.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rt.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yi.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zl.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tt.shtwfgs.cn

[H03] 主动抛出异常
来源：http://lg.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://vg.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lk.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://ts.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://fh.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://et.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lr.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qb.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ri.jctech888.com.cn

[H04] 自定义异常类型
来源：http://he.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://sr.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oc.521024.cn

JS:   class MyError extends Error {}
来源：http://bk.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://bb.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://hd.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mq.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://vz.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://bv.lnxyls.cn

[H05] 捕获特定类型
来源：http://zl.chemitech.net.cn

Py:   except ValueError as e:
来源：http://fb.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fl.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://wu.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://sp.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://dl.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ix.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://jr.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yc.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://kf.nicolike.cn

Py:   value = d.get("k") or default
来源：http://hj.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kr.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://si.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kc.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sl.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yn.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://ak.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://bd.newstarts.cn

[H07] 断言
来源：http://jb.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://mk.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://gh.asd995.cn

JS:   console.assert(x > 0);
来源：http://nv.hahajie.cn

TS:   console.assert(x > 0);
来源：http://bn.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://bi.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jx.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ri.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://gr.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://pf.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://cs.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dl.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://mg.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bz.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bf.jianghongdianzi.cn

Go:   err.Error()
来源：http://po.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://ba.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://qe.yuexingan06.cn

[H09] 带错误码的异常
来源：http://pw.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oz.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ri.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qh.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gx.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jr.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yg.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zu.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ve.chemitech.net.cn

[H10] 资源自动释放
来源：http://bz.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ei.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ak.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cy.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cw.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oc.szxytkj.cn

Go:   defer f.Close()
来源：http://da.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ol.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hn.nicolike.cn

================================================================================
来源：http://cj.szxytkj.cn

I. 正则表达式
来源：http://kw.newstarts.cn

================================================================================
来源：http://zx.bjjhwx.cn

[I01] 判断是否匹配
来源：http://ug.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ac.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bx.521024.cn

JS:   /\d+/.test(s)
来源：http://is.nicolike.cn

TS:   /\d+/.test(s)
来源：http://xk.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hy.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://de.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://dl.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sp.nszjky.cn

[I02] 提取所有匹配
来源：http://yk.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ng.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sq.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ez.521024.cn

TS:   s.match(/\d+/g)
来源：http://wh.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bs.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dc.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://st.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bb.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://wp.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ud.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cw.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sb.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xb.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gu.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pi.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lx.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://as.shxzskj.cn

[I04] 正则替换
来源：http://pf.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ru.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nf.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bi.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ae.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ek.bjjhwx.cn


<!-- 参考信息 -->