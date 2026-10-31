代发 wailian999

Py:   class User: pass
来源：http://ss.huixiangedu.cn

PHP:  class User {}
来源：http://nn.lnxyls.cn

JS:   class User {}
来源：http://wk.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://vx.bookmarksfly.cn

Java: class User {}
来源：http://kz.szsharing.cn

Go:   type User struct { Name string }
来源：http://fa.szsharing.cn

Ruby: class User; end
来源：http://es.colortex.cn

C#:   class User {}
来源：http://ay.jianghongdianzi.cn

[G02] 构造函数
来源：http://qm.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://ri.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://pp.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://mw.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://mq.521024.cn

Java: User(String name) { this.name = name; }
来源：http://nz.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://em.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://yx.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://dr.jctech888.com.cn

[G03] 实例属性
来源：http://sw.gzmigu.cn

Py:   self.name = "x"
来源：http://dy.hnjuh.cn

PHP:  public string $name = "x";
来源：http://ec.shxzskj.cn

JS:   this.name = "x";
来源：http://dj.shxzskj.cn

TS:   name: string = "x";
来源：http://nz.9csxet.cn

Java: private String name;
来源：http://yk.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pe.huixiangedu.cn

Ruby: @name = "x"
来源：http://fw.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://os.wgjwhj.cn

[G04] 定义方法
来源：http://id.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://vt.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hg.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://ql.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://au.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://bp.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bj.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://dz.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://jl.szxytkj.cn

[G05] 继承
来源：http://gf.9csxet.cn

Py:   class Admin(User): pass
来源：http://lv.9csxet.cn

PHP:  class Admin extends User {}
来源：http://pk.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://li.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://zl.newstarts.cn

Java: class Admin extends User {}
来源：http://zj.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ll.asd995.cn

Ruby: class Admin < User; end
来源：http://zg.shtwfgs.cn

C#:   class Admin : User {}
来源：http://cc.yuntaijiaju.cn

[G06] 重写方法
来源：http://hf.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://ir.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jf.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://uh.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://is.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://uc.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oi.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://uy.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://fo.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://ir.gzmigu.cn

Py:   super().greet()
来源：http://tn.szsharing.cn

PHP:  parent::greet();
来源：http://ie.huixiangedu.cn

JS:   super.greet();
来源：http://rc.bjjhwx.cn

TS:   super.greet();
来源：http://go.lnxyls.cn

Java: super.greet();
来源：http://lz.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ye.bookmarksfly.cn

Ruby: super
来源：http://wz.nszjky.cn

C#:   base.Greet();
来源：http://aw.gzmigu.cn

[G08] 静态方法与属性
来源：http://jk.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ne.muxihuayi.cn

PHP:  public static function f() {}
来源：http://qx.shxzukj.cn

JS:   static f() {}
来源：http://rw.bookmarksfly.cn

TS:   static f(): void {}
来源：http://cm.nicolike.cn

Java: static void f() {}
来源：http://tu.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wp.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://rw.asd995.cn

C#:   public static void F() {}
来源：http://xg.9csxet.cn

[G09] 接口 / 抽象类
来源：http://ci.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://pd.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zd.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jn.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://cw.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://mj.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://nu.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://na.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://af.9csxet.cn

[G10] 访问控制
来源：http://zl.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://da.yuexingan06.cn

PHP:  public / protected / private
来源：http://qu.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://xp.colortex.cn

TS:   public / protected / private
来源：http://vh.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://fy.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ga.yuexingan06.cn

Ruby: public / protected / private
来源：http://xr.asd995.cn

C#:   public / protected / private / internal
来源：http://bg.panjiajie.cn

[G11] getter / setter
来源：http://wr.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://qh.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mt.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://zp.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://kp.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://dk.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oj.shxzukj.cn

Ruby: attr_accessor :name
来源：http://zn.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ys.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://qk.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://qq.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://iq.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://fd.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://qt.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://vy.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://th.szsharing.cn

Ruby: def to_s; @name; end
来源：http://hm.colortex.cn

C#:   public override string ToString() => Name;
来源：http://fc.bjjhwx.cn

[G13] 判断对象类型
来源：http://uw.lnxyls.cn

Py:   isinstance(u, User)
来源：http://hj.shtwfgs.cn

PHP:  $u instanceof User
来源：http://bh.shxzukj.cn

JS:   u instanceof User
来源：http://sp.yuntaijiaju.cn

TS:   u instanceof User
来源：http://hx.yuexingan06.cn

Java: u instanceof User
来源：http://gp.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://us.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://lj.yuexingan06.cn

C#:   u is User
来源：http://vs.bookmarksfly.cn

[G14] 数据类 / record
来源：http://tt.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ql.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://no.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gu.521024.cn

TS:   type User = { name: string; age: number };
来源：http://on.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://qs.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://oi.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xf.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://ox.asd995.cn

[G15] 枚举
来源：http://oe.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ao.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oo.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ys.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lq.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://dt.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iv.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://bv.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sk.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://hk.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cs.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://fn.nicolike.cn

JS:   Object.entries(obj)
来源：http://jf.lnxyls.cn

TS:   Object.entries(obj)
来源：http://zb.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wa.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jk.shxzukj.cn

Ruby: obj.instance_variables
来源：http://vm.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://tm.lnxyls.cn

================================================================================
来源：http://jq.huixiangedu.cn

H. 异常与错误处理
来源：http://fm.hnjuh.cn

================================================================================
来源：http://hx.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://qh.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ob.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nf.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ft.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cq.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xj.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yd.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ov.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ad.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://nh.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ud.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tu.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wd.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xu.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cr.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vq.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wh.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://va.shxzskj.cn

[H03] 主动抛出异常
来源：http://vn.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://xx.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xn.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://tr.asd995.cn

TS:   throw new Error("错误信息");
来源：http://ko.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ve.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://df.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ym.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://at.hnjuh.cn

[H04] 自定义异常类型
来源：http://ru.521024.cn

Py:   class MyError(Exception): pass
来源：http://sm.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://km.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://ea.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://vu.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://xx.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cy.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://cq.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://zt.asd995.cn

[H05] 捕获特定类型
来源：http://oi.jctech888.com.cn

Py:   except ValueError as e:
来源：http://mm.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vn.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://yo.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://ib.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://hg.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lf.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://js.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ib.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://yk.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://ae.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fm.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nm.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vp.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://za.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fx.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://if.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://wq.haigaiapp.cn

[H07] 断言
来源：http://vy.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://dp.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://re.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://wi.newstarts.cn

TS:   console.assert(x > 0);
来源：http://mm.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://ta.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://me.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pn.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://io.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ro.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://lp.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sz.szsharing.cn

JS:   e.message;  e.stack
来源：http://nf.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lx.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qf.yuexingan06.cn

Go:   err.Error()
来源：http://jk.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://ac.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://mq.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ga.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yp.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xv.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vb.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pu.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kg.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sv.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ur.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://px.asd995.cn

[H10] 资源自动释放
来源：http://cd.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nk.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zc.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ww.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jn.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nc.haigaiapp.cn

Go:   defer f.Close()
来源：http://ef.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xu.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vp.9csxet.cn

================================================================================
来源：http://dy.bookmarksfly.cn

I. 正则表达式
来源：http://eu.lnxyls.cn

================================================================================
来源：http://cr.hahajie.cn

[I01] 判断是否匹配
来源：http://ex.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vu.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eg.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://vg.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://cn.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rh.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xd.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://kd.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pl.bjjhwx.cn

[I02] 提取所有匹配
来源：http://ap.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://fx.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ta.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kg.colortex.cn

TS:   s.match(/\d+/g)
来源：http://on.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sj.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cm.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://mp.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jq.chemitech.net.cn

[I03] 提取捕获分组
来源：http://qz.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://en.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qf.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zo.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gx.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ss.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vz.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oi.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ed.colortex.cn

[I04] 正则替换
来源：http://tn.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wl.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fd.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rh.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xy.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vm.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ae.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://re.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://an.nszjky.cn

[I05] 按正则拆分
来源：http://vs.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rs.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://od.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ru.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://kx.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://sx.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ja.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rc.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cm.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cp.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zg.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oq.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ih.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wx.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gh.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fy.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vc.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ey.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://hz.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://df.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cc.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://px.szsharing.cn

TS:   /error/gim
来源：http://qs.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uw.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zz.huixiangedu.cn


<!-- 参考信息 -->