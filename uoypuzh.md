代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://jr.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://rt.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fg.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vm.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vt.newstarts.cn

TS:   path.extname("a.txt")
来源：http://zf.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qe.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yl.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ki.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wz.nszjky.cn

[F11] 复制与移动文件
来源：http://hz.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gd.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ou.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cr.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rt.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ak.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hn.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ch.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hx.gzmigu.cn

[F12] CSV 读写
来源：http://ru.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rt.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ka.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xu.gzmigu.cn

TS:   // 同上
来源：http://vy.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://od.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wi.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mc.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pz.yuexingan06.cn

================================================================================
来源：http://lz.hnjuh.cn

G. 面向对象
来源：http://wy.bjjhwx.cn

================================================================================
来源：http://dc.shxzskj.cn

[G01] 定义类
来源：http://sw.jianghongdianzi.cn

Py:   class User: pass
来源：http://wh.asd995.cn

PHP:  class User {}
来源：http://ru.shtwfgs.cn

JS:   class User {}
来源：http://px.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://nw.gzmigu.cn

Java: class User {}
来源：http://ug.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://yc.wgjwhj.cn

Ruby: class User; end
来源：http://al.chemitech.net.cn

C#:   class User {}
来源：http://cs.muxihuayi.cn

[G02] 构造函数
来源：http://ow.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://br.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://hx.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ov.colortex.cn

TS:   constructor(public name: string) {}
来源：http://tv.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://ov.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nc.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://lt.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ao.huixinmuqiang.cn

[G03] 实例属性
来源：http://fd.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://lc.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://wq.haigaiapp.cn

JS:   this.name = "x";
来源：http://ih.wgjwhj.cn

TS:   name: string = "x";
来源：http://ki.nicolike.cn

Java: private String name;
来源：http://ka.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ug.chemitech.net.cn

Ruby: @name = "x"
来源：http://lv.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://yr.shxzukj.cn

[G04] 定义方法
来源：http://uq.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://gw.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nx.colortex.cn

JS:   greet() { return this.name; }
来源：http://tn.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://sd.lnxyls.cn

Java: String greet() { return name; }
来源：http://ny.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tz.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://ae.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://wo.szxytkj.cn

[G05] 继承
来源：http://ie.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://st.nicolike.cn

PHP:  class Admin extends User {}
来源：http://um.shxzskj.cn

JS:   class Admin extends User {}
来源：http://vi.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://al.nszjky.cn

Java: class Admin extends User {}
来源：http://wz.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bm.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://la.shxzskj.cn

C#:   class Admin : User {}
来源：http://pp.nicolike.cn

[G06] 重写方法
来源：http://ty.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://wm.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ki.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://gl.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://zo.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://fl.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nv.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://wq.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://ec.nicolike.cn

[G07] 调用父类方法
来源：http://ah.jianghongdianzi.cn

Py:   super().greet()
来源：http://qm.shxzskj.cn

PHP:  parent::greet();
来源：http://mx.szsharing.cn

JS:   super.greet();
来源：http://cn.chemitech.net.cn

TS:   super.greet();
来源：http://de.jianghongdianzi.cn

Java: super.greet();
来源：http://qn.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fz.bookmarksfly.cn

Ruby: super
来源：http://ar.hahajie.cn

C#:   base.Greet();
来源：http://yi.szxytkj.cn

[G08] 静态方法与属性
来源：http://xy.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lh.huixiangedu.cn

PHP:  public static function f() {}
来源：http://ee.newstarts.cn

JS:   static f() {}
来源：http://bf.bjjhwx.cn

TS:   static f(): void {}
来源：http://qq.chemitech.net.cn

Java: static void f() {}
来源：http://yd.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mt.nicolike.cn

Ruby: def self.f; end
来源：http://ln.hnjuh.cn

C#:   public static void F() {}
来源：http://cd.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://un.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://et.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gx.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kt.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://bb.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://te.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://qn.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cn.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://xc.shxzskj.cn

[G10] 访问控制
来源：http://di.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://cw.bookmarksfly.cn

PHP:  public / protected / private
来源：http://pf.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://xx.colortex.cn

TS:   public / protected / private
来源：http://oz.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://th.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nx.huixiangedu.cn

Ruby: public / protected / private
来源：http://rx.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://fh.shtwfgs.cn

[G11] getter / setter
来源：http://sv.hahajie.cn

Py:   @property 与 @x.setter
来源：http://ct.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ee.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://sf.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://rx.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://hx.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vb.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://jv.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://qv.lnxyls.cn

[G12] 对象转字符串
来源：http://ht.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://xt.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ne.521024.cn

JS:   toString() { return this.name; }
来源：http://tm.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://zd.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://gd.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xc.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://qf.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://co.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://gn.nszjky.cn

Py:   isinstance(u, User)
来源：http://pg.nszjky.cn

PHP:  $u instanceof User
来源：http://ae.szsharing.cn

JS:   u instanceof User
来源：http://qz.muxihuayi.cn

TS:   u instanceof User
来源：http://bu.yuexingan06.cn

Java: u instanceof User
来源：http://jn.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vi.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://og.yuexingan06.cn

C#:   u is User
来源：http://mk.szsharing.cn

[G14] 数据类 / record
来源：http://jz.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vv.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://ck.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lh.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://mk.nszjky.cn

Java: record User(String name, int age) {}
来源：http://ty.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://pl.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jq.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://bc.asd995.cn

[G15] 枚举
来源：http://xl.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pt.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fb.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xn.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ll.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://oi.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dt.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://rh.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tr.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://ut.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://on.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://zf.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://kn.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://gc.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yz.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zh.panjiajie.cn

Ruby: obj.instance_variables
来源：http://ba.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://px.chemitech.net.cn

================================================================================
来源：http://xh.szxytkj.cn

H. 异常与错误处理
来源：http://dk.szsharing.cn

================================================================================
来源：http://cx.bookmarksfly.cn

[H01] try / catch 基础
来源：http://mk.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://we.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yn.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yg.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xd.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uo.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ek.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zt.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nq.9csxet.cn

[H02] finally / ensure 收尾
来源：http://mf.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bb.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fu.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tl.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jv.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gc.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vr.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xt.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mr.colortex.cn

[H03] 主动抛出异常
来源：http://tp.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://xr.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://js.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://mt.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://ah.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bx.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dh.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ex.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vt.shxzukj.cn

[H04] 自定义异常类型
来源：http://av.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://no.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qu.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://pc.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://yq.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://wz.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lg.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://gh.asd995.cn

C#:   class MyException : Exception {}
来源：http://oa.9csxet.cn

[H05] 捕获特定类型
来源：http://sp.panjiajie.cn

Py:   except ValueError as e:
来源：http://xh.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ho.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://av.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://tl.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://tj.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fy.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://ze.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aq.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://iv.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://qo.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xc.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xg.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xo.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xn.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ns.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://gk.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://uz.521024.cn

[H07] 断言
来源：http://mv.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://to.newstarts.cn

PHP:  assert($x > 0);
来源：http://ov.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://pv.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://zn.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://eb.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ho.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ex.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://xk.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://iq.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://jy.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bd.521024.cn

JS:   e.message;  e.stack
来源：http://lz.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mj.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vk.szsharing.cn

Go:   err.Error()
来源：http://vu.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://vf.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://hm.hnjuh.cn

[H09] 带错误码的异常
来源：http://ls.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oq.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fb.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zr.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hx.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://op.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rp.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nj.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ri.shtwfgs.cn

[H10] 资源自动释放
来源：http://ps.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pz.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tb.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gt.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sv.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dt.szxytkj.cn

Go:   defer f.Close()
来源：http://ql.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cs.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hi.wgjwhj.cn

================================================================================
来源：http://za.hahajie.cn

I. 正则表达式
来源：http://zc.shxzskj.cn

================================================================================
来源：http://ig.huanxung.cn

[I01] 判断是否匹配
来源：http://wy.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fg.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://po.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://op.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://uu.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mk.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lf.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://el.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cw.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ec.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://gy.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mb.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qr.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://ex.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ec.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bh.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://rv.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nm.521024.cn

[I03] 提取捕获分组
来源：http://lu.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yg.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wx.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tj.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ll.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://il.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cd.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wl.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vk.yuntaijiaju.cn

[I04] 正则替换
来源：http://ah.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ok.szxytkj.cn


<!-- 参考信息 -->