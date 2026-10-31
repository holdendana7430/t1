代发 wailian999

================================================================================
来源：http://bp.panjiajie.cn

G. 面向对象
来源：http://ty.huanxung.cn

================================================================================
来源：http://yx.szsharing.cn

[G01] 定义类
来源：http://mo.chemitech.net.cn

Py:   class User: pass
来源：http://cj.szxytkj.cn

PHP:  class User {}
来源：http://yd.haigaiapp.cn

JS:   class User {}
来源：http://iz.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://sb.haigaiapp.cn

Java: class User {}
来源：http://pz.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://ag.shxzskj.cn

Ruby: class User; end
来源：http://gf.521024.cn

C#:   class User {}
来源：http://as.yuntaijiaju.cn

[G02] 构造函数
来源：http://wx.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://vf.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://ow.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://cp.colortex.cn

TS:   constructor(public name: string) {}
来源：http://xm.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://xk.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pb.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://qr.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://nb.9csxet.cn

[G03] 实例属性
来源：http://hi.colortex.cn

Py:   self.name = "x"
来源：http://wy.szsharing.cn

PHP:  public string $name = "x";
来源：http://uz.lnxyls.cn

JS:   this.name = "x";
来源：http://wo.wgjwhj.cn

TS:   name: string = "x";
来源：http://fh.hahajie.cn

Java: private String name;
来源：http://te.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dd.bookmarksfly.cn

Ruby: @name = "x"
来源：http://ap.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://ww.shxzskj.cn

[G04] 定义方法
来源：http://ia.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://at.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rd.521024.cn

JS:   greet() { return this.name; }
来源：http://mf.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://bo.colortex.cn

Java: String greet() { return name; }
来源：http://iz.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://um.lnxyls.cn

Ruby: def greet; @name; end
来源：http://pn.521024.cn

C#:   public string Greet() => Name;
来源：http://fr.lnxyls.cn

[G05] 继承
来源：http://kt.gzmigu.cn

Py:   class Admin(User): pass
来源：http://nk.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://ax.panjiajie.cn

JS:   class Admin extends User {}
来源：http://ze.newstarts.cn

TS:   class Admin extends User {}
来源：http://xw.jctech888.com.cn

Java: class Admin extends User {}
来源：http://bn.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://le.colortex.cn

Ruby: class Admin < User; end
来源：http://wi.nszjky.cn

C#:   class Admin : User {}
来源：http://em.muxihuayi.cn

[G06] 重写方法
来源：http://kv.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://oy.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://be.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://oe.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://kc.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://ni.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gl.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://km.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://ki.shxzskj.cn

[G07] 调用父类方法
来源：http://up.yuexingan06.cn

Py:   super().greet()
来源：http://cq.gzmigu.cn

PHP:  parent::greet();
来源：http://ld.huixinmuqiang.cn

JS:   super.greet();
来源：http://he.haigaiapp.cn

TS:   super.greet();
来源：http://py.wgjwhj.cn

Java: super.greet();
来源：http://rz.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ar.asd995.cn

Ruby: super
来源：http://pq.asd995.cn

C#:   base.Greet();
来源：http://bn.gzmigu.cn

[G08] 静态方法与属性
来源：http://jw.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hv.9csxet.cn

PHP:  public static function f() {}
来源：http://tc.hnjuh.cn

JS:   static f() {}
来源：http://vr.bookmarksfly.cn

TS:   static f(): void {}
来源：http://ja.yuexingan06.cn

Java: static void f() {}
来源：http://ov.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://if.wgjwhj.cn

Ruby: def self.f; end
来源：http://tw.9csxet.cn

C#:   public static void F() {}
来源：http://yw.hahajie.cn

[G09] 接口 / 抽象类
来源：http://uf.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://gf.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iv.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ef.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://kx.521024.cn

Java: interface Shape { double area(); }
来源：http://rv.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://en.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://od.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://vg.nszjky.cn

[G10] 访问控制
来源：http://zx.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://st.haigaiapp.cn

PHP:  public / protected / private
来源：http://bk.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ui.bookmarksfly.cn

TS:   public / protected / private
来源：http://oz.asd995.cn

Java: public / protected / private / 默认包级
来源：http://zh.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kc.bookmarksfly.cn

Ruby: public / protected / private
来源：http://es.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://yd.yuntaijiaju.cn

[G11] getter / setter
来源：http://gd.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://nr.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aq.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://if.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://gz.shxzskj.cn

Java: public String getName() { return name; }
来源：http://ls.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cs.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://qk.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://wy.wgjwhj.cn

[G12] 对象转字符串
来源：http://lh.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://by.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sh.newstarts.cn

JS:   toString() { return this.name; }
来源：http://lj.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://xm.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://tb.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://py.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://ji.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://as.colortex.cn

[G13] 判断对象类型
来源：http://qk.nszjky.cn

Py:   isinstance(u, User)
来源：http://sl.lnxyls.cn

PHP:  $u instanceof User
来源：http://sq.nicolike.cn

JS:   u instanceof User
来源：http://an.huanxung.cn

TS:   u instanceof User
来源：http://hc.newstarts.cn

Java: u instanceof User
来源：http://mk.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gi.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://il.9csxet.cn

C#:   u is User
来源：http://wo.huixiangedu.cn

[G14] 数据类 / record
来源：http://ak.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fi.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://fz.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cy.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://jf.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://kl.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://hb.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wu.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://cd.gzmigu.cn

[G15] 枚举
来源：http://pk.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cy.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ce.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zi.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qs.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://fo.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sd.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://kg.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bz.521024.cn

[G16] 对象转数组 / 字典
来源：http://sl.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fi.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://gb.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://pt.nszjky.cn

TS:   Object.entries(obj)
来源：http://hm.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vq.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wl.asd995.cn

Ruby: obj.instance_variables
来源：http://ks.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://ps.jctech888.com.cn

================================================================================
来源：http://vn.jctech888.com.cn

H. 异常与错误处理
来源：http://xx.asd995.cn

================================================================================
来源：http://oe.asd995.cn

[H01] try / catch 基础
来源：http://vy.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ha.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pb.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wa.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fq.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://si.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xc.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yn.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://em.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://hm.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://af.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wl.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mh.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nu.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hm.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vx.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ax.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rf.asd995.cn

[H03] 主动抛出异常
来源：http://pu.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://kv.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vz.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://uh.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ad.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tq.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sf.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xy.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gn.huixiangedu.cn

[H04] 自定义异常类型
来源：http://io.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://au.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rz.hahajie.cn

JS:   class MyError extends Error {}
来源：http://zy.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://kd.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://hb.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://io.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://vl.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://ee.jctech888.com.cn

[H05] 捕获特定类型
来源：http://wk.szsharing.cn

Py:   except ValueError as e:
来源：http://fx.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mm.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://te.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://cu.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://tm.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hd.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://qw.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://au.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://ky.szsharing.cn

Py:   value = d.get("k") or default
来源：http://go.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fg.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dm.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vr.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yp.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ji.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://wi.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://xi.szsharing.cn

[H07] 断言
来源：http://hy.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://zn.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://gc.colortex.cn

JS:   console.assert(x > 0);
来源：http://vc.asd995.cn

TS:   console.assert(x > 0);
来源：http://eg.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://wz.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jm.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jv.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://pu.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://yj.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://fk.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fq.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://zd.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://em.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qj.hahajie.cn

Go:   err.Error()
来源：http://qr.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://ef.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://um.szxytkj.cn

[H09] 带错误码的异常
来源：http://vn.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qg.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jm.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sr.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qc.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zq.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vf.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xw.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yx.gzmigu.cn

[H10] 资源自动释放
来源：http://ej.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dp.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ts.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tt.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tx.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ts.nszjky.cn

Go:   defer f.Close()
来源：http://nt.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ut.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lj.nszjky.cn

================================================================================
来源：http://vs.nicolike.cn

I. 正则表达式
来源：http://ip.panjiajie.cn

================================================================================
来源：http://lj.chemitech.net.cn

[I01] 判断是否匹配
来源：http://vs.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ph.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uh.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://gx.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://bj.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ye.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://si.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://zl.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fp.colortex.cn

[I02] 提取所有匹配
来源：http://el.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://vz.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://my.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lx.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://lk.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bj.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ws.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://sx.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hj.muxihuayi.cn

[I03] 提取捕获分组
来源：http://oe.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zv.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fd.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nm.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wk.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yd.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oi.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bv.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uw.jctech888.com.cn

[I04] 正则替换
来源：http://kl.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://af.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jm.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sc.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mq.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pf.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xd.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bw.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ya.newstarts.cn

[I05] 按正则拆分
来源：http://tv.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ob.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vy.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://bk.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://gt.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://wu.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pz.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gm.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mv.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eq.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qk.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tk.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pu.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rk.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zq.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vo.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ch.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ri.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://mg.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yg.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cp.newstarts.cn


<!-- 参考信息 -->