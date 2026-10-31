代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://ck.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uo.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ke.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://mu.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://sy.colortex.cn

C#:   File.Delete("a.txt");
来源：http://pe.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://ii.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dh.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vy.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sn.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://se.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hp.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kw.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fg.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bq.yuexingan06.cn

[F08] 遍历目录
来源：http://cv.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://np.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nq.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://pr.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://lt.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qx.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ab.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ak.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://uh.shxzukj.cn

[F09] 获取文件大小
来源：http://zk.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://xw.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://za.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://iw.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://zk.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pi.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nl.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://sh.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://rl.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ts.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vu.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zk.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pa.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://oq.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yd.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cc.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yx.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yq.huixiangedu.cn

[F11] 复制与移动文件
来源：http://lc.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mv.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iu.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jx.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qf.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jz.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cs.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cv.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ow.szxytkj.cn

[F12] CSV 读写
来源：http://ku.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ae.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://er.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sm.chemitech.net.cn

TS:   // 同上
来源：http://mv.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qo.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://br.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://so.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lu.szxytkj.cn

================================================================================
来源：http://qx.yuexingan06.cn

G. 面向对象
来源：http://sa.shxzukj.cn

================================================================================
来源：http://zg.hahajie.cn

[G01] 定义类
来源：http://va.huixinmuqiang.cn

Py:   class User: pass
来源：http://ea.huanxung.cn

PHP:  class User {}
来源：http://ef.yuntaijiaju.cn

JS:   class User {}
来源：http://xf.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://eg.shxzukj.cn

Java: class User {}
来源：http://tb.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://mg.jctech888.com.cn

Ruby: class User; end
来源：http://zk.nszjky.cn

C#:   class User {}
来源：http://sg.muxihuayi.cn

[G02] 构造函数
来源：http://qp.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://mj.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://bd.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://jc.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://qi.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://uh.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nc.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://zx.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://kx.huanxung.cn

[G03] 实例属性
来源：http://eg.9csxet.cn

Py:   self.name = "x"
来源：http://rw.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://yb.nszjky.cn

JS:   this.name = "x";
来源：http://pw.nicolike.cn

TS:   name: string = "x";
来源：http://cp.bookmarksfly.cn

Java: private String name;
来源：http://hs.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rx.521024.cn

Ruby: @name = "x"
来源：http://yv.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://jx.huixinmuqiang.cn

[G04] 定义方法
来源：http://sy.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://ve.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ft.521024.cn

JS:   greet() { return this.name; }
来源：http://hy.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://bw.asd995.cn

Java: String greet() { return name; }
来源：http://ix.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bh.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://kg.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://ww.shxzskj.cn

[G05] 继承
来源：http://xw.hahajie.cn

Py:   class Admin(User): pass
来源：http://kd.521024.cn

PHP:  class Admin extends User {}
来源：http://ui.nicolike.cn

JS:   class Admin extends User {}
来源：http://it.asd995.cn

TS:   class Admin extends User {}
来源：http://cm.colortex.cn

Java: class Admin extends User {}
来源：http://au.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jk.shxzskj.cn

Ruby: class Admin < User; end
来源：http://cr.lnxyls.cn

C#:   class Admin : User {}
来源：http://lo.shxzukj.cn

[G06] 重写方法
来源：http://ov.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://cc.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xv.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://go.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://nm.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://oh.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sv.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://hg.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://it.gzmigu.cn

[G07] 调用父类方法
来源：http://wz.yuexingan06.cn

Py:   super().greet()
来源：http://af.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://kj.huixinmuqiang.cn

JS:   super.greet();
来源：http://kw.shxzukj.cn

TS:   super.greet();
来源：http://mp.newstarts.cn

Java: super.greet();
来源：http://jf.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xy.chemitech.net.cn

Ruby: super
来源：http://px.hnjuh.cn

C#:   base.Greet();
来源：http://cd.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://cy.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jw.lnxyls.cn

PHP:  public static function f() {}
来源：http://by.asd995.cn

JS:   static f() {}
来源：http://yo.wgjwhj.cn

TS:   static f(): void {}
来源：http://cx.bjjhwx.cn

Java: static void f() {}
来源：http://wj.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cy.jctech888.com.cn

Ruby: def self.f; end
来源：http://ct.lnxyls.cn

C#:   public static void F() {}
来源：http://gq.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://lk.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://vg.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zi.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cz.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://lf.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://vo.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ob.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wn.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://nz.colortex.cn

[G10] 访问控制
来源：http://bd.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://ev.newstarts.cn

PHP:  public / protected / private
来源：http://qx.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://rc.nicolike.cn

TS:   public / protected / private
来源：http://uo.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://xb.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cu.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://wz.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://uy.chemitech.net.cn

[G11] getter / setter
来源：http://sc.hahajie.cn

Py:   @property 与 @x.setter
来源：http://fw.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cv.nszjky.cn

JS:   get name() { return this._name; }
来源：http://pk.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://sh.lnxyls.cn

Java: public String getName() { return name; }
来源：http://gi.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dv.9csxet.cn

Ruby: attr_accessor :name
来源：http://ww.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://ch.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://tv.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://gz.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kb.colortex.cn

JS:   toString() { return this.name; }
来源：http://zl.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://tc.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://xg.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zf.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://we.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://re.shxzskj.cn

[G13] 判断对象类型
来源：http://iz.nicolike.cn

Py:   isinstance(u, User)
来源：http://cf.chemitech.net.cn

PHP:  $u instanceof User
来源：http://pt.panjiajie.cn

JS:   u instanceof User
来源：http://ic.newstarts.cn

TS:   u instanceof User
来源：http://pr.hahajie.cn

Java: u instanceof User
来源：http://hw.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cg.colortex.cn

Ruby: u.is_a?(User)
来源：http://cw.bjjhwx.cn

C#:   u is User
来源：http://an.hahajie.cn

[G14] 数据类 / record
来源：http://zs.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xn.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://km.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://do.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://iu.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://rw.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ws.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ts.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://bq.nszjky.cn

[G15] 枚举
来源：http://gt.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ye.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lp.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cm.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wa.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://rl.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pq.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://rv.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nz.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://ft.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://js.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://fb.hnjuh.cn

JS:   Object.entries(obj)
来源：http://sc.hnjuh.cn

TS:   Object.entries(obj)
来源：http://ro.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bh.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zl.nszjky.cn

Ruby: obj.instance_variables
来源：http://we.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://vf.jianghongdianzi.cn

================================================================================
来源：http://oy.nicolike.cn

H. 异常与错误处理
来源：http://tp.panjiajie.cn

================================================================================
来源：http://ge.newstarts.cn

[H01] try / catch 基础
来源：http://ut.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ik.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fy.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dm.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sw.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jz.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gy.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sg.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fa.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://nt.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ih.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bh.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nn.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nz.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pv.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pa.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ef.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lf.szsharing.cn

[H03] 主动抛出异常
来源：http://qc.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://nm.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qa.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://wp.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://qf.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yx.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://le.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sf.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rj.huixiangedu.cn

[H04] 自定义异常类型
来源：http://wp.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://jf.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xa.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ad.nszjky.cn

TS:   class MyError extends Error {}
来源：http://mx.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://dx.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zp.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://as.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://qq.521024.cn

[H05] 捕获特定类型
来源：http://yn.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://fs.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qo.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://zx.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://uh.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://kf.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ay.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://xk.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://af.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://qb.nszjky.cn

Py:   value = d.get("k") or default
来源：http://jj.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xr.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eu.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qk.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mn.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gl.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://ge.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://wn.szsharing.cn

[H07] 断言
来源：http://bu.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://wp.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://ww.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://wg.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://ef.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://jq.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wd.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://se.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://kh.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://jl.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://ek.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xn.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://jt.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://np.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://el.newstarts.cn

Go:   err.Error()
来源：http://xh.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://bk.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://sh.jctech888.com.cn

[H09] 带错误码的异常
来源：http://ay.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://it.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nn.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nt.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xi.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ov.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wx.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uy.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oc.asd995.cn

[H10] 资源自动释放
来源：http://gt.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nm.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://br.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sh.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cf.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wl.yuexingan06.cn

Go:   defer f.Close()
来源：http://kg.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yj.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ag.9csxet.cn


<!-- 参考信息 -->