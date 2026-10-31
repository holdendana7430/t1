代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://nb.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://yc.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ly.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rg.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kj.9csxet.cn

TS:   path.extname("a.txt")
来源：http://oj.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yy.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://is.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eh.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yq.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://jv.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fx.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rq.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cw.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://td.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aw.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kv.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mh.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tq.colortex.cn

[F12] CSV 读写
来源：http://yz.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qy.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bq.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vs.nicolike.cn

TS:   // 同上
来源：http://cj.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wd.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cs.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fi.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ck.shtwfgs.cn

================================================================================
来源：http://ae.521024.cn

G. 面向对象
来源：http://bp.521024.cn

================================================================================
来源：http://ph.shxzskj.cn

[G01] 定义类
来源：http://ie.nicolike.cn

Py:   class User: pass
来源：http://zt.yuntaijiaju.cn

PHP:  class User {}
来源：http://ij.wgjwhj.cn

JS:   class User {}
来源：http://dw.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://du.colortex.cn

Java: class User {}
来源：http://dx.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://tw.nicolike.cn

Ruby: class User; end
来源：http://vg.huixinmuqiang.cn

C#:   class User {}
来源：http://oj.shtwfgs.cn

[G02] 构造函数
来源：http://cg.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://fb.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://so.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://dk.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://uh.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://fc.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://va.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://wv.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://sy.bjjhwx.cn

[G03] 实例属性
来源：http://sk.szxytkj.cn

Py:   self.name = "x"
来源：http://jh.shxzukj.cn

PHP:  public string $name = "x";
来源：http://vz.szxytkj.cn

JS:   this.name = "x";
来源：http://wz.bjjhwx.cn

TS:   name: string = "x";
来源：http://jx.newstarts.cn

Java: private String name;
来源：http://nx.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ol.shxzukj.cn

Ruby: @name = "x"
来源：http://so.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://ro.chemitech.net.cn

[G04] 定义方法
来源：http://yc.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://dk.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://se.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://gk.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://op.gzmigu.cn

Java: String greet() { return name; }
来源：http://ic.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xo.lnxyls.cn

Ruby: def greet; @name; end
来源：http://kt.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://mf.haigaiapp.cn

[G05] 继承
来源：http://rx.gzmigu.cn

Py:   class Admin(User): pass
来源：http://xl.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://lg.newstarts.cn

JS:   class Admin extends User {}
来源：http://ri.shxzskj.cn

TS:   class Admin extends User {}
来源：http://by.newstarts.cn

Java: class Admin extends User {}
来源：http://cf.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mt.lnxyls.cn

Ruby: class Admin < User; end
来源：http://xn.hahajie.cn

C#:   class Admin : User {}
来源：http://iu.huanxung.cn

[G06] 重写方法
来源：http://wy.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://lt.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wg.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://dw.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://yj.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://tr.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gh.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://jd.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://vr.huixiangedu.cn

[G07] 调用父类方法
来源：http://zs.colortex.cn

Py:   super().greet()
来源：http://vm.shxzukj.cn

PHP:  parent::greet();
来源：http://ht.gzmigu.cn

JS:   super.greet();
来源：http://jy.lnxyls.cn

TS:   super.greet();
来源：http://px.9csxet.cn

Java: super.greet();
来源：http://oj.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ak.yuntaijiaju.cn

Ruby: super
来源：http://nk.jctech888.com.cn

C#:   base.Greet();
来源：http://cw.shtwfgs.cn

[G08] 静态方法与属性
来源：http://sb.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lg.haigaiapp.cn

PHP:  public static function f() {}
来源：http://ya.yuntaijiaju.cn

JS:   static f() {}
来源：http://vt.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://ph.nszjky.cn

Java: static void f() {}
来源：http://sl.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ry.szsharing.cn

Ruby: def self.f; end
来源：http://hn.szsharing.cn

C#:   public static void F() {}
来源：http://dm.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://wk.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://bq.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wb.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://he.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://bl.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://vj.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ue.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nc.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://lc.521024.cn

[G10] 访问控制
来源：http://pl.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://nh.szsharing.cn

PHP:  public / protected / private
来源：http://hp.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://xk.521024.cn

TS:   public / protected / private
来源：http://vd.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://sk.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ah.hahajie.cn

Ruby: public / protected / private
来源：http://eo.panjiajie.cn

C#:   public / protected / private / internal
来源：http://qp.jianghongdianzi.cn

[G11] getter / setter
来源：http://xr.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://qp.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ep.nicolike.cn

JS:   get name() { return this._name; }
来源：http://cj.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://ma.lnxyls.cn

Java: public String getName() { return name; }
来源：http://ah.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rp.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://vq.nicolike.cn

C#:   public string Name { get; set; }
来源：http://mo.shtwfgs.cn

[G12] 对象转字符串
来源：http://hi.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://rk.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sl.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://ki.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://vl.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://ge.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://df.hahajie.cn

Ruby: def to_s; @name; end
来源：http://lc.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://gs.newstarts.cn

[G13] 判断对象类型
来源：http://me.521024.cn

Py:   isinstance(u, User)
来源：http://hq.9csxet.cn

PHP:  $u instanceof User
来源：http://sg.yuexingan06.cn

JS:   u instanceof User
来源：http://rr.muxihuayi.cn

TS:   u instanceof User
来源：http://nf.hnjuh.cn

Java: u instanceof User
来源：http://qn.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://op.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://fp.yuexingan06.cn

C#:   u is User
来源：http://an.colortex.cn

[G14] 数据类 / record
来源：http://mk.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yj.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://lk.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xk.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://gx.hahajie.cn

Java: record User(String name, int age) {}
来源：http://eg.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://qx.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nm.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://wy.huanxung.cn

[G15] 枚举
来源：http://zi.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ka.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://st.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jk.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pe.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://jj.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kz.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://oq.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yt.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://hf.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eh.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://mo.huanxung.cn

JS:   Object.entries(obj)
来源：http://na.hahajie.cn

TS:   Object.entries(obj)
来源：http://ha.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wc.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ty.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://zh.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://kn.lnxyls.cn

================================================================================
来源：http://yc.shxzskj.cn

H. 异常与错误处理
来源：http://rx.9csxet.cn

================================================================================
来源：http://fn.bookmarksfly.cn

[H01] try / catch 基础
来源：http://ps.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fg.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://le.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lr.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://io.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ag.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kd.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fw.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ay.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://fq.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://po.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uy.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://et.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cq.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fs.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://of.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yb.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ld.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://rl.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://lm.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://of.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://yv.colortex.cn

TS:   throw new Error("错误信息");
来源：http://rn.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zd.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ph.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yt.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fi.hahajie.cn

[H04] 自定义异常类型
来源：http://ok.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://vx.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dd.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://hw.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://qi.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://tn.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rf.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://bj.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://dy.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://pa.bjjhwx.cn

Py:   except ValueError as e:
来源：http://ds.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tr.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://mu.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://ef.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://pj.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ii.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://ej.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tt.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://ng.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://qz.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qh.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://he.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bk.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wg.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kx.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ov.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://nl.jianghongdianzi.cn

[H07] 断言
来源：http://nh.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://nj.colortex.cn

PHP:  assert($x > 0);
来源：http://ti.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://zb.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://mb.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://gg.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mn.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xk.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://bo.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://tw.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://qt.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vg.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://dg.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yj.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bb.wgjwhj.cn

Go:   err.Error()
来源：http://uz.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://lq.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ke.521024.cn

[H09] 带错误码的异常
来源：http://nv.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zr.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wf.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wc.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kx.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qj.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lf.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vq.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tg.hnjuh.cn

[H10] 资源自动释放
来源：http://od.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pi.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iu.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wo.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tl.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ro.huanxung.cn

Go:   defer f.Close()
来源：http://ug.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cx.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iw.huixinmuqiang.cn

================================================================================
来源：http://iw.wgjwhj.cn

I. 正则表达式
来源：http://nw.shxzskj.cn

================================================================================
来源：http://bd.chemitech.net.cn

[I01] 判断是否匹配
来源：http://ue.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jp.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://no.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://tv.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://sb.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gi.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eb.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://xe.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wu.shxzskj.cn

[I02] 提取所有匹配
来源：http://ou.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://bx.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oe.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mg.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://dy.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yi.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fy.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://yb.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ur.lnxyls.cn

[I03] 提取捕获分组
来源：http://zf.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sq.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://df.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hf.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yj.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lv.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yd.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fk.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pk.yuntaijiaju.cn

[I04] 正则替换
来源：http://ne.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ry.lnxyls.cn


<!-- 参考信息 -->