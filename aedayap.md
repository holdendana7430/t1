代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nl.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hs.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://va.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ek.huanxung.cn

================================================================================
来源：http://mt.asd995.cn

G. 面向对象
来源：http://dw.muxihuayi.cn

================================================================================
来源：http://ml.huanxung.cn

[G01] 定义类
来源：http://wk.bookmarksfly.cn

Py:   class User: pass
来源：http://av.panjiajie.cn

PHP:  class User {}
来源：http://tj.huixiangedu.cn

JS:   class User {}
来源：http://ju.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://jm.jianghongdianzi.cn

Java: class User {}
来源：http://oq.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://vb.huixinmuqiang.cn

Ruby: class User; end
来源：http://jf.panjiajie.cn

C#:   class User {}
来源：http://ib.huixinmuqiang.cn

[G02] 构造函数
来源：http://yw.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://bp.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://sn.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://hc.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://pb.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://xy.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gp.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://mh.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://vs.shtwfgs.cn

[G03] 实例属性
来源：http://du.shtwfgs.cn

Py:   self.name = "x"
来源：http://ok.szxytkj.cn

PHP:  public string $name = "x";
来源：http://iv.haigaiapp.cn

JS:   this.name = "x";
来源：http://nh.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://rc.hahajie.cn

Java: private String name;
来源：http://ac.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ww.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://et.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://br.huixiangedu.cn

[G04] 定义方法
来源：http://mt.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://kd.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ez.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://ed.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://ic.panjiajie.cn

Java: String greet() { return name; }
来源：http://te.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fk.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://qi.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://mw.bookmarksfly.cn

[G05] 继承
来源：http://om.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://ra.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://wt.szxytkj.cn

JS:   class Admin extends User {}
来源：http://mv.nszjky.cn

TS:   class Admin extends User {}
来源：http://ta.huixiangedu.cn

Java: class Admin extends User {}
来源：http://jk.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jq.szxytkj.cn

Ruby: class Admin < User; end
来源：http://rp.muxihuayi.cn

C#:   class Admin : User {}
来源：http://vg.colortex.cn

[G06] 重写方法
来源：http://oh.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://sg.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gp.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://bs.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://rw.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://zn.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://do.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://uy.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://qf.nicolike.cn

[G07] 调用父类方法
来源：http://il.yuexingan06.cn

Py:   super().greet()
来源：http://zn.shxzukj.cn

PHP:  parent::greet();
来源：http://ql.huixiangedu.cn

JS:   super.greet();
来源：http://kd.szsharing.cn

TS:   super.greet();
来源：http://bn.bookmarksfly.cn

Java: super.greet();
来源：http://iq.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lr.haigaiapp.cn

Ruby: super
来源：http://wz.yuntaijiaju.cn

C#:   base.Greet();
来源：http://fl.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://op.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mb.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://ou.yuexingan06.cn

JS:   static f() {}
来源：http://te.haigaiapp.cn

TS:   static f(): void {}
来源：http://ny.hahajie.cn

Java: static void f() {}
来源：http://mj.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mf.521024.cn

Ruby: def self.f; end
来源：http://lu.shtwfgs.cn

C#:   public static void F() {}
来源：http://yy.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://yf.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://qt.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vd.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fd.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://ux.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://gi.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ii.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rp.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://cb.yuntaijiaju.cn

[G10] 访问控制
来源：http://qe.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://eu.bjjhwx.cn

PHP:  public / protected / private
来源：http://uk.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://mx.chemitech.net.cn

TS:   public / protected / private
来源：http://la.521024.cn

Java: public / protected / private / 默认包级
来源：http://xn.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://it.bookmarksfly.cn

Ruby: public / protected / private
来源：http://yz.gzmigu.cn

C#:   public / protected / private / internal
来源：http://vl.szxytkj.cn

[G11] getter / setter
来源：http://bb.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://cf.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ji.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://lf.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://dc.lnxyls.cn

Java: public String getName() { return name; }
来源：http://lt.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jf.colortex.cn

Ruby: attr_accessor :name
来源：http://dc.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://pm.newstarts.cn

[G12] 对象转字符串
来源：http://es.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://kg.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ca.colortex.cn

JS:   toString() { return this.name; }
来源：http://ms.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://ea.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://dm.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lp.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://pb.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://rk.szsharing.cn

[G13] 判断对象类型
来源：http://la.asd995.cn

Py:   isinstance(u, User)
来源：http://yn.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://hf.panjiajie.cn

JS:   u instanceof User
来源：http://sm.szxytkj.cn

TS:   u instanceof User
来源：http://wz.huanxung.cn

Java: u instanceof User
来源：http://bj.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ap.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://oh.jctech888.com.cn

C#:   u is User
来源：http://ot.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://cf.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qg.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://dz.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://em.521024.cn

TS:   type User = { name: string; age: number };
来源：http://fl.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://ia.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://sc.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ak.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://oq.szsharing.cn

[G15] 枚举
来源：http://ug.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nm.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xs.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wi.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ee.521024.cn

Java: enum Color { RED, GREEN }
来源：http://op.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ku.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://do.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wi.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://iz.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mz.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://ij.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://lq.nszjky.cn

TS:   Object.entries(obj)
来源：http://ax.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ml.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rd.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://uh.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://sp.szsharing.cn

================================================================================
来源：http://om.hnjuh.cn

H. 异常与错误处理
来源：http://ch.nszjky.cn

================================================================================
来源：http://na.lnxyls.cn

[H01] try / catch 基础
来源：http://xk.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ha.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ft.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dd.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xx.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cd.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lp.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://of.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qe.9csxet.cn

[H02] finally / ensure 收尾
来源：http://jo.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ch.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iq.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jf.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iv.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cn.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bo.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fc.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ky.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://qc.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://sg.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sy.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://vf.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://wz.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eq.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vv.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xu.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ql.lnxyls.cn

[H04] 自定义异常类型
来源：http://bp.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://ms.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lt.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://qv.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://bu.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://dx.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gd.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://fa.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://qo.colortex.cn

[H05] 捕获特定类型
来源：http://jl.nszjky.cn

Py:   except ValueError as e:
来源：http://wy.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ts.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://wj.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://zg.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://df.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ea.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://lu.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hj.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://cq.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://st.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jm.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ix.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zb.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fb.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cq.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://ez.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://yi.nicolike.cn

[H07] 断言
来源：http://ri.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://wy.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://yh.nszjky.cn

JS:   console.assert(x > 0);
来源：http://zt.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://rs.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://ee.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yi.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kj.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://jx.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://fg.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://jp.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jl.gzmigu.cn

JS:   e.message;  e.stack
来源：http://la.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pe.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://za.shxzskj.cn

Go:   err.Error()
来源：http://ru.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://ak.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://en.huixiangedu.cn

[H09] 带错误码的异常
来源：http://of.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sh.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tu.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://os.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ua.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ju.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ki.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://el.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ew.bookmarksfly.cn

[H10] 资源自动释放
来源：http://xw.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wv.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ir.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://et.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sr.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wd.newstarts.cn

Go:   defer f.Close()
来源：http://lp.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jw.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jm.newstarts.cn

================================================================================
来源：http://te.haigaiapp.cn

I. 正则表达式
来源：http://ed.shxzskj.cn

================================================================================
来源：http://us.521024.cn

[I01] 判断是否匹配
来源：http://fk.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wy.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ju.colortex.cn

JS:   /\d+/.test(s)
来源：http://ph.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://yq.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://il.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ia.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://xo.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pi.szsharing.cn

[I02] 提取所有匹配
来源：http://jv.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://hw.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sm.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ax.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://ro.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gh.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hr.521024.cn

Ruby: s.scan(/\d+/)
来源：http://if.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dv.yuexingan06.cn

[I03] 提取捕获分组
来源：http://sm.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fo.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sr.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mr.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ey.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mh.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sl.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tu.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.panjiajie.cn

[I04] 正则替换
来源：http://hv.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cu.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jy.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://je.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sq.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ga.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jb.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://la.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uh.shtwfgs.cn

[I05] 按正则拆分
来源：http://ft.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gv.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vi.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://vu.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://xp.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://bv.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ip.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ne.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fl.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://je.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bd.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://et.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bw.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sw.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://un.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pa.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wo.shxzskj.cn


<!-- 参考信息 -->