代发 wailian999

Py:   class User: pass
来源：http://cx.asd995.cn

PHP:  class User {}
来源：http://za.asd995.cn

JS:   class User {}
来源：http://rt.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://pq.nicolike.cn

Java: class User {}
来源：http://vo.gzmigu.cn

Go:   type User struct { Name string }
来源：http://gh.asd995.cn

Ruby: class User; end
来源：http://eg.jctech888.com.cn

C#:   class User {}
来源：http://te.9csxet.cn

[G02] 构造函数
来源：http://ym.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://oz.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://es.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://xe.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://ye.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://rp.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bz.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://zc.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://dt.muxihuayi.cn

[G03] 实例属性
来源：http://gd.haigaiapp.cn

Py:   self.name = "x"
来源：http://il.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://zh.hnjuh.cn

JS:   this.name = "x";
来源：http://ao.chemitech.net.cn

TS:   name: string = "x";
来源：http://qw.haigaiapp.cn

Java: private String name;
来源：http://dn.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wh.9csxet.cn

Ruby: @name = "x"
来源：http://ac.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://zw.shxzukj.cn

[G04] 定义方法
来源：http://yo.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://ct.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fg.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://fq.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://wl.wgjwhj.cn

Java: String greet() { return name; }
来源：http://vc.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xl.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://uh.colortex.cn

C#:   public string Greet() => Name;
来源：http://ed.jctech888.com.cn

[G05] 继承
来源：http://ms.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://xz.newstarts.cn

PHP:  class Admin extends User {}
来源：http://pe.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://rg.asd995.cn

TS:   class Admin extends User {}
来源：http://xa.hahajie.cn

Java: class Admin extends User {}
来源：http://ee.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://om.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://ey.yuexingan06.cn

C#:   class Admin : User {}
来源：http://ja.jianghongdianzi.cn

[G06] 重写方法
来源：http://xd.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://yq.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ei.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://en.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://hl.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://mn.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dt.521024.cn

Ruby: def greet; "admin"; end
来源：http://ws.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://vh.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://ee.huixiangedu.cn

Py:   super().greet()
来源：http://mp.nszjky.cn

PHP:  parent::greet();
来源：http://xm.nicolike.cn

JS:   super.greet();
来源：http://vj.huixiangedu.cn

TS:   super.greet();
来源：http://ii.521024.cn

Java: super.greet();
来源：http://yv.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yh.colortex.cn

Ruby: super
来源：http://tu.szsharing.cn

C#:   base.Greet();
来源：http://ek.shtwfgs.cn

[G08] 静态方法与属性
来源：http://ym.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rh.chemitech.net.cn

PHP:  public static function f() {}
来源：http://au.shxzukj.cn

JS:   static f() {}
来源：http://zp.muxihuayi.cn

TS:   static f(): void {}
来源：http://sy.newstarts.cn

Java: static void f() {}
来源：http://ff.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://md.jctech888.com.cn

Ruby: def self.f; end
来源：http://hu.huanxung.cn

C#:   public static void F() {}
来源：http://bs.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://km.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://jx.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://re.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ol.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://vg.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://xg.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://lh.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eb.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://so.jianghongdianzi.cn

[G10] 访问控制
来源：http://zj.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://ql.huanxung.cn

PHP:  public / protected / private
来源：http://tq.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://nc.szxytkj.cn

TS:   public / protected / private
来源：http://lp.asd995.cn

Java: public / protected / private / 默认包级
来源：http://of.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bi.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ui.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://qx.huixiangedu.cn

[G11] getter / setter
来源：http://gn.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://zg.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lz.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://hd.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://he.shxzukj.cn

Java: public String getName() { return name; }
来源：http://em.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fi.hahajie.cn

Ruby: attr_accessor :name
来源：http://ln.colortex.cn

C#:   public string Name { get; set; }
来源：http://vn.huanxung.cn

[G12] 对象转字符串
来源：http://hv.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://mz.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gt.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://di.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://hs.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ut.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yq.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://iq.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://vt.gzmigu.cn

[G13] 判断对象类型
来源：http://gi.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://bo.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://jm.huixiangedu.cn

JS:   u instanceof User
来源：http://vm.521024.cn

TS:   u instanceof User
来源：http://jq.hnjuh.cn

Java: u instanceof User
来源：http://ag.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wm.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://jr.chemitech.net.cn

C#:   u is User
来源：http://ec.521024.cn

[G14] 数据类 / record
来源：http://qo.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://im.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://zo.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://he.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://bg.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://mp.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://ak.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://or.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://dp.521024.cn

[G15] 枚举
来源：http://fu.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zw.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uk.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kq.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ua.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://xn.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sx.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://gw.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ug.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://qw.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sz.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://oz.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://bq.hahajie.cn

TS:   Object.entries(obj)
来源：http://em.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vm.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hs.lnxyls.cn

Ruby: obj.instance_variables
来源：http://ec.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://nq.newstarts.cn

================================================================================
来源：http://ld.nicolike.cn

H. 异常与错误处理
来源：http://td.bjjhwx.cn

================================================================================
来源：http://ke.nszjky.cn

[H01] try / catch 基础
来源：http://nf.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oy.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qz.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jg.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nb.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ou.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qs.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://df.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vt.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://ac.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zg.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vk.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ye.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wc.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zv.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vf.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ic.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xr.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://lw.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://pb.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vx.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://ob.521024.cn

TS:   throw new Error("错误信息");
来源：http://qo.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://aw.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://we.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pz.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yx.gzmigu.cn

[H04] 自定义异常类型
来源：http://dx.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://hm.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sr.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://eo.521024.cn

TS:   class MyError extends Error {}
来源：http://nu.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://bg.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nj.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://kk.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://aj.huanxung.cn

[H05] 捕获特定类型
来源：http://dj.newstarts.cn

Py:   except ValueError as e:
来源：http://nf.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sm.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://kx.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://pz.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://lc.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jv.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://xa.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kb.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://fc.colortex.cn

Py:   value = d.get("k") or default
来源：http://ll.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lc.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kp.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xf.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hp.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jc.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://qo.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://rv.nszjky.cn

[H07] 断言
来源：http://bo.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://tj.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://nl.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://sj.hahajie.cn

TS:   console.assert(x > 0);
来源：http://kd.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://ct.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kc.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vi.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://lg.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://kp.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://su.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fc.szsharing.cn

JS:   e.message;  e.stack
来源：http://ut.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ru.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ys.521024.cn

Go:   err.Error()
来源：http://uy.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://ru.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://vd.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://rq.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://py.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fn.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fz.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wn.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ca.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mw.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://en.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yg.shxzskj.cn

[H10] 资源自动释放
来源：http://lm.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bx.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rm.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dh.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ea.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wd.szsharing.cn

Go:   defer f.Close()
来源：http://kt.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nh.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vi.jctech888.com.cn

================================================================================
来源：http://jb.shtwfgs.cn

I. 正则表达式
来源：http://lb.shtwfgs.cn

================================================================================
来源：http://np.colortex.cn

[I01] 判断是否匹配
来源：http://bg.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iy.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pe.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://mj.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://ms.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cu.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bg.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://ch.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ej.szsharing.cn

[I02] 提取所有匹配
来源：http://pv.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://mn.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ko.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eu.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://ln.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nh.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bk.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://dm.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wq.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://hm.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://be.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aw.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uk.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ll.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gm.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xj.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rv.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ni.lnxyls.cn

[I04] 正则替换
来源：http://lc.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bq.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ak.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xi.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yr.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ud.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xm.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jr.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mo.nszjky.cn

[I05] 按正则拆分
来源：http://vw.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hg.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pi.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://af.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://aa.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://bi.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aq.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nc.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vx.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sf.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aj.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ac.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zl.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://so.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ze.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ul.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sq.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xh.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://sx.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://op.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://te.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ow.huanxung.cn

TS:   /error/gim
来源：http://tw.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yh.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qz.jctech888.com.cn


<!-- 参考信息 -->