代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://an.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tk.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wd.colortex.cn

TS:   // 同上
来源：http://ep.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wu.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yc.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://is.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gp.wgjwhj.cn

================================================================================
来源：http://oe.colortex.cn

G. 面向对象
来源：http://et.szsharing.cn

================================================================================
来源：http://gq.jianghongdianzi.cn

[G01] 定义类
来源：http://sk.nicolike.cn

Py:   class User: pass
来源：http://bp.bjjhwx.cn

PHP:  class User {}
来源：http://cv.yuexingan06.cn

JS:   class User {}
来源：http://ut.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://lz.shxzskj.cn

Java: class User {}
来源：http://uq.lnxyls.cn

Go:   type User struct { Name string }
来源：http://mx.panjiajie.cn

Ruby: class User; end
来源：http://ef.hnjuh.cn

C#:   class User {}
来源：http://ed.yuexingan06.cn

[G02] 构造函数
来源：http://uj.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://tk.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://ue.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://ab.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://zp.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://ui.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uo.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://rw.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://lt.huanxung.cn

[G03] 实例属性
来源：http://sc.panjiajie.cn

Py:   self.name = "x"
来源：http://uc.gzmigu.cn

PHP:  public string $name = "x";
来源：http://ip.shxzukj.cn

JS:   this.name = "x";
来源：http://is.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://qs.hnjuh.cn

Java: private String name;
来源：http://ew.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rc.gzmigu.cn

Ruby: @name = "x"
来源：http://ii.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://tf.chemitech.net.cn

[G04] 定义方法
来源：http://qm.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://ny.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xd.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://xf.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://hi.shxzukj.cn

Java: String greet() { return name; }
来源：http://to.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nf.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://lz.asd995.cn

C#:   public string Greet() => Name;
来源：http://wp.shtwfgs.cn

[G05] 继承
来源：http://em.521024.cn

Py:   class Admin(User): pass
来源：http://gb.nszjky.cn

PHP:  class Admin extends User {}
来源：http://oa.521024.cn

JS:   class Admin extends User {}
来源：http://bz.szxytkj.cn

TS:   class Admin extends User {}
来源：http://yo.haigaiapp.cn

Java: class Admin extends User {}
来源：http://bo.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://id.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://xq.chemitech.net.cn

C#:   class Admin : User {}
来源：http://wx.colortex.cn

[G06] 重写方法
来源：http://lj.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://oe.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lt.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://nn.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://kr.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://vl.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ff.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://mz.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://eh.bookmarksfly.cn

[G07] 调用父类方法
来源：http://tt.panjiajie.cn

Py:   super().greet()
来源：http://as.9csxet.cn

PHP:  parent::greet();
来源：http://ie.bookmarksfly.cn

JS:   super.greet();
来源：http://fk.nicolike.cn

TS:   super.greet();
来源：http://mo.haigaiapp.cn

Java: super.greet();
来源：http://uc.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mt.yuexingan06.cn

Ruby: super
来源：http://gr.bjjhwx.cn

C#:   base.Greet();
来源：http://fh.shxzskj.cn

[G08] 静态方法与属性
来源：http://tk.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bc.nszjky.cn

PHP:  public static function f() {}
来源：http://iq.huanxung.cn

JS:   static f() {}
来源：http://lp.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://mw.hnjuh.cn

Java: static void f() {}
来源：http://aj.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kx.bookmarksfly.cn

Ruby: def self.f; end
来源：http://dt.521024.cn

C#:   public static void F() {}
来源：http://mx.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://jo.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://df.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lv.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vp.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://du.hahajie.cn

Java: interface Shape { double area(); }
来源：http://mi.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://pe.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ih.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://hf.lnxyls.cn

[G10] 访问控制
来源：http://dp.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://tl.hahajie.cn

PHP:  public / protected / private
来源：http://qq.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://nm.huixiangedu.cn

TS:   public / protected / private
来源：http://gf.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://ke.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dj.panjiajie.cn

Ruby: public / protected / private
来源：http://wp.newstarts.cn

C#:   public / protected / private / internal
来源：http://pj.gzmigu.cn

[G11] getter / setter
来源：http://nt.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ou.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jg.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://an.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://tf.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://jb.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pz.9csxet.cn

Ruby: attr_accessor :name
来源：http://bb.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://ie.lnxyls.cn

[G12] 对象转字符串
来源：http://hm.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://ta.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xr.szsharing.cn

JS:   toString() { return this.name; }
来源：http://cx.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://ol.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://nm.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fi.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://ru.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://eq.chemitech.net.cn

[G13] 判断对象类型
来源：http://yb.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://av.nszjky.cn

PHP:  $u instanceof User
来源：http://oz.lnxyls.cn

JS:   u instanceof User
来源：http://gw.muxihuayi.cn

TS:   u instanceof User
来源：http://wc.521024.cn

Java: u instanceof User
来源：http://zy.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vv.521024.cn

Ruby: u.is_a?(User)
来源：http://tm.9csxet.cn

C#:   u is User
来源：http://sh.shxzskj.cn

[G14] 数据类 / record
来源：http://zr.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xv.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://in.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eo.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://vi.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://ei.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://eg.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cr.colortex.cn

C#:   record User(string Name, int Age);
来源：http://ha.hnjuh.cn

[G15] 枚举
来源：http://an.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pi.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://je.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://na.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pt.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://yp.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ue.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://ca.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ti.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://rm.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bl.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://pm.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ks.panjiajie.cn

TS:   Object.entries(obj)
来源：http://hk.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ap.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ex.asd995.cn

Ruby: obj.instance_variables
来源：http://zu.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://dw.gzmigu.cn

================================================================================
来源：http://ny.gzmigu.cn

H. 异常与错误处理
来源：http://zi.asd995.cn

================================================================================
来源：http://zy.shtwfgs.cn

[H01] try / catch 基础
来源：http://pn.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hm.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gs.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wa.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zw.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nc.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nw.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gy.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://us.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://mm.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jk.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pl.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sh.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oq.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://go.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xt.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ya.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bg.jctech888.com.cn

[H03] 主动抛出异常
来源：http://fb.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://wo.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ep.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://ub.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://bd.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mf.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vh.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xd.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ov.9csxet.cn

[H04] 自定义异常类型
来源：http://xb.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://yl.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rs.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://sy.nicolike.cn

TS:   class MyError extends Error {}
来源：http://vz.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://cw.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cm.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ye.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://di.huanxung.cn

[H05] 捕获特定类型
来源：http://gt.szsharing.cn

Py:   except ValueError as e:
来源：http://gz.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ta.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://yx.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ut.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://dz.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bf.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://xm.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cg.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://eo.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://qf.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sh.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xu.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gu.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kf.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nj.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://ts.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://kp.shtwfgs.cn

[H07] 断言
来源：http://jv.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://dw.gzmigu.cn

PHP:  assert($x > 0);
来源：http://sh.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://ul.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://ef.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://fy.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yr.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://se.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://bw.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://mz.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://ir.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ak.shxzskj.cn

JS:   e.message;  e.stack
来源：http://lz.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wg.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tk.jianghongdianzi.cn

Go:   err.Error()
来源：http://zm.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://gm.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://nq.szsharing.cn

[H09] 带错误码的异常
来源：http://za.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lx.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hq.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://km.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pg.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tm.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gq.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dp.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vr.shtwfgs.cn

[H10] 资源自动释放
来源：http://nj.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tl.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sn.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ef.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cl.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ik.panjiajie.cn

Go:   defer f.Close()
来源：http://ve.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dy.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kj.bookmarksfly.cn

================================================================================
来源：http://ye.gzmigu.cn

I. 正则表达式
来源：http://xv.shtwfgs.cn

================================================================================
来源：http://vc.szxytkj.cn

[I01] 判断是否匹配
来源：http://vx.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hq.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sg.colortex.cn

JS:   /\d+/.test(s)
来源：http://zy.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://op.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://op.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bo.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://lu.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nq.shxzskj.cn

[I02] 提取所有匹配
来源：http://oi.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://kc.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ca.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xt.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://kn.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fe.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eu.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://tm.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yp.nicolike.cn

[I03] 提取捕获分组
来源：http://hi.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bg.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pu.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mu.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://do.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kl.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sz.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mn.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yx.huixinmuqiang.cn

[I04] 正则替换
来源：http://iy.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zq.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ny.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wz.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pv.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zs.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://td.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ng.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yx.bookmarksfly.cn

[I05] 按正则拆分
来源：http://wk.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://az.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gw.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://af.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://hl.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ou.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qu.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hr.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qn.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hy.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zk.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ia.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jj.lnxyls.cn


<!-- 参考信息 -->