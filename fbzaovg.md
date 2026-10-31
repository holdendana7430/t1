代发 wailian999

================================================================================
来源：http://jy.yuexingan06.cn

G. 面向对象
来源：http://iv.jctech888.com.cn

================================================================================
来源：http://ix.yuexingan06.cn

[G01] 定义类
来源：http://bu.jctech888.com.cn

Py:   class User: pass
来源：http://sm.muxihuayi.cn

PHP:  class User {}
来源：http://jv.jctech888.com.cn

JS:   class User {}
来源：http://wj.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://pj.asd995.cn

Java: class User {}
来源：http://qh.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://nm.yuexingan06.cn

Ruby: class User; end
来源：http://rj.jianghongdianzi.cn

C#:   class User {}
来源：http://gd.colortex.cn

[G02] 构造函数
来源：http://je.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://zh.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://in.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://li.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://jt.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://vz.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mw.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://xe.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ev.yuexingan06.cn

[G03] 实例属性
来源：http://ph.panjiajie.cn

Py:   self.name = "x"
来源：http://jd.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://ip.szxytkj.cn

JS:   this.name = "x";
来源：http://mq.szsharing.cn

TS:   name: string = "x";
来源：http://ah.muxihuayi.cn

Java: private String name;
来源：http://ah.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ra.hahajie.cn

Ruby: @name = "x"
来源：http://so.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://zd.huixiangedu.cn

[G04] 定义方法
来源：http://we.colortex.cn

Py:   def greet(self): return self.name
来源：http://ip.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gx.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://tg.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://gm.nszjky.cn

Java: String greet() { return name; }
来源：http://nv.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gc.521024.cn

Ruby: def greet; @name; end
来源：http://zh.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://mg.9csxet.cn

[G05] 继承
来源：http://mk.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://zl.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://bi.lnxyls.cn

JS:   class Admin extends User {}
来源：http://ua.huanxung.cn

TS:   class Admin extends User {}
来源：http://xc.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://zb.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cd.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://tr.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://yk.9csxet.cn

[G06] 重写方法
来源：http://no.asd995.cn

Py:   def greet(self): return "admin"
来源：http://tl.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cv.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://jx.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://fj.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://oa.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gn.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://af.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://yc.hahajie.cn

[G07] 调用父类方法
来源：http://xy.haigaiapp.cn

Py:   super().greet()
来源：http://kl.newstarts.cn

PHP:  parent::greet();
来源：http://iv.bjjhwx.cn

JS:   super.greet();
来源：http://ea.asd995.cn

TS:   super.greet();
来源：http://zy.shxzukj.cn

Java: super.greet();
来源：http://yu.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://un.hahajie.cn

Ruby: super
来源：http://in.hahajie.cn

C#:   base.Greet();
来源：http://yb.huanxung.cn

[G08] 静态方法与属性
来源：http://se.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vs.szsharing.cn

PHP:  public static function f() {}
来源：http://sr.haigaiapp.cn

JS:   static f() {}
来源：http://ib.huanxung.cn

TS:   static f(): void {}
来源：http://xv.huanxung.cn

Java: static void f() {}
来源：http://mo.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://we.szsharing.cn

Ruby: def self.f; end
来源：http://bw.wgjwhj.cn

C#:   public static void F() {}
来源：http://nc.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://sh.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://dy.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rz.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zs.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://sl.asd995.cn

Java: interface Shape { double area(); }
来源：http://fd.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://dn.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fe.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://uj.shtwfgs.cn

[G10] 访问控制
来源：http://re.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://wq.chemitech.net.cn

PHP:  public / protected / private
来源：http://yu.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://cc.jianghongdianzi.cn

TS:   public / protected / private
来源：http://is.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://qa.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oy.colortex.cn

Ruby: public / protected / private
来源：http://kq.521024.cn

C#:   public / protected / private / internal
来源：http://fs.colortex.cn

[G11] getter / setter
来源：http://ci.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://pr.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lf.szsharing.cn

JS:   get name() { return this._name; }
来源：http://wz.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://nt.shxzskj.cn

Java: public String getName() { return name; }
来源：http://pb.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fs.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://tc.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://gr.yuexingan06.cn

[G12] 对象转字符串
来源：http://me.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://gq.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://od.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://gy.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://tt.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://jg.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cw.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://eg.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://ab.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://qe.colortex.cn

Py:   isinstance(u, User)
来源：http://zw.szsharing.cn

PHP:  $u instanceof User
来源：http://ze.nszjky.cn

JS:   u instanceof User
来源：http://xg.lnxyls.cn

TS:   u instanceof User
来源：http://fq.newstarts.cn

Java: u instanceof User
来源：http://sf.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yo.9csxet.cn

Ruby: u.is_a?(User)
来源：http://cp.shxzskj.cn

C#:   u is User
来源：http://xv.huixiangedu.cn

[G14] 数据类 / record
来源：http://ag.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fd.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://ml.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gi.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://ly.huanxung.cn

Java: record User(String name, int age) {}
来源：http://pn.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://co.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dg.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://qi.bookmarksfly.cn

[G15] 枚举
来源：http://lv.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kz.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hi.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://un.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dv.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://ew.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vw.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://or.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ig.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://cz.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fk.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://md.shxzskj.cn

JS:   Object.entries(obj)
来源：http://gl.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://zf.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vg.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://me.huanxung.cn

Ruby: obj.instance_variables
来源：http://jl.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ml.hahajie.cn

================================================================================
来源：http://nu.haigaiapp.cn

H. 异常与错误处理
来源：http://ff.newstarts.cn

================================================================================
来源：http://mo.szxytkj.cn

[H01] try / catch 基础
来源：http://zn.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oh.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rl.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://as.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jy.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zd.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mg.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tk.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ma.hahajie.cn

[H02] finally / ensure 收尾
来源：http://rm.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mq.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://he.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hi.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://am.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mf.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mf.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lr.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://me.shxzskj.cn

[H03] 主动抛出异常
来源：http://vf.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://rx.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hs.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://nr.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://ex.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ag.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zh.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ph.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://aj.haigaiapp.cn

[H04] 自定义异常类型
来源：http://ar.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://ok.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://va.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://ok.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://ow.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://xt.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gk.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://ea.nszjky.cn

C#:   class MyException : Exception {}
来源：http://sd.muxihuayi.cn

[H05] 捕获特定类型
来源：http://or.hahajie.cn

Py:   except ValueError as e:
来源：http://be.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aa.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://px.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://js.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://kq.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://no.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://nh.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ka.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://zq.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://dv.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ch.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lu.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bp.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://en.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xb.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://tm.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://rf.huixiangedu.cn

[H07] 断言
来源：http://zl.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://zu.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://ge.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://rk.colortex.cn

TS:   console.assert(x > 0);
来源：http://sb.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://py.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rg.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ix.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://oj.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://hg.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://dz.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ww.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://fe.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://il.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dh.jctech888.com.cn

Go:   err.Error()
来源：http://br.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://mk.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://xl.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://lf.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jq.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uw.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ut.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dc.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://op.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rz.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://em.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qx.9csxet.cn

[H10] 资源自动释放
来源：http://rz.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fa.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lc.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oj.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iz.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wj.hnjuh.cn

Go:   defer f.Close()
来源：http://vs.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bq.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://if.9csxet.cn

================================================================================
来源：http://xk.shtwfgs.cn

I. 正则表达式
来源：http://ee.hahajie.cn

================================================================================
来源：http://wz.yuexingan06.cn

[I01] 判断是否匹配
来源：http://as.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pd.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yf.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://qc.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://mb.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vg.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xf.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://va.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xk.gzmigu.cn

[I02] 提取所有匹配
来源：http://ld.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://si.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fv.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yl.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://mp.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zv.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wf.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://ps.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sv.newstarts.cn

[I03] 提取捕获分组
来源：http://tx.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mq.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wd.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ir.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hw.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nt.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bl.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bd.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ih.asd995.cn

[I04] 正则替换
来源：http://lv.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jq.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kp.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lc.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ad.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sv.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oj.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rp.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xh.521024.cn

[I05] 按正则拆分
来源：http://ph.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bb.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://el.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://cj.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://cy.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://mv.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ua.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ab.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pu.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ow.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wr.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xw.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kx.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://st.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yw.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qs.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bb.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tw.521024.cn

[I07] 忽略大小写与多行模式
来源：http://je.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lm.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wv.muxihuayi.cn


<!-- 参考信息 -->