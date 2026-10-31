代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ym.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sp.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mu.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mv.shxzukj.cn

================================================================================
来源：http://jv.huixinmuqiang.cn

G. 面向对象
来源：http://au.yuexingan06.cn

================================================================================
来源：http://qe.9csxet.cn

[G01] 定义类
来源：http://el.szsharing.cn

Py:   class User: pass
来源：http://hf.nszjky.cn

PHP:  class User {}
来源：http://ss.hnjuh.cn

JS:   class User {}
来源：http://ri.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://rb.huixinmuqiang.cn

Java: class User {}
来源：http://tx.hnjuh.cn

Go:   type User struct { Name string }
来源：http://fk.huixiangedu.cn

Ruby: class User; end
来源：http://sl.yuexingan06.cn

C#:   class User {}
来源：http://ih.yuntaijiaju.cn

[G02] 构造函数
来源：http://so.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://pu.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://nw.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://dj.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://da.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://pd.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hx.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://bq.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://lc.shxzskj.cn

[G03] 实例属性
来源：http://so.szxytkj.cn

Py:   self.name = "x"
来源：http://vt.shxzukj.cn

PHP:  public string $name = "x";
来源：http://vx.wgjwhj.cn

JS:   this.name = "x";
来源：http://nz.chemitech.net.cn

TS:   name: string = "x";
来源：http://le.haigaiapp.cn

Java: private String name;
来源：http://zn.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sp.shxzskj.cn

Ruby: @name = "x"
来源：http://nz.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ak.haigaiapp.cn

[G04] 定义方法
来源：http://dn.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://lp.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ey.colortex.cn

JS:   greet() { return this.name; }
来源：http://eu.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://jn.nszjky.cn

Java: String greet() { return name; }
来源：http://ey.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vs.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://bp.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://nw.wgjwhj.cn

[G05] 继承
来源：http://au.nicolike.cn

Py:   class Admin(User): pass
来源：http://bf.nicolike.cn

PHP:  class Admin extends User {}
来源：http://pq.hahajie.cn

JS:   class Admin extends User {}
来源：http://ds.colortex.cn

TS:   class Admin extends User {}
来源：http://io.hnjuh.cn

Java: class Admin extends User {}
来源：http://hi.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gu.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://bl.huixiangedu.cn

C#:   class Admin : User {}
来源：http://ng.colortex.cn

[G06] 重写方法
来源：http://pr.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://da.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ht.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://wx.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://sl.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://sy.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vt.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://qo.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://kx.bjjhwx.cn

[G07] 调用父类方法
来源：http://wy.yuntaijiaju.cn

Py:   super().greet()
来源：http://mz.shxzukj.cn

PHP:  parent::greet();
来源：http://zu.hnjuh.cn

JS:   super.greet();
来源：http://pi.shtwfgs.cn

TS:   super.greet();
来源：http://ec.yuexingan06.cn

Java: super.greet();
来源：http://im.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gs.huixinmuqiang.cn

Ruby: super
来源：http://yy.bookmarksfly.cn

C#:   base.Greet();
来源：http://ff.haigaiapp.cn

[G08] 静态方法与属性
来源：http://ca.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ia.yuexingan06.cn

PHP:  public static function f() {}
来源：http://rm.hahajie.cn

JS:   static f() {}
来源：http://pz.huanxung.cn

TS:   static f(): void {}
来源：http://ve.chemitech.net.cn

Java: static void f() {}
来源：http://sq.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://el.hnjuh.cn

Ruby: def self.f; end
来源：http://sj.huixiangedu.cn

C#:   public static void F() {}
来源：http://li.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://qn.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://rm.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cz.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jc.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://wp.nszjky.cn

Java: interface Shape { double area(); }
来源：http://pb.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://dg.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kb.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://rb.chemitech.net.cn

[G10] 访问控制
来源：http://ok.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ng.newstarts.cn

PHP:  public / protected / private
来源：http://qd.521024.cn

JS:   #private 字段；其余公开
来源：http://ar.haigaiapp.cn

TS:   public / protected / private
来源：http://zw.colortex.cn

Java: public / protected / private / 默认包级
来源：http://mj.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bb.shtwfgs.cn

Ruby: public / protected / private
来源：http://bp.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://hj.huixinmuqiang.cn

[G11] getter / setter
来源：http://da.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://ld.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mo.521024.cn

JS:   get name() { return this._name; }
来源：http://sr.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://ys.szxytkj.cn

Java: public String getName() { return name; }
来源：http://sf.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cn.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://vv.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://fh.muxihuayi.cn

[G12] 对象转字符串
来源：http://ni.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://yn.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dk.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://xz.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://ar.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://xo.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vk.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://im.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://eu.chemitech.net.cn

[G13] 判断对象类型
来源：http://mr.asd995.cn

Py:   isinstance(u, User)
来源：http://fu.shtwfgs.cn

PHP:  $u instanceof User
来源：http://dt.szsharing.cn

JS:   u instanceof User
来源：http://za.szxytkj.cn

TS:   u instanceof User
来源：http://mr.chemitech.net.cn

Java: u instanceof User
来源：http://wd.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kt.colortex.cn

Ruby: u.is_a?(User)
来源：http://fu.chemitech.net.cn

C#:   u is User
来源：http://tt.shtwfgs.cn

[G14] 数据类 / record
来源：http://yu.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ql.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://az.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://at.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://gf.hahajie.cn

Java: record User(String name, int age) {}
来源：http://bd.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://pc.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nu.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://lq.huixiangedu.cn

[G15] 枚举
来源：http://ns.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tq.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ip.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kf.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tj.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://vq.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dy.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://an.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ju.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://ui.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yu.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://qg.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://rh.9csxet.cn

TS:   Object.entries(obj)
来源：http://kf.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ef.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xm.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://dn.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://lb.huixiangedu.cn

================================================================================
来源：http://ii.yuexingan06.cn

H. 异常与错误处理
来源：http://te.bookmarksfly.cn

================================================================================
来源：http://vm.szsharing.cn

[H01] try / catch 基础
来源：http://yc.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lg.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vb.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gf.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ym.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lp.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uu.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yb.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://de.nszjky.cn

[H02] finally / ensure 收尾
来源：http://xk.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nm.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://td.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cf.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://im.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mv.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://px.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yv.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ni.nszjky.cn

[H03] 主动抛出异常
来源：http://li.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://yb.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://um.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://sn.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://pz.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xv.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://av.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ai.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lx.huixiangedu.cn

[H04] 自定义异常类型
来源：http://dp.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://yc.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jr.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://vv.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://jw.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://pr.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wu.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://ng.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://ot.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://cq.wgjwhj.cn

Py:   except ValueError as e:
来源：http://fq.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ma.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://rl.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://hh.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://lg.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://au.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://ld.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sw.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://gc.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://qr.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kc.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gm.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rd.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xp.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fz.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://oo.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://ih.nszjky.cn

[H07] 断言
来源：http://em.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://pn.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://jd.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://jt.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://rn.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://sl.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ld.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://py.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://qi.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://ct.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://js.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pb.9csxet.cn

JS:   e.message;  e.stack
来源：http://yc.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ud.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hi.muxihuayi.cn

Go:   err.Error()
来源：http://lo.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://zx.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://oa.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ci.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oh.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://he.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lx.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yb.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cm.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oa.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bd.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dx.asd995.cn

[H10] 资源自动释放
来源：http://op.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ox.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gc.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lq.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vo.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dh.chemitech.net.cn

Go:   defer f.Close()
来源：http://nv.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ci.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yr.szxytkj.cn

================================================================================
来源：http://tl.panjiajie.cn

I. 正则表达式
来源：http://zn.huixiangedu.cn

================================================================================
来源：http://qw.haigaiapp.cn

[I01] 判断是否匹配
来源：http://os.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://od.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oo.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://os.nicolike.cn

TS:   /\d+/.test(s)
来源：http://yj.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rk.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yw.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://uy.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vj.colortex.cn

[I02] 提取所有匹配
来源：http://tl.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://iy.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vy.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sy.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://gh.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wi.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dm.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://sw.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bi.huanxung.cn

[I03] 提取捕获分组
来源：http://br.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uk.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hc.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://er.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xd.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rc.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ww.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sl.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sj.huanxung.cn

[I04] 正则替换
来源：http://vj.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vg.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xy.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tz.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fw.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tk.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gj.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dh.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ld.shtwfgs.cn

[I05] 按正则拆分
来源：http://yj.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kw.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://de.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://rj.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://ew.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://cd.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://up.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qb.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lu.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nw.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fn.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kf.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nl.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yx.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://px.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://no.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://db.nicolike.cn


<!-- 参考信息 -->