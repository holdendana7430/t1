代发 wailian999

================================================================================
来源：http://sn.huixinmuqiang.cn

G. 面向对象
来源：http://dh.asd995.cn

================================================================================
来源：http://xp.chemitech.net.cn

[G01] 定义类
来源：http://np.9csxet.cn

Py:   class User: pass
来源：http://wo.huanxung.cn

PHP:  class User {}
来源：http://aa.szxytkj.cn

JS:   class User {}
来源：http://rb.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://cz.colortex.cn

Java: class User {}
来源：http://lo.gzmigu.cn

Go:   type User struct { Name string }
来源：http://lq.yuntaijiaju.cn

Ruby: class User; end
来源：http://ec.shxzukj.cn

C#:   class User {}
来源：http://ya.panjiajie.cn

[G02] 构造函数
来源：http://lw.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ly.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ep.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://bl.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://ef.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://ug.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yz.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://yo.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://vm.521024.cn

[G03] 实例属性
来源：http://yg.huanxung.cn

Py:   self.name = "x"
来源：http://jq.szxytkj.cn

PHP:  public string $name = "x";
来源：http://qd.asd995.cn

JS:   this.name = "x";
来源：http://zb.wgjwhj.cn

TS:   name: string = "x";
来源：http://rd.huixiangedu.cn

Java: private String name;
来源：http://zr.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://np.nicolike.cn

Ruby: @name = "x"
来源：http://wq.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://sq.jianghongdianzi.cn

[G04] 定义方法
来源：http://gj.colortex.cn

Py:   def greet(self): return self.name
来源：http://ld.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ee.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://lw.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://pn.muxihuayi.cn

Java: String greet() { return name; }
来源：http://ny.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lz.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://zf.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://ov.newstarts.cn

[G05] 继承
来源：http://ej.huanxung.cn

Py:   class Admin(User): pass
来源：http://vn.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://iu.colortex.cn

JS:   class Admin extends User {}
来源：http://pt.asd995.cn

TS:   class Admin extends User {}
来源：http://at.haigaiapp.cn

Java: class Admin extends User {}
来源：http://jb.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vb.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://af.shxzskj.cn

C#:   class Admin : User {}
来源：http://xn.asd995.cn

[G06] 重写方法
来源：http://is.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://jh.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iz.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://pl.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://nk.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://wh.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hj.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://jy.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://zs.newstarts.cn

[G07] 调用父类方法
来源：http://sz.gzmigu.cn

Py:   super().greet()
来源：http://bt.panjiajie.cn

PHP:  parent::greet();
来源：http://ou.haigaiapp.cn

JS:   super.greet();
来源：http://eh.hahajie.cn

TS:   super.greet();
来源：http://jv.haigaiapp.cn

Java: super.greet();
来源：http://wa.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://di.gzmigu.cn

Ruby: super
来源：http://yl.jctech888.com.cn

C#:   base.Greet();
来源：http://nn.shtwfgs.cn

[G08] 静态方法与属性
来源：http://sg.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cl.huixiangedu.cn

PHP:  public static function f() {}
来源：http://ow.asd995.cn

JS:   static f() {}
来源：http://ul.chemitech.net.cn

TS:   static f(): void {}
来源：http://ef.shtwfgs.cn

Java: static void f() {}
来源：http://zi.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bx.asd995.cn

Ruby: def self.f; end
来源：http://no.panjiajie.cn

C#:   public static void F() {}
来源：http://py.521024.cn

[G09] 接口 / 抽象类
来源：http://jc.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://km.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vb.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fm.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://mf.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://io.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://sw.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lw.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://ha.bjjhwx.cn

[G10] 访问控制
来源：http://vt.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://ih.bookmarksfly.cn

PHP:  public / protected / private
来源：http://oi.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://ah.jctech888.com.cn

TS:   public / protected / private
来源：http://sg.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://xa.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bi.szsharing.cn

Ruby: public / protected / private
来源：http://kz.hahajie.cn

C#:   public / protected / private / internal
来源：http://xy.521024.cn

[G11] getter / setter
来源：http://te.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://nd.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xo.asd995.cn

JS:   get name() { return this._name; }
来源：http://ro.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://tf.9csxet.cn

Java: public String getName() { return name; }
来源：http://hz.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://db.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://pn.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://xp.huanxung.cn

[G12] 对象转字符串
来源：http://ww.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://nd.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ph.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://vg.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://nt.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://kp.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mn.521024.cn

Ruby: def to_s; @name; end
来源：http://rz.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://lx.nszjky.cn

[G13] 判断对象类型
来源：http://vq.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://re.lnxyls.cn

PHP:  $u instanceof User
来源：http://gg.yuexingan06.cn

JS:   u instanceof User
来源：http://vu.shxzukj.cn

TS:   u instanceof User
来源：http://vu.jianghongdianzi.cn

Java: u instanceof User
来源：http://iy.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nq.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://ob.hnjuh.cn

C#:   u is User
来源：http://th.bjjhwx.cn

[G14] 数据类 / record
来源：http://gz.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gw.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://sm.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ty.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://pt.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://nl.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://ns.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jb.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://pb.nszjky.cn

[G15] 枚举
来源：http://cm.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pq.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hm.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qh.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ix.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://mr.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://li.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://hg.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hi.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://vt.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dz.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://cu.szxytkj.cn

JS:   Object.entries(obj)
来源：http://oo.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://co.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bn.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kk.shxzskj.cn

Ruby: obj.instance_variables
来源：http://wp.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://vy.hahajie.cn

================================================================================
来源：http://tj.huixiangedu.cn

H. 异常与错误处理
来源：http://or.huanxung.cn

================================================================================
来源：http://td.huixiangedu.cn

[H01] try / catch 基础
来源：http://uo.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://je.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uq.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ri.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bh.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://li.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wy.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zd.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ta.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://ry.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qk.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pg.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jz.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ao.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://go.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nt.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ax.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ew.szsharing.cn

[H03] 主动抛出异常
来源：http://os.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://zz.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fb.asd995.cn

JS:   throw new Error("错误信息");
来源：http://kk.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://ta.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ct.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jj.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://km.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wb.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://ho.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://nz.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jh.9csxet.cn

JS:   class MyError extends Error {}
来源：http://fx.newstarts.cn

TS:   class MyError extends Error {}
来源：http://sg.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://ii.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://he.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://zw.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://ls.hahajie.cn

[H05] 捕获特定类型
来源：http://zg.bjjhwx.cn

Py:   except ValueError as e:
来源：http://yo.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jw.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://zg.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://uf.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://fu.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ps.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://eb.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cv.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://mx.521024.cn

Py:   value = d.get("k") or default
来源：http://tu.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lq.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cw.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cr.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vm.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kk.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://yz.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://xv.bookmarksfly.cn

[H07] 断言
来源：http://ig.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://wl.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://to.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://cz.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://ln.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://yt.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ml.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nr.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://bk.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://jr.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://bj.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yb.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://lx.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wq.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rx.nicolike.cn

Go:   err.Error()
来源：http://yx.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://mm.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://ow.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://zh.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hx.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dy.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gq.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ze.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kn.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://li.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ma.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xj.9csxet.cn

[H10] 资源自动释放
来源：http://wx.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oe.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://up.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zi.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kn.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uu.muxihuayi.cn

Go:   defer f.Close()
来源：http://vk.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sr.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tk.hahajie.cn

================================================================================
来源：http://hy.chemitech.net.cn

I. 正则表达式
来源：http://jx.nicolike.cn

================================================================================
来源：http://eh.chemitech.net.cn

[I01] 判断是否匹配
来源：http://el.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iz.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rb.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://xb.asd995.cn

TS:   /\d+/.test(s)
来源：http://xx.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qk.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ky.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://nd.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zv.wgjwhj.cn

[I02] 提取所有匹配
来源：http://ym.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://xj.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rt.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nr.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://gg.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sv.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://um.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://hz.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ig.szsharing.cn

[I03] 提取捕获分组
来源：http://ej.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qb.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yb.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fh.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vz.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nj.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xz.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sb.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bf.colortex.cn

[I04] 正则替换
来源：http://cm.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zr.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ze.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gj.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hd.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jl.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iz.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jx.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yz.panjiajie.cn

[I05] 按正则拆分
来源：http://rt.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gl.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cp.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://dv.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://sr.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://lq.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vo.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fn.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://om.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ap.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tu.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bz.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hl.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yd.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zn.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gs.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yu.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nh.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://cg.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ac.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fz.nszjky.cn


<!-- 参考信息 -->