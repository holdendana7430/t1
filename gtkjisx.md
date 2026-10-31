代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ys.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aq.gzmigu.cn

[F11] 复制与移动文件
来源：http://pr.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nd.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ub.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fi.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fp.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://by.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hx.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zm.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://et.jctech888.com.cn

[F12] CSV 读写
来源：http://bf.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nd.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ip.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pr.hnjuh.cn

TS:   // 同上
来源：http://tp.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vy.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yq.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ot.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oc.wgjwhj.cn

================================================================================
来源：http://so.huixiangedu.cn

G. 面向对象
来源：http://cl.jctech888.com.cn

================================================================================
来源：http://mh.asd995.cn

[G01] 定义类
来源：http://pw.jianghongdianzi.cn

Py:   class User: pass
来源：http://yb.wgjwhj.cn

PHP:  class User {}
来源：http://zn.bjjhwx.cn

JS:   class User {}
来源：http://ol.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://yi.521024.cn

Java: class User {}
来源：http://wy.lnxyls.cn

Go:   type User struct { Name string }
来源：http://ub.panjiajie.cn

Ruby: class User; end
来源：http://ci.szsharing.cn

C#:   class User {}
来源：http://qh.shxzukj.cn

[G02] 构造函数
来源：http://rh.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://wn.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://gs.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://pq.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://kk.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://hq.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nb.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://lo.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://bs.szxytkj.cn

[G03] 实例属性
来源：http://gb.nicolike.cn

Py:   self.name = "x"
来源：http://zu.szxytkj.cn

PHP:  public string $name = "x";
来源：http://qf.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://oz.haigaiapp.cn

TS:   name: string = "x";
来源：http://he.haigaiapp.cn

Java: private String name;
来源：http://hf.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ho.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://uw.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://hr.huixiangedu.cn

[G04] 定义方法
来源：http://rb.nicolike.cn

Py:   def greet(self): return self.name
来源：http://ef.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bu.asd995.cn

JS:   greet() { return this.name; }
来源：http://gk.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://ml.huixiangedu.cn

Java: String greet() { return name; }
来源：http://tw.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qy.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://sc.newstarts.cn

C#:   public string Greet() => Name;
来源：http://sq.shxzukj.cn

[G05] 继承
来源：http://yj.szsharing.cn

Py:   class Admin(User): pass
来源：http://nj.colortex.cn

PHP:  class Admin extends User {}
来源：http://wr.nszjky.cn

JS:   class Admin extends User {}
来源：http://gr.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://xo.haigaiapp.cn

Java: class Admin extends User {}
来源：http://vd.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://an.colortex.cn

Ruby: class Admin < User; end
来源：http://gd.nicolike.cn

C#:   class Admin : User {}
来源：http://oq.521024.cn

[G06] 重写方法
来源：http://cc.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://yj.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mx.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://xx.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://xa.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://qw.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dv.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://dg.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://mm.shxzskj.cn

[G07] 调用父类方法
来源：http://jx.bookmarksfly.cn

Py:   super().greet()
来源：http://sb.chemitech.net.cn

PHP:  parent::greet();
来源：http://ds.bookmarksfly.cn

JS:   super.greet();
来源：http://su.hahajie.cn

TS:   super.greet();
来源：http://zx.9csxet.cn

Java: super.greet();
来源：http://cr.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://he.huanxung.cn

Ruby: super
来源：http://cj.jctech888.com.cn

C#:   base.Greet();
来源：http://wt.nicolike.cn

[G08] 静态方法与属性
来源：http://nq.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gy.muxihuayi.cn

PHP:  public static function f() {}
来源：http://xo.szsharing.cn

JS:   static f() {}
来源：http://uc.huanxung.cn

TS:   static f(): void {}
来源：http://rb.gzmigu.cn

Java: static void f() {}
来源：http://yj.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ua.muxihuayi.cn

Ruby: def self.f; end
来源：http://fy.shxzukj.cn

C#:   public static void F() {}
来源：http://bc.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://ny.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://qa.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uz.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zy.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://tz.szsharing.cn

Java: interface Shape { double area(); }
来源：http://si.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://tm.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://av.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://wx.asd995.cn

[G10] 访问控制
来源：http://nn.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://qu.asd995.cn

PHP:  public / protected / private
来源：http://oq.9csxet.cn

JS:   #private 字段；其余公开
来源：http://wp.chemitech.net.cn

TS:   public / protected / private
来源：http://rh.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://de.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gf.huanxung.cn

Ruby: public / protected / private
来源：http://qa.colortex.cn

C#:   public / protected / private / internal
来源：http://hw.shxzukj.cn

[G11] getter / setter
来源：http://mc.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://dz.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ow.huanxung.cn

JS:   get name() { return this._name; }
来源：http://ed.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://wf.asd995.cn

Java: public String getName() { return name; }
来源：http://or.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fx.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://ti.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://fg.chemitech.net.cn

[G12] 对象转字符串
来源：http://hq.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://bz.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://su.9csxet.cn

JS:   toString() { return this.name; }
来源：http://wn.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://rf.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://zt.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nw.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://gx.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://qi.szsharing.cn

[G13] 判断对象类型
来源：http://hx.hahajie.cn

Py:   isinstance(u, User)
来源：http://dp.gzmigu.cn

PHP:  $u instanceof User
来源：http://xu.yuexingan06.cn

JS:   u instanceof User
来源：http://sj.yuntaijiaju.cn

TS:   u instanceof User
来源：http://yo.muxihuayi.cn

Java: u instanceof User
来源：http://yx.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yu.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://li.bjjhwx.cn

C#:   u is User
来源：http://wu.hahajie.cn

[G14] 数据类 / record
来源：http://hm.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wp.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://jm.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gv.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://jh.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://jc.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://bl.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ma.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://qq.haigaiapp.cn

[G15] 枚举
来源：http://vy.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ms.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qz.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wl.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dj.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://vn.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tk.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://qg.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gm.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://wv.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vl.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://wk.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://wa.asd995.cn

TS:   Object.entries(obj)
来源：http://vn.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ez.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fq.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://uk.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://rq.hnjuh.cn

================================================================================
来源：http://bw.szsharing.cn

H. 异常与错误处理
来源：http://bn.asd995.cn

================================================================================
来源：http://ld.521024.cn

[H01] try / catch 基础
来源：http://zj.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fh.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://un.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gh.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ps.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bi.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vt.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ww.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oz.hahajie.cn

[H02] finally / ensure 收尾
来源：http://bq.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fq.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pg.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://li.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qt.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ad.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mx.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yg.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ua.lnxyls.cn

[H03] 主动抛出异常
来源：http://dd.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://jh.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kg.521024.cn

JS:   throw new Error("错误信息");
来源：http://ox.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://rm.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jo.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lo.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ng.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ab.9csxet.cn

[H04] 自定义异常类型
来源：http://pz.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://aw.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lx.521024.cn

JS:   class MyError extends Error {}
来源：http://yz.newstarts.cn

TS:   class MyError extends Error {}
来源：http://cl.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://cz.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bw.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://cu.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://pn.szsharing.cn

[H05] 捕获特定类型
来源：http://wa.huixiangedu.cn

Py:   except ValueError as e:
来源：http://kp.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sd.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://po.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://tc.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://xy.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lg.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://xf.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gz.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://ui.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://yn.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qn.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://om.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mn.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iy.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rd.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://wg.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://cl.bookmarksfly.cn

[H07] 断言
来源：http://gl.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://oc.szxytkj.cn

PHP:  assert($x > 0);
来源：http://hk.asd995.cn

JS:   console.assert(x > 0);
来源：http://pl.hahajie.cn

TS:   console.assert(x > 0);
来源：http://fj.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://mi.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vw.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://of.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://xq.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://fe.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ja.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ci.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://no.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://do.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zq.newstarts.cn

Go:   err.Error()
来源：http://iy.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://pj.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://gl.colortex.cn

[H09] 带错误码的异常
来源：http://fz.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lf.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pz.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hg.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ab.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pj.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lt.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://se.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zr.haigaiapp.cn

[H10] 资源自动释放
来源：http://lr.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lr.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gm.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cc.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vq.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ps.wgjwhj.cn

Go:   defer f.Close()
来源：http://dm.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ni.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://el.haigaiapp.cn

================================================================================
来源：http://pm.yuntaijiaju.cn

I. 正则表达式
来源：http://hj.hahajie.cn

================================================================================
来源：http://gy.huanxung.cn

[I01] 判断是否匹配
来源：http://mq.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pp.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://de.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://so.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://rr.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ew.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rv.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://sc.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bl.bjjhwx.cn

[I02] 提取所有匹配
来源：http://oa.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://ly.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bw.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://if.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://zq.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sd.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://us.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://yg.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wy.wgjwhj.cn

[I03] 提取捕获分组
来源：http://sd.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pj.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uh.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wd.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tw.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fb.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://io.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eb.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cz.wgjwhj.cn

[I04] 正则替换
来源：http://he.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tq.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ld.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ay.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iu.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://if.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vt.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ut.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zo.9csxet.cn

[I05] 按正则拆分
来源：http://pz.haigaiapp.cn


<!-- 参考信息 -->