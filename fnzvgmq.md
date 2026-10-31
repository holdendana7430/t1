代发 wailian999

[G02] 构造函数
来源：http://pt.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://kp.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://qc.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://gb.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://cg.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://xf.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jd.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://mn.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://vu.nszjky.cn

[G03] 实例属性
来源：http://mb.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://pb.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://vb.wgjwhj.cn

JS:   this.name = "x";
来源：http://ic.haigaiapp.cn

TS:   name: string = "x";
来源：http://bs.nszjky.cn

Java: private String name;
来源：http://dm.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tt.yuexingan06.cn

Ruby: @name = "x"
来源：http://lh.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://fg.jianghongdianzi.cn

[G04] 定义方法
来源：http://kc.huanxung.cn

Py:   def greet(self): return self.name
来源：http://hy.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aw.9csxet.cn

JS:   greet() { return this.name; }
来源：http://kn.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://uz.muxihuayi.cn

Java: String greet() { return name; }
来源：http://ef.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vx.newstarts.cn

Ruby: def greet; @name; end
来源：http://pz.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://zx.haigaiapp.cn

[G05] 继承
来源：http://yz.szxytkj.cn

Py:   class Admin(User): pass
来源：http://kb.nicolike.cn

PHP:  class Admin extends User {}
来源：http://ii.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://kp.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://zg.gzmigu.cn

Java: class Admin extends User {}
来源：http://bg.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tz.szsharing.cn

Ruby: class Admin < User; end
来源：http://nd.szxytkj.cn

C#:   class Admin : User {}
来源：http://ob.panjiajie.cn

[G06] 重写方法
来源：http://sz.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://nz.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nf.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://te.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://hv.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://jq.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ty.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://ju.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://ov.hahajie.cn

[G07] 调用父类方法
来源：http://ky.chemitech.net.cn

Py:   super().greet()
来源：http://dp.bookmarksfly.cn

PHP:  parent::greet();
来源：http://wg.bookmarksfly.cn

JS:   super.greet();
来源：http://cf.huixiangedu.cn

TS:   super.greet();
来源：http://rm.shtwfgs.cn

Java: super.greet();
来源：http://zl.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://th.panjiajie.cn

Ruby: super
来源：http://fu.szsharing.cn

C#:   base.Greet();
来源：http://fv.gzmigu.cn

[G08] 静态方法与属性
来源：http://pw.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://th.shxzukj.cn

PHP:  public static function f() {}
来源：http://jc.shtwfgs.cn

JS:   static f() {}
来源：http://xd.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://nk.szsharing.cn

Java: static void f() {}
来源：http://hg.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qp.lnxyls.cn

Ruby: def self.f; end
来源：http://zz.shxzukj.cn

C#:   public static void F() {}
来源：http://he.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://rd.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://wh.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jk.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://si.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://gt.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://ht.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ox.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wx.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://wc.szsharing.cn

[G10] 访问控制
来源：http://fk.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://eb.asd995.cn

PHP:  public / protected / private
来源：http://oj.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://tc.jianghongdianzi.cn

TS:   public / protected / private
来源：http://pe.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://ux.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vy.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://rt.panjiajie.cn

C#:   public / protected / private / internal
来源：http://wa.wgjwhj.cn

[G11] getter / setter
来源：http://bh.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://oz.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://se.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://vs.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://un.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://xe.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://du.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://gl.nicolike.cn

C#:   public string Name { get; set; }
来源：http://ej.newstarts.cn

[G12] 对象转字符串
来源：http://xp.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://lh.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fj.szsharing.cn

JS:   toString() { return this.name; }
来源：http://gp.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://fz.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://yx.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dr.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://ri.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://se.521024.cn

[G13] 判断对象类型
来源：http://iq.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://gf.shxzukj.cn

PHP:  $u instanceof User
来源：http://wv.jctech888.com.cn

JS:   u instanceof User
来源：http://gt.newstarts.cn

TS:   u instanceof User
来源：http://ad.521024.cn

Java: u instanceof User
来源：http://ia.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gq.nszjky.cn

Ruby: u.is_a?(User)
来源：http://vg.huixiangedu.cn

C#:   u is User
来源：http://dz.wgjwhj.cn

[G14] 数据类 / record
来源：http://zz.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sr.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://yo.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gr.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://me.szsharing.cn

Java: record User(String name, int age) {}
来源：http://dk.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://nr.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jr.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://wt.521024.cn

[G15] 枚举
来源：http://cx.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qg.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uf.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://td.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://la.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://wb.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ah.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://oz.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hm.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://pl.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lq.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://ts.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://qz.shxzskj.cn

TS:   Object.entries(obj)
来源：http://oz.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uh.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://di.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://lc.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://zv.9csxet.cn

================================================================================
来源：http://lm.hnjuh.cn

H. 异常与错误处理
来源：http://wx.asd995.cn

================================================================================
来源：http://op.newstarts.cn

[H01] try / catch 基础
来源：http://xq.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gg.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mu.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wv.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oe.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vu.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wu.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kn.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zz.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://zz.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://io.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oz.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qs.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xe.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dp.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ft.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ym.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rx.bjjhwx.cn

[H03] 主动抛出异常
来源：http://kt.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://fs.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ee.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://hi.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://ry.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kj.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iv.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cu.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tb.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://cu.521024.cn

Py:   class MyError(Exception): pass
来源：http://xc.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://br.521024.cn

JS:   class MyError extends Error {}
来源：http://ty.newstarts.cn

TS:   class MyError extends Error {}
来源：http://nc.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://id.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nd.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://ee.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://xk.521024.cn

[H05] 捕获特定类型
来源：http://zi.hnjuh.cn

Py:   except ValueError as e:
来源：http://vl.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tr.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://yp.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://uq.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://ly.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qk.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://fz.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jv.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://ye.nszjky.cn

Py:   value = d.get("k") or default
来源：http://ca.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dc.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pc.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ld.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ld.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sw.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://er.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://sz.yuntaijiaju.cn

[H07] 断言
来源：http://ya.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://ww.szxytkj.cn

PHP:  assert($x > 0);
来源：http://nt.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://fg.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://je.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://xc.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kf.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gf.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://lm.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://ar.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://jo.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fm.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://kf.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wa.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ku.hahajie.cn

Go:   err.Error()
来源：http://my.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://nu.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://qt.jctech888.com.cn

[H09] 带错误码的异常
来源：http://fz.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wf.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://om.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qn.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oa.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yx.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gf.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fl.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fe.huixiangedu.cn

[H10] 资源自动释放
来源：http://wa.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vs.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ck.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qm.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ra.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ei.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://hm.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tv.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ml.panjiajie.cn

================================================================================
来源：http://zg.gzmigu.cn

I. 正则表达式
来源：http://yt.huixinmuqiang.cn

================================================================================
来源：http://kq.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://ld.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xn.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ut.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://vp.nszjky.cn

TS:   /\d+/.test(s)
来源：http://sy.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hq.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ct.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://nz.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xb.huanxung.cn

[I02] 提取所有匹配
来源：http://wr.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://lw.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bw.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qv.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://pp.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gm.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wa.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://qe.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mj.asd995.cn

[I03] 提取捕获分组
来源：http://fr.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yl.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kn.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kt.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ej.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ta.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uq.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oo.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wl.colortex.cn

[I04] 正则替换
来源：http://rr.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wa.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bs.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yv.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://af.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dc.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gg.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gg.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bq.9csxet.cn

[I05] 按正则拆分
来源：http://xu.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hp.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nr.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://mi.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://ym.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://zg.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://im.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ka.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vt.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xk.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ru.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sa.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tb.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yu.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sd.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cu.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yk.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://au.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://rt.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hh.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cv.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cd.muxihuayi.cn

TS:   /error/gim
来源：http://qm.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qs.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qe.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://ga.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pd.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://ti.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xu.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nz.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ut.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mr.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cn.shtwfgs.cn


<!-- 参考信息 -->