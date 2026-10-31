代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dg.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://tb.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ui.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ai.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fq.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sl.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://fq.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nr.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qz.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://af.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cm.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ty.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sp.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jx.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aa.huanxung.cn

[F12] CSV 读写
来源：http://qz.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://in.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kj.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lc.wgjwhj.cn

TS:   // 同上
来源：http://ok.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ha.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qz.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://af.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ga.lnxyls.cn

================================================================================
来源：http://ni.huixiangedu.cn

G. 面向对象
来源：http://yq.nicolike.cn

================================================================================
来源：http://zk.yuexingan06.cn

[G01] 定义类
来源：http://bo.newstarts.cn

Py:   class User: pass
来源：http://kq.haigaiapp.cn

PHP:  class User {}
来源：http://ga.haigaiapp.cn

JS:   class User {}
来源：http://ht.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://yy.yuexingan06.cn

Java: class User {}
来源：http://am.huanxung.cn

Go:   type User struct { Name string }
来源：http://ob.lnxyls.cn

Ruby: class User; end
来源：http://ru.szxytkj.cn

C#:   class User {}
来源：http://vo.jctech888.com.cn

[G02] 构造函数
来源：http://xj.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://xb.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://oi.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://cu.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://kf.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://wd.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://il.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://nh.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://ef.521024.cn

[G03] 实例属性
来源：http://gf.huixiangedu.cn

Py:   self.name = "x"
来源：http://wr.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://lh.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://it.shtwfgs.cn

TS:   name: string = "x";
来源：http://qc.huixiangedu.cn

Java: private String name;
来源：http://gq.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xn.gzmigu.cn

Ruby: @name = "x"
来源：http://mr.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://xh.9csxet.cn

[G04] 定义方法
来源：http://en.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://tl.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mm.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://eq.521024.cn

TS:   greet(): string { return this.name; }
来源：http://pg.bjjhwx.cn

Java: String greet() { return name; }
来源：http://nd.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oq.gzmigu.cn

Ruby: def greet; @name; end
来源：http://mv.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://at.shtwfgs.cn

[G05] 继承
来源：http://vz.huanxung.cn

Py:   class Admin(User): pass
来源：http://bx.nszjky.cn

PHP:  class Admin extends User {}
来源：http://fi.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://xm.asd995.cn

TS:   class Admin extends User {}
来源：http://mh.yuexingan06.cn

Java: class Admin extends User {}
来源：http://sm.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yw.colortex.cn

Ruby: class Admin < User; end
来源：http://bm.wgjwhj.cn

C#:   class Admin : User {}
来源：http://mt.jctech888.com.cn

[G06] 重写方法
来源：http://af.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://cy.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qm.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://me.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://wj.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://fj.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iq.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://my.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://nm.hnjuh.cn

[G07] 调用父类方法
来源：http://nw.bookmarksfly.cn

Py:   super().greet()
来源：http://fb.nicolike.cn

PHP:  parent::greet();
来源：http://qr.hahajie.cn

JS:   super.greet();
来源：http://bf.nicolike.cn

TS:   super.greet();
来源：http://ax.chemitech.net.cn

Java: super.greet();
来源：http://nb.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oe.szxytkj.cn

Ruby: super
来源：http://us.jianghongdianzi.cn

C#:   base.Greet();
来源：http://fl.nicolike.cn

[G08] 静态方法与属性
来源：http://dl.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://te.huanxung.cn

PHP:  public static function f() {}
来源：http://ql.huanxung.cn

JS:   static f() {}
来源：http://hu.muxihuayi.cn

TS:   static f(): void {}
来源：http://kj.bookmarksfly.cn

Java: static void f() {}
来源：http://ay.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iw.9csxet.cn

Ruby: def self.f; end
来源：http://ma.shxzskj.cn

C#:   public static void F() {}
来源：http://ui.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://td.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://oq.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qw.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sc.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://dv.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://ab.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://nb.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://em.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://dj.gzmigu.cn

[G10] 访问控制
来源：http://sp.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://nv.gzmigu.cn

PHP:  public / protected / private
来源：http://kj.asd995.cn

JS:   #private 字段；其余公开
来源：http://vt.521024.cn

TS:   public / protected / private
来源：http://ok.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://bl.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://js.chemitech.net.cn

Ruby: public / protected / private
来源：http://dg.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://oz.bjjhwx.cn

[G11] getter / setter
来源：http://nr.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://dh.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xk.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://bu.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://lj.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://zg.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zm.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://xt.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://pp.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://zs.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://ql.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uq.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://ey.521024.cn

TS:   toString(): string { return this.name; }
来源：http://vv.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://wd.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qc.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://cy.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://hz.colortex.cn

[G13] 判断对象类型
来源：http://vw.asd995.cn

Py:   isinstance(u, User)
来源：http://au.asd995.cn

PHP:  $u instanceof User
来源：http://ty.panjiajie.cn

JS:   u instanceof User
来源：http://ja.gzmigu.cn

TS:   u instanceof User
来源：http://wj.jianghongdianzi.cn

Java: u instanceof User
来源：http://aw.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ey.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://fi.colortex.cn

C#:   u is User
来源：http://ul.asd995.cn

[G14] 数据类 / record
来源：http://ub.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iv.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://jr.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tv.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://pg.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ga.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://mf.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mu.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://rr.newstarts.cn

[G15] 枚举
来源：http://pf.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pp.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rm.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pg.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pd.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://od.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uj.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://pg.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wf.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://gl.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iy.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://fo.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://av.nicolike.cn

TS:   Object.entries(obj)
来源：http://pv.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ad.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://si.szsharing.cn

Ruby: obj.instance_variables
来源：http://tx.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://gy.shxzukj.cn

================================================================================
来源：http://gu.shxzukj.cn

H. 异常与错误处理
来源：http://om.hnjuh.cn

================================================================================
来源：http://rb.szsharing.cn

[H01] try / catch 基础
来源：http://gw.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dw.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ra.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kt.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dj.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rh.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vt.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yg.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sc.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://vj.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://un.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mv.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nl.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bv.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yw.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yn.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xc.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://be.colortex.cn

[H03] 主动抛出异常
来源：http://aj.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://nw.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xl.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://si.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://en.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ap.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cj.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wo.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://su.haigaiapp.cn

[H04] 自定义异常类型
来源：http://zk.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://kp.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pj.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://pb.nszjky.cn

TS:   class MyError extends Error {}
来源：http://cs.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://zt.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cm.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://rl.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://sj.szxytkj.cn

[H05] 捕获特定类型
来源：http://cj.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://vd.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cm.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://hu.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://ow.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://ob.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://of.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://bb.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://py.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://kw.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://jn.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rk.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ag.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fx.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eg.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tn.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://zu.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://qd.newstarts.cn

[H07] 断言
来源：http://qx.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://jc.newstarts.cn

PHP:  assert($x > 0);
来源：http://zu.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://to.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://xc.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://bo.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sn.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xn.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://gh.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://de.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://kg.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gj.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://yo.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cc.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ey.jctech888.com.cn

Go:   err.Error()
来源：http://yc.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://dr.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://pb.chemitech.net.cn

[H09] 带错误码的异常
来源：http://ef.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cx.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gp.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wt.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tu.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ua.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wv.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ps.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wt.jctech888.com.cn

[H10] 资源自动释放
来源：http://ts.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dn.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uo.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ui.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dh.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ul.bookmarksfly.cn

Go:   defer f.Close()
来源：http://xg.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ar.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xi.hnjuh.cn

================================================================================
来源：http://sr.yuntaijiaju.cn

I. 正则表达式
来源：http://tn.9csxet.cn

================================================================================
来源：http://sx.huanxung.cn

[I01] 判断是否匹配
来源：http://gx.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ri.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sv.huanxung.cn

JS:   /\d+/.test(s)
来源：http://vt.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://ok.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wn.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ff.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://aa.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lz.szsharing.cn

[I02] 提取所有匹配
来源：http://qq.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://pq.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://so.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vl.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://tj.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wk.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kc.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://iu.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ld.colortex.cn

[I03] 提取捕获分组
来源：http://ez.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vi.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xz.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uh.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qc.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rv.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://by.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fd.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cb.yuexingan06.cn

[I04] 正则替换
来源：http://rf.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fl.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ni.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dx.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nn.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ho.nszjky.cn


<!-- 参考信息 -->