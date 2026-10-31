代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dk.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://di.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://df.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://zg.nszjky.cn

[F09] 获取文件大小
来源：http://jg.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://mt.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://ke.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://xd.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://ah.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lc.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ff.nszjky.cn

Ruby: File.size("a.txt")
来源：http://sa.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://wt.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://tr.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vl.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ec.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xu.asd995.cn

TS:   path.extname("a.txt")
来源：http://ds.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rd.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ns.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zr.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://to.muxihuayi.cn

[F11] 复制与移动文件
来源：http://lv.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vf.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jd.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aq.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cg.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tq.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tl.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qv.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lg.jianghongdianzi.cn

[F12] CSV 读写
来源：http://px.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zm.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pi.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qz.haigaiapp.cn

TS:   // 同上
来源：http://qq.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qs.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://id.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zs.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sw.nicolike.cn

================================================================================
来源：http://vb.colortex.cn

G. 面向对象
来源：http://qd.gzmigu.cn

================================================================================
来源：http://rl.shxzukj.cn

[G01] 定义类
来源：http://nb.chemitech.net.cn

Py:   class User: pass
来源：http://fe.asd995.cn

PHP:  class User {}
来源：http://xh.nicolike.cn

JS:   class User {}
来源：http://bw.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://hu.9csxet.cn

Java: class User {}
来源：http://qh.huanxung.cn

Go:   type User struct { Name string }
来源：http://xb.shtwfgs.cn

Ruby: class User; end
来源：http://cr.nicolike.cn

C#:   class User {}
来源：http://nj.huixinmuqiang.cn

[G02] 构造函数
来源：http://sc.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://nj.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://yr.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://ws.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ao.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://uw.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://en.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://ux.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://ee.huixiangedu.cn

[G03] 实例属性
来源：http://hv.shxzskj.cn

Py:   self.name = "x"
来源：http://tb.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://js.bookmarksfly.cn

JS:   this.name = "x";
来源：http://kv.shxzukj.cn

TS:   name: string = "x";
来源：http://qa.hnjuh.cn

Java: private String name;
来源：http://sf.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://en.nicolike.cn

Ruby: @name = "x"
来源：http://vx.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://vr.shtwfgs.cn

[G04] 定义方法
来源：http://ld.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://yb.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gt.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://ft.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://ac.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ii.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sp.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://rx.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://gz.chemitech.net.cn

[G05] 继承
来源：http://ov.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://la.szsharing.cn

PHP:  class Admin extends User {}
来源：http://th.lnxyls.cn

JS:   class Admin extends User {}
来源：http://fw.shxzukj.cn

TS:   class Admin extends User {}
来源：http://tz.shtwfgs.cn

Java: class Admin extends User {}
来源：http://au.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cg.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://hr.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://hp.panjiajie.cn

[G06] 重写方法
来源：http://rr.asd995.cn

Py:   def greet(self): return "admin"
来源：http://rw.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nu.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://rz.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://cm.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://jw.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sk.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://lj.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://ek.chemitech.net.cn

[G07] 调用父类方法
来源：http://an.huixinmuqiang.cn

Py:   super().greet()
来源：http://xt.panjiajie.cn

PHP:  parent::greet();
来源：http://ip.nszjky.cn

JS:   super.greet();
来源：http://wz.jianghongdianzi.cn

TS:   super.greet();
来源：http://vw.9csxet.cn

Java: super.greet();
来源：http://rp.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ii.jianghongdianzi.cn

Ruby: super
来源：http://fh.bookmarksfly.cn

C#:   base.Greet();
来源：http://on.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://hy.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pn.panjiajie.cn

PHP:  public static function f() {}
来源：http://ep.9csxet.cn

JS:   static f() {}
来源：http://nq.lnxyls.cn

TS:   static f(): void {}
来源：http://sx.nicolike.cn

Java: static void f() {}
来源：http://vx.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://go.szsharing.cn

Ruby: def self.f; end
来源：http://md.szxytkj.cn

C#:   public static void F() {}
来源：http://aa.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://eu.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ao.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wi.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zq.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://tj.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://yg.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://fx.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yd.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://qe.panjiajie.cn

[G10] 访问控制
来源：http://rt.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://zs.521024.cn

PHP:  public / protected / private
来源：http://gq.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://pq.wgjwhj.cn

TS:   public / protected / private
来源：http://xp.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://bt.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hc.jctech888.com.cn

Ruby: public / protected / private
来源：http://me.hahajie.cn

C#:   public / protected / private / internal
来源：http://xo.bjjhwx.cn

[G11] getter / setter
来源：http://tc.colortex.cn

Py:   @property 与 @x.setter
来源：http://gm.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ig.nszjky.cn

JS:   get name() { return this._name; }
来源：http://iw.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://vu.9csxet.cn

Java: public String getName() { return name; }
来源：http://ek.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sm.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://ew.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://uh.huanxung.cn

[G12] 对象转字符串
来源：http://tz.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://fy.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sa.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://bu.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://ro.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://rq.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mv.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://or.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://tj.yuexingan06.cn

[G13] 判断对象类型
来源：http://hn.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://hk.jctech888.com.cn

PHP:  $u instanceof User
来源：http://ni.panjiajie.cn

JS:   u instanceof User
来源：http://rw.yuexingan06.cn

TS:   u instanceof User
来源：http://uz.huixinmuqiang.cn

Java: u instanceof User
来源：http://hq.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tu.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://rw.szsharing.cn

C#:   u is User
来源：http://cj.colortex.cn

[G14] 数据类 / record
来源：http://ze.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pc.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://mh.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iu.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://lf.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://hs.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://yq.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lp.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://es.lnxyls.cn

[G15] 枚举
来源：http://ig.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ay.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yl.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gg.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nt.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://hi.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ve.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://fg.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://je.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://fk.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pv.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://ad.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://bg.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://fd.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yk.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gj.nicolike.cn

Ruby: obj.instance_variables
来源：http://bs.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ai.bookmarksfly.cn

================================================================================
来源：http://gf.huanxung.cn

H. 异常与错误处理
来源：http://bh.szxytkj.cn

================================================================================
来源：http://ke.szxytkj.cn

[H01] try / catch 基础
来源：http://se.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eq.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ky.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aj.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://he.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ka.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lo.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://og.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vu.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://lm.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nd.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dh.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ks.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vp.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ig.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aj.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xe.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xv.9csxet.cn

[H03] 主动抛出异常
来源：http://jf.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://aa.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://br.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://lr.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://fy.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://is.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mr.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gi.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xd.hnjuh.cn

[H04] 自定义异常类型
来源：http://ns.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://jg.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ag.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://vn.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://gs.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://qf.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dg.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://mg.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://rs.yuexingan06.cn

[H05] 捕获特定类型
来源：http://ya.muxihuayi.cn

Py:   except ValueError as e:
来源：http://pq.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ii.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://xn.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ll.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://xq.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nc.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://cj.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gf.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://cv.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://nb.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gb.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sj.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vw.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ew.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hk.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://sq.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://cw.9csxet.cn

[H07] 断言
来源：http://sh.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://un.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://eg.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://zo.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://jn.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://hn.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qm.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dq.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://tz.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://tg.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://li.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sf.521024.cn

JS:   e.message;  e.stack
来源：http://ea.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pp.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ro.shxzukj.cn

Go:   err.Error()
来源：http://xi.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://lz.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://va.shxzukj.cn

[H09] 带错误码的异常
来源：http://lq.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kc.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yh.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uz.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eh.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lq.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qp.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kn.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wf.gzmigu.cn

[H10] 资源自动释放
来源：http://bi.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hx.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xw.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jw.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oy.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://es.asd995.cn

Go:   defer f.Close()
来源：http://lf.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hg.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ua.bjjhwx.cn

================================================================================
来源：http://yl.newstarts.cn

I. 正则表达式
来源：http://cg.nszjky.cn

================================================================================
来源：http://jo.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://qd.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lx.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oq.9csxet.cn

JS:   /\d+/.test(s)
来源：http://dh.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://cg.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rp.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cp.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://wt.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://az.521024.cn

[I02] 提取所有匹配
来源：http://wi.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://wc.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vb.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wk.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://zr.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kj.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rs.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://ek.huanxung.cn


<!-- 参考信息 -->