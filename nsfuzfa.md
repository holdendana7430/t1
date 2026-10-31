代发 wailian999

[F09] 获取文件大小
来源：http://cn.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://td.szsharing.cn

PHP:  filesize("a.txt");
来源：http://bj.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://ko.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://wn.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ar.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hb.huanxung.cn

Ruby: File.size("a.txt")
来源：http://hd.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://nn.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://yl.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vf.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zx.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eb.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://kj.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tr.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ry.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ty.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qy.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://fr.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eu.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iw.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dw.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vx.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ga.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uy.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ho.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vw.colortex.cn

[F12] CSV 读写
来源：http://am.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://un.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ic.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qs.521024.cn

TS:   // 同上
来源：http://ib.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dm.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zu.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wj.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yh.huixinmuqiang.cn

================================================================================
来源：http://xp.asd995.cn

G. 面向对象
来源：http://sz.521024.cn

================================================================================
来源：http://mq.yuntaijiaju.cn

[G01] 定义类
来源：http://lo.muxihuayi.cn

Py:   class User: pass
来源：http://in.jctech888.com.cn

PHP:  class User {}
来源：http://lq.yuexingan06.cn

JS:   class User {}
来源：http://ev.asd995.cn

TS:   class User { name: string = ""; }
来源：http://es.shxzskj.cn

Java: class User {}
来源：http://mx.newstarts.cn

Go:   type User struct { Name string }
来源：http://zs.yuexingan06.cn

Ruby: class User; end
来源：http://ad.9csxet.cn

C#:   class User {}
来源：http://wr.shxzskj.cn

[G02] 构造函数
来源：http://hi.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://yg.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://gr.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://kc.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://fh.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://cd.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bs.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://hc.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://ke.szxytkj.cn

[G03] 实例属性
来源：http://mh.shtwfgs.cn

Py:   self.name = "x"
来源：http://rj.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://ed.bookmarksfly.cn

JS:   this.name = "x";
来源：http://lo.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://co.bjjhwx.cn

Java: private String name;
来源：http://ir.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ku.panjiajie.cn

Ruby: @name = "x"
来源：http://xo.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://zn.shxzukj.cn

[G04] 定义方法
来源：http://zr.szsharing.cn

Py:   def greet(self): return self.name
来源：http://mt.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xq.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://iq.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://zu.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://gp.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ie.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://an.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ce.shtwfgs.cn

[G05] 继承
来源：http://st.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://bk.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://rw.shxzukj.cn

JS:   class Admin extends User {}
来源：http://rx.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://gp.shtwfgs.cn

Java: class Admin extends User {}
来源：http://gw.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uz.hnjuh.cn

Ruby: class Admin < User; end
来源：http://uk.shxzukj.cn

C#:   class Admin : User {}
来源：http://fr.shtwfgs.cn

[G06] 重写方法
来源：http://wf.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://jt.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hc.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://hi.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://sc.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://fg.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mf.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://wu.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://fx.shxzukj.cn

[G07] 调用父类方法
来源：http://pt.bookmarksfly.cn

Py:   super().greet()
来源：http://ma.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://yp.newstarts.cn

JS:   super.greet();
来源：http://oc.haigaiapp.cn

TS:   super.greet();
来源：http://rh.huixinmuqiang.cn

Java: super.greet();
来源：http://of.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yp.huixinmuqiang.cn

Ruby: super
来源：http://ox.jctech888.com.cn

C#:   base.Greet();
来源：http://ac.muxihuayi.cn

[G08] 静态方法与属性
来源：http://ll.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://af.lnxyls.cn

PHP:  public static function f() {}
来源：http://hb.shxzukj.cn

JS:   static f() {}
来源：http://pk.huanxung.cn

TS:   static f(): void {}
来源：http://do.muxihuayi.cn

Java: static void f() {}
来源：http://he.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rl.szxytkj.cn

Ruby: def self.f; end
来源：http://fi.yuexingan06.cn

C#:   public static void F() {}
来源：http://oc.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://fd.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://cu.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gr.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kj.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://mf.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://fu.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://yl.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kq.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://ai.asd995.cn

[G10] 访问控制
来源：http://eo.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://kb.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://ve.newstarts.cn

JS:   #private 字段；其余公开
来源：http://vk.shxzskj.cn

TS:   public / protected / private
来源：http://rs.colortex.cn

Java: public / protected / private / 默认包级
来源：http://lq.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sn.muxihuayi.cn

Ruby: public / protected / private
来源：http://pp.colortex.cn

C#:   public / protected / private / internal
来源：http://od.yuntaijiaju.cn

[G11] getter / setter
来源：http://yw.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ok.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qd.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://jx.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://jl.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://za.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fk.521024.cn

Ruby: attr_accessor :name
来源：http://hn.szsharing.cn

C#:   public string Name { get; set; }
来源：http://zg.colortex.cn

[G12] 对象转字符串
来源：http://qr.asd995.cn

Py:   def __str__(self): return self.name
来源：http://bu.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fl.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://kz.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://gj.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://sx.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://by.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://id.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://ez.panjiajie.cn

[G13] 判断对象类型
来源：http://ku.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://rm.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://ig.hnjuh.cn

JS:   u instanceof User
来源：http://qp.chemitech.net.cn

TS:   u instanceof User
来源：http://va.jianghongdianzi.cn

Java: u instanceof User
来源：http://is.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xr.huanxung.cn

Ruby: u.is_a?(User)
来源：http://sb.bjjhwx.cn

C#:   u is User
来源：http://qd.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://hl.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://te.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://qn.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://os.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://qf.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://ib.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://fs.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vs.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://ob.jctech888.com.cn

[G15] 枚举
来源：http://xb.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rc.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rz.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nr.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aw.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://jq.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tg.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://lh.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ai.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://yq.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vv.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://um.newstarts.cn

JS:   Object.entries(obj)
来源：http://am.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://ik.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://we.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ej.shxzskj.cn

Ruby: obj.instance_variables
来源：http://yb.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://of.lnxyls.cn

================================================================================
来源：http://ex.bookmarksfly.cn

H. 异常与错误处理
来源：http://pm.bookmarksfly.cn

================================================================================
来源：http://fm.gzmigu.cn

[H01] try / catch 基础
来源：http://eg.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kg.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ar.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qa.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://df.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nx.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sr.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://im.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vh.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://aj.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ff.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rz.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mo.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zs.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mz.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://al.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hp.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lk.bjjhwx.cn

[H03] 主动抛出异常
来源：http://wn.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://tl.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yq.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://ju.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://kh.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ej.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://di.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iz.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sn.gzmigu.cn

[H04] 自定义异常类型
来源：http://or.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://ns.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qb.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://fd.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://je.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://wm.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vr.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://fr.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://zr.9csxet.cn

[H05] 捕获特定类型
来源：http://vj.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://oz.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ey.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://ev.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://cg.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://fz.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xz.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://nm.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ax.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://zm.szsharing.cn

Py:   value = d.get("k") or default
来源：http://ml.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cy.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ff.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iw.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iu.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qt.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://ah.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://po.szsharing.cn

[H07] 断言
来源：http://xl.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://hj.panjiajie.cn

PHP:  assert($x > 0);
来源：http://pi.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://at.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://pq.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://zy.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ak.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tb.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://tb.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://yq.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://dg.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://un.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://em.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rr.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://de.chemitech.net.cn

Go:   err.Error()
来源：http://nu.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://wr.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://rc.shxzskj.cn

[H09] 带错误码的异常
来源：http://dz.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eh.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mq.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://da.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://im.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://go.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yw.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ok.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cb.muxihuayi.cn

[H10] 资源自动释放
来源：http://ph.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cb.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vr.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vo.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zz.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ug.shtwfgs.cn

Go:   defer f.Close()
来源：http://ut.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gc.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://os.newstarts.cn

================================================================================
来源：http://ne.shtwfgs.cn

I. 正则表达式
来源：http://gj.shxzskj.cn

================================================================================
来源：http://ad.szxytkj.cn

[I01] 判断是否匹配
来源：http://ml.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dg.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fl.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://ab.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://hg.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ly.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oj.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://gw.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pg.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://zu.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://vc.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://os.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ln.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://my.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cc.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lp.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://co.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cc.shxzukj.cn

[I03] 提取捕获分组
来源：http://tb.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lu.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wv.huixiangedu.cn


<!-- 参考信息 -->