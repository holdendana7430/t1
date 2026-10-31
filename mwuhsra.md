代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qr.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rw.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qv.shtwfgs.cn

[F12] CSV 读写
来源：http://gw.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xz.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bb.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yn.jctech888.com.cn

TS:   // 同上
来源：http://ya.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mc.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fp.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tb.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ul.asd995.cn

================================================================================
来源：http://hq.huanxung.cn

G. 面向对象
来源：http://bt.wgjwhj.cn

================================================================================
来源：http://kg.huixiangedu.cn

[G01] 定义类
来源：http://on.haigaiapp.cn

Py:   class User: pass
来源：http://mh.muxihuayi.cn

PHP:  class User {}
来源：http://zy.bookmarksfly.cn

JS:   class User {}
来源：http://pd.asd995.cn

TS:   class User { name: string = ""; }
来源：http://yx.521024.cn

Java: class User {}
来源：http://tq.huanxung.cn

Go:   type User struct { Name string }
来源：http://gm.huanxung.cn

Ruby: class User; end
来源：http://qj.9csxet.cn

C#:   class User {}
来源：http://bw.nicolike.cn

[G02] 构造函数
来源：http://ae.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://ma.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://cl.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://xg.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://qr.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://vk.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vz.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://gw.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://qn.lnxyls.cn

[G03] 实例属性
来源：http://tr.nszjky.cn

Py:   self.name = "x"
来源：http://rd.panjiajie.cn

PHP:  public string $name = "x";
来源：http://ju.szxytkj.cn

JS:   this.name = "x";
来源：http://ey.huanxung.cn

TS:   name: string = "x";
来源：http://vd.bjjhwx.cn

Java: private String name;
来源：http://aq.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gp.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://lf.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://xa.lnxyls.cn

[G04] 定义方法
来源：http://pm.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://fs.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://av.colortex.cn

JS:   greet() { return this.name; }
来源：http://ii.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://ed.shtwfgs.cn

Java: String greet() { return name; }
来源：http://li.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pq.nicolike.cn

Ruby: def greet; @name; end
来源：http://sc.newstarts.cn

C#:   public string Greet() => Name;
来源：http://nc.nicolike.cn

[G05] 继承
来源：http://pz.nszjky.cn

Py:   class Admin(User): pass
来源：http://hj.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://vk.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://wi.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://ui.bjjhwx.cn

Java: class Admin extends User {}
来源：http://sx.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sg.521024.cn

Ruby: class Admin < User; end
来源：http://ek.gzmigu.cn

C#:   class Admin : User {}
来源：http://dr.asd995.cn

[G06] 重写方法
来源：http://za.asd995.cn

Py:   def greet(self): return "admin"
来源：http://jq.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ra.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://pr.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://bk.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://xx.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sh.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://dx.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://ri.hahajie.cn

[G07] 调用父类方法
来源：http://cq.9csxet.cn

Py:   super().greet()
来源：http://av.bookmarksfly.cn

PHP:  parent::greet();
来源：http://dj.szsharing.cn

JS:   super.greet();
来源：http://lh.szxytkj.cn

TS:   super.greet();
来源：http://ru.yuntaijiaju.cn

Java: super.greet();
来源：http://bo.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ry.hnjuh.cn

Ruby: super
来源：http://wt.chemitech.net.cn

C#:   base.Greet();
来源：http://uy.muxihuayi.cn

[G08] 静态方法与属性
来源：http://fu.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yv.gzmigu.cn

PHP:  public static function f() {}
来源：http://lr.huixinmuqiang.cn

JS:   static f() {}
来源：http://qe.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://xe.newstarts.cn

Java: static void f() {}
来源：http://gj.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vv.wgjwhj.cn

Ruby: def self.f; end
来源：http://ft.yuexingan06.cn

C#:   public static void F() {}
来源：http://lp.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://jq.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://qk.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ic.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cd.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://gt.newstarts.cn

Java: interface Shape { double area(); }
来源：http://qe.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://yr.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pj.521024.cn

C#:   interface IShape { double Area(); }
来源：http://oi.9csxet.cn

[G10] 访问控制
来源：http://vf.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://bv.wgjwhj.cn

PHP:  public / protected / private
来源：http://py.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://lx.bjjhwx.cn

TS:   public / protected / private
来源：http://vh.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://kt.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ad.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://bu.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://pq.wgjwhj.cn

[G11] getter / setter
来源：http://pu.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://hd.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fp.hahajie.cn

JS:   get name() { return this._name; }
来源：http://ou.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://ko.nszjky.cn

Java: public String getName() { return name; }
来源：http://hr.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lf.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://ep.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://lc.nicolike.cn

[G12] 对象转字符串
来源：http://tp.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://rr.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mp.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://lv.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://sr.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://jq.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vm.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://ai.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://le.shxzskj.cn

[G13] 判断对象类型
来源：http://iq.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://lp.wgjwhj.cn

PHP:  $u instanceof User
来源：http://lc.szxytkj.cn

JS:   u instanceof User
来源：http://xm.nicolike.cn

TS:   u instanceof User
来源：http://aj.muxihuayi.cn

Java: u instanceof User
来源：http://sw.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rw.nszjky.cn

Ruby: u.is_a?(User)
来源：http://vp.huixiangedu.cn

C#:   u is User
来源：http://qe.jctech888.com.cn

[G14] 数据类 / record
来源：http://cu.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tf.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://nu.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vs.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://hz.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://ye.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://mg.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://db.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://vm.yuntaijiaju.cn

[G15] 枚举
来源：http://je.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bn.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pa.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vx.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://or.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://ga.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nz.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://we.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ff.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://ek.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://va.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://mk.shxzukj.cn

JS:   Object.entries(obj)
来源：http://pv.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://qy.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ae.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mv.szsharing.cn

Ruby: obj.instance_variables
来源：http://kp.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ai.chemitech.net.cn

================================================================================
来源：http://tp.gzmigu.cn

H. 异常与错误处理
来源：http://qe.shtwfgs.cn

================================================================================
来源：http://cp.jctech888.com.cn

[H01] try / catch 基础
来源：http://he.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://li.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xi.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ul.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jc.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://an.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://my.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zf.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://us.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://ng.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gg.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xu.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lt.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bw.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gd.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mj.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cy.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pz.hahajie.cn

[H03] 主动抛出异常
来源：http://iy.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://zi.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ao.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://ho.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://cz.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gr.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ri.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wa.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sm.hahajie.cn

[H04] 自定义异常类型
来源：http://ns.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://qp.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ym.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://ry.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://kn.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://mx.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ow.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://pn.521024.cn

C#:   class MyException : Exception {}
来源：http://fv.huixiangedu.cn

[H05] 捕获特定类型
来源：http://vb.huixiangedu.cn

Py:   except ValueError as e:
来源：http://xm.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zb.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://xa.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://dk.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://du.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qz.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://xm.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ej.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://ym.szsharing.cn

Py:   value = d.get("k") or default
来源：http://jv.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://et.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bh.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cm.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://py.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://il.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://ui.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://nb.muxihuayi.cn

[H07] 断言
来源：http://py.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://ov.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://hc.newstarts.cn

JS:   console.assert(x > 0);
来源：http://tb.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://px.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://dg.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://my.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tn.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://xm.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://jv.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ki.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vn.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://rk.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ar.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kf.chemitech.net.cn

Go:   err.Error()
来源：http://xf.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://ze.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://ur.szxytkj.cn

[H09] 带错误码的异常
来源：http://zc.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tt.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bi.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pf.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sq.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nu.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oe.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nw.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rz.521024.cn

[H10] 资源自动释放
来源：http://df.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bd.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bt.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yb.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xl.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fq.chemitech.net.cn

Go:   defer f.Close()
来源：http://tr.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yq.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tx.jianghongdianzi.cn

================================================================================
来源：http://cq.huixiangedu.cn

I. 正则表达式
来源：http://zm.gzmigu.cn

================================================================================
来源：http://ob.gzmigu.cn

[I01] 判断是否匹配
来源：http://eo.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sd.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wz.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://es.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://of.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qk.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ip.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://jg.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vm.yuexingan06.cn

[I02] 提取所有匹配
来源：http://pt.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://vb.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dq.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yi.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://pj.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cf.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eo.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://sm.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fd.jctech888.com.cn

[I03] 提取捕获分组
来源：http://ic.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vj.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kx.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ys.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yf.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ao.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aj.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pb.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zw.bjjhwx.cn

[I04] 正则替换
来源：http://jb.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ea.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fc.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://je.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yf.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zg.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://co.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ap.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://er.muxihuayi.cn

[I05] 按正则拆分
来源：http://lf.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lr.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uz.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://ik.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://jo.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://ci.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cz.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jh.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wi.asd995.cn


<!-- 参考信息 -->