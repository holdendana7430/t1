代发 wailian999

TS:   constructor(public name: string) {}
来源：http://ii.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://da.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://da.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://ju.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://yk.hnjuh.cn

[G03] 实例属性
来源：http://og.chemitech.net.cn

Py:   self.name = "x"
来源：http://yd.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://eb.nszjky.cn

JS:   this.name = "x";
来源：http://ym.shtwfgs.cn

TS:   name: string = "x";
来源：http://vm.panjiajie.cn

Java: private String name;
来源：http://iq.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://is.colortex.cn

Ruby: @name = "x"
来源：http://hm.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://js.haigaiapp.cn

[G04] 定义方法
来源：http://ox.asd995.cn

Py:   def greet(self): return self.name
来源：http://uu.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fr.huanxung.cn

JS:   greet() { return this.name; }
来源：http://xw.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://uv.yuexingan06.cn

Java: String greet() { return name; }
来源：http://vi.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xu.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://gc.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://sk.muxihuayi.cn

[G05] 继承
来源：http://qw.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://jr.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://bv.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://mn.shxzukj.cn

TS:   class Admin extends User {}
来源：http://qd.haigaiapp.cn

Java: class Admin extends User {}
来源：http://ub.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dg.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://qi.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://ys.huanxung.cn

[G06] 重写方法
来源：http://ky.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://dq.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xn.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://jf.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://yx.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://sl.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://va.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://ax.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://ns.asd995.cn

[G07] 调用父类方法
来源：http://mj.muxihuayi.cn

Py:   super().greet()
来源：http://wl.yuexingan06.cn

PHP:  parent::greet();
来源：http://og.muxihuayi.cn

JS:   super.greet();
来源：http://ae.bjjhwx.cn

TS:   super.greet();
来源：http://tx.muxihuayi.cn

Java: super.greet();
来源：http://gu.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yd.jctech888.com.cn

Ruby: super
来源：http://bf.wgjwhj.cn

C#:   base.Greet();
来源：http://dp.shxzukj.cn

[G08] 静态方法与属性
来源：http://fz.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kf.lnxyls.cn

PHP:  public static function f() {}
来源：http://cn.hnjuh.cn

JS:   static f() {}
来源：http://bd.9csxet.cn

TS:   static f(): void {}
来源：http://sa.panjiajie.cn

Java: static void f() {}
来源：http://dg.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aa.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://xh.bjjhwx.cn

C#:   public static void F() {}
来源：http://yc.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://dj.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://rb.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ta.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bm.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://hp.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://ac.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://mr.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://el.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://zk.chemitech.net.cn

[G10] 访问控制
来源：http://zb.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://pn.nszjky.cn

PHP:  public / protected / private
来源：http://sk.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://hi.szsharing.cn

TS:   public / protected / private
来源：http://vr.521024.cn

Java: public / protected / private / 默认包级
来源：http://vs.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vk.chemitech.net.cn

Ruby: public / protected / private
来源：http://eu.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://ez.panjiajie.cn

[G11] getter / setter
来源：http://ak.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://fa.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bg.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://ko.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://qg.shxzskj.cn

Java: public String getName() { return name; }
来源：http://wk.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://my.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://dh.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://vs.wgjwhj.cn

[G12] 对象转字符串
来源：http://sf.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://sa.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gh.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://iy.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://qa.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://hr.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lw.nszjky.cn

Ruby: def to_s; @name; end
来源：http://gs.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://gd.panjiajie.cn

[G13] 判断对象类型
来源：http://jt.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://cl.nicolike.cn

PHP:  $u instanceof User
来源：http://hc.chemitech.net.cn

JS:   u instanceof User
来源：http://at.hahajie.cn

TS:   u instanceof User
来源：http://lb.chemitech.net.cn

Java: u instanceof User
来源：http://xb.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ha.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://ir.jctech888.com.cn

C#:   u is User
来源：http://tn.colortex.cn

[G14] 数据类 / record
来源：http://pj.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://of.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://zz.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://od.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://bi.newstarts.cn

Java: record User(String name, int age) {}
来源：http://gh.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://pp.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vj.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://ed.jctech888.com.cn

[G15] 枚举
来源：http://ud.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fb.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yv.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sw.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cb.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://ti.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zb.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://xt.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://og.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://fi.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://er.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://al.huanxung.cn

JS:   Object.entries(obj)
来源：http://vv.hnjuh.cn

TS:   Object.entries(obj)
来源：http://uw.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cn.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bo.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://yb.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://ni.shxzukj.cn

================================================================================
来源：http://yf.gzmigu.cn

H. 异常与错误处理
来源：http://sh.yuntaijiaju.cn

================================================================================
来源：http://fu.szxytkj.cn

[H01] try / catch 基础
来源：http://xs.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wr.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ro.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pi.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xs.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pd.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cv.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nb.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rr.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://ij.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qv.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lr.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qf.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iu.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dp.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fc.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yl.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pw.shxzskj.cn

[H03] 主动抛出异常
来源：http://mn.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://ph.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rc.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://rk.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://vj.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nc.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oo.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sp.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pc.hahajie.cn

[H04] 自定义异常类型
来源：http://vp.asd995.cn

Py:   class MyError(Exception): pass
来源：http://to.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jp.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://tb.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://is.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://xj.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mp.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://re.hahajie.cn

C#:   class MyException : Exception {}
来源：http://dc.panjiajie.cn

[H05] 捕获特定类型
来源：http://od.9csxet.cn

Py:   except ValueError as e:
来源：http://sj.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fo.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://ka.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://at.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://rx.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ta.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://nk.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xw.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://su.asd995.cn

Py:   value = d.get("k") or default
来源：http://uj.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sb.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dd.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ee.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ud.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ot.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://xk.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://xa.shxzukj.cn

[H07] 断言
来源：http://dx.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://at.521024.cn

PHP:  assert($x > 0);
来源：http://mg.newstarts.cn

JS:   console.assert(x > 0);
来源：http://kq.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://sd.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://gu.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jm.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wm.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://if.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://zq.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://ib.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rb.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://rn.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jf.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mb.yuntaijiaju.cn

Go:   err.Error()
来源：http://xl.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://hx.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://pv.yuexingan06.cn

[H09] 带错误码的异常
来源：http://mq.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oz.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://os.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yk.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qq.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gu.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://by.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nz.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wx.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://ru.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bb.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://il.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uc.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mo.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://es.shtwfgs.cn

Go:   defer f.Close()
来源：http://ba.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tn.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pk.colortex.cn

================================================================================
来源：http://yy.bookmarksfly.cn

I. 正则表达式
来源：http://pe.jctech888.com.cn

================================================================================
来源：http://ai.szsharing.cn

[I01] 判断是否匹配
来源：http://pu.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kk.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hh.huanxung.cn

JS:   /\d+/.test(s)
来源：http://ce.huanxung.cn

TS:   /\d+/.test(s)
来源：http://ag.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xw.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pa.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://at.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://as.nicolike.cn

[I02] 提取所有匹配
来源：http://cr.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://op.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://in.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qt.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://fu.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nd.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sa.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://lb.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rt.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://qg.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pm.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zw.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dg.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yt.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ld.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hy.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rj.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ql.shxzukj.cn

[I04] 正则替换
来源：http://px.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zp.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qq.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qm.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ni.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zq.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://te.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hp.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gj.asd995.cn

[I05] 按正则拆分
来源：http://xy.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vw.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://of.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://qz.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://bz.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://yy.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ff.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ys.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ai.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://le.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mm.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bo.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tt.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tj.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rx.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ck.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xw.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kd.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://ui.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kj.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bh.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tq.bookmarksfly.cn

TS:   /error/gim
来源：http://af.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xl.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sd.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://af.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lz.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://lv.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ol.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wy.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ft.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fu.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xb.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sw.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://es.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oi.hnjuh.cn

================================================================================
来源：http://lx.521024.cn


<!-- 参考信息 -->