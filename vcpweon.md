代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fj.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xd.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bn.shxzskj.cn

TS:   // 同上
来源：http://yg.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bq.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://os.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yq.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vu.9csxet.cn

================================================================================
来源：http://tr.bookmarksfly.cn

G. 面向对象
来源：http://uj.9csxet.cn

================================================================================
来源：http://hu.szsharing.cn

[G01] 定义类
来源：http://nz.nszjky.cn

Py:   class User: pass
来源：http://zr.szsharing.cn

PHP:  class User {}
来源：http://pv.bookmarksfly.cn

JS:   class User {}
来源：http://is.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://cz.9csxet.cn

Java: class User {}
来源：http://cc.huanxung.cn

Go:   type User struct { Name string }
来源：http://ra.shxzskj.cn

Ruby: class User; end
来源：http://cz.haigaiapp.cn

C#:   class User {}
来源：http://mi.colortex.cn

[G02] 构造函数
来源：http://zx.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://ms.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://my.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://mz.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://cj.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://rv.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aj.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://co.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://cn.muxihuayi.cn

[G03] 实例属性
来源：http://oo.asd995.cn

Py:   self.name = "x"
来源：http://mm.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://ra.szxytkj.cn

JS:   this.name = "x";
来源：http://hj.bookmarksfly.cn

TS:   name: string = "x";
来源：http://yu.asd995.cn

Java: private String name;
来源：http://vb.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rd.gzmigu.cn

Ruby: @name = "x"
来源：http://tt.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://rf.lnxyls.cn

[G04] 定义方法
来源：http://mr.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://lq.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qb.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://na.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://bg.asd995.cn

Java: String greet() { return name; }
来源：http://du.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eo.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://jo.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://nq.521024.cn

[G05] 继承
来源：http://ob.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://dh.nszjky.cn

PHP:  class Admin extends User {}
来源：http://kp.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://xx.panjiajie.cn

TS:   class Admin extends User {}
来源：http://nz.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://mx.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ux.9csxet.cn

Ruby: class Admin < User; end
来源：http://ne.yuexingan06.cn

C#:   class Admin : User {}
来源：http://mi.hnjuh.cn

[G06] 重写方法
来源：http://qh.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://nr.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wp.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://pf.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://yu.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://dp.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qe.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://yv.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://nt.szsharing.cn

[G07] 调用父类方法
来源：http://ge.szsharing.cn

Py:   super().greet()
来源：http://bq.lnxyls.cn

PHP:  parent::greet();
来源：http://uj.chemitech.net.cn

JS:   super.greet();
来源：http://tg.jctech888.com.cn

TS:   super.greet();
来源：http://gt.muxihuayi.cn

Java: super.greet();
来源：http://hj.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mq.jianghongdianzi.cn

Ruby: super
来源：http://yn.hahajie.cn

C#:   base.Greet();
来源：http://wp.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://fl.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pt.wgjwhj.cn

PHP:  public static function f() {}
来源：http://by.shxzukj.cn

JS:   static f() {}
来源：http://wu.hahajie.cn

TS:   static f(): void {}
来源：http://dh.shxzskj.cn

Java: static void f() {}
来源：http://zo.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yx.muxihuayi.cn

Ruby: def self.f; end
来源：http://qp.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://aj.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://kf.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://oj.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qd.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jv.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://xp.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://fn.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://sg.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bk.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://ki.huixinmuqiang.cn

[G10] 访问控制
来源：http://iv.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://yd.asd995.cn

PHP:  public / protected / private
来源：http://of.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://cs.bjjhwx.cn

TS:   public / protected / private
来源：http://ca.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://bg.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nj.haigaiapp.cn

Ruby: public / protected / private
来源：http://wg.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://rz.muxihuayi.cn

[G11] getter / setter
来源：http://dq.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://vi.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cs.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://az.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://ba.shxzukj.cn

Java: public String getName() { return name; }
来源：http://yj.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ns.huanxung.cn

Ruby: attr_accessor :name
来源：http://qx.hahajie.cn

C#:   public string Name { get; set; }
来源：http://iz.huanxung.cn

[G12] 对象转字符串
来源：http://mw.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://pt.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nr.colortex.cn

JS:   toString() { return this.name; }
来源：http://pq.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://tg.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://mv.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vp.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://mu.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://fa.huixiangedu.cn

[G13] 判断对象类型
来源：http://il.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://iw.huixiangedu.cn

PHP:  $u instanceof User
来源：http://oh.nszjky.cn

JS:   u instanceof User
来源：http://ii.nszjky.cn

TS:   u instanceof User
来源：http://xh.jianghongdianzi.cn

Java: u instanceof User
来源：http://jb.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bw.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://rk.521024.cn

C#:   u is User
来源：http://xt.asd995.cn

[G14] 数据类 / record
来源：http://wr.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qk.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://sc.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hr.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://xv.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://su.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://je.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zw.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://mt.newstarts.cn

[G15] 枚举
来源：http://ik.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dn.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hf.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bt.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oq.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://wo.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nw.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://qh.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xp.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://hz.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qi.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://vd.colortex.cn

JS:   Object.entries(obj)
来源：http://bb.colortex.cn

TS:   Object.entries(obj)
来源：http://ob.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oa.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fu.hahajie.cn

Ruby: obj.instance_variables
来源：http://yv.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://zy.lnxyls.cn

================================================================================
来源：http://rg.szsharing.cn

H. 异常与错误处理
来源：http://fg.wgjwhj.cn

================================================================================
来源：http://ei.yuexingan06.cn

[H01] try / catch 基础
来源：http://or.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xo.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ee.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ey.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sn.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yw.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fk.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hs.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ue.asd995.cn

[H02] finally / ensure 收尾
来源：http://rh.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mo.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://me.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xu.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cn.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tk.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ev.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kr.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fv.shxzskj.cn

[H03] 主动抛出异常
来源：http://ih.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://kq.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jx.asd995.cn

JS:   throw new Error("错误信息");
来源：http://ti.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://dc.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fd.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lr.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fx.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://il.haigaiapp.cn

[H04] 自定义异常类型
来源：http://eu.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://cy.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mk.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://ss.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://xy.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://on.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ez.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://tb.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://ek.muxihuayi.cn

[H05] 捕获特定类型
来源：http://fb.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://sq.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dn.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://tt.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://ch.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://rs.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ly.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://cr.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ub.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://sa.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://mi.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cw.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ip.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xs.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ef.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cp.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://la.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://zn.nicolike.cn

[H07] 断言
来源：http://ot.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://wf.hnjuh.cn

PHP:  assert($x > 0);
来源：http://bt.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://up.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://at.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://tu.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hi.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gk.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://ms.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://dj.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ml.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dg.nszjky.cn

JS:   e.message;  e.stack
来源：http://jt.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ri.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vo.huanxung.cn

Go:   err.Error()
来源：http://rx.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://xn.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://jr.panjiajie.cn

[H09] 带错误码的异常
来源：http://tj.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bk.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jh.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ab.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qx.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gh.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wb.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://km.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qz.muxihuayi.cn

[H10] 资源自动释放
来源：http://re.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://du.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qt.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xr.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bl.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://le.szsharing.cn

Go:   defer f.Close()
来源：http://cz.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xt.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jk.yuexingan06.cn

================================================================================
来源：http://ee.jctech888.com.cn

I. 正则表达式
来源：http://mu.hahajie.cn

================================================================================
来源：http://lk.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://da.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://or.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xq.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://hd.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://iy.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mu.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pf.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://ib.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pv.wgjwhj.cn

[I02] 提取所有匹配
来源：http://vu.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ph.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ii.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://fo.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ec.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mp.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://vt.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sg.hnjuh.cn

[I03] 提取捕获分组
来源：http://uw.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ip.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mo.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kd.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ex.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://en.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gv.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ff.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fy.asd995.cn

[I04] 正则替换
来源：http://eh.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dg.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ie.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gc.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mg.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bc.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ad.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yw.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qp.521024.cn

[I05] 按正则拆分
来源：http://ja.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ea.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://af.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://vi.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://zo.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://zc.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dn.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gs.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://is.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://in.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bd.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ew.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jp.newstarts.cn


<!-- 参考信息 -->