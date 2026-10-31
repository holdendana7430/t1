代发 wailian999

[G02] 构造函数
来源：http://oh.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://hp.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://ar.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://ux.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://sl.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://te.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lr.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://kb.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://jc.huixinmuqiang.cn

[G03] 实例属性
来源：http://id.9csxet.cn

Py:   self.name = "x"
来源：http://pw.panjiajie.cn

PHP:  public string $name = "x";
来源：http://oy.521024.cn

JS:   this.name = "x";
来源：http://fz.shxzskj.cn

TS:   name: string = "x";
来源：http://ig.521024.cn

Java: private String name;
来源：http://gx.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eq.nszjky.cn

Ruby: @name = "x"
来源：http://qh.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://qe.muxihuayi.cn

[G04] 定义方法
来源：http://xn.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://ok.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hw.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://wy.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://pq.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://dt.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ag.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://mp.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://lg.hnjuh.cn

[G05] 继承
来源：http://lf.hnjuh.cn

Py:   class Admin(User): pass
来源：http://bh.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://et.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://wy.nicolike.cn

TS:   class Admin extends User {}
来源：http://rp.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://fo.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pl.lnxyls.cn

Ruby: class Admin < User; end
来源：http://ex.panjiajie.cn

C#:   class Admin : User {}
来源：http://yq.shtwfgs.cn

[G06] 重写方法
来源：http://fy.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://dr.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sm.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://mm.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://xu.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://yl.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pp.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://jz.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://dq.nszjky.cn

[G07] 调用父类方法
来源：http://sr.shxzskj.cn

Py:   super().greet()
来源：http://pq.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://pj.yuntaijiaju.cn

JS:   super.greet();
来源：http://ty.yuntaijiaju.cn

TS:   super.greet();
来源：http://es.shtwfgs.cn

Java: super.greet();
来源：http://yx.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rr.szsharing.cn

Ruby: super
来源：http://yk.lnxyls.cn

C#:   base.Greet();
来源：http://ft.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://sp.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dc.521024.cn

PHP:  public static function f() {}
来源：http://bp.shxzskj.cn

JS:   static f() {}
来源：http://hr.521024.cn

TS:   static f(): void {}
来源：http://yr.hnjuh.cn

Java: static void f() {}
来源：http://ox.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ku.bookmarksfly.cn

Ruby: def self.f; end
来源：http://rl.gzmigu.cn

C#:   public static void F() {}
来源：http://fm.nicolike.cn

[G09] 接口 / 抽象类
来源：http://sh.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://sb.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://we.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ib.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://ru.colortex.cn

Java: interface Shape { double area(); }
来源：http://bz.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://bv.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sa.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://xg.szxytkj.cn

[G10] 访问控制
来源：http://bj.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://np.chemitech.net.cn

PHP:  public / protected / private
来源：http://qm.hahajie.cn

JS:   #private 字段；其余公开
来源：http://ku.shtwfgs.cn

TS:   public / protected / private
来源：http://kj.colortex.cn

Java: public / protected / private / 默认包级
来源：http://if.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wt.jctech888.com.cn

Ruby: public / protected / private
来源：http://ay.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://mx.nszjky.cn

[G11] getter / setter
来源：http://oo.nicolike.cn

Py:   @property 与 @x.setter
来源：http://jp.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jh.hahajie.cn

JS:   get name() { return this._name; }
来源：http://ud.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://dg.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://ow.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wj.hahajie.cn

Ruby: attr_accessor :name
来源：http://qm.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://kf.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://zm.asd995.cn

Py:   def __str__(self): return self.name
来源：http://nr.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tg.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://eh.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://yf.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://id.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fa.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://wx.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ua.colortex.cn

[G13] 判断对象类型
来源：http://gz.asd995.cn

Py:   isinstance(u, User)
来源：http://gr.szxytkj.cn

PHP:  $u instanceof User
来源：http://oy.gzmigu.cn

JS:   u instanceof User
来源：http://sz.huanxung.cn

TS:   u instanceof User
来源：http://qo.chemitech.net.cn

Java: u instanceof User
来源：http://bh.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://en.hahajie.cn

Ruby: u.is_a?(User)
来源：http://ao.panjiajie.cn

C#:   u is User
来源：http://td.gzmigu.cn

[G14] 数据类 / record
来源：http://bj.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gj.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://zu.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wo.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://me.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://im.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://yq.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://li.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://rs.colortex.cn

[G15] 枚举
来源：http://to.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vi.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vy.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iz.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hj.521024.cn

Java: enum Color { RED, GREEN }
来源：http://jn.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fg.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://cb.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qq.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://hm.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ah.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://vf.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://qx.colortex.cn

TS:   Object.entries(obj)
来源：http://be.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yy.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gu.szxytkj.cn

Ruby: obj.instance_variables
来源：http://kk.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://yf.shtwfgs.cn

================================================================================
来源：http://hm.wgjwhj.cn

H. 异常与错误处理
来源：http://jo.szsharing.cn

================================================================================
来源：http://vu.chemitech.net.cn

[H01] try / catch 基础
来源：http://yd.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://so.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xo.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aw.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gd.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zr.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bp.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vi.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hf.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://wy.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xf.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pa.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://of.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xv.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xn.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mz.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rt.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ur.nszjky.cn

[H03] 主动抛出异常
来源：http://lg.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://lu.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://za.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://cz.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://nt.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bo.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ts.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hs.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yy.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://ae.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://re.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eo.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://ac.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://ce.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://hu.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ex.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://lf.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://wd.panjiajie.cn

[H05] 捕获特定类型
来源：http://pj.hnjuh.cn

Py:   except ValueError as e:
来源：http://jg.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://de.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://em.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://jt.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://kh.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bh.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://wl.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://br.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://hb.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://uw.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lq.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kh.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hq.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ci.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zr.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://zm.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://qa.yuexingan06.cn

[H07] 断言
来源：http://du.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://au.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://cw.9csxet.cn

JS:   console.assert(x > 0);
来源：http://zo.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://sj.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://eb.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nn.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jj.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://aq.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://pp.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://et.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fl.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://fd.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zw.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kl.bjjhwx.cn

Go:   err.Error()
来源：http://kf.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://lg.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://tx.nszjky.cn

[H09] 带错误码的异常
来源：http://hu.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zf.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ci.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kr.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cf.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vp.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fx.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wg.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://id.szsharing.cn

[H10] 资源自动释放
来源：http://ab.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nc.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bf.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fm.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ih.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oc.szsharing.cn

Go:   defer f.Close()
来源：http://ad.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xs.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zr.jctech888.com.cn

================================================================================
来源：http://ao.jianghongdianzi.cn

I. 正则表达式
来源：http://lo.jctech888.com.cn

================================================================================
来源：http://yb.muxihuayi.cn

[I01] 判断是否匹配
来源：http://cy.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ct.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qw.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://uu.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://ir.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cl.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yf.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://uy.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://az.colortex.cn

[I02] 提取所有匹配
来源：http://to.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ih.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ki.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zj.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://lc.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ls.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gk.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://oy.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oo.shxzskj.cn

[I03] 提取捕获分组
来源：http://yw.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nd.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://li.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vx.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dm.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sf.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rd.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ph.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vw.jctech888.com.cn

[I04] 正则替换
来源：http://sj.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jl.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yx.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wg.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cw.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wb.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ae.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sr.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vu.yuexingan06.cn

[I05] 按正则拆分
来源：http://sa.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cj.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ch.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://to.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://sd.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://oh.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ma.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zy.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fn.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dq.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ft.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kv.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pl.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ek.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://id.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://se.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rj.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ez.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://da.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ke.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ly.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://su.colortex.cn

TS:   /error/gim
来源：http://fl.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wp.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gr.asd995.cn

Ruby: s.scan(/error/i)
来源：http://zs.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://od.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://yi.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lw.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bt.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xq.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vd.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ll.wgjwhj.cn


<!-- 参考信息 -->