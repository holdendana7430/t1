代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://to.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wl.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hj.nszjky.cn

[F12] CSV 读写
来源：http://un.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xp.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ym.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tu.jianghongdianzi.cn

TS:   // 同上
来源：http://xa.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yb.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iy.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gc.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qs.9csxet.cn

================================================================================
来源：http://jz.shxzukj.cn

G. 面向对象
来源：http://vr.nicolike.cn

================================================================================
来源：http://je.shxzukj.cn

[G01] 定义类
来源：http://tj.haigaiapp.cn

Py:   class User: pass
来源：http://bp.shxzukj.cn

PHP:  class User {}
来源：http://jo.haigaiapp.cn

JS:   class User {}
来源：http://uo.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://nf.gzmigu.cn

Java: class User {}
来源：http://jf.hnjuh.cn

Go:   type User struct { Name string }
来源：http://cd.szxytkj.cn

Ruby: class User; end
来源：http://co.chemitech.net.cn

C#:   class User {}
来源：http://fq.yuexingan06.cn

[G02] 构造函数
来源：http://cq.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://lj.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://fg.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://nq.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://nh.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://fz.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://os.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://ie.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://hb.hnjuh.cn

[G03] 实例属性
来源：http://rp.hahajie.cn

Py:   self.name = "x"
来源：http://qu.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://bd.haigaiapp.cn

JS:   this.name = "x";
来源：http://ex.muxihuayi.cn

TS:   name: string = "x";
来源：http://fs.shtwfgs.cn

Java: private String name;
来源：http://sm.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nr.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://yu.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://cr.huixinmuqiang.cn

[G04] 定义方法
来源：http://wv.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://sv.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eu.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://vf.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://sr.hnjuh.cn

Java: String greet() { return name; }
来源：http://gy.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zj.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://ho.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://ik.haigaiapp.cn

[G05] 继承
来源：http://as.nszjky.cn

Py:   class Admin(User): pass
来源：http://se.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://xj.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://lz.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://gu.haigaiapp.cn

Java: class Admin extends User {}
来源：http://fj.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lu.huanxung.cn

Ruby: class Admin < User; end
来源：http://zd.lnxyls.cn

C#:   class Admin : User {}
来源：http://kd.szsharing.cn

[G06] 重写方法
来源：http://jb.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://hi.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tu.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://td.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://ly.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://vr.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pf.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://in.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://kf.jctech888.com.cn

[G07] 调用父类方法
来源：http://ia.nicolike.cn

Py:   super().greet()
来源：http://xq.newstarts.cn

PHP:  parent::greet();
来源：http://jn.muxihuayi.cn

JS:   super.greet();
来源：http://ll.asd995.cn

TS:   super.greet();
来源：http://jt.bjjhwx.cn

Java: super.greet();
来源：http://wd.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pd.chemitech.net.cn

Ruby: super
来源：http://pe.haigaiapp.cn

C#:   base.Greet();
来源：http://cw.9csxet.cn

[G08] 静态方法与属性
来源：http://zq.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dj.bjjhwx.cn

PHP:  public static function f() {}
来源：http://ie.yuntaijiaju.cn

JS:   static f() {}
来源：http://zv.szxytkj.cn

TS:   static f(): void {}
来源：http://sh.shxzskj.cn

Java: static void f() {}
来源：http://xq.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ue.yuexingan06.cn

Ruby: def self.f; end
来源：http://lg.nicolike.cn

C#:   public static void F() {}
来源：http://dn.newstarts.cn

[G09] 接口 / 抽象类
来源：http://ya.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://gb.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ie.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://no.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://as.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://ev.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://kx.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hh.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://hk.shxzskj.cn

[G10] 访问控制
来源：http://cl.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://xe.yuexingan06.cn

PHP:  public / protected / private
来源：http://hz.hahajie.cn

JS:   #private 字段；其余公开
来源：http://yk.lnxyls.cn

TS:   public / protected / private
来源：http://ed.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://bo.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gc.colortex.cn

Ruby: public / protected / private
来源：http://ys.nszjky.cn

C#:   public / protected / private / internal
来源：http://js.yuntaijiaju.cn

[G11] getter / setter
来源：http://bj.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://oz.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eq.newstarts.cn

JS:   get name() { return this._name; }
来源：http://lb.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://fg.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://vn.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ps.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://ap.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://ee.huanxung.cn

[G12] 对象转字符串
来源：http://xh.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://az.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://to.nszjky.cn

JS:   toString() { return this.name; }
来源：http://de.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://zw.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://ba.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fw.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://xd.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://hw.huanxung.cn

[G13] 判断对象类型
来源：http://wz.hnjuh.cn

Py:   isinstance(u, User)
来源：http://lt.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://xw.yuntaijiaju.cn

JS:   u instanceof User
来源：http://ly.huixiangedu.cn

TS:   u instanceof User
来源：http://bo.wgjwhj.cn

Java: u instanceof User
来源：http://po.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ts.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://ms.bookmarksfly.cn

C#:   u is User
来源：http://pp.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://pt.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://su.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://mp.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jm.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://lx.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://pu.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://hy.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lo.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://kf.nszjky.cn

[G15] 枚举
来源：http://iu.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wh.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ee.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ym.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vz.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://vv.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fc.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://vu.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sg.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://md.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ht.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ic.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://gq.9csxet.cn

TS:   Object.entries(obj)
来源：http://wr.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dm.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ji.shxzukj.cn

Ruby: obj.instance_variables
来源：http://zf.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://bj.lnxyls.cn

================================================================================
来源：http://ro.shxzskj.cn

H. 异常与错误处理
来源：http://kq.lnxyls.cn

================================================================================
来源：http://pn.huixiangedu.cn

[H01] try / catch 基础
来源：http://vq.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zv.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zc.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cc.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ac.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xm.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vx.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fp.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dt.9csxet.cn

[H02] finally / ensure 收尾
来源：http://wa.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jo.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://er.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cl.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rq.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ca.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fh.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oo.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ow.panjiajie.cn

[H03] 主动抛出异常
来源：http://sz.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://bx.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sd.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://nk.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://fq.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vs.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lh.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jr.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uj.gzmigu.cn

[H04] 自定义异常类型
来源：http://vb.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://ej.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ci.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://ww.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://nt.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://rp.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cv.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://lx.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://na.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://sz.wgjwhj.cn

Py:   except ValueError as e:
来源：http://no.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vz.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://oq.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://lf.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://hg.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://di.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://vv.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bw.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://om.asd995.cn

Py:   value = d.get("k") or default
来源：http://es.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fh.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sy.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://le.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://um.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ef.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://nx.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://av.hnjuh.cn

[H07] 断言
来源：http://xp.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://oz.szxytkj.cn

PHP:  assert($x > 0);
来源：http://in.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://rt.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://ce.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://mj.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uq.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hk.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://wx.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://ja.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ow.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jf.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://ny.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ns.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cd.panjiajie.cn

Go:   err.Error()
来源：http://ib.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://ry.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://sp.szsharing.cn

[H09] 带错误码的异常
来源：http://em.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ar.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gx.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ae.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nj.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kw.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bz.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kb.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gw.szxytkj.cn

[H10] 资源自动释放
来源：http://cz.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ph.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ob.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xs.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dk.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ie.szxytkj.cn

Go:   defer f.Close()
来源：http://ai.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ma.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://az.wgjwhj.cn

================================================================================
来源：http://tc.szsharing.cn

I. 正则表达式
来源：http://za.hnjuh.cn

================================================================================
来源：http://xv.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://dc.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://og.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ym.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://ey.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://yl.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gh.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bo.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://fz.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xv.huanxung.cn

[I02] 提取所有匹配
来源：http://jd.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://ha.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ax.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wz.521024.cn

TS:   s.match(/\d+/g)
来源：http://ih.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cv.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pe.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://ub.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bi.chemitech.net.cn

[I03] 提取捕获分组
来源：http://qh.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qx.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ko.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://du.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ks.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://su.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ye.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mf.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mr.muxihuayi.cn

[I04] 正则替换
来源：http://pn.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kt.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qv.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ni.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qd.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dw.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hu.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ae.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zi.huanxung.cn

[I05] 按正则拆分
来源：http://yr.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zd.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://og.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://lm.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://mf.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://pk.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gd.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uo.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oi.szxytkj.cn


<!-- 参考信息 -->