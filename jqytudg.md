代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://ob.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qy.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yd.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://aj.521024.cn

Ruby: File.delete("a.txt")
来源：http://lk.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://bh.szsharing.cn

[F07] 创建目录（含多级）
来源：http://jt.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dr.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ts.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cw.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nq.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nn.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yx.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pu.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yr.chemitech.net.cn

[F08] 遍历目录
来源：http://pe.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yo.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oa.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://af.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://ix.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jy.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gh.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://vf.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://rm.hahajie.cn

[F09] 获取文件大小
来源：http://pr.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://zr.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://cf.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://hf.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://ma.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ca.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dk.newstarts.cn

Ruby: File.size("a.txt")
来源：http://kr.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ii.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://yg.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mr.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://do.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dw.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://iy.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sm.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hl.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gi.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qq.shtwfgs.cn

[F11] 复制与移动文件
来源：http://ja.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oh.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ej.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lo.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lm.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ec.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bs.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ss.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hu.szxytkj.cn

[F12] CSV 读写
来源：http://ca.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dr.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wc.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nd.colortex.cn

TS:   // 同上
来源：http://ua.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kk.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ya.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nc.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mq.jctech888.com.cn

================================================================================
来源：http://pk.szxytkj.cn

G. 面向对象
来源：http://ty.nicolike.cn

================================================================================
来源：http://fe.shxzukj.cn

[G01] 定义类
来源：http://gw.szsharing.cn

Py:   class User: pass
来源：http://yi.hnjuh.cn

PHP:  class User {}
来源：http://kq.shtwfgs.cn

JS:   class User {}
来源：http://hk.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://sp.gzmigu.cn

Java: class User {}
来源：http://wh.hahajie.cn

Go:   type User struct { Name string }
来源：http://fl.newstarts.cn

Ruby: class User; end
来源：http://si.bookmarksfly.cn

C#:   class User {}
来源：http://ro.chemitech.net.cn

[G02] 构造函数
来源：http://rr.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://jp.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://hi.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://qf.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://zf.521024.cn

Java: User(String name) { this.name = name; }
来源：http://hq.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nn.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://na.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://hq.yuntaijiaju.cn

[G03] 实例属性
来源：http://xg.nicolike.cn

Py:   self.name = "x"
来源：http://os.nicolike.cn

PHP:  public string $name = "x";
来源：http://rk.panjiajie.cn

JS:   this.name = "x";
来源：http://fu.shxzskj.cn

TS:   name: string = "x";
来源：http://jh.shtwfgs.cn

Java: private String name;
来源：http://ip.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hy.wgjwhj.cn

Ruby: @name = "x"
来源：http://yp.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://mv.hnjuh.cn

[G04] 定义方法
来源：http://kx.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://bq.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nn.colortex.cn

JS:   greet() { return this.name; }
来源：http://ql.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://yd.chemitech.net.cn

Java: String greet() { return name; }
来源：http://fh.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dk.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://oh.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://bw.hnjuh.cn

[G05] 继承
来源：http://fq.newstarts.cn

Py:   class Admin(User): pass
来源：http://ap.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://zm.shxzukj.cn

JS:   class Admin extends User {}
来源：http://of.newstarts.cn

TS:   class Admin extends User {}
来源：http://od.wgjwhj.cn

Java: class Admin extends User {}
来源：http://pz.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yc.shxzskj.cn

Ruby: class Admin < User; end
来源：http://zh.asd995.cn

C#:   class Admin : User {}
来源：http://vj.9csxet.cn

[G06] 重写方法
来源：http://ag.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://la.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fu.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://er.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://cv.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://hy.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ay.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://ou.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://ep.newstarts.cn

[G07] 调用父类方法
来源：http://ll.panjiajie.cn

Py:   super().greet()
来源：http://cu.haigaiapp.cn

PHP:  parent::greet();
来源：http://ot.wgjwhj.cn

JS:   super.greet();
来源：http://wc.muxihuayi.cn

TS:   super.greet();
来源：http://km.lnxyls.cn

Java: super.greet();
来源：http://gg.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://el.shxzskj.cn

Ruby: super
来源：http://ut.haigaiapp.cn

C#:   base.Greet();
来源：http://ls.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://ww.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mi.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://ms.9csxet.cn

JS:   static f() {}
来源：http://vo.huixiangedu.cn

TS:   static f(): void {}
来源：http://ob.huixinmuqiang.cn

Java: static void f() {}
来源：http://gk.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rb.hahajie.cn

Ruby: def self.f; end
来源：http://dr.hnjuh.cn

C#:   public static void F() {}
来源：http://wd.asd995.cn

[G09] 接口 / 抽象类
来源：http://bo.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://nw.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mr.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://up.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://oq.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://mg.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://xm.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://og.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://ou.9csxet.cn

[G10] 访问控制
来源：http://do.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ee.jctech888.com.cn

PHP:  public / protected / private
来源：http://sy.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://mm.lnxyls.cn

TS:   public / protected / private
来源：http://eq.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://yl.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mf.gzmigu.cn

Ruby: public / protected / private
来源：http://zu.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://ut.newstarts.cn

[G11] getter / setter
来源：http://vn.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://zu.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qo.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://tl.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://ye.shxzskj.cn

Java: public String getName() { return name; }
来源：http://nv.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qc.nszjky.cn

Ruby: attr_accessor :name
来源：http://cn.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://uy.hnjuh.cn

[G12] 对象转字符串
来源：http://cy.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://nh.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bh.hahajie.cn

JS:   toString() { return this.name; }
来源：http://nh.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://yj.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://mo.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dg.newstarts.cn

Ruby: def to_s; @name; end
来源：http://zf.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://ju.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://jq.huanxung.cn

Py:   isinstance(u, User)
来源：http://ap.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://wl.asd995.cn

JS:   u instanceof User
来源：http://dv.yuexingan06.cn

TS:   u instanceof User
来源：http://ap.bjjhwx.cn

Java: u instanceof User
来源：http://bx.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sl.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://to.jctech888.com.cn

C#:   u is User
来源：http://sy.lnxyls.cn

[G14] 数据类 / record
来源：http://an.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wg.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://vm.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xi.521024.cn

TS:   type User = { name: string; age: number };
来源：http://gr.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ft.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://na.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ie.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://zq.shxzukj.cn

[G15] 枚举
来源：http://go.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sm.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fd.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eo.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bx.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://wi.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ew.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://tt.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sw.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://pm.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nj.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://uy.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://xk.hnjuh.cn

TS:   Object.entries(obj)
来源：http://nk.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://si.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://va.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://tv.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://yl.gzmigu.cn

================================================================================
来源：http://hh.nszjky.cn

H. 异常与错误处理
来源：http://ah.shxzukj.cn

================================================================================
来源：http://ua.shxzukj.cn

[H01] try / catch 基础
来源：http://eb.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://db.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qf.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qi.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sd.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xo.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ap.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://em.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mf.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://ps.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tx.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tw.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ux.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gn.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lq.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sm.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ll.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qt.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://ur.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://nj.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tx.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://rn.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://ec.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zq.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jy.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nw.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dz.shxzskj.cn

[H04] 自定义异常类型
来源：http://sq.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://sf.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aj.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://ia.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://yl.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://xh.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zq.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://cl.colortex.cn

C#:   class MyException : Exception {}
来源：http://vb.szsharing.cn

[H05] 捕获特定类型
来源：http://jz.521024.cn

Py:   except ValueError as e:
来源：http://tr.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ho.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://ge.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://px.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://dq.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tp.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://xv.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uz.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://as.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://id.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ng.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ru.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aw.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lh.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yz.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://kg.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://gc.yuntaijiaju.cn

[H07] 断言
来源：http://uz.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://mi.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://eh.hahajie.cn

JS:   console.assert(x > 0);
来源：http://aw.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://ko.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://jf.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wr.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wu.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://ys.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://ql.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://eu.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://si.szsharing.cn

JS:   e.message;  e.stack
来源：http://jy.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xa.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kq.wgjwhj.cn

Go:   err.Error()
来源：http://nw.521024.cn

Ruby: e.message;  e.backtrace
来源：http://vt.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://fx.jctech888.com.cn

[H09] 带错误码的异常
来源：http://bg.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kn.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://at.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hi.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tr.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sb.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://db.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fx.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tt.shxzukj.cn

[H10] 资源自动释放
来源：http://bw.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lk.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ad.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ns.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zr.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iu.yuexingan06.cn

Go:   defer f.Close()
来源：http://lv.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fx.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jy.521024.cn


<!-- 参考信息 -->