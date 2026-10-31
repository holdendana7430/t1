代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yk.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dk.colortex.cn

Ruby: Dir.children("dir")
来源：http://rg.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://lh.lnxyls.cn

[F09] 获取文件大小
来源：http://hc.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://ih.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://xe.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://yt.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://fb.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pd.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zz.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://hv.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://dv.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://ir.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qz.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://po.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aw.nszjky.cn

TS:   path.extname("a.txt")
来源：http://hg.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zp.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rf.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ao.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wo.shxzskj.cn

[F11] 复制与移动文件
来源：http://my.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pw.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wd.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vj.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yp.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pz.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sf.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mt.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lt.nicolike.cn

[F12] CSV 读写
来源：http://sx.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ob.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zv.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yq.nszjky.cn

TS:   // 同上
来源：http://lk.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://om.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://io.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ff.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bf.521024.cn

================================================================================
来源：http://ia.shtwfgs.cn

G. 面向对象
来源：http://hl.muxihuayi.cn

================================================================================
来源：http://ta.szxytkj.cn

[G01] 定义类
来源：http://ox.yuntaijiaju.cn

Py:   class User: pass
来源：http://kz.huixiangedu.cn

PHP:  class User {}
来源：http://cu.yuexingan06.cn

JS:   class User {}
来源：http://hy.521024.cn

TS:   class User { name: string = ""; }
来源：http://zs.yuexingan06.cn

Java: class User {}
来源：http://lw.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://lz.huixiangedu.cn

Ruby: class User; end
来源：http://ta.huixinmuqiang.cn

C#:   class User {}
来源：http://tf.newstarts.cn

[G02] 构造函数
来源：http://qw.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://wa.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ok.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://qz.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://kt.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://ez.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xe.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://mg.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://lr.haigaiapp.cn

[G03] 实例属性
来源：http://ky.lnxyls.cn

Py:   self.name = "x"
来源：http://gc.lnxyls.cn

PHP:  public string $name = "x";
来源：http://ho.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://su.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://tm.nszjky.cn

Java: private String name;
来源：http://jw.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kc.shxzukj.cn

Ruby: @name = "x"
来源：http://dw.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://he.huixiangedu.cn

[G04] 定义方法
来源：http://ba.nszjky.cn

Py:   def greet(self): return self.name
来源：http://vd.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://si.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://ov.521024.cn

TS:   greet(): string { return this.name; }
来源：http://nm.shxzukj.cn

Java: String greet() { return name; }
来源：http://na.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bv.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://zs.nicolike.cn

C#:   public string Greet() => Name;
来源：http://qk.hnjuh.cn

[G05] 继承
来源：http://ol.521024.cn

Py:   class Admin(User): pass
来源：http://mc.newstarts.cn

PHP:  class Admin extends User {}
来源：http://ag.lnxyls.cn

JS:   class Admin extends User {}
来源：http://ui.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://wa.shtwfgs.cn

Java: class Admin extends User {}
来源：http://vj.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bs.asd995.cn

Ruby: class Admin < User; end
来源：http://rd.jctech888.com.cn

C#:   class Admin : User {}
来源：http://oj.asd995.cn

[G06] 重写方法
来源：http://jz.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://pk.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wn.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://zx.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://mp.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://id.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tt.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://un.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://lq.lnxyls.cn

[G07] 调用父类方法
来源：http://xt.szxytkj.cn

Py:   super().greet()
来源：http://bu.newstarts.cn

PHP:  parent::greet();
来源：http://rz.huixinmuqiang.cn

JS:   super.greet();
来源：http://ra.huixinmuqiang.cn

TS:   super.greet();
来源：http://yk.gzmigu.cn

Java: super.greet();
来源：http://kn.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xa.nicolike.cn

Ruby: super
来源：http://uw.521024.cn

C#:   base.Greet();
来源：http://sr.huixiangedu.cn

[G08] 静态方法与属性
来源：http://bv.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vl.shxzskj.cn

PHP:  public static function f() {}
来源：http://wy.521024.cn

JS:   static f() {}
来源：http://bd.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://kh.huanxung.cn

Java: static void f() {}
来源：http://zz.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ko.haigaiapp.cn

Ruby: def self.f; end
来源：http://ez.hahajie.cn

C#:   public static void F() {}
来源：http://ze.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://cm.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://sa.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ms.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lr.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://rl.newstarts.cn

Java: interface Shape { double area(); }
来源：http://tp.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://op.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fk.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://gz.521024.cn

[G10] 访问控制
来源：http://lt.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://ab.wgjwhj.cn

PHP:  public / protected / private
来源：http://wn.huanxung.cn

JS:   #private 字段；其余公开
来源：http://qp.gzmigu.cn

TS:   public / protected / private
来源：http://lq.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://ee.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cg.lnxyls.cn

Ruby: public / protected / private
来源：http://rr.nszjky.cn

C#:   public / protected / private / internal
来源：http://yk.haigaiapp.cn

[G11] getter / setter
来源：http://zk.nszjky.cn

Py:   @property 与 @x.setter
来源：http://ry.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ja.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://in.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://sw.lnxyls.cn

Java: public String getName() { return name; }
来源：http://ka.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ju.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://mw.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://vh.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://xe.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://ea.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xi.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://iy.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://zp.521024.cn

Java: @Override public String toString() { return name; }
来源：http://pr.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bz.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://kt.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://ur.szsharing.cn

[G13] 判断对象类型
来源：http://em.lnxyls.cn

Py:   isinstance(u, User)
来源：http://lz.hahajie.cn

PHP:  $u instanceof User
来源：http://lc.huanxung.cn

JS:   u instanceof User
来源：http://jg.huixinmuqiang.cn

TS:   u instanceof User
来源：http://id.bookmarksfly.cn

Java: u instanceof User
来源：http://vy.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://id.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://ba.lnxyls.cn

C#:   u is User
来源：http://cx.hahajie.cn

[G14] 数据类 / record
来源：http://io.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ji.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://yv.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ud.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://oz.huanxung.cn

Java: record User(String name, int age) {}
来源：http://xk.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://fs.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vu.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://dy.huixiangedu.cn

[G15] 枚举
来源：http://be.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nl.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qz.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bl.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rq.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://ga.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tz.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://vo.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yz.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://ss.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ip.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://tl.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://px.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://yh.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jq.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ly.521024.cn

Ruby: obj.instance_variables
来源：http://gq.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://ex.huixiangedu.cn

================================================================================
来源：http://ma.huixiangedu.cn

H. 异常与错误处理
来源：http://rx.asd995.cn

================================================================================
来源：http://dp.shxzskj.cn

[H01] try / catch 基础
来源：http://ln.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fg.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wm.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sg.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lp.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zb.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wj.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rz.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sa.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://jz.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fs.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cb.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://va.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://at.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ns.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ta.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ie.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mt.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://hr.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://gj.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://km.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://mp.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://hg.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ta.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nk.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ww.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yt.hahajie.cn

[H04] 自定义异常类型
来源：http://it.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://nn.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zu.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://qv.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://cz.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://yu.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sy.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://hf.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://hf.newstarts.cn

[H05] 捕获特定类型
来源：http://xc.asd995.cn

Py:   except ValueError as e:
来源：http://sb.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tl.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://oj.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ka.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://gk.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zu.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://wo.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ab.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://ws.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://cp.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bi.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ow.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ah.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tk.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bd.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://vl.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://sv.szsharing.cn

[H07] 断言
来源：http://ct.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://rd.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://yv.nicolike.cn

JS:   console.assert(x > 0);
来源：http://tx.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://rb.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://eu.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wj.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bt.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://ok.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://zc.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://pt.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tl.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://pr.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uv.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qx.szxytkj.cn

Go:   err.Error()
来源：http://hs.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://qt.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://hz.gzmigu.cn

[H09] 带错误码的异常
来源：http://mq.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sd.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fo.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yd.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bf.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hn.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mk.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zh.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cr.hnjuh.cn

[H10] 资源自动释放
来源：http://yk.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lf.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xc.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sl.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pv.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hn.gzmigu.cn

Go:   defer f.Close()
来源：http://ah.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fn.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mc.bjjhwx.cn

================================================================================
来源：http://au.chemitech.net.cn

I. 正则表达式
来源：http://bq.szxytkj.cn

================================================================================
来源：http://ar.chemitech.net.cn

[I01] 判断是否匹配
来源：http://zd.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fl.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jy.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://op.huanxung.cn

TS:   /\d+/.test(s)
来源：http://le.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://il.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ax.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://dk.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lg.nszjky.cn

[I02] 提取所有匹配
来源：http://ei.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://co.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oy.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ye.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://nq.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wg.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jh.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://cl.chemitech.net.cn


<!-- 参考信息 -->