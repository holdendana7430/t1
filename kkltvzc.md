代发 wailian999

Java: class User {}
来源：http://xp.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://qs.panjiajie.cn

Ruby: class User; end
来源：http://so.colortex.cn

C#:   class User {}
来源：http://ll.panjiajie.cn

[G02] 构造函数
来源：http://ab.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ir.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://tp.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://zx.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://so.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://iz.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ih.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://tn.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://lp.muxihuayi.cn

[G03] 实例属性
来源：http://zf.nicolike.cn

Py:   self.name = "x"
来源：http://lf.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://yo.huanxung.cn

JS:   this.name = "x";
来源：http://gu.hnjuh.cn

TS:   name: string = "x";
来源：http://ma.lnxyls.cn

Java: private String name;
来源：http://ix.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sz.shxzskj.cn

Ruby: @name = "x"
来源：http://ph.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://oe.szsharing.cn

[G04] 定义方法
来源：http://yk.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://jy.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://um.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://af.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://sj.muxihuayi.cn

Java: String greet() { return name; }
来源：http://hn.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hl.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://un.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://wo.haigaiapp.cn

[G05] 继承
来源：http://ww.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://wk.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://sj.colortex.cn

JS:   class Admin extends User {}
来源：http://yd.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://ia.jctech888.com.cn

Java: class Admin extends User {}
来源：http://zw.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oz.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://ko.lnxyls.cn

C#:   class Admin : User {}
来源：http://dl.9csxet.cn

[G06] 重写方法
来源：http://yt.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://na.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://so.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://tb.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://dk.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://rk.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mx.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://on.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://es.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://gb.nicolike.cn

Py:   super().greet()
来源：http://ob.panjiajie.cn

PHP:  parent::greet();
来源：http://wd.bjjhwx.cn

JS:   super.greet();
来源：http://zp.jianghongdianzi.cn

TS:   super.greet();
来源：http://wd.bjjhwx.cn

Java: super.greet();
来源：http://dw.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oq.huixinmuqiang.cn

Ruby: super
来源：http://jv.521024.cn

C#:   base.Greet();
来源：http://cx.szsharing.cn

[G08] 静态方法与属性
来源：http://vk.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zi.newstarts.cn

PHP:  public static function f() {}
来源：http://kc.jianghongdianzi.cn

JS:   static f() {}
来源：http://qm.shtwfgs.cn

TS:   static f(): void {}
来源：http://ns.panjiajie.cn

Java: static void f() {}
来源：http://ta.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://te.panjiajie.cn

Ruby: def self.f; end
来源：http://zb.hahajie.cn

C#:   public static void F() {}
来源：http://ao.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://kw.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://lk.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dc.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zn.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://of.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://iv.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://yi.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wx.521024.cn

C#:   interface IShape { double Area(); }
来源：http://cu.hahajie.cn

[G10] 访问控制
来源：http://xc.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://jd.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://au.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://tw.asd995.cn

TS:   public / protected / private
来源：http://gm.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://iq.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://io.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://ri.shxzukj.cn

C#:   public / protected / private / internal
来源：http://ny.yuexingan06.cn

[G11] getter / setter
来源：http://bf.nicolike.cn

Py:   @property 与 @x.setter
来源：http://lp.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hx.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://ud.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://gb.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://uf.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://io.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://te.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://ru.shxzskj.cn

[G12] 对象转字符串
来源：http://sj.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://vf.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sk.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://nx.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://kj.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://bc.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://af.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://oq.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://ck.newstarts.cn

[G13] 判断对象类型
来源：http://te.shxzukj.cn

Py:   isinstance(u, User)
来源：http://jn.shtwfgs.cn

PHP:  $u instanceof User
来源：http://iq.jctech888.com.cn

JS:   u instanceof User
来源：http://ow.nszjky.cn

TS:   u instanceof User
来源：http://uk.colortex.cn

Java: u instanceof User
来源：http://vf.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://va.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://td.huixiangedu.cn

C#:   u is User
来源：http://cj.nicolike.cn

[G14] 数据类 / record
来源：http://fx.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qz.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://hj.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bi.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://vo.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://pv.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://au.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sm.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://dq.bjjhwx.cn

[G15] 枚举
来源：http://bj.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bk.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wx.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gy.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://py.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://sy.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vg.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://cb.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://es.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://ug.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ca.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://vh.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://lg.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://vs.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rs.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kh.521024.cn

Ruby: obj.instance_variables
来源：http://nt.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://kj.hnjuh.cn

================================================================================
来源：http://if.521024.cn

H. 异常与错误处理
来源：http://nn.nicolike.cn

================================================================================
来源：http://fu.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://qp.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ir.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jy.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rw.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zf.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hn.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ge.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ci.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ps.9csxet.cn

[H02] finally / ensure 收尾
来源：http://gl.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yi.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xv.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xt.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gi.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kt.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://le.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pr.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zl.nszjky.cn

[H03] 主动抛出异常
来源：http://hd.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://jd.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ch.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://ec.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://zj.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kh.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ji.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ql.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://si.haigaiapp.cn

[H04] 自定义异常类型
来源：http://vb.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://jr.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://en.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://hk.521024.cn

TS:   class MyError extends Error {}
来源：http://bw.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://rz.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hn.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://lx.nszjky.cn

C#:   class MyException : Exception {}
来源：http://sj.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://ou.muxihuayi.cn

Py:   except ValueError as e:
来源：http://ca.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pn.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://eh.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://uq.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://up.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cb.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://yz.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iv.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://am.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://tm.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kp.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ry.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jz.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://go.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hw.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://bg.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://la.bookmarksfly.cn

[H07] 断言
来源：http://px.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://pz.newstarts.cn

PHP:  assert($x > 0);
来源：http://ax.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://tq.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://xo.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://ti.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dd.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fe.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://cx.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://xn.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://uj.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cu.gzmigu.cn

JS:   e.message;  e.stack
来源：http://mf.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dr.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hu.shxzskj.cn

Go:   err.Error()
来源：http://bc.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://gc.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://zf.jctech888.com.cn

[H09] 带错误码的异常
来源：http://rh.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://au.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wz.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ma.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rc.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tt.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gs.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jf.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cx.jctech888.com.cn

[H10] 资源自动释放
来源：http://ju.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sm.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pt.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pp.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tq.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://by.hnjuh.cn

Go:   defer f.Close()
来源：http://fh.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pf.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wn.bookmarksfly.cn

================================================================================
来源：http://ry.bjjhwx.cn

I. 正则表达式
来源：http://oh.szsharing.cn

================================================================================
来源：http://df.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://iw.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://et.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://po.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://yb.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://sm.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jl.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ga.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://fj.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://au.asd995.cn

[I02] 提取所有匹配
来源：http://hv.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://xk.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mw.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gq.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://eh.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yl.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oy.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://dg.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ar.hahajie.cn

[I03] 提取捕获分组
来源：http://wd.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pf.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kv.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uq.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pz.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://da.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ut.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ce.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dd.colortex.cn

[I04] 正则替换
来源：http://uy.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pb.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gr.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bq.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wc.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ep.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ad.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xs.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hs.hnjuh.cn

[I05] 按正则拆分
来源：http://mn.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nj.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ic.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://no.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://ey.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://hf.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://we.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ue.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wu.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fc.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lw.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://me.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kp.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zi.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bf.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xf.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xw.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ro.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://gv.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ff.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rp.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ee.wgjwhj.cn

TS:   /error/gim
来源：http://od.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iz.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xg.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://is.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oe.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://qd.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hw.jianghongdianzi.cn


<!-- 参考信息 -->