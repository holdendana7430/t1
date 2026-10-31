代发 wailian999

================================================================================
来源：http://yk.shxzskj.cn

G. 面向对象
来源：http://sq.huixiangedu.cn

================================================================================
来源：http://kz.haigaiapp.cn

[G01] 定义类
来源：http://fy.bookmarksfly.cn

Py:   class User: pass
来源：http://km.szsharing.cn

PHP:  class User {}
来源：http://ay.huanxung.cn

JS:   class User {}
来源：http://fv.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ss.nszjky.cn

Java: class User {}
来源：http://qx.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://zs.shxzukj.cn

Ruby: class User; end
来源：http://mm.szxytkj.cn

C#:   class User {}
来源：http://hn.huanxung.cn

[G02] 构造函数
来源：http://pa.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://jx.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://vk.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ul.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://ms.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://el.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wl.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://gx.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://vc.muxihuayi.cn

[G03] 实例属性
来源：http://yu.bookmarksfly.cn

Py:   self.name = "x"
来源：http://qd.huanxung.cn

PHP:  public string $name = "x";
来源：http://fl.huanxung.cn

JS:   this.name = "x";
来源：http://sp.muxihuayi.cn

TS:   name: string = "x";
来源：http://qk.huanxung.cn

Java: private String name;
来源：http://wa.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ib.muxihuayi.cn

Ruby: @name = "x"
来源：http://qk.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://xb.hahajie.cn

[G04] 定义方法
来源：http://zt.hahajie.cn

Py:   def greet(self): return self.name
来源：http://qo.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cs.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://xn.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://rp.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://ql.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ed.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://ld.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://oh.huanxung.cn

[G05] 继承
来源：http://ye.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://dt.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://at.gzmigu.cn

JS:   class Admin extends User {}
来源：http://of.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://sa.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://nt.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pd.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://pj.hahajie.cn

C#:   class Admin : User {}
来源：http://ji.huanxung.cn

[G06] 重写方法
来源：http://cu.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://hn.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fi.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://vj.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://qc.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://wz.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vy.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://jr.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://os.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://hg.521024.cn

Py:   super().greet()
来源：http://au.asd995.cn

PHP:  parent::greet();
来源：http://wy.nicolike.cn

JS:   super.greet();
来源：http://pb.shxzukj.cn

TS:   super.greet();
来源：http://kn.shxzskj.cn

Java: super.greet();
来源：http://ut.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vr.shtwfgs.cn

Ruby: super
来源：http://tq.hnjuh.cn

C#:   base.Greet();
来源：http://sw.521024.cn

[G08] 静态方法与属性
来源：http://kn.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dn.yuexingan06.cn

PHP:  public static function f() {}
来源：http://eo.jianghongdianzi.cn

JS:   static f() {}
来源：http://yt.newstarts.cn

TS:   static f(): void {}
来源：http://kb.newstarts.cn

Java: static void f() {}
来源：http://nf.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://am.jctech888.com.cn

Ruby: def self.f; end
来源：http://tf.asd995.cn

C#:   public static void F() {}
来源：http://mi.colortex.cn

[G09] 接口 / 抽象类
来源：http://ic.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://gz.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lj.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hf.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://uo.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://yn.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://se.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cz.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://mn.nszjky.cn

[G10] 访问控制
来源：http://on.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://ee.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://re.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://cp.colortex.cn

TS:   public / protected / private
来源：http://qb.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://zv.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nv.szxytkj.cn

Ruby: public / protected / private
来源：http://xq.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://zd.chemitech.net.cn

[G11] getter / setter
来源：http://ng.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://yo.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yg.colortex.cn

JS:   get name() { return this._name; }
来源：http://ly.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://wi.9csxet.cn

Java: public String getName() { return name; }
来源：http://lh.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ji.huanxung.cn

Ruby: attr_accessor :name
来源：http://am.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://im.newstarts.cn

[G12] 对象转字符串
来源：http://az.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://yw.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://us.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://nh.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://gy.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://jo.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://de.newstarts.cn

Ruby: def to_s; @name; end
来源：http://no.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://uh.huixiangedu.cn

[G13] 判断对象类型
来源：http://ao.9csxet.cn

Py:   isinstance(u, User)
来源：http://hj.jctech888.com.cn

PHP:  $u instanceof User
来源：http://zo.szsharing.cn

JS:   u instanceof User
来源：http://mc.huixiangedu.cn

TS:   u instanceof User
来源：http://fn.shtwfgs.cn

Java: u instanceof User
来源：http://dr.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tj.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://jq.nszjky.cn

C#:   u is User
来源：http://pb.shxzukj.cn

[G14] 数据类 / record
来源：http://um.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pz.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://zk.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qa.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://db.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://tq.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://ld.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://up.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://nn.jctech888.com.cn

[G15] 枚举
来源：http://ze.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hj.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jo.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kn.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://el.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://qz.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lz.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://uw.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xj.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://ph.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uo.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://rj.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://sn.9csxet.cn

TS:   Object.entries(obj)
来源：http://aq.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wp.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://te.521024.cn

Ruby: obj.instance_variables
来源：http://kv.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://qu.bjjhwx.cn

================================================================================
来源：http://uy.colortex.cn

H. 异常与错误处理
来源：http://ap.haigaiapp.cn

================================================================================
来源：http://ae.muxihuayi.cn

[H01] try / catch 基础
来源：http://da.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qx.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uo.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://je.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ju.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wa.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ad.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pf.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mc.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://yg.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ld.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ub.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wh.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://of.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ld.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rv.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gr.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jo.521024.cn

[H03] 主动抛出异常
来源：http://ck.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://cw.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fa.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://ej.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://rp.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ru.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ti.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nr.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ex.chemitech.net.cn

[H04] 自定义异常类型
来源：http://uc.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://yh.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xy.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://vu.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://rc.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://yd.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ss.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://ai.huanxung.cn

C#:   class MyException : Exception {}
来源：http://dg.newstarts.cn

[H05] 捕获特定类型
来源：http://wi.szxytkj.cn

Py:   except ValueError as e:
来源：http://sj.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dc.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://ub.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://dx.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://dk.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yx.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://bd.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qj.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://sc.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://rh.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xe.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hj.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zt.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pt.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hb.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://ja.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://kh.jctech888.com.cn

[H07] 断言
来源：http://de.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://ic.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://rp.asd995.cn

JS:   console.assert(x > 0);
来源：http://sk.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://hv.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://gl.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sh.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gx.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://lj.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://wk.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://mu.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://io.shxzskj.cn

JS:   e.message;  e.stack
来源：http://qp.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fm.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tu.9csxet.cn

Go:   err.Error()
来源：http://sg.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://ga.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://pe.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://lo.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ty.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ua.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jr.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tn.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gx.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://av.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wd.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vp.wgjwhj.cn

[H10] 资源自动释放
来源：http://ne.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dm.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ih.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rw.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yf.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ca.wgjwhj.cn

Go:   defer f.Close()
来源：http://bg.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ns.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ay.jctech888.com.cn

================================================================================
来源：http://cz.huixiangedu.cn

I. 正则表达式
来源：http://an.shxzskj.cn

================================================================================
来源：http://ks.9csxet.cn

[I01] 判断是否匹配
来源：http://ey.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vd.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yf.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://dl.nszjky.cn

TS:   /\d+/.test(s)
来源：http://nu.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wy.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://su.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://vd.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nf.huixiangedu.cn

[I02] 提取所有匹配
来源：http://qx.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://jd.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jf.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fg.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://ip.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kq.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pl.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://vn.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ho.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ee.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bo.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fr.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pr.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xh.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kw.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kl.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bv.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iq.hahajie.cn

[I04] 正则替换
来源：http://ex.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fq.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kn.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fe.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dv.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eq.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ds.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yh.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oh.jctech888.com.cn

[I05] 按正则拆分
来源：http://mo.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oe.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zl.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://eg.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://bj.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://jt.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://is.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sa.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qx.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yd.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dw.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rc.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vg.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eb.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://to.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lm.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ir.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cn.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://zp.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sw.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dz.jctech888.com.cn


<!-- 参考信息 -->