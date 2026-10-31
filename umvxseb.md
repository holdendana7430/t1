代发 wailian999

Py:   class User: pass
来源：http://xc.haigaiapp.cn

PHP:  class User {}
来源：http://er.huixiangedu.cn

JS:   class User {}
来源：http://ql.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://jj.yuntaijiaju.cn

Java: class User {}
来源：http://zv.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://vi.huanxung.cn

Ruby: class User; end
来源：http://yv.jctech888.com.cn

C#:   class User {}
来源：http://kg.wgjwhj.cn

[G02] 构造函数
来源：http://ze.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ol.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://mk.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://op.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://ht.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://rj.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kc.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://ix.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://ij.shxzskj.cn

[G03] 实例属性
来源：http://uc.szsharing.cn

Py:   self.name = "x"
来源：http://zn.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://qr.muxihuayi.cn

JS:   this.name = "x";
来源：http://hf.yuexingan06.cn

TS:   name: string = "x";
来源：http://cr.asd995.cn

Java: private String name;
来源：http://nq.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gi.newstarts.cn

Ruby: @name = "x"
来源：http://iv.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://zj.bjjhwx.cn

[G04] 定义方法
来源：http://yi.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://sr.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yt.9csxet.cn

JS:   greet() { return this.name; }
来源：http://va.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://rt.jctech888.com.cn

Java: String greet() { return name; }
来源：http://vw.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wu.asd995.cn

Ruby: def greet; @name; end
来源：http://kn.newstarts.cn

C#:   public string Greet() => Name;
来源：http://vb.nicolike.cn

[G05] 继承
来源：http://eq.szxytkj.cn

Py:   class Admin(User): pass
来源：http://mw.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://cf.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://le.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://lr.nszjky.cn

Java: class Admin extends User {}
来源：http://ac.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://io.colortex.cn

Ruby: class Admin < User; end
来源：http://pk.521024.cn

C#:   class Admin : User {}
来源：http://hs.huixiangedu.cn

[G06] 重写方法
来源：http://th.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://ig.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ey.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://nb.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://tr.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://rz.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lx.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://lg.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://ck.szxytkj.cn

[G07] 调用父类方法
来源：http://ph.asd995.cn

Py:   super().greet()
来源：http://we.muxihuayi.cn

PHP:  parent::greet();
来源：http://ng.bookmarksfly.cn

JS:   super.greet();
来源：http://oy.asd995.cn

TS:   super.greet();
来源：http://ns.jianghongdianzi.cn

Java: super.greet();
来源：http://hp.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sc.jctech888.com.cn

Ruby: super
来源：http://yd.panjiajie.cn

C#:   base.Greet();
来源：http://qt.chemitech.net.cn

[G08] 静态方法与属性
来源：http://lf.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qv.wgjwhj.cn

PHP:  public static function f() {}
来源：http://ie.9csxet.cn

JS:   static f() {}
来源：http://wu.lnxyls.cn

TS:   static f(): void {}
来源：http://kq.9csxet.cn

Java: static void f() {}
来源：http://yr.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ru.nszjky.cn

Ruby: def self.f; end
来源：http://jg.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://xw.521024.cn

[G09] 接口 / 抽象类
来源：http://le.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://sr.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ry.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jg.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://bb.nicolike.cn

Java: interface Shape { double area(); }
来源：http://ht.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://dc.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hw.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://ar.hnjuh.cn

[G10] 访问控制
来源：http://fi.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://zr.bjjhwx.cn

PHP:  public / protected / private
来源：http://dn.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://ff.wgjwhj.cn

TS:   public / protected / private
来源：http://re.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://do.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wa.nicolike.cn

Ruby: public / protected / private
来源：http://gh.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://wg.haigaiapp.cn

[G11] getter / setter
来源：http://jz.hahajie.cn

Py:   @property 与 @x.setter
来源：http://nz.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ga.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://nz.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://sb.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://yj.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ym.szxytkj.cn

Ruby: attr_accessor :name
来源：http://tz.nszjky.cn

C#:   public string Name { get; set; }
来源：http://ce.colortex.cn

[G12] 对象转字符串
来源：http://im.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://wq.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qz.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://ox.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://id.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://xc.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sw.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://cd.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://zp.521024.cn

[G13] 判断对象类型
来源：http://no.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://pr.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://ci.bjjhwx.cn

JS:   u instanceof User
来源：http://yz.nicolike.cn

TS:   u instanceof User
来源：http://ti.jctech888.com.cn

Java: u instanceof User
来源：http://if.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://va.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://az.haigaiapp.cn

C#:   u is User
来源：http://mb.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://cg.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qo.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://ah.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uw.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://rd.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://ue.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://ez.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jn.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://rv.hahajie.cn

[G15] 枚举
来源：http://vu.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pn.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oo.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yq.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xr.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://vg.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mx.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://oz.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ok.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://cj.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lh.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://bs.521024.cn

JS:   Object.entries(obj)
来源：http://bg.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://du.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cq.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rd.nszjky.cn

Ruby: obj.instance_variables
来源：http://ml.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://bt.asd995.cn

================================================================================
来源：http://km.panjiajie.cn

H. 异常与错误处理
来源：http://yq.muxihuayi.cn

================================================================================
来源：http://od.szxytkj.cn

[H01] try / catch 基础
来源：http://iw.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jx.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ej.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ji.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ty.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gw.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oo.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iy.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kw.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://jp.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://al.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sk.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ss.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cy.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yc.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rw.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iy.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kg.lnxyls.cn

[H03] 主动抛出异常
来源：http://gb.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://ro.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dk.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://yc.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://ds.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oq.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ff.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zg.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ty.asd995.cn

[H04] 自定义异常类型
来源：http://mi.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://lc.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cc.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://xw.nicolike.cn

TS:   class MyError extends Error {}
来源：http://om.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://np.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mt.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://wo.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://kq.huanxung.cn

[H05] 捕获特定类型
来源：http://bh.hnjuh.cn

Py:   except ValueError as e:
来源：http://cj.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tj.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://eo.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://tm.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://jp.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jm.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://bs.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jm.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://zh.521024.cn

Py:   value = d.get("k") or default
来源：http://hh.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cw.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nj.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lj.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qk.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sk.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://qm.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://zh.lnxyls.cn

[H07] 断言
来源：http://qz.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://um.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://qb.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://un.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ue.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://cq.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mu.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lq.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://bh.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://td.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://gq.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zm.hahajie.cn

JS:   e.message;  e.stack
来源：http://gd.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nn.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ge.panjiajie.cn

Go:   err.Error()
来源：http://ii.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://by.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://zw.szxytkj.cn

[H09] 带错误码的异常
来源：http://ji.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://on.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nm.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ka.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fk.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://un.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ff.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bk.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cy.shxzskj.cn

[H10] 资源自动释放
来源：http://ht.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://am.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eq.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://al.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iq.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wv.hahajie.cn

Go:   defer f.Close()
来源：http://tv.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hp.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vp.bookmarksfly.cn

================================================================================
来源：http://ri.panjiajie.cn

I. 正则表达式
来源：http://sl.szsharing.cn

================================================================================
来源：http://to.muxihuayi.cn

[I01] 判断是否匹配
来源：http://xj.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wg.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mz.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://pv.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://ou.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zc.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aq.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://in.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iv.9csxet.cn

[I02] 提取所有匹配
来源：http://ef.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://nn.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iu.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yk.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://rv.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qs.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qy.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ho.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gn.muxihuayi.cn

[I03] 提取捕获分组
来源：http://aw.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nl.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rt.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://db.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yl.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://db.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yu.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iv.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gc.bookmarksfly.cn

[I04] 正则替换
来源：http://gn.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nf.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tz.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://no.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uc.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bb.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ye.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wr.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://og.9csxet.cn

[I05] 按正则拆分
来源：http://aj.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iv.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oz.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://vv.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://xn.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://ij.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lb.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zx.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nj.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ly.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xh.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nw.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uq.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ls.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xg.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gg.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oq.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jf.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://fl.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ou.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rg.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tn.nszjky.cn

TS:   /error/gim
来源：http://qe.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zl.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gt.shxzskj.cn


<!-- 参考信息 -->