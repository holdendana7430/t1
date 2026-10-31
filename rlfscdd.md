代发 wailian999

Py:   class User: pass
来源：http://do.bookmarksfly.cn

PHP:  class User {}
来源：http://nb.jianghongdianzi.cn

JS:   class User {}
来源：http://zr.asd995.cn

TS:   class User { name: string = ""; }
来源：http://iq.colortex.cn

Java: class User {}
来源：http://tg.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://de.nszjky.cn

Ruby: class User; end
来源：http://gd.jctech888.com.cn

C#:   class User {}
来源：http://ur.nszjky.cn

[G02] 构造函数
来源：http://hx.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://bi.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://mi.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://ee.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://wm.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://nu.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hu.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://jw.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://tv.muxihuayi.cn

[G03] 实例属性
来源：http://eq.yuexingan06.cn

Py:   self.name = "x"
来源：http://zi.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://ir.chemitech.net.cn

JS:   this.name = "x";
来源：http://jv.chemitech.net.cn

TS:   name: string = "x";
来源：http://jx.wgjwhj.cn

Java: private String name;
来源：http://hw.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oc.bookmarksfly.cn

Ruby: @name = "x"
来源：http://zs.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://rq.colortex.cn

[G04] 定义方法
来源：http://ro.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ej.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xo.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://zx.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://qh.shtwfgs.cn

Java: String greet() { return name; }
来源：http://ok.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zw.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://pt.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://ct.hahajie.cn

[G05] 继承
来源：http://lh.shxzskj.cn

Py:   class Admin(User): pass
来源：http://sk.nszjky.cn

PHP:  class Admin extends User {}
来源：http://wb.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://vb.shxzukj.cn

TS:   class Admin extends User {}
来源：http://ei.hnjuh.cn

Java: class Admin extends User {}
来源：http://fv.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nx.huanxung.cn

Ruby: class Admin < User; end
来源：http://gy.bjjhwx.cn

C#:   class Admin : User {}
来源：http://kv.asd995.cn

[G06] 重写方法
来源：http://qk.asd995.cn

Py:   def greet(self): return "admin"
来源：http://kr.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pe.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://sb.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://rg.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://bn.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dj.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://oi.521024.cn

C#:   public override string Greet() => "admin";
来源：http://ae.hnjuh.cn

[G07] 调用父类方法
来源：http://gf.bookmarksfly.cn

Py:   super().greet()
来源：http://sn.colortex.cn

PHP:  parent::greet();
来源：http://xy.shxzskj.cn

JS:   super.greet();
来源：http://jh.muxihuayi.cn

TS:   super.greet();
来源：http://vk.panjiajie.cn

Java: super.greet();
来源：http://jz.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yd.hahajie.cn

Ruby: super
来源：http://ab.szxytkj.cn

C#:   base.Greet();
来源：http://aq.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://eo.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tl.newstarts.cn

PHP:  public static function f() {}
来源：http://td.bjjhwx.cn

JS:   static f() {}
来源：http://jm.asd995.cn

TS:   static f(): void {}
来源：http://qp.bookmarksfly.cn

Java: static void f() {}
来源：http://un.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hb.panjiajie.cn

Ruby: def self.f; end
来源：http://bx.colortex.cn

C#:   public static void F() {}
来源：http://mg.asd995.cn

[G09] 接口 / 抽象类
来源：http://qn.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://hw.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://el.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wh.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://ka.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://eq.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://hp.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://po.521024.cn

C#:   interface IShape { double Area(); }
来源：http://pa.9csxet.cn

[G10] 访问控制
来源：http://cs.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://jm.haigaiapp.cn

PHP:  public / protected / private
来源：http://hf.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://zz.bjjhwx.cn

TS:   public / protected / private
来源：http://tv.asd995.cn

Java: public / protected / private / 默认包级
来源：http://dt.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qu.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://gz.521024.cn

C#:   public / protected / private / internal
来源：http://qc.chemitech.net.cn

[G11] getter / setter
来源：http://jt.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://ya.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ba.asd995.cn

JS:   get name() { return this._name; }
来源：http://xk.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://lv.huanxung.cn

Java: public String getName() { return name; }
来源：http://wl.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qg.huanxung.cn

Ruby: attr_accessor :name
来源：http://ka.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://cy.521024.cn

[G12] 对象转字符串
来源：http://go.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://it.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pm.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://lv.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://uo.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://mw.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yx.521024.cn

Ruby: def to_s; @name; end
来源：http://ky.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://jv.chemitech.net.cn

[G13] 判断对象类型
来源：http://lp.521024.cn

Py:   isinstance(u, User)
来源：http://wf.panjiajie.cn

PHP:  $u instanceof User
来源：http://te.lnxyls.cn

JS:   u instanceof User
来源：http://cn.chemitech.net.cn

TS:   u instanceof User
来源：http://lw.szxytkj.cn

Java: u instanceof User
来源：http://rw.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://il.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://wk.chemitech.net.cn

C#:   u is User
来源：http://td.shtwfgs.cn

[G14] 数据类 / record
来源：http://jl.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ts.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://vk.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zc.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://gu.asd995.cn

Java: record User(String name, int age) {}
来源：http://da.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://hj.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lb.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://lt.jctech888.com.cn

[G15] 枚举
来源：http://vg.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gv.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rb.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ck.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sc.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://by.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rv.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://mc.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://do.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://mq.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ql.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ck.szxytkj.cn

JS:   Object.entries(obj)
来源：http://ia.nszjky.cn

TS:   Object.entries(obj)
来源：http://ts.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ua.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kc.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://to.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://qj.wgjwhj.cn

================================================================================
来源：http://qj.haigaiapp.cn

H. 异常与错误处理
来源：http://hv.nicolike.cn

================================================================================
来源：http://nr.hahajie.cn

[H01] try / catch 基础
来源：http://my.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://af.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nu.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ya.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iv.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pg.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kw.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uc.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nf.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://af.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cw.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wr.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lc.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://le.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ot.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ym.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fb.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ib.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://lr.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://lh.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://la.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://gd.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://px.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ty.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ty.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dl.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bg.chemitech.net.cn

[H04] 自定义异常类型
来源：http://cz.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://ip.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ab.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://xf.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://jh.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://aj.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wf.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://by.colortex.cn

C#:   class MyException : Exception {}
来源：http://hp.panjiajie.cn

[H05] 捕获特定类型
来源：http://gs.shxzskj.cn

Py:   except ValueError as e:
来源：http://vk.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sf.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://tk.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://jj.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://hj.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kp.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://qw.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ja.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://st.asd995.cn

Py:   value = d.get("k") or default
来源：http://xq.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ia.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://av.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ic.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xx.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rz.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://im.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://zt.huixiangedu.cn

[H07] 断言
来源：http://ud.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://lo.panjiajie.cn

PHP:  assert($x > 0);
来源：http://ca.newstarts.cn

JS:   console.assert(x > 0);
来源：http://tn.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://fz.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://qa.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ev.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vn.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://jt.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://gm.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://to.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cj.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://tz.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zv.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zc.shxzukj.cn

Go:   err.Error()
来源：http://qj.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://yl.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://yz.chemitech.net.cn

[H09] 带错误码的异常
来源：http://fh.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yu.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mv.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xv.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://la.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pu.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nc.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yz.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jb.hahajie.cn

[H10] 资源自动释放
来源：http://fk.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pu.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gb.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qc.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cx.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lc.szxytkj.cn

Go:   defer f.Close()
来源：http://pk.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yi.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yc.nszjky.cn

================================================================================
来源：http://sn.9csxet.cn

I. 正则表达式
来源：http://cw.hnjuh.cn

================================================================================
来源：http://pl.bjjhwx.cn

[I01] 判断是否匹配
来源：http://sl.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sr.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uk.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://xf.colortex.cn

TS:   /\d+/.test(s)
来源：http://fg.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zu.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qb.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://xr.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hw.panjiajie.cn

[I02] 提取所有匹配
来源：http://be.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://fs.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fi.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aj.521024.cn

TS:   s.match(/\d+/g)
来源：http://qb.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vj.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nz.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://sb.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cm.521024.cn

[I03] 提取捕获分组
来源：http://tx.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uj.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dy.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ol.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wt.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rq.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ki.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fi.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mv.asd995.cn

[I04] 正则替换
来源：http://lg.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yk.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://it.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://po.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zj.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://we.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xb.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://my.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ob.huanxung.cn

[I05] 按正则拆分
来源：http://fq.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dt.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fr.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://yp.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://du.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://dm.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xp.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sv.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gc.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aw.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mk.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sh.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ym.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ud.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nr.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://la.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vd.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yr.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://ci.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qn.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xn.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mt.muxihuayi.cn

TS:   /error/gim
来源：http://xr.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ld.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zf.huanxung.cn


<!-- 参考信息 -->