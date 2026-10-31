代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zv.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fr.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qk.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nh.haigaiapp.cn

================================================================================
来源：http://hb.newstarts.cn

G. 面向对象
来源：http://pn.wgjwhj.cn

================================================================================
来源：http://mt.huixiangedu.cn

[G01] 定义类
来源：http://lr.gzmigu.cn

Py:   class User: pass
来源：http://uk.lnxyls.cn

PHP:  class User {}
来源：http://ii.jianghongdianzi.cn

JS:   class User {}
来源：http://xu.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://sb.nszjky.cn

Java: class User {}
来源：http://xz.9csxet.cn

Go:   type User struct { Name string }
来源：http://mv.9csxet.cn

Ruby: class User; end
来源：http://ra.lnxyls.cn

C#:   class User {}
来源：http://cr.nszjky.cn

[G02] 构造函数
来源：http://rh.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://nf.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ug.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://sb.colortex.cn

TS:   constructor(public name: string) {}
来源：http://fa.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://wi.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jr.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://xc.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://ee.shtwfgs.cn

[G03] 实例属性
来源：http://zn.huanxung.cn

Py:   self.name = "x"
来源：http://os.huanxung.cn

PHP:  public string $name = "x";
来源：http://jb.haigaiapp.cn

JS:   this.name = "x";
来源：http://ev.lnxyls.cn

TS:   name: string = "x";
来源：http://fd.521024.cn

Java: private String name;
来源：http://re.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dv.shxzskj.cn

Ruby: @name = "x"
来源：http://hn.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://dr.521024.cn

[G04] 定义方法
来源：http://ko.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://eg.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://so.9csxet.cn

JS:   greet() { return this.name; }
来源：http://nk.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://qc.521024.cn

Java: String greet() { return name; }
来源：http://xa.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vo.gzmigu.cn

Ruby: def greet; @name; end
来源：http://ih.521024.cn

C#:   public string Greet() => Name;
来源：http://ot.panjiajie.cn

[G05] 继承
来源：http://ir.nszjky.cn

Py:   class Admin(User): pass
来源：http://ya.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://we.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://tc.szxytkj.cn

TS:   class Admin extends User {}
来源：http://ow.wgjwhj.cn

Java: class Admin extends User {}
来源：http://rm.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bc.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://ci.521024.cn

C#:   class Admin : User {}
来源：http://gr.huanxung.cn

[G06] 重写方法
来源：http://di.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://io.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tu.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://wx.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://nk.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ec.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fi.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://sb.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://zb.newstarts.cn

[G07] 调用父类方法
来源：http://za.shxzskj.cn

Py:   super().greet()
来源：http://ku.colortex.cn

PHP:  parent::greet();
来源：http://qs.shxzukj.cn

JS:   super.greet();
来源：http://rw.panjiajie.cn

TS:   super.greet();
来源：http://mw.yuntaijiaju.cn

Java: super.greet();
来源：http://fm.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uy.hahajie.cn

Ruby: super
来源：http://ne.hahajie.cn

C#:   base.Greet();
来源：http://ec.shxzukj.cn

[G08] 静态方法与属性
来源：http://ml.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cr.nszjky.cn

PHP:  public static function f() {}
来源：http://bq.muxihuayi.cn

JS:   static f() {}
来源：http://qb.newstarts.cn

TS:   static f(): void {}
来源：http://vm.jianghongdianzi.cn

Java: static void f() {}
来源：http://yd.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cx.asd995.cn

Ruby: def self.f; end
来源：http://oa.chemitech.net.cn

C#:   public static void F() {}
来源：http://lb.asd995.cn

[G09] 接口 / 抽象类
来源：http://ex.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ko.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gn.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hd.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://mp.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://uq.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://ie.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kv.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://ej.521024.cn

[G10] 访问控制
来源：http://qc.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://de.asd995.cn

PHP:  public / protected / private
来源：http://ao.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://kk.shtwfgs.cn

TS:   public / protected / private
来源：http://uz.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://ac.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rl.shtwfgs.cn

Ruby: public / protected / private
来源：http://mg.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://fy.chemitech.net.cn

[G11] getter / setter
来源：http://fx.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://qc.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sh.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://hm.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://uu.colortex.cn

Java: public String getName() { return name; }
来源：http://wb.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pp.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://ln.szsharing.cn

C#:   public string Name { get; set; }
来源：http://ko.shxzukj.cn

[G12] 对象转字符串
来源：http://dc.colortex.cn

Py:   def __str__(self): return self.name
来源：http://xc.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xd.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://wi.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://cv.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://xx.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cd.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://jp.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://yr.huixiangedu.cn

[G13] 判断对象类型
来源：http://wt.szxytkj.cn

Py:   isinstance(u, User)
来源：http://xk.521024.cn

PHP:  $u instanceof User
来源：http://fl.9csxet.cn

JS:   u instanceof User
来源：http://ar.asd995.cn

TS:   u instanceof User
来源：http://fk.yuexingan06.cn

Java: u instanceof User
来源：http://dq.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fy.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://nv.yuntaijiaju.cn

C#:   u is User
来源：http://bp.szsharing.cn

[G14] 数据类 / record
来源：http://ju.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kr.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://sm.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://li.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://ik.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://pn.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://qm.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://za.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://yh.gzmigu.cn

[G15] 枚举
来源：http://wd.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://by.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yc.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vw.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nx.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://qb.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nf.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://dh.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lw.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://tc.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wk.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://bv.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://ff.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://za.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mw.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fn.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://kk.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://lb.asd995.cn

================================================================================
来源：http://tl.huixinmuqiang.cn

H. 异常与错误处理
来源：http://mu.bjjhwx.cn

================================================================================
来源：http://bn.huanxung.cn

[H01] try / catch 基础
来源：http://he.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ip.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vn.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xl.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hf.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gx.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vi.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sy.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qb.huanxung.cn

[H02] finally / ensure 收尾
来源：http://wm.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rw.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sa.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qa.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zl.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://el.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oj.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bj.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hb.haigaiapp.cn

[H03] 主动抛出异常
来源：http://vz.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://bw.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bv.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://nl.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://xc.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ag.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gk.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wj.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kq.asd995.cn

[H04] 自定义异常类型
来源：http://my.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://ul.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qb.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://fy.szsharing.cn

TS:   class MyError extends Error {}
来源：http://sk.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://gf.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pd.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://kd.szsharing.cn

C#:   class MyException : Exception {}
来源：http://qa.yuexingan06.cn

[H05] 捕获特定类型
来源：http://bb.newstarts.cn

Py:   except ValueError as e:
来源：http://nw.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aq.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://kv.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://xs.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://mj.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nl.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://mu.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mm.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://fl.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://hu.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rj.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cr.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xk.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ub.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mq.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://za.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://js.shxzskj.cn

[H07] 断言
来源：http://vn.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://zs.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://hr.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://sb.521024.cn

TS:   console.assert(x > 0);
来源：http://xu.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://su.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ja.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xd.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://ct.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://rg.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://sv.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rg.shxzskj.cn

JS:   e.message;  e.stack
来源：http://ac.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ki.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ev.szsharing.cn

Go:   err.Error()
来源：http://hd.521024.cn

Ruby: e.message;  e.backtrace
来源：http://sh.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://ss.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ki.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yk.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nk.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ug.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aj.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pn.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ak.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aa.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sx.521024.cn

[H10] 资源自动释放
来源：http://no.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ml.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://me.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yx.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pt.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gn.szsharing.cn

Go:   defer f.Close()
来源：http://en.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dj.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ez.jianghongdianzi.cn

================================================================================
来源：http://ca.huixinmuqiang.cn

I. 正则表达式
来源：http://xg.yuntaijiaju.cn

================================================================================
来源：http://he.yuexingan06.cn

[I01] 判断是否匹配
来源：http://ia.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cn.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ic.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://mw.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://cy.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cb.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yd.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://vr.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ih.shxzskj.cn

[I02] 提取所有匹配
来源：http://pt.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://sm.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yu.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nz.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://zq.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rf.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ce.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://xs.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jw.shxzukj.cn

[I03] 提取捕获分组
来源：http://ej.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uj.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pe.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://as.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rr.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pr.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qr.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ue.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qs.haigaiapp.cn

[I04] 正则替换
来源：http://ki.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ad.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oa.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cm.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ud.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oq.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bo.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vz.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://og.hahajie.cn

[I05] 按正则拆分
来源：http://gd.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://up.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ad.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://ps.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://yj.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://bk.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ht.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ir.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vt.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pn.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gm.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yk.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ub.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tw.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oz.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ii.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://um.huixiangedu.cn


<!-- 参考信息 -->