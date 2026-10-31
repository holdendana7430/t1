代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://js.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zr.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dt.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://kx.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://am.9csxet.cn

[F06] 删除文件
来源：http://rq.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://jd.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://xo.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jj.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eb.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lo.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://wf.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://dn.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://ul.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://dt.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jp.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qh.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ho.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ic.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yp.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ch.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vw.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ym.jctech888.com.cn

[F08] 遍历目录
来源：http://zf.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ek.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xr.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://xe.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://yp.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sf.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dj.newstarts.cn

Ruby: Dir.children("dir")
来源：http://ti.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://cc.shxzskj.cn

[F09] 获取文件大小
来源：http://fo.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://fh.521024.cn

PHP:  filesize("a.txt");
来源：http://fh.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://bd.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://cp.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://km.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hv.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://je.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://ts.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://cl.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ur.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ni.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jk.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://le.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nq.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dw.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xs.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qy.hahajie.cn

[F11] 复制与移动文件
来源：http://la.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jr.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lx.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vb.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ol.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lf.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xy.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bx.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ip.hahajie.cn

[F12] CSV 读写
来源：http://zy.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mb.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cc.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ut.521024.cn

TS:   // 同上
来源：http://sd.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://it.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kr.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sm.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cp.521024.cn

================================================================================
来源：http://ph.yuntaijiaju.cn

G. 面向对象
来源：http://nz.shtwfgs.cn

================================================================================
来源：http://hw.huanxung.cn

[G01] 定义类
来源：http://bs.hahajie.cn

Py:   class User: pass
来源：http://zh.yuntaijiaju.cn

PHP:  class User {}
来源：http://da.newstarts.cn

JS:   class User {}
来源：http://om.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://rl.521024.cn

Java: class User {}
来源：http://fs.nszjky.cn

Go:   type User struct { Name string }
来源：http://ed.chemitech.net.cn

Ruby: class User; end
来源：http://ul.bookmarksfly.cn

C#:   class User {}
来源：http://lf.huixinmuqiang.cn

[G02] 构造函数
来源：http://kp.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://oi.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://zb.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://yy.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ki.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://dr.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sz.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://ge.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://da.jianghongdianzi.cn

[G03] 实例属性
来源：http://af.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://qb.asd995.cn

PHP:  public string $name = "x";
来源：http://iy.colortex.cn

JS:   this.name = "x";
来源：http://go.chemitech.net.cn

TS:   name: string = "x";
来源：http://kl.chemitech.net.cn

Java: private String name;
来源：http://cw.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://js.huanxung.cn

Ruby: @name = "x"
来源：http://nz.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://gj.nszjky.cn

[G04] 定义方法
来源：http://ze.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://us.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xm.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://rs.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://ub.hahajie.cn

Java: String greet() { return name; }
来源：http://dk.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qm.521024.cn

Ruby: def greet; @name; end
来源：http://iv.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://ha.shxzukj.cn

[G05] 继承
来源：http://jl.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://pi.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://xv.colortex.cn

JS:   class Admin extends User {}
来源：http://bj.hahajie.cn

TS:   class Admin extends User {}
来源：http://pk.9csxet.cn

Java: class Admin extends User {}
来源：http://gc.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wc.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://bo.szsharing.cn

C#:   class Admin : User {}
来源：http://zq.shxzukj.cn

[G06] 重写方法
来源：http://gn.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://xn.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bl.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://ey.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://xj.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://gr.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cb.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://zc.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://ua.chemitech.net.cn

[G07] 调用父类方法
来源：http://dh.wgjwhj.cn

Py:   super().greet()
来源：http://ri.panjiajie.cn

PHP:  parent::greet();
来源：http://lv.gzmigu.cn

JS:   super.greet();
来源：http://sp.colortex.cn

TS:   super.greet();
来源：http://dr.521024.cn

Java: super.greet();
来源：http://bx.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ox.yuntaijiaju.cn

Ruby: super
来源：http://jb.nicolike.cn

C#:   base.Greet();
来源：http://hx.shxzukj.cn

[G08] 静态方法与属性
来源：http://oc.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hb.asd995.cn

PHP:  public static function f() {}
来源：http://jn.nszjky.cn

JS:   static f() {}
来源：http://ua.nicolike.cn

TS:   static f(): void {}
来源：http://ct.hnjuh.cn

Java: static void f() {}
来源：http://tu.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jr.colortex.cn

Ruby: def self.f; end
来源：http://uv.lnxyls.cn

C#:   public static void F() {}
来源：http://nx.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://js.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://eq.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jt.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fe.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://to.521024.cn

Java: interface Shape { double area(); }
来源：http://az.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://cm.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ve.521024.cn

C#:   interface IShape { double Area(); }
来源：http://fn.asd995.cn

[G10] 访问控制
来源：http://ef.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ij.szsharing.cn

PHP:  public / protected / private
来源：http://bb.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://ra.hnjuh.cn

TS:   public / protected / private
来源：http://ux.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://gb.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kz.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://yz.shxzukj.cn

C#:   public / protected / private / internal
来源：http://tv.hnjuh.cn

[G11] getter / setter
来源：http://xj.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://bs.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mi.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://bj.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://hd.521024.cn

Java: public String getName() { return name; }
来源：http://uf.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://az.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ub.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://xt.nicolike.cn

[G12] 对象转字符串
来源：http://xv.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://nd.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ay.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://zo.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://pg.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://yc.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hl.521024.cn

Ruby: def to_s; @name; end
来源：http://tb.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://mm.9csxet.cn

[G13] 判断对象类型
来源：http://bl.nszjky.cn

Py:   isinstance(u, User)
来源：http://jf.9csxet.cn

PHP:  $u instanceof User
来源：http://sj.bjjhwx.cn

JS:   u instanceof User
来源：http://qx.hnjuh.cn

TS:   u instanceof User
来源：http://xo.shxzukj.cn

Java: u instanceof User
来源：http://vi.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ea.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://ou.szxytkj.cn

C#:   u is User
来源：http://wv.lnxyls.cn

[G14] 数据类 / record
来源：http://bt.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ko.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://tm.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sg.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://gj.szsharing.cn

Java: record User(String name, int age) {}
来源：http://uk.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://bk.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iu.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://it.shtwfgs.cn

[G15] 枚举
来源：http://wq.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gi.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ze.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zk.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fr.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://ur.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jm.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://qv.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qn.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://wi.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uw.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://wh.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://bg.panjiajie.cn

TS:   Object.entries(obj)
来源：http://qk.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pr.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gm.asd995.cn

Ruby: obj.instance_variables
来源：http://qp.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://dc.huixiangedu.cn

================================================================================
来源：http://ff.huixinmuqiang.cn

H. 异常与错误处理
来源：http://hp.huanxung.cn

================================================================================
来源：http://ek.yuexingan06.cn

[H01] try / catch 基础
来源：http://vl.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zc.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vn.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ih.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xz.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fy.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hf.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ft.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nt.nicolike.cn

[H02] finally / ensure 收尾
来源：http://yt.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pq.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zn.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ws.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ky.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zv.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nb.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ii.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bg.colortex.cn

[H03] 主动抛出异常
来源：http://cw.521024.cn

Py:   raise ValueError("错误信息")
来源：http://fn.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ig.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://rd.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://wd.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iw.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bp.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qc.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rj.asd995.cn

[H04] 自定义异常类型
来源：http://xk.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://nd.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jn.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://tv.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ms.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://jo.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fb.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://rw.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://mc.jctech888.com.cn

[H05] 捕获特定类型
来源：http://vs.lnxyls.cn

Py:   except ValueError as e:
来源：http://zw.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://li.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://aq.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://yp.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://zq.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fb.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://zy.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ul.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://en.9csxet.cn

Py:   value = d.get("k") or default
来源：http://pt.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cw.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fl.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jj.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://my.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bx.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://sk.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://hn.huanxung.cn

[H07] 断言
来源：http://hy.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://pk.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://gc.asd995.cn

JS:   console.assert(x > 0);
来源：http://oh.9csxet.cn

TS:   console.assert(x > 0);
来源：http://bk.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://gw.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tc.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yg.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://rb.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://dj.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://kc.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hf.nicolike.cn

JS:   e.message;  e.stack
来源：http://mi.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://am.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://km.jianghongdianzi.cn

Go:   err.Error()
来源：http://hl.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://qf.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://el.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://lj.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qg.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gb.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tb.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ds.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ki.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gt.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aq.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zt.shtwfgs.cn

[H10] 资源自动释放
来源：http://xo.hahajie.cn


<!-- 参考信息 -->