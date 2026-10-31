代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uw.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ib.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fm.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vj.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kt.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oy.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tk.yuntaijiaju.cn

[F12] CSV 读写
来源：http://xa.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bj.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bl.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ar.huixiangedu.cn

TS:   // 同上
来源：http://xz.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wt.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vq.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rq.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pa.huixiangedu.cn

================================================================================
来源：http://uj.panjiajie.cn

G. 面向对象
来源：http://dm.panjiajie.cn

================================================================================
来源：http://jf.wgjwhj.cn

[G01] 定义类
来源：http://id.szxytkj.cn

Py:   class User: pass
来源：http://ch.bjjhwx.cn

PHP:  class User {}
来源：http://jy.haigaiapp.cn

JS:   class User {}
来源：http://cm.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://ei.hnjuh.cn

Java: class User {}
来源：http://mf.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://wj.huixiangedu.cn

Ruby: class User; end
来源：http://sf.muxihuayi.cn

C#:   class User {}
来源：http://kt.shtwfgs.cn

[G02] 构造函数
来源：http://ec.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://vz.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://wo.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://hz.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://wd.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://in.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bj.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://vc.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://tm.shxzukj.cn

[G03] 实例属性
来源：http://ou.521024.cn

Py:   self.name = "x"
来源：http://uq.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://si.asd995.cn

JS:   this.name = "x";
来源：http://ha.panjiajie.cn

TS:   name: string = "x";
来源：http://ar.huixinmuqiang.cn

Java: private String name;
来源：http://pj.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xz.shtwfgs.cn

Ruby: @name = "x"
来源：http://wl.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ra.hahajie.cn

[G04] 定义方法
来源：http://qc.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://kx.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zt.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://xu.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ld.panjiajie.cn

Java: String greet() { return name; }
来源：http://lg.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uf.asd995.cn

Ruby: def greet; @name; end
来源：http://gv.colortex.cn

C#:   public string Greet() => Name;
来源：http://nm.hahajie.cn

[G05] 继承
来源：http://wv.lnxyls.cn

Py:   class Admin(User): pass
来源：http://sm.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://kh.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://fv.shxzskj.cn

TS:   class Admin extends User {}
来源：http://di.panjiajie.cn

Java: class Admin extends User {}
来源：http://ut.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bv.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://mc.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://fm.asd995.cn

[G06] 重写方法
来源：http://oq.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://wm.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xr.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ee.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://bp.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://he.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cl.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://sn.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://ui.wgjwhj.cn

[G07] 调用父类方法
来源：http://pc.gzmigu.cn

Py:   super().greet()
来源：http://fv.huanxung.cn

PHP:  parent::greet();
来源：http://ke.colortex.cn

JS:   super.greet();
来源：http://be.szsharing.cn

TS:   super.greet();
来源：http://ml.muxihuayi.cn

Java: super.greet();
来源：http://ln.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zh.newstarts.cn

Ruby: super
来源：http://yl.hnjuh.cn

C#:   base.Greet();
来源：http://hp.colortex.cn

[G08] 静态方法与属性
来源：http://vy.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sb.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://vy.nszjky.cn

JS:   static f() {}
来源：http://dr.nicolike.cn

TS:   static f(): void {}
来源：http://cf.bjjhwx.cn

Java: static void f() {}
来源：http://ry.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bd.huanxung.cn

Ruby: def self.f; end
来源：http://mc.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://ft.colortex.cn

[G09] 接口 / 抽象类
来源：http://dd.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://de.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fe.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wq.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://yd.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://ki.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://fd.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mh.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ry.bjjhwx.cn

[G10] 访问控制
来源：http://nt.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://ta.shxzskj.cn

PHP:  public / protected / private
来源：http://up.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://cq.szsharing.cn

TS:   public / protected / private
来源：http://na.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://rc.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ia.chemitech.net.cn

Ruby: public / protected / private
来源：http://tr.colortex.cn

C#:   public / protected / private / internal
来源：http://ne.huixiangedu.cn

[G11] getter / setter
来源：http://sw.newstarts.cn

Py:   @property 与 @x.setter
来源：http://hc.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mw.newstarts.cn

JS:   get name() { return this._name; }
来源：http://kv.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://rr.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://pt.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dk.lnxyls.cn

Ruby: attr_accessor :name
来源：http://sl.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://ay.newstarts.cn

[G12] 对象转字符串
来源：http://hi.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://ba.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vc.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://pp.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://tx.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://rt.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wk.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://bg.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://cv.hahajie.cn

[G13] 判断对象类型
来源：http://ua.asd995.cn

Py:   isinstance(u, User)
来源：http://uv.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://pk.huixiangedu.cn

JS:   u instanceof User
来源：http://ut.521024.cn

TS:   u instanceof User
来源：http://jr.huanxung.cn

Java: u instanceof User
来源：http://lo.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bn.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://lb.shtwfgs.cn

C#:   u is User
来源：http://jj.colortex.cn

[G14] 数据类 / record
来源：http://pp.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nj.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://bq.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xp.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://lh.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://zw.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://tc.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://up.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://he.jianghongdianzi.cn

[G15] 枚举
来源：http://hl.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ri.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://it.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dy.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ri.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://tx.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ci.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://cb.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ax.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://ot.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://js.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://bj.gzmigu.cn

JS:   Object.entries(obj)
来源：http://cw.shxzskj.cn

TS:   Object.entries(obj)
来源：http://gb.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aa.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wd.szxytkj.cn

Ruby: obj.instance_variables
来源：http://eo.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://ec.yuntaijiaju.cn

================================================================================
来源：http://fu.hahajie.cn

H. 异常与错误处理
来源：http://nr.shxzskj.cn

================================================================================
来源：http://ne.szsharing.cn

[H01] try / catch 基础
来源：http://sa.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vr.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mk.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lu.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://we.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fd.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qo.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://im.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xy.huanxung.cn

[H02] finally / ensure 收尾
来源：http://tk.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mi.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fp.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zy.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jc.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gs.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tz.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fa.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pu.chemitech.net.cn

[H03] 主动抛出异常
来源：http://oz.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://sy.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ya.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://vf.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://tr.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fm.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ta.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oe.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bv.chemitech.net.cn

[H04] 自定义异常类型
来源：http://oa.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://dm.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ac.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://mb.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://vm.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://wm.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gp.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://jq.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://zt.wgjwhj.cn

[H05] 捕获特定类型
来源：http://gx.9csxet.cn

Py:   except ValueError as e:
来源：http://xa.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dv.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://hj.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://ik.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://lt.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jx.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://tm.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://px.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://ud.asd995.cn

Py:   value = d.get("k") or default
来源：http://xu.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sw.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vr.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vy.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zb.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yi.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://oo.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://hn.nicolike.cn

[H07] 断言
来源：http://jv.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://xe.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://jt.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://qk.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://km.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://cr.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mh.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yr.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://to.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://cd.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://yq.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nt.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://nn.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bm.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pl.chemitech.net.cn

Go:   err.Error()
来源：http://ra.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://zi.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://gk.asd995.cn

[H09] 带错误码的异常
来源：http://vw.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://me.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gh.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yb.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bl.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nj.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kr.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ce.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ud.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://yy.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ay.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zt.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xw.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ru.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oq.gzmigu.cn

Go:   defer f.Close()
来源：http://vq.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fu.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qn.nicolike.cn

================================================================================
来源：http://uo.asd995.cn

I. 正则表达式
来源：http://wj.chemitech.net.cn

================================================================================
来源：http://rc.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://cl.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xu.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vb.nicolike.cn

JS:   /\d+/.test(s)
来源：http://eu.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://iw.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gd.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://my.521024.cn

Ruby: s.match?(/\d+/)
来源：http://oa.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ib.shxzskj.cn

[I02] 提取所有匹配
来源：http://ll.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://um.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sr.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nn.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://nu.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gj.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://st.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://ea.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fs.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://kb.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dl.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wz.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ge.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ws.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lx.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gk.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bv.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zi.jianghongdianzi.cn

[I04] 正则替换
来源：http://po.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://al.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ve.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zg.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ow.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dy.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xz.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://da.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ve.shxzskj.cn

[I05] 按正则拆分
来源：http://qq.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qw.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jl.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://hp.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ao.szsharing.cn


<!-- 参考信息 -->