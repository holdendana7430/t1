代发 wailian999

================================================================================
来源：http://kh.muxihuayi.cn

G. 面向对象
来源：http://hg.hnjuh.cn

================================================================================
来源：http://rq.bookmarksfly.cn

[G01] 定义类
来源：http://qd.haigaiapp.cn

Py:   class User: pass
来源：http://mi.newstarts.cn

PHP:  class User {}
来源：http://eg.9csxet.cn

JS:   class User {}
来源：http://vx.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://pl.yuntaijiaju.cn

Java: class User {}
来源：http://aj.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://dg.asd995.cn

Ruby: class User; end
来源：http://sk.nszjky.cn

C#:   class User {}
来源：http://pf.panjiajie.cn

[G02] 构造函数
来源：http://re.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://rw.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hf.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://rx.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://vt.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://fo.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wk.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://nz.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://ec.yuexingan06.cn

[G03] 实例属性
来源：http://se.shxzukj.cn

Py:   self.name = "x"
来源：http://ti.521024.cn

PHP:  public string $name = "x";
来源：http://to.wgjwhj.cn

JS:   this.name = "x";
来源：http://zk.lnxyls.cn

TS:   name: string = "x";
来源：http://lx.panjiajie.cn

Java: private String name;
来源：http://ia.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ya.hnjuh.cn

Ruby: @name = "x"
来源：http://zm.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://qd.shxzukj.cn

[G04] 定义方法
来源：http://fu.szsharing.cn

Py:   def greet(self): return self.name
来源：http://xq.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://to.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://kn.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://ow.shtwfgs.cn

Java: String greet() { return name; }
来源：http://es.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bc.asd995.cn

Ruby: def greet; @name; end
来源：http://kq.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://kn.asd995.cn

[G05] 继承
来源：http://qk.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ow.newstarts.cn

PHP:  class Admin extends User {}
来源：http://he.nszjky.cn

JS:   class Admin extends User {}
来源：http://zz.szsharing.cn

TS:   class Admin extends User {}
来源：http://by.hnjuh.cn

Java: class Admin extends User {}
来源：http://jk.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zx.szsharing.cn

Ruby: class Admin < User; end
来源：http://me.yuexingan06.cn

C#:   class Admin : User {}
来源：http://ie.nicolike.cn

[G06] 重写方法
来源：http://ts.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://od.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nb.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://iy.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://co.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://lz.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lt.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://ae.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://oo.hahajie.cn

[G07] 调用父类方法
来源：http://ch.haigaiapp.cn

Py:   super().greet()
来源：http://ft.wgjwhj.cn

PHP:  parent::greet();
来源：http://nv.colortex.cn

JS:   super.greet();
来源：http://ed.colortex.cn

TS:   super.greet();
来源：http://oy.haigaiapp.cn

Java: super.greet();
来源：http://to.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ky.yuntaijiaju.cn

Ruby: super
来源：http://mv.lnxyls.cn

C#:   base.Greet();
来源：http://hq.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://ih.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jv.hahajie.cn

PHP:  public static function f() {}
来源：http://bp.hnjuh.cn

JS:   static f() {}
来源：http://qr.muxihuayi.cn

TS:   static f(): void {}
来源：http://xl.9csxet.cn

Java: static void f() {}
来源：http://dn.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hy.wgjwhj.cn

Ruby: def self.f; end
来源：http://jn.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://fb.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://ze.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://hs.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qm.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://la.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://xq.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://mj.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://ga.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ht.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://hz.huanxung.cn

[G10] 访问控制
来源：http://rx.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://zb.lnxyls.cn

PHP:  public / protected / private
来源：http://wp.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://tt.asd995.cn

TS:   public / protected / private
来源：http://ti.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://cs.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://od.nicolike.cn

Ruby: public / protected / private
来源：http://nr.lnxyls.cn

C#:   public / protected / private / internal
来源：http://na.bookmarksfly.cn

[G11] getter / setter
来源：http://du.9csxet.cn

Py:   @property 与 @x.setter
来源：http://gi.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rw.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://hx.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://ix.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://bg.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ar.shxzukj.cn

Ruby: attr_accessor :name
来源：http://jb.nszjky.cn

C#:   public string Name { get; set; }
来源：http://to.huixiangedu.cn

[G12] 对象转字符串
来源：http://ep.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://xq.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://go.nicolike.cn

JS:   toString() { return this.name; }
来源：http://eh.521024.cn

TS:   toString(): string { return this.name; }
来源：http://lm.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://ff.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gf.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://nx.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://cn.gzmigu.cn

[G13] 判断对象类型
来源：http://cz.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://gb.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://qz.huixinmuqiang.cn

JS:   u instanceof User
来源：http://ts.shtwfgs.cn

TS:   u instanceof User
来源：http://fb.gzmigu.cn

Java: u instanceof User
来源：http://pi.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nd.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://tr.panjiajie.cn

C#:   u is User
来源：http://tj.newstarts.cn

[G14] 数据类 / record
来源：http://ih.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://or.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://lq.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ks.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://ah.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://ez.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://ut.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lf.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://xu.9csxet.cn

[G15] 枚举
来源：http://pd.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://or.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dc.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wb.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wy.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://uw.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sa.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://ol.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kl.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://lp.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zb.521024.cn

PHP:  get_object_vars($obj);
来源：http://hs.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://ds.521024.cn

TS:   Object.entries(obj)
来源：http://hz.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nk.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bn.colortex.cn

Ruby: obj.instance_variables
来源：http://rt.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://zy.nicolike.cn

================================================================================
来源：http://ip.muxihuayi.cn

H. 异常与错误处理
来源：http://zo.haigaiapp.cn

================================================================================
来源：http://qe.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://gu.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jr.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://je.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jj.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xh.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xr.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ol.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qd.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nm.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://lz.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ik.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nn.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rz.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ih.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xf.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jr.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ym.haigaiapp.cn

[H03] 主动抛出异常
来源：http://nh.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://lc.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ri.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://bl.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://xk.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hw.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vc.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dh.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://on.521024.cn

[H04] 自定义异常类型
来源：http://sa.colortex.cn

Py:   class MyError(Exception): pass
来源：http://of.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wo.newstarts.cn

JS:   class MyError extends Error {}
来源：http://vu.nszjky.cn

TS:   class MyError extends Error {}
来源：http://wq.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://py.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kn.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://yq.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://bj.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://pl.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://qi.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tv.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://gg.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://ku.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://fl.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gq.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://fy.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ra.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://tc.521024.cn

Py:   value = d.get("k") or default
来源：http://op.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ra.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ou.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fx.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yr.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jx.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://an.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://li.shxzukj.cn

[H07] 断言
来源：http://yk.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://no.gzmigu.cn

PHP:  assert($x > 0);
来源：http://bh.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://ja.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://ve.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://rf.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xf.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yu.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://mo.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://jt.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://gj.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xe.gzmigu.cn

JS:   e.message;  e.stack
来源：http://es.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nx.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://je.muxihuayi.cn

Go:   err.Error()
来源：http://ts.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://um.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://le.gzmigu.cn

[H09] 带错误码的异常
来源：http://bn.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bt.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rf.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://af.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dt.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mo.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zx.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sg.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ga.yuexingan06.cn

[H10] 资源自动释放
来源：http://mt.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hh.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://br.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ts.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yj.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cd.9csxet.cn

Go:   defer f.Close()
来源：http://ft.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xx.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jw.jianghongdianzi.cn

================================================================================
来源：http://fp.szxytkj.cn

I. 正则表达式
来源：http://bg.colortex.cn

================================================================================
来源：http://pk.muxihuayi.cn

[I01] 判断是否匹配
来源：http://wh.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://we.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oo.nszjky.cn

JS:   /\d+/.test(s)
来源：http://jb.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://fq.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xg.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hl.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://ai.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bz.nicolike.cn

[I02] 提取所有匹配
来源：http://eu.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://ph.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zp.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ot.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://jz.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tt.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lf.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://pb.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ry.panjiajie.cn

[I03] 提取捕获分组
来源：http://ye.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cx.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ut.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://py.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ez.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iz.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tm.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://at.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vn.jianghongdianzi.cn

[I04] 正则替换
来源：http://fz.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wv.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ef.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ld.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yc.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://og.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bm.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fy.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wn.panjiajie.cn

[I05] 按正则拆分
来源：http://fo.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://on.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ik.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://uj.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://un.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://ru.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zw.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ng.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dx.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gv.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://is.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pn.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pg.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sn.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://we.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dj.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ue.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iw.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://rx.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vl.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nk.panjiajie.cn


<!-- 参考信息 -->