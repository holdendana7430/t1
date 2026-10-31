代发 wailian999

================================================================================
来源：http://ef.bjjhwx.cn

G. 面向对象
来源：http://qb.yuexingan06.cn

================================================================================
来源：http://ru.bookmarksfly.cn

[G01] 定义类
来源：http://kc.yuexingan06.cn

Py:   class User: pass
来源：http://rk.jctech888.com.cn

PHP:  class User {}
来源：http://eg.huixiangedu.cn

JS:   class User {}
来源：http://zx.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://tn.9csxet.cn

Java: class User {}
来源：http://tr.gzmigu.cn

Go:   type User struct { Name string }
来源：http://gy.chemitech.net.cn

Ruby: class User; end
来源：http://de.bookmarksfly.cn

C#:   class User {}
来源：http://jg.nszjky.cn

[G02] 构造函数
来源：http://qh.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://bz.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://db.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://ae.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://ix.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://ze.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qp.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://jd.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://dw.szxytkj.cn

[G03] 实例属性
来源：http://kc.wgjwhj.cn

Py:   self.name = "x"
来源：http://fd.huanxung.cn

PHP:  public string $name = "x";
来源：http://cv.colortex.cn

JS:   this.name = "x";
来源：http://ne.nszjky.cn

TS:   name: string = "x";
来源：http://el.lnxyls.cn

Java: private String name;
来源：http://yg.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wd.haigaiapp.cn

Ruby: @name = "x"
来源：http://np.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://sv.wgjwhj.cn

[G04] 定义方法
来源：http://uk.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://jn.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kd.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://eh.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://dt.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://vz.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ln.szsharing.cn

Ruby: def greet; @name; end
来源：http://sy.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://yo.521024.cn

[G05] 继承
来源：http://ju.szsharing.cn

Py:   class Admin(User): pass
来源：http://fs.newstarts.cn

PHP:  class Admin extends User {}
来源：http://xt.lnxyls.cn

JS:   class Admin extends User {}
来源：http://ry.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://we.huixiangedu.cn

Java: class Admin extends User {}
来源：http://wt.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iu.newstarts.cn

Ruby: class Admin < User; end
来源：http://og.szsharing.cn

C#:   class Admin : User {}
来源：http://pz.shxzukj.cn

[G06] 重写方法
来源：http://vd.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://yy.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ct.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://ns.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://av.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://zf.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vt.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://gc.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://ll.jctech888.com.cn

[G07] 调用父类方法
来源：http://ob.haigaiapp.cn

Py:   super().greet()
来源：http://yj.jctech888.com.cn

PHP:  parent::greet();
来源：http://kb.panjiajie.cn

JS:   super.greet();
来源：http://sz.gzmigu.cn

TS:   super.greet();
来源：http://zf.nszjky.cn

Java: super.greet();
来源：http://ty.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jf.shtwfgs.cn

Ruby: super
来源：http://nn.yuntaijiaju.cn

C#:   base.Greet();
来源：http://lb.bjjhwx.cn

[G08] 静态方法与属性
来源：http://qa.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oe.shxzskj.cn

PHP:  public static function f() {}
来源：http://fe.chemitech.net.cn

JS:   static f() {}
来源：http://kc.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://nw.hnjuh.cn

Java: static void f() {}
来源：http://jf.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://on.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://mb.shxzukj.cn

C#:   public static void F() {}
来源：http://fr.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://ab.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://js.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ca.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hc.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://dc.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://zo.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://pf.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://og.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://hn.shxzukj.cn

[G10] 访问控制
来源：http://gu.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ym.521024.cn

PHP:  public / protected / private
来源：http://yh.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://mc.shxzskj.cn

TS:   public / protected / private
来源：http://uq.521024.cn

Java: public / protected / private / 默认包级
来源：http://ri.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bq.gzmigu.cn

Ruby: public / protected / private
来源：http://bt.nszjky.cn

C#:   public / protected / private / internal
来源：http://fp.shxzukj.cn

[G11] getter / setter
来源：http://hl.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://ii.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zr.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://ka.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://lg.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://qn.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gm.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://vo.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://ba.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://rb.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://oj.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rj.huanxung.cn

JS:   toString() { return this.name; }
来源：http://fm.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://mv.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://xq.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kv.hahajie.cn

Ruby: def to_s; @name; end
来源：http://nf.colortex.cn

C#:   public override string ToString() => Name;
来源：http://aj.jctech888.com.cn

[G13] 判断对象类型
来源：http://vh.asd995.cn

Py:   isinstance(u, User)
来源：http://ps.huixiangedu.cn

PHP:  $u instanceof User
来源：http://kz.bookmarksfly.cn

JS:   u instanceof User
来源：http://ky.szsharing.cn

TS:   u instanceof User
来源：http://df.asd995.cn

Java: u instanceof User
来源：http://bs.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wq.521024.cn

Ruby: u.is_a?(User)
来源：http://no.bjjhwx.cn

C#:   u is User
来源：http://qg.shtwfgs.cn

[G14] 数据类 / record
来源：http://tn.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tj.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://rn.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lb.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://rq.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://xf.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://qq.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vx.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://vo.haigaiapp.cn

[G15] 枚举
来源：http://nh.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bo.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://me.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://or.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://le.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://xy.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://al.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://hu.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://po.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://gg.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bi.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://rh.hahajie.cn

JS:   Object.entries(obj)
来源：http://pt.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://zt.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jf.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nv.nicolike.cn

Ruby: obj.instance_variables
来源：http://ql.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://nc.huanxung.cn

================================================================================
来源：http://hs.muxihuayi.cn

H. 异常与错误处理
来源：http://di.yuntaijiaju.cn

================================================================================
来源：http://tb.haigaiapp.cn

[H01] try / catch 基础
来源：http://du.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cm.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rg.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uh.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fs.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tj.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bu.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ly.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kb.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://rw.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wv.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bl.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yq.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gq.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jy.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mc.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sv.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xt.nicolike.cn

[H03] 主动抛出异常
来源：http://ia.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://bf.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qu.colortex.cn

JS:   throw new Error("错误信息");
来源：http://gw.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://zi.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xz.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wz.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cx.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xn.hahajie.cn

[H04] 自定义异常类型
来源：http://jf.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://ac.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sy.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://al.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://mj.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://js.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pz.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://ha.colortex.cn

C#:   class MyException : Exception {}
来源：http://dj.hahajie.cn

[H05] 捕获特定类型
来源：http://hv.szsharing.cn

Py:   except ValueError as e:
来源：http://zr.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yg.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://yk.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://lq.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://zv.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hu.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://ou.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dp.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://oo.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://ab.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wd.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xs.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nv.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fz.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ce.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://ul.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://uh.yuexingan06.cn

[H07] 断言
来源：http://wt.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://wx.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://xx.colortex.cn

JS:   console.assert(x > 0);
来源：http://tt.szsharing.cn

TS:   console.assert(x > 0);
来源：http://gp.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://nt.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gv.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wa.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://ty.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://bn.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://nr.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vj.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://yj.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jx.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hq.hahajie.cn

Go:   err.Error()
来源：http://xn.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://vs.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://bo.huanxung.cn

[H09] 带错误码的异常
来源：http://px.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fs.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cn.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jn.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ei.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ac.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sz.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xj.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hw.jctech888.com.cn

[H10] 资源自动释放
来源：http://ic.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jc.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xm.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://da.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tx.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ko.bjjhwx.cn

Go:   defer f.Close()
来源：http://po.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sm.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yg.haigaiapp.cn

================================================================================
来源：http://am.chemitech.net.cn

I. 正则表达式
来源：http://on.shxzskj.cn

================================================================================
来源：http://kn.newstarts.cn

[I01] 判断是否匹配
来源：http://lm.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yi.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oj.szsharing.cn

JS:   /\d+/.test(s)
来源：http://xc.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://ol.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://su.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oh.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://mr.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lx.asd995.cn

[I02] 提取所有匹配
来源：http://el.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://br.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gs.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yu.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://dg.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ea.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xu.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://bs.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wz.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://us.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://it.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://th.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rq.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ut.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ms.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xw.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tt.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mt.hnjuh.cn

[I04] 正则替换
来源：http://bq.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://me.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mk.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://va.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sa.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jd.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wq.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xp.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bd.hahajie.cn

[I05] 按正则拆分
来源：http://rb.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vj.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bb.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://gz.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rz.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://zv.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://az.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dm.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lt.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bn.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lw.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xp.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gx.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cs.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gp.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tn.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tw.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wk.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://in.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sn.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vt.bjjhwx.cn


<!-- 参考信息 -->