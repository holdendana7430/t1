代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://em.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zb.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gl.newstarts.cn

Ruby: File.size("a.txt")
来源：http://qd.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://cn.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://fk.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ly.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xu.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bv.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://oa.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vq.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kx.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qg.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mg.hahajie.cn

[F11] 复制与移动文件
来源：http://zf.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jr.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tf.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bo.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bk.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hw.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sq.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vg.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://db.yuexingan06.cn

[F12] CSV 读写
来源：http://dh.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fb.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ql.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://om.hahajie.cn

TS:   // 同上
来源：http://kk.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ra.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xm.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mf.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bi.nicolike.cn

================================================================================
来源：http://ke.hahajie.cn

G. 面向对象
来源：http://hw.9csxet.cn

================================================================================
来源：http://pb.szxytkj.cn

[G01] 定义类
来源：http://hb.haigaiapp.cn

Py:   class User: pass
来源：http://bt.huixiangedu.cn

PHP:  class User {}
来源：http://ht.nicolike.cn

JS:   class User {}
来源：http://wf.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://ca.jctech888.com.cn

Java: class User {}
来源：http://kn.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://ki.jianghongdianzi.cn

Ruby: class User; end
来源：http://tn.asd995.cn

C#:   class User {}
来源：http://ga.panjiajie.cn

[G02] 构造函数
来源：http://qx.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://gl.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://qn.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://ap.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://kz.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://te.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cg.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://jx.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://ys.haigaiapp.cn

[G03] 实例属性
来源：http://sa.521024.cn

Py:   self.name = "x"
来源：http://ez.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://dp.szxytkj.cn

JS:   this.name = "x";
来源：http://tm.huixiangedu.cn

TS:   name: string = "x";
来源：http://kp.haigaiapp.cn

Java: private String name;
来源：http://iz.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zk.haigaiapp.cn

Ruby: @name = "x"
来源：http://bb.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://ef.521024.cn

[G04] 定义方法
来源：http://qx.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ko.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fd.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://ed.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://wz.bjjhwx.cn

Java: String greet() { return name; }
来源：http://jg.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hq.gzmigu.cn

Ruby: def greet; @name; end
来源：http://li.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://at.jctech888.com.cn

[G05] 继承
来源：http://ay.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://kk.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://tk.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://bo.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://og.lnxyls.cn

Java: class Admin extends User {}
来源：http://fu.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lr.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://kl.lnxyls.cn

C#:   class Admin : User {}
来源：http://df.nszjky.cn

[G06] 重写方法
来源：http://vq.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://wt.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gd.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://cb.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://ou.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://by.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rt.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ek.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://vl.shtwfgs.cn

[G07] 调用父类方法
来源：http://pr.hnjuh.cn

Py:   super().greet()
来源：http://rl.jctech888.com.cn

PHP:  parent::greet();
来源：http://gj.muxihuayi.cn

JS:   super.greet();
来源：http://zh.yuexingan06.cn

TS:   super.greet();
来源：http://hv.gzmigu.cn

Java: super.greet();
来源：http://al.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hi.521024.cn

Ruby: super
来源：http://pg.9csxet.cn

C#:   base.Greet();
来源：http://zm.hnjuh.cn

[G08] 静态方法与属性
来源：http://iv.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bu.hahajie.cn

PHP:  public static function f() {}
来源：http://sv.colortex.cn

JS:   static f() {}
来源：http://hb.521024.cn

TS:   static f(): void {}
来源：http://la.newstarts.cn

Java: static void f() {}
来源：http://vx.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ve.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://av.newstarts.cn

C#:   public static void F() {}
来源：http://lv.szsharing.cn

[G09] 接口 / 抽象类
来源：http://pe.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://pg.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://js.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ea.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://is.9csxet.cn

Java: interface Shape { double area(); }
来源：http://ng.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://fl.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xq.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ed.gzmigu.cn

[G10] 访问控制
来源：http://gz.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://nd.muxihuayi.cn

PHP:  public / protected / private
来源：http://hq.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://jo.chemitech.net.cn

TS:   public / protected / private
来源：http://ix.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://ck.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ud.shxzukj.cn

Ruby: public / protected / private
来源：http://dt.newstarts.cn

C#:   public / protected / private / internal
来源：http://ov.521024.cn

[G11] getter / setter
来源：http://is.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://ta.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zc.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://vt.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://qq.hahajie.cn

Java: public String getName() { return name; }
来源：http://nh.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ss.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ws.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://oe.yuexingan06.cn

[G12] 对象转字符串
来源：http://in.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://vh.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ic.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://bv.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://cu.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://yj.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zp.521024.cn

Ruby: def to_s; @name; end
来源：http://rl.colortex.cn

C#:   public override string ToString() => Name;
来源：http://tk.yuexingan06.cn

[G13] 判断对象类型
来源：http://ru.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://kh.muxihuayi.cn

PHP:  $u instanceof User
来源：http://bk.shtwfgs.cn

JS:   u instanceof User
来源：http://si.szsharing.cn

TS:   u instanceof User
来源：http://xt.shxzskj.cn

Java: u instanceof User
来源：http://if.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pi.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://nl.gzmigu.cn

C#:   u is User
来源：http://sf.asd995.cn

[G14] 数据类 / record
来源：http://jj.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gf.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://nr.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ld.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://zv.nszjky.cn

Java: record User(String name, int age) {}
来源：http://vl.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://il.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fz.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://jx.yuntaijiaju.cn

[G15] 枚举
来源：http://lu.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vf.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xt.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zy.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ax.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://tx.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rb.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://oh.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ay.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://im.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cz.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://al.newstarts.cn

JS:   Object.entries(obj)
来源：http://jm.gzmigu.cn

TS:   Object.entries(obj)
来源：http://qs.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://re.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pb.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://ky.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://gy.huixinmuqiang.cn

================================================================================
来源：http://ny.521024.cn

H. 异常与错误处理
来源：http://ax.yuexingan06.cn

================================================================================
来源：http://ds.gzmigu.cn

[H01] try / catch 基础
来源：http://hd.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uu.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kh.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sj.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ul.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nb.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uy.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fx.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ef.newstarts.cn

[H02] finally / ensure 收尾
来源：http://xd.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ch.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://te.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tg.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zj.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ib.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mx.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jx.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fk.huixiangedu.cn

[H03] 主动抛出异常
来源：http://qc.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://uu.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pr.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://at.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://ej.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nh.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://on.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ex.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rw.nszjky.cn

[H04] 自定义异常类型
来源：http://gi.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://ac.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vb.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ht.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://yt.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://tp.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://am.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://ns.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://ta.gzmigu.cn

[H05] 捕获特定类型
来源：http://bm.shtwfgs.cn

Py:   except ValueError as e:
来源：http://lo.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kw.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://jw.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://ym.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://yg.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ib.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://cq.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zi.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://sj.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://yn.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://na.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vf.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://po.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://df.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ai.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://vm.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://uv.nicolike.cn

[H07] 断言
来源：http://la.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://bh.huanxung.cn

PHP:  assert($x > 0);
来源：http://zf.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://hi.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://pa.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://nu.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ie.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fq.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://xz.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://tz.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://bc.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gz.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://ig.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pi.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kg.shxzskj.cn

Go:   err.Error()
来源：http://wb.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://ch.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://bu.wgjwhj.cn

[H09] 带错误码的异常
来源：http://pz.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gf.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nx.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kl.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hl.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://un.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lu.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gk.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cw.jctech888.com.cn

[H10] 资源自动释放
来源：http://lp.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ju.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vf.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wm.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tj.shtwfgs.cn

Go:   defer f.Close()
来源：http://bb.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dm.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ut.jianghongdianzi.cn

================================================================================
来源：http://sz.shxzskj.cn

I. 正则表达式
来源：http://dt.9csxet.cn

================================================================================
来源：http://ug.jctech888.com.cn

[I01] 判断是否匹配
来源：http://la.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dg.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nt.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://sc.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://ry.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gm.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://es.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://ky.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cg.wgjwhj.cn

[I02] 提取所有匹配
来源：http://gj.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://em.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://of.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jr.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://gk.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vt.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://av.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://hv.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ns.huanxung.cn

[I03] 提取捕获分组
来源：http://zd.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ii.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://my.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gr.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nn.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jg.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ee.jianghongdianzi.cn


<!-- 参考信息 -->