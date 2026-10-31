代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mx.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ra.szsharing.cn

[F11] 复制与移动文件
来源：http://sl.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qz.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pn.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dp.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sh.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bb.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yx.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://id.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xy.lnxyls.cn

[F12] CSV 读写
来源：http://am.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qj.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lt.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bv.newstarts.cn

TS:   // 同上
来源：http://rt.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sc.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ug.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pr.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vz.newstarts.cn

================================================================================
来源：http://jj.nicolike.cn

G. 面向对象
来源：http://co.haigaiapp.cn

================================================================================
来源：http://ag.521024.cn

[G01] 定义类
来源：http://qo.huixiangedu.cn

Py:   class User: pass
来源：http://nq.szxytkj.cn

PHP:  class User {}
来源：http://go.shxzskj.cn

JS:   class User {}
来源：http://pu.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://bm.hahajie.cn

Java: class User {}
来源：http://ct.shxzskj.cn

Go:   type User struct { Name string }
来源：http://ls.colortex.cn

Ruby: class User; end
来源：http://zx.hnjuh.cn

C#:   class User {}
来源：http://gk.szxytkj.cn

[G02] 构造函数
来源：http://dv.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://yg.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://vv.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://zm.521024.cn

TS:   constructor(public name: string) {}
来源：http://dv.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://gf.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mr.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://oh.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://sz.wgjwhj.cn

[G03] 实例属性
来源：http://uc.yuexingan06.cn

Py:   self.name = "x"
来源：http://ty.newstarts.cn

PHP:  public string $name = "x";
来源：http://nv.bjjhwx.cn

JS:   this.name = "x";
来源：http://sh.hahajie.cn

TS:   name: string = "x";
来源：http://vc.huixinmuqiang.cn

Java: private String name;
来源：http://qn.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ao.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://qy.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://ap.haigaiapp.cn

[G04] 定义方法
来源：http://ss.9csxet.cn

Py:   def greet(self): return self.name
来源：http://xh.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jt.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://on.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://gk.wgjwhj.cn

Java: String greet() { return name; }
来源：http://go.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fn.hahajie.cn

Ruby: def greet; @name; end
来源：http://bh.asd995.cn

C#:   public string Greet() => Name;
来源：http://vf.muxihuayi.cn

[G05] 继承
来源：http://wd.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://da.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://xh.gzmigu.cn

JS:   class Admin extends User {}
来源：http://wk.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://wd.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://ml.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://km.gzmigu.cn

Ruby: class Admin < User; end
来源：http://xy.panjiajie.cn

C#:   class Admin : User {}
来源：http://op.jianghongdianzi.cn

[G06] 重写方法
来源：http://va.521024.cn

Py:   def greet(self): return "admin"
来源：http://wb.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ys.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://cs.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://fi.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://rd.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://il.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://ta.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://ol.muxihuayi.cn

[G07] 调用父类方法
来源：http://yo.huanxung.cn

Py:   super().greet()
来源：http://et.nszjky.cn

PHP:  parent::greet();
来源：http://ak.haigaiapp.cn

JS:   super.greet();
来源：http://lo.szxytkj.cn

TS:   super.greet();
来源：http://iw.hnjuh.cn

Java: super.greet();
来源：http://gc.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ov.lnxyls.cn

Ruby: super
来源：http://bv.nszjky.cn

C#:   base.Greet();
来源：http://ub.521024.cn

[G08] 静态方法与属性
来源：http://ii.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ki.bjjhwx.cn

PHP:  public static function f() {}
来源：http://pu.colortex.cn

JS:   static f() {}
来源：http://ly.nszjky.cn

TS:   static f(): void {}
来源：http://jf.9csxet.cn

Java: static void f() {}
来源：http://nd.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jo.gzmigu.cn

Ruby: def self.f; end
来源：http://gp.bookmarksfly.cn

C#:   public static void F() {}
来源：http://lp.nszjky.cn

[G09] 接口 / 抽象类
来源：http://wu.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://lv.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mf.shtwfgs.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://da.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://tw.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://pq.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://sy.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bo.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://uk.szxytkj.cn

[G10] 访问控制
来源：http://no.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://pk.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://yl.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://dp.panjiajie.cn

TS:   public / protected / private
来源：http://pv.colortex.cn

Java: public / protected / private / 默认包级
来源：http://li.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fh.shxzskj.cn

Ruby: public / protected / private
来源：http://zw.shxzskj.cn

C#:   public / protected / private / internal
来源：http://vp.huanxung.cn

[G11] getter / setter
来源：http://xc.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ys.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gf.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://zn.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://jc.newstarts.cn

Java: public String getName() { return name; }
来源：http://yj.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cx.asd995.cn

Ruby: attr_accessor :name
来源：http://qb.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://jn.wgjwhj.cn

[G12] 对象转字符串
来源：http://ya.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://ph.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ee.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://qj.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://xw.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://vl.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qo.nicolike.cn

Ruby: def to_s; @name; end
来源：http://xt.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://pi.muxihuayi.cn

[G13] 判断对象类型
来源：http://nr.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://wj.szxytkj.cn

PHP:  $u instanceof User
来源：http://yv.muxihuayi.cn

JS:   u instanceof User
来源：http://or.9csxet.cn

TS:   u instanceof User
来源：http://la.hnjuh.cn

Java: u instanceof User
来源：http://zv.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jv.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://sd.chemitech.net.cn

C#:   u is User
来源：http://cp.bookmarksfly.cn

[G14] 数据类 / record
来源：http://hi.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fi.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://vz.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eo.521024.cn

TS:   type User = { name: string; age: number };
来源：http://hz.hahajie.cn

Java: record User(String name, int age) {}
来源：http://bx.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://eb.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rl.asd995.cn

C#:   record User(string Name, int Age);
来源：http://fw.yuexingan06.cn

[G15] 枚举
来源：http://zz.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ye.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ek.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nu.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pp.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://ge.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qf.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://yc.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://td.521024.cn

[G16] 对象转数组 / 字典
来源：http://eh.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yj.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://qs.szsharing.cn

JS:   Object.entries(obj)
来源：http://jl.shxzskj.cn

TS:   Object.entries(obj)
来源：http://cs.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gd.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pj.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://ih.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://nr.hnjuh.cn

================================================================================
来源：http://ob.nicolike.cn

H. 异常与错误处理
来源：http://li.9csxet.cn

================================================================================
来源：http://wh.bookmarksfly.cn

[H01] try / catch 基础
来源：http://na.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nc.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wh.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ax.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kf.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fa.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kx.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sv.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yt.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://ht.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://me.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wh.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://th.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ae.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lw.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ll.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ed.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qt.huanxung.cn

[H03] 主动抛出异常
来源：http://mw.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://uk.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jc.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://nq.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://vw.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ry.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ez.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zv.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eu.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://pa.colortex.cn

Py:   class MyError(Exception): pass
来源：http://gg.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wd.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://fa.szsharing.cn

TS:   class MyError extends Error {}
来源：http://em.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://cd.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fz.521024.cn

Ruby: class MyError < StandardError; end
来源：http://sh.szsharing.cn

C#:   class MyException : Exception {}
来源：http://tw.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://gr.haigaiapp.cn

Py:   except ValueError as e:
来源：http://kd.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://az.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://pl.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://dm.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://jv.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jw.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://aj.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ve.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://te.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://jf.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wx.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xg.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fs.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xs.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dz.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://mi.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://vr.asd995.cn

[H07] 断言
来源：http://wk.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://sc.szsharing.cn

PHP:  assert($x > 0);
来源：http://nk.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://xw.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://el.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://dw.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hy.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ry.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://kx.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://qn.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://ke.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ql.gzmigu.cn

JS:   e.message;  e.stack
来源：http://er.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hy.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zw.jctech888.com.cn

Go:   err.Error()
来源：http://jo.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://gh.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://ar.colortex.cn

[H09] 带错误码的异常
来源：http://fm.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ax.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zh.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qo.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rl.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nx.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://er.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ae.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xf.nszjky.cn

[H10] 资源自动释放
来源：http://cw.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ky.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wc.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://or.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ag.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lm.yuexingan06.cn

Go:   defer f.Close()
来源：http://vj.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gm.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tf.yuntaijiaju.cn

================================================================================
来源：http://ha.asd995.cn

I. 正则表达式
来源：http://re.nszjky.cn

================================================================================
来源：http://yj.hahajie.cn

[I01] 判断是否匹配
来源：http://bz.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nq.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tz.colortex.cn

JS:   /\d+/.test(s)
来源：http://cb.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://px.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ii.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hi.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://dy.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wy.wgjwhj.cn

[I02] 提取所有匹配
来源：http://ik.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://sr.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bh.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qp.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://xh.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ti.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dr.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://po.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tp.yuexingan06.cn

[I03] 提取捕获分组
来源：http://yy.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lc.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vu.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ql.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tr.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hy.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jc.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sm.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://we.chemitech.net.cn

[I04] 正则替换
来源：http://pk.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qj.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xo.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qf.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kf.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rv.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rh.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fr.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dt.chemitech.net.cn

[I05] 按正则拆分
来源：http://iu.muxihuayi.cn


<!-- 参考信息 -->