代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ir.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sy.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hj.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qt.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ix.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xl.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://en.yuntaijiaju.cn

[F12] CSV 读写
来源：http://kp.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xw.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ls.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yj.muxihuayi.cn

TS:   // 同上
来源：http://la.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hh.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zt.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ia.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gw.shxzukj.cn

================================================================================
来源：http://zk.bjjhwx.cn

G. 面向对象
来源：http://vh.hnjuh.cn

================================================================================
来源：http://ts.jianghongdianzi.cn

[G01] 定义类
来源：http://xj.yuntaijiaju.cn

Py:   class User: pass
来源：http://qd.shxzukj.cn

PHP:  class User {}
来源：http://pk.shxzukj.cn

JS:   class User {}
来源：http://xh.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://nk.haigaiapp.cn

Java: class User {}
来源：http://bw.shxzukj.cn

Go:   type User struct { Name string }
来源：http://fh.nszjky.cn

Ruby: class User; end
来源：http://br.haigaiapp.cn

C#:   class User {}
来源：http://bd.szxytkj.cn

[G02] 构造函数
来源：http://um.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://cw.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://en.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://aq.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://cz.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://jw.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qp.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://nb.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://kc.newstarts.cn

[G03] 实例属性
来源：http://aw.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://gh.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://rz.wgjwhj.cn

JS:   this.name = "x";
来源：http://ks.shxzskj.cn

TS:   name: string = "x";
来源：http://sw.hahajie.cn

Java: private String name;
来源：http://gp.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lt.newstarts.cn

Ruby: @name = "x"
来源：http://bz.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://db.szxytkj.cn

[G04] 定义方法
来源：http://zh.9csxet.cn

Py:   def greet(self): return self.name
来源：http://tm.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://et.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://zr.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://ih.gzmigu.cn

Java: String greet() { return name; }
来源：http://io.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yw.nicolike.cn

Ruby: def greet; @name; end
来源：http://vp.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://zu.nszjky.cn

[G05] 继承
来源：http://xt.hnjuh.cn

Py:   class Admin(User): pass
来源：http://ne.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://rn.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://xh.hnjuh.cn

TS:   class Admin extends User {}
来源：http://ar.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://cg.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://le.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://bq.haigaiapp.cn

C#:   class Admin : User {}
来源：http://tr.hahajie.cn

[G06] 重写方法
来源：http://dr.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://xk.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xx.colortex.cn

JS:   greet() { return "admin"; }
来源：http://iy.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://vv.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://qd.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ca.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://lm.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://wy.jctech888.com.cn

[G07] 调用父类方法
来源：http://sf.wgjwhj.cn

Py:   super().greet()
来源：http://pj.szsharing.cn

PHP:  parent::greet();
来源：http://kv.szsharing.cn

JS:   super.greet();
来源：http://yn.colortex.cn

TS:   super.greet();
来源：http://rq.nicolike.cn

Java: super.greet();
来源：http://bv.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bl.bjjhwx.cn

Ruby: super
来源：http://kw.chemitech.net.cn

C#:   base.Greet();
来源：http://az.shtwfgs.cn

[G08] 静态方法与属性
来源：http://kq.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lz.haigaiapp.cn

PHP:  public static function f() {}
来源：http://ba.nicolike.cn

JS:   static f() {}
来源：http://hm.panjiajie.cn

TS:   static f(): void {}
来源：http://mi.jctech888.com.cn

Java: static void f() {}
来源：http://eg.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://et.hahajie.cn

Ruby: def self.f; end
来源：http://ni.bookmarksfly.cn

C#:   public static void F() {}
来源：http://pd.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ka.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://ju.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bx.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nh.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://ck.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://cj.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://an.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ak.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://fk.shxzskj.cn

[G10] 访问控制
来源：http://ns.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://pv.shtwfgs.cn

PHP:  public / protected / private
来源：http://xx.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ks.shxzukj.cn

TS:   public / protected / private
来源：http://pz.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://rl.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sn.muxihuayi.cn

Ruby: public / protected / private
来源：http://bc.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://dl.lnxyls.cn

[G11] getter / setter
来源：http://nq.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://xx.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ar.nicolike.cn

JS:   get name() { return this._name; }
来源：http://ec.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://or.lnxyls.cn

Java: public String getName() { return name; }
来源：http://pe.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jt.9csxet.cn

Ruby: attr_accessor :name
来源：http://vt.nszjky.cn

C#:   public string Name { get; set; }
来源：http://kx.hnjuh.cn

[G12] 对象转字符串
来源：http://rb.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://ks.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jd.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://fc.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://td.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://lz.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xe.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://wm.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://wz.shtwfgs.cn

[G13] 判断对象类型
来源：http://gw.huanxung.cn

Py:   isinstance(u, User)
来源：http://wj.haigaiapp.cn

PHP:  $u instanceof User
来源：http://ue.huixinmuqiang.cn

JS:   u instanceof User
来源：http://wc.huixiangedu.cn

TS:   u instanceof User
来源：http://ah.hahajie.cn

Java: u instanceof User
来源：http://bz.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gp.colortex.cn

Ruby: u.is_a?(User)
来源：http://lu.szsharing.cn

C#:   u is User
来源：http://qg.asd995.cn

[G14] 数据类 / record
来源：http://dj.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sx.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://mt.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sg.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://eq.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://fp.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://qt.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xp.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://ia.huixinmuqiang.cn

[G15] 枚举
来源：http://wf.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vi.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://il.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ia.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ys.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://jg.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ud.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://tj.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://su.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://ix.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://or.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://hu.szxytkj.cn

JS:   Object.entries(obj)
来源：http://xa.shxzukj.cn

TS:   Object.entries(obj)
来源：http://tc.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://du.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uh.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://gz.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://kq.jctech888.com.cn

================================================================================
来源：http://vw.shxzskj.cn

H. 异常与错误处理
来源：http://tb.haigaiapp.cn

================================================================================
来源：http://uy.szxytkj.cn

[H01] try / catch 基础
来源：http://wp.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mf.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qo.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sz.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qk.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xt.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lm.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hq.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pk.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://kf.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jy.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xj.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dk.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://op.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fz.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cl.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vx.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gw.huixiangedu.cn

[H03] 主动抛出异常
来源：http://lm.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://kz.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sn.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://wy.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://qw.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ij.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bz.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wd.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gm.hnjuh.cn

[H04] 自定义异常类型
来源：http://yc.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://gg.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ah.hahajie.cn

JS:   class MyError extends Error {}
来源：http://rr.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ej.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://pz.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://en.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ir.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://bu.shxzskj.cn

[H05] 捕获特定类型
来源：http://ri.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://we.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://px.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://sj.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://uf.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://mw.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qx.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://mt.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vo.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://jp.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://vs.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vy.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pg.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yj.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eu.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://em.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://it.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://kc.colortex.cn

[H07] 断言
来源：http://xe.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://fj.colortex.cn

PHP:  assert($x > 0);
来源：http://kf.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://oh.huanxung.cn

TS:   console.assert(x > 0);
来源：http://wp.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://ub.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://td.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fn.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://wn.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://du.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://rr.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sm.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://ed.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ej.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hk.lnxyls.cn

Go:   err.Error()
来源：http://yb.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://hp.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://co.colortex.cn

[H09] 带错误码的异常
来源：http://ze.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ww.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vg.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fd.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sv.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nv.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tr.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ym.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ww.huanxung.cn

[H10] 资源自动释放
来源：http://vy.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hd.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nq.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://co.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yc.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xh.lnxyls.cn

Go:   defer f.Close()
来源：http://sw.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://do.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qq.wgjwhj.cn

================================================================================
来源：http://eq.panjiajie.cn

I. 正则表达式
来源：http://gk.bjjhwx.cn

================================================================================
来源：http://kz.gzmigu.cn

[I01] 判断是否匹配
来源：http://ia.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ex.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pa.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://dt.9csxet.cn

TS:   /\d+/.test(s)
来源：http://pz.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tf.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ax.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://kd.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uo.shtwfgs.cn

[I02] 提取所有匹配
来源：http://fp.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://zj.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eh.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jx.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://xn.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ty.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xv.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://vk.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hx.huixiangedu.cn

[I03] 提取捕获分组
来源：http://nb.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ja.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oc.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://up.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vn.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ts.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ht.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bf.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oa.jianghongdianzi.cn

[I04] 正则替换
来源：http://pv.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://er.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xw.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cs.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hj.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iu.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fz.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nx.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qm.haigaiapp.cn

[I05] 按正则拆分
来源：http://eb.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tv.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nz.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://up.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ta.bjjhwx.cn


<!-- 参考信息 -->