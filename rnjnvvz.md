代发 wailian999

================================================================================
来源：http://xl.huixiangedu.cn

G. 面向对象
来源：http://um.shtwfgs.cn

================================================================================
来源：http://jg.hahajie.cn

[G01] 定义类
来源：http://kn.shxzukj.cn

Py:   class User: pass
来源：http://na.bookmarksfly.cn

PHP:  class User {}
来源：http://hv.asd995.cn

JS:   class User {}
来源：http://kz.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://bt.jctech888.com.cn

Java: class User {}
来源：http://vk.shxzukj.cn

Go:   type User struct { Name string }
来源：http://qm.nicolike.cn

Ruby: class User; end
来源：http://xd.newstarts.cn

C#:   class User {}
来源：http://bh.szsharing.cn

[G02] 构造函数
来源：http://ly.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://xv.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://qo.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://vr.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://sy.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://wk.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lu.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://oi.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://zm.panjiajie.cn

[G03] 实例属性
来源：http://qq.nszjky.cn

Py:   self.name = "x"
来源：http://qp.hnjuh.cn

PHP:  public string $name = "x";
来源：http://rd.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://ez.newstarts.cn

TS:   name: string = "x";
来源：http://xj.szsharing.cn

Java: private String name;
来源：http://xr.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zn.haigaiapp.cn

Ruby: @name = "x"
来源：http://zr.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ax.hahajie.cn

[G04] 定义方法
来源：http://ff.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://lj.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ie.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://dq.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://em.muxihuayi.cn

Java: String greet() { return name; }
来源：http://nx.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wn.9csxet.cn

Ruby: def greet; @name; end
来源：http://yt.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://im.hahajie.cn

[G05] 继承
来源：http://fs.lnxyls.cn

Py:   class Admin(User): pass
来源：http://wv.9csxet.cn

PHP:  class Admin extends User {}
来源：http://dm.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://ox.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://gs.shxzskj.cn

Java: class Admin extends User {}
来源：http://xh.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xw.nicolike.cn

Ruby: class Admin < User; end
来源：http://cl.nicolike.cn

C#:   class Admin : User {}
来源：http://ug.huixiangedu.cn

[G06] 重写方法
来源：http://xd.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://vg.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dm.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://fo.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://ry.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://rs.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zy.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://ti.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://no.muxihuayi.cn

[G07] 调用父类方法
来源：http://di.newstarts.cn

Py:   super().greet()
来源：http://lt.muxihuayi.cn

PHP:  parent::greet();
来源：http://vl.yuntaijiaju.cn

JS:   super.greet();
来源：http://cd.nszjky.cn

TS:   super.greet();
来源：http://kr.shxzukj.cn

Java: super.greet();
来源：http://ka.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://up.9csxet.cn

Ruby: super
来源：http://vt.jianghongdianzi.cn

C#:   base.Greet();
来源：http://qq.gzmigu.cn

[G08] 静态方法与属性
来源：http://yz.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://im.asd995.cn

PHP:  public static function f() {}
来源：http://oz.shtwfgs.cn

JS:   static f() {}
来源：http://zv.huixiangedu.cn

TS:   static f(): void {}
来源：http://ag.chemitech.net.cn

Java: static void f() {}
来源：http://ug.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hw.huanxung.cn

Ruby: def self.f; end
来源：http://oj.chemitech.net.cn

C#:   public static void F() {}
来源：http://dg.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://wn.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://wc.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cm.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wd.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://ex.asd995.cn

Java: interface Shape { double area(); }
来源：http://lv.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://yl.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wx.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://xm.521024.cn

[G10] 访问控制
来源：http://dk.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://rh.huanxung.cn

PHP:  public / protected / private
来源：http://bw.colortex.cn

JS:   #private 字段；其余公开
来源：http://rl.wgjwhj.cn

TS:   public / protected / private
来源：http://ol.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://qe.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rk.nicolike.cn

Ruby: public / protected / private
来源：http://xl.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://tg.yuexingan06.cn

[G11] getter / setter
来源：http://hz.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://xd.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gq.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://vw.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://lg.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://hi.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tg.hnjuh.cn

Ruby: attr_accessor :name
来源：http://vz.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://rf.lnxyls.cn

[G12] 对象转字符串
来源：http://vp.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://zd.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rc.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://yz.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://im.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://ps.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ul.9csxet.cn

Ruby: def to_s; @name; end
来源：http://wo.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://te.hahajie.cn

[G13] 判断对象类型
来源：http://fv.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://cr.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://ez.szxytkj.cn

JS:   u instanceof User
来源：http://ua.nicolike.cn

TS:   u instanceof User
来源：http://kr.panjiajie.cn

Java: u instanceof User
来源：http://kj.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kg.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://eu.colortex.cn

C#:   u is User
来源：http://wc.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://sf.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fp.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://ei.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ny.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://vj.nicolike.cn

Java: record User(String name, int age) {}
来源：http://nd.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://yw.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bl.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://rq.jianghongdianzi.cn

[G15] 枚举
来源：http://lo.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sj.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://em.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://po.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mt.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://uy.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kh.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://kv.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://te.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://di.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mo.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://vb.nicolike.cn

JS:   Object.entries(obj)
来源：http://la.szxytkj.cn

TS:   Object.entries(obj)
来源：http://bf.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zj.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sf.huanxung.cn

Ruby: obj.instance_variables
来源：http://tn.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://ij.yuexingan06.cn

================================================================================
来源：http://dx.huanxung.cn

H. 异常与错误处理
来源：http://li.gzmigu.cn

================================================================================
来源：http://ea.huixiangedu.cn

[H01] try / catch 基础
来源：http://hd.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nb.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gt.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nx.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lh.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pc.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ol.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cp.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yj.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://dl.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wg.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xq.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fg.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jm.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ap.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ej.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ge.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wk.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://kg.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://ql.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nb.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://ic.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://nt.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ku.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ny.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dm.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qi.wgjwhj.cn

[H04] 自定义异常类型
来源：http://rg.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://na.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uw.szsharing.cn

JS:   class MyError extends Error {}
来源：http://sm.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://nu.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://ov.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pw.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://mc.nszjky.cn

C#:   class MyException : Exception {}
来源：http://na.521024.cn

[H05] 捕获特定类型
来源：http://wq.gzmigu.cn

Py:   except ValueError as e:
来源：http://pu.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xb.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://xw.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://mf.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://wi.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bh.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://fd.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eg.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://oe.newstarts.cn

Py:   value = d.get("k") or default
来源：http://hw.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://or.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mu.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fu.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xl.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ps.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://yv.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://rd.chemitech.net.cn

[H07] 断言
来源：http://gu.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://wb.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://ov.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://hp.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://mi.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://ud.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://le.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yb.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://nx.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://rl.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://oi.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xv.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://bd.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ru.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jb.521024.cn

Go:   err.Error()
来源：http://is.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://ru.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://wz.lnxyls.cn

[H09] 带错误码的异常
来源：http://lb.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hs.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ju.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ij.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yd.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qh.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://td.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cw.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wt.521024.cn

[H10] 资源自动释放
来源：http://xp.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cn.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yo.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vj.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lm.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hahajie.cn

Go:   defer f.Close()
来源：http://me.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ev.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xk.szsharing.cn

================================================================================
来源：http://fb.shxzskj.cn

I. 正则表达式
来源：http://wm.gzmigu.cn

================================================================================
来源：http://sf.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://ao.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xe.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rk.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://uw.nszjky.cn

TS:   /\d+/.test(s)
来源：http://tr.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dq.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yk.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://sh.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oq.521024.cn

[I02] 提取所有匹配
来源：http://ns.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://gd.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cb.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gr.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://dz.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ve.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ou.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://xb.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sn.gzmigu.cn

[I03] 提取捕获分组
来源：http://lp.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xa.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dj.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://if.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zg.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hd.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jy.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://df.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ne.colortex.cn

[I04] 正则替换
来源：http://aa.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dk.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://im.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sz.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pq.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vo.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gk.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aw.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rg.nszjky.cn

[I05] 按正则拆分
来源：http://xm.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hv.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zi.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://gt.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://mt.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://nr.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xi.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kd.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qb.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tc.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ty.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://os.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dn.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qz.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mz.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yg.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dz.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jg.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://fl.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fz.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ou.newstarts.cn


<!-- 参考信息 -->