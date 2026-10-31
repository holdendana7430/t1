代发 wailian999

Java: class User {}
来源：http://xy.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://qr.yuexingan06.cn

Ruby: class User; end
来源：http://ud.bookmarksfly.cn

C#:   class User {}
来源：http://xu.nszjky.cn

[G02] 构造函数
来源：http://ch.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://dt.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://xg.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://zm.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://gv.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://ra.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://by.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://ua.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://tc.bjjhwx.cn

[G03] 实例属性
来源：http://oe.hnjuh.cn

Py:   self.name = "x"
来源：http://xd.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://wz.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://qn.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://me.nszjky.cn

Java: private String name;
来源：http://jc.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uk.hahajie.cn

Ruby: @name = "x"
来源：http://cv.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://jc.jctech888.com.cn

[G04] 定义方法
来源：http://jy.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://cl.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ao.hahajie.cn

JS:   greet() { return this.name; }
来源：http://pg.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://ag.muxihuayi.cn

Java: String greet() { return name; }
来源：http://gd.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ne.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://ee.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://vx.szxytkj.cn

[G05] 继承
来源：http://um.hnjuh.cn

Py:   class Admin(User): pass
来源：http://ep.nicolike.cn

PHP:  class Admin extends User {}
来源：http://ri.gzmigu.cn

JS:   class Admin extends User {}
来源：http://hb.szsharing.cn

TS:   class Admin extends User {}
来源：http://mg.jctech888.com.cn

Java: class Admin extends User {}
来源：http://ww.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ec.9csxet.cn

Ruby: class Admin < User; end
来源：http://kr.yuexingan06.cn

C#:   class Admin : User {}
来源：http://ul.hnjuh.cn

[G06] 重写方法
来源：http://ef.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://me.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dg.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://gm.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://kj.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://jb.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sa.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://ap.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://qr.jctech888.com.cn

[G07] 调用父类方法
来源：http://qx.shxzskj.cn

Py:   super().greet()
来源：http://tb.shtwfgs.cn

PHP:  parent::greet();
来源：http://lj.asd995.cn

JS:   super.greet();
来源：http://sy.521024.cn

TS:   super.greet();
来源：http://ex.chemitech.net.cn

Java: super.greet();
来源：http://ym.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uc.huixinmuqiang.cn

Ruby: super
来源：http://fj.9csxet.cn

C#:   base.Greet();
来源：http://df.muxihuayi.cn

[G08] 静态方法与属性
来源：http://rk.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hx.9csxet.cn

PHP:  public static function f() {}
来源：http://to.wgjwhj.cn

JS:   static f() {}
来源：http://ci.newstarts.cn

TS:   static f(): void {}
来源：http://rb.9csxet.cn

Java: static void f() {}
来源：http://wg.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qm.chemitech.net.cn

Ruby: def self.f; end
来源：http://ro.panjiajie.cn

C#:   public static void F() {}
来源：http://rz.colortex.cn

[G09] 接口 / 抽象类
来源：http://sb.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://qo.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mg.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fy.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://bl.nszjky.cn

Java: interface Shape { double area(); }
来源：http://ad.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://dr.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xk.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://is.huanxung.cn

[G10] 访问控制
来源：http://jw.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://fo.colortex.cn

PHP:  public / protected / private
来源：http://xm.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://gv.haigaiapp.cn

TS:   public / protected / private
来源：http://xu.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://kv.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eu.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://vg.shxzukj.cn

C#:   public / protected / private / internal
来源：http://bx.bjjhwx.cn

[G11] getter / setter
来源：http://kv.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://nv.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fb.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://mn.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://eu.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://dk.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dz.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://cr.hahajie.cn

C#:   public string Name { get; set; }
来源：http://su.colortex.cn

[G12] 对象转字符串
来源：http://so.asd995.cn

Py:   def __str__(self): return self.name
来源：http://fw.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ed.newstarts.cn

JS:   toString() { return this.name; }
来源：http://hn.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://xi.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://mg.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fh.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://di.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://rz.wgjwhj.cn

[G13] 判断对象类型
来源：http://jc.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://pz.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://xd.asd995.cn

JS:   u instanceof User
来源：http://hd.yuexingan06.cn

TS:   u instanceof User
来源：http://kx.szxytkj.cn

Java: u instanceof User
来源：http://qz.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mb.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://ne.bookmarksfly.cn

C#:   u is User
来源：http://hm.shxzukj.cn

[G14] 数据类 / record
来源：http://dl.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xt.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://lt.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://um.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://ip.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://hm.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://en.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wf.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://wa.haigaiapp.cn

[G15] 枚举
来源：http://ab.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://os.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dq.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sk.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ft.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://jd.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oi.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://uf.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ew.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://rc.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ym.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://sj.nszjky.cn

JS:   Object.entries(obj)
来源：http://en.521024.cn

TS:   Object.entries(obj)
来源：http://ez.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tt.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ez.hahajie.cn

Ruby: obj.instance_variables
来源：http://gv.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://ot.wgjwhj.cn

================================================================================
来源：http://pi.yuexingan06.cn

H. 异常与错误处理
来源：http://ew.newstarts.cn

================================================================================
来源：http://ok.gzmigu.cn

[H01] try / catch 基础
来源：http://dq.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cm.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kr.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sw.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jo.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://so.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://by.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qj.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cm.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ee.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ec.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fn.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gh.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jw.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ds.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ac.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ys.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cn.szsharing.cn

[H03] 主动抛出异常
来源：http://hi.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://uc.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ma.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://mk.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://mx.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vv.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ym.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ho.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kf.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://ih.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://ul.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dg.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://pi.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://ul.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://vp.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ql.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://as.asd995.cn

C#:   class MyException : Exception {}
来源：http://oe.nszjky.cn

[H05] 捕获特定类型
来源：http://bv.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://ps.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cq.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://zj.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://qu.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://rz.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xk.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://om.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zi.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://fb.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://se.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bh.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vw.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yu.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uz.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fj.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://er.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://sh.muxihuayi.cn

[H07] 断言
来源：http://nq.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://ej.gzmigu.cn

PHP:  assert($x > 0);
来源：http://qp.hahajie.cn

JS:   console.assert(x > 0);
来源：http://mq.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://kh.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://cs.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ud.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ik.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://yg.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://wd.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://sy.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://da.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://xu.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bq.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rx.jianghongdianzi.cn

Go:   err.Error()
来源：http://nj.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://cf.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://pc.shxzukj.cn

[H09] 带错误码的异常
来源：http://ew.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xt.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ra.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ts.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://no.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ig.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xa.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pv.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ol.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://cq.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ky.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ai.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ts.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jf.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://es.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://jk.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dr.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jx.shtwfgs.cn

================================================================================
来源：http://dd.huanxung.cn

I. 正则表达式
来源：http://al.huixinmuqiang.cn

================================================================================
来源：http://bo.jctech888.com.cn

[I01] 判断是否匹配
来源：http://ym.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bk.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ya.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://wg.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://bm.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vx.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ze.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://vg.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nf.gzmigu.cn

[I02] 提取所有匹配
来源：http://ub.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://gk.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xe.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xx.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://vl.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lr.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wg.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://fy.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pl.chemitech.net.cn

[I03] 提取捕获分组
来源：http://om.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://we.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kd.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mc.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://el.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ha.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gp.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tu.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bl.chemitech.net.cn

[I04] 正则替换
来源：http://cs.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://of.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tj.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kq.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cl.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sd.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yb.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ta.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iq.shxzukj.cn

[I05] 按正则拆分
来源：http://db.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://az.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kb.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://gv.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://dd.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://qo.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ha.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sx.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ed.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mq.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cd.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ux.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wm.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ee.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rv.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yi.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uu.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yp.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://zx.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ds.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nr.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ox.nszjky.cn

TS:   /error/gim
来源：http://xa.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cv.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xh.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://vs.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jo.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://pe.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jr.wgjwhj.cn


<!-- 参考信息 -->