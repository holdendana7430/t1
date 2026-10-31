代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lv.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://zx.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jy.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fi.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bf.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vo.shtwfgs.cn

[F11] 复制与移动文件
来源：http://ux.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hd.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xu.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kc.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nr.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vy.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vz.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://im.nszjky.cn

[F12] CSV 读写
来源：http://gy.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nn.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qu.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wa.hahajie.cn

TS:   // 同上
来源：http://cs.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zo.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ej.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hw.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qi.bjjhwx.cn

================================================================================
来源：http://ar.nicolike.cn

G. 面向对象
来源：http://nq.huixiangedu.cn

================================================================================
来源：http://yz.shxzukj.cn

[G01] 定义类
来源：http://dw.shtwfgs.cn

Py:   class User: pass
来源：http://my.shxzukj.cn

PHP:  class User {}
来源：http://cf.colortex.cn

JS:   class User {}
来源：http://hr.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://cp.nicolike.cn

Java: class User {}
来源：http://yr.colortex.cn

Go:   type User struct { Name string }
来源：http://zf.yuexingan06.cn

Ruby: class User; end
来源：http://bu.521024.cn

C#:   class User {}
来源：http://eq.hahajie.cn

[G02] 构造函数
来源：http://hh.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://jt.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://qq.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://hk.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://un.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://jd.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oc.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://em.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://sy.bjjhwx.cn

[G03] 实例属性
来源：http://eu.asd995.cn

Py:   self.name = "x"
来源：http://nv.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://zm.chemitech.net.cn

JS:   this.name = "x";
来源：http://zq.hnjuh.cn

TS:   name: string = "x";
来源：http://tq.muxihuayi.cn

Java: private String name;
来源：http://ty.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dc.bookmarksfly.cn

Ruby: @name = "x"
来源：http://wa.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://dq.panjiajie.cn

[G04] 定义方法
来源：http://ze.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://wv.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gd.colortex.cn

JS:   greet() { return this.name; }
来源：http://zg.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://cf.colortex.cn

Java: String greet() { return name; }
来源：http://ey.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ve.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://ms.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://py.jctech888.com.cn

[G05] 继承
来源：http://wy.szxytkj.cn

Py:   class Admin(User): pass
来源：http://hq.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://yp.newstarts.cn

JS:   class Admin extends User {}
来源：http://je.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://qd.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://qn.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lk.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://km.colortex.cn

C#:   class Admin : User {}
来源：http://am.hnjuh.cn

[G06] 重写方法
来源：http://it.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://ey.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://om.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://pc.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://hz.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://qp.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ve.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://hi.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://zu.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://zf.panjiajie.cn

Py:   super().greet()
来源：http://od.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://aa.szsharing.cn

JS:   super.greet();
来源：http://me.nszjky.cn

TS:   super.greet();
来源：http://hs.gzmigu.cn

Java: super.greet();
来源：http://mw.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cd.hahajie.cn

Ruby: super
来源：http://mq.haigaiapp.cn

C#:   base.Greet();
来源：http://vv.wgjwhj.cn

[G08] 静态方法与属性
来源：http://nh.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dq.haigaiapp.cn

PHP:  public static function f() {}
来源：http://om.panjiajie.cn

JS:   static f() {}
来源：http://ws.yuexingan06.cn

TS:   static f(): void {}
来源：http://rg.nszjky.cn

Java: static void f() {}
来源：http://az.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ra.hnjuh.cn

Ruby: def self.f; end
来源：http://ib.wgjwhj.cn

C#:   public static void F() {}
来源：http://ss.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://yj.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://wp.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ze.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gn.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://na.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://lm.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://vt.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hw.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://dz.nszjky.cn

[G10] 访问控制
来源：http://ce.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://gn.shtwfgs.cn

PHP:  public / protected / private
来源：http://tu.nicolike.cn

JS:   #private 字段；其余公开
来源：http://sh.chemitech.net.cn

TS:   public / protected / private
来源：http://ik.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://ot.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xu.yuexingan06.cn

Ruby: public / protected / private
来源：http://ru.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://sd.huixinmuqiang.cn

[G11] getter / setter
来源：http://nr.hahajie.cn

Py:   @property 与 @x.setter
来源：http://oz.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jg.hahajie.cn

JS:   get name() { return this._name; }
来源：http://bb.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://py.hahajie.cn

Java: public String getName() { return name; }
来源：http://vu.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bi.huanxung.cn

Ruby: attr_accessor :name
来源：http://vu.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://np.muxihuayi.cn

[G12] 对象转字符串
来源：http://vs.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://bc.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eb.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://nh.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://wz.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://uq.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rd.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://ca.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://jb.szxytkj.cn

[G13] 判断对象类型
来源：http://dr.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://yy.szsharing.cn

PHP:  $u instanceof User
来源：http://pn.jctech888.com.cn

JS:   u instanceof User
来源：http://bt.colortex.cn

TS:   u instanceof User
来源：http://sm.shxzukj.cn

Java: u instanceof User
来源：http://yo.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rj.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://nz.yuexingan06.cn

C#:   u is User
来源：http://si.colortex.cn

[G14] 数据类 / record
来源：http://kj.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tr.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://sy.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://un.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://li.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ci.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://bd.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://my.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://vi.bjjhwx.cn

[G15] 枚举
来源：http://va.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ri.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lt.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hb.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aa.521024.cn

Java: enum Color { RED, GREEN }
来源：http://hw.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qm.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://xo.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://um.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://aw.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xj.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://om.hnjuh.cn

JS:   Object.entries(obj)
来源：http://dh.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://yr.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ic.asd995.cn

Ruby: obj.instance_variables
来源：http://ra.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://oq.nicolike.cn

================================================================================
来源：http://qc.panjiajie.cn

H. 异常与错误处理
来源：http://nw.nszjky.cn

================================================================================
来源：http://yk.jctech888.com.cn

[H01] try / catch 基础
来源：http://jy.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bk.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xe.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sc.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cy.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iw.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cl.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pi.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vm.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://oe.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gi.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pl.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ek.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xw.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xl.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zl.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jz.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sw.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://cp.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://kg.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uc.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://bz.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://op.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vp.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ls.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://af.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ov.shxzukj.cn

[H04] 自定义异常类型
来源：http://dg.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://jc.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lh.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ri.colortex.cn

TS:   class MyError extends Error {}
来源：http://hx.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://gj.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wo.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://uy.hahajie.cn

C#:   class MyException : Exception {}
来源：http://ct.asd995.cn

[H05] 捕获特定类型
来源：http://no.huixiangedu.cn

Py:   except ValueError as e:
来源：http://dq.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yu.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://li.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://ta.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://gt.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wh.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://oz.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fx.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://gl.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://it.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://of.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tu.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dg.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xi.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kp.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://kg.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://fb.hahajie.cn

[H07] 断言
来源：http://bh.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://ox.newstarts.cn

PHP:  assert($x > 0);
来源：http://om.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://vf.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://in.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://vb.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ec.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ft.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://sx.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://oi.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://bw.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jx.shxzskj.cn

JS:   e.message;  e.stack
来源：http://dp.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vp.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pg.nszjky.cn

Go:   err.Error()
来源：http://oz.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://jp.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://jb.chemitech.net.cn

[H09] 带错误码的异常
来源：http://lz.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xk.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ry.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://km.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bp.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wj.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kg.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rs.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lt.hnjuh.cn

[H10] 资源自动释放
来源：http://cr.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uf.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://em.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nu.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zg.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kv.szxytkj.cn

Go:   defer f.Close()
来源：http://cn.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nj.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fc.hahajie.cn

================================================================================
来源：http://fr.huixiangedu.cn

I. 正则表达式
来源：http://vk.muxihuayi.cn

================================================================================
来源：http://vx.hnjuh.cn

[I01] 判断是否匹配
来源：http://zd.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://is.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://us.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://ly.asd995.cn

TS:   /\d+/.test(s)
来源：http://yw.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nq.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://al.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://bm.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tx.lnxyls.cn

[I02] 提取所有匹配
来源：http://oj.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://an.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cz.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iv.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://rz.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://av.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pn.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://tr.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zv.9csxet.cn

[I03] 提取捕获分组
来源：http://yg.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zn.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pz.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tp.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ew.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sr.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xa.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mo.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ll.bjjhwx.cn

[I04] 正则替换
来源：http://pk.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dw.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rd.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bq.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nu.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pg.shxzskj.cn


<!-- 参考信息 -->