代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://ke.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bh.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fm.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://xk.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://yz.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://zn.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://yk.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zu.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ga.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vr.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rn.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hd.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fl.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bp.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fo.jianghongdianzi.cn

[F08] 遍历目录
来源：http://ij.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uy.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://el.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://lv.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://tm.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hx.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lb.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://wr.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://aj.asd995.cn

[F09] 获取文件大小
来源：http://ma.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://ac.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://mh.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://np.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://xw.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oz.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oi.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://yn.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://sf.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://vu.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yk.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dh.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pn.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://iy.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://it.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ab.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nt.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rf.9csxet.cn

[F11] 复制与移动文件
来源：http://ui.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gb.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gb.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ra.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hu.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pk.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vy.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bz.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iw.yuexingan06.cn

[F12] CSV 读写
来源：http://gr.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://en.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kk.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lw.lnxyls.cn

TS:   // 同上
来源：http://go.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ff.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yf.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://na.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xl.newstarts.cn

================================================================================
来源：http://uj.szxytkj.cn

G. 面向对象
来源：http://zm.chemitech.net.cn

================================================================================
来源：http://xg.colortex.cn

[G01] 定义类
来源：http://yj.haigaiapp.cn

Py:   class User: pass
来源：http://ix.yuexingan06.cn

PHP:  class User {}
来源：http://bk.jianghongdianzi.cn

JS:   class User {}
来源：http://gt.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://ac.szsharing.cn

Java: class User {}
来源：http://si.gzmigu.cn

Go:   type User struct { Name string }
来源：http://bf.bjjhwx.cn

Ruby: class User; end
来源：http://vo.huixinmuqiang.cn

C#:   class User {}
来源：http://fu.asd995.cn

[G02] 构造函数
来源：http://gg.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://lw.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://pw.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://in.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://zl.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://fu.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://so.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://mj.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://jc.jianghongdianzi.cn

[G03] 实例属性
来源：http://zv.huixiangedu.cn

Py:   self.name = "x"
来源：http://mb.shxzskj.cn

PHP:  public string $name = "x";
来源：http://dh.szsharing.cn

JS:   this.name = "x";
来源：http://nm.newstarts.cn

TS:   name: string = "x";
来源：http://ky.lnxyls.cn

Java: private String name;
来源：http://lp.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xj.panjiajie.cn

Ruby: @name = "x"
来源：http://iu.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://yz.jianghongdianzi.cn

[G04] 定义方法
来源：http://yy.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://qu.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hl.asd995.cn

JS:   greet() { return this.name; }
来源：http://tq.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://vd.haigaiapp.cn

Java: String greet() { return name; }
来源：http://ai.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zy.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://nu.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://iw.newstarts.cn

[G05] 继承
来源：http://in.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://dn.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://mm.asd995.cn

JS:   class Admin extends User {}
来源：http://lz.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://vq.haigaiapp.cn

Java: class Admin extends User {}
来源：http://pd.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xc.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://tw.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://kd.shtwfgs.cn

[G06] 重写方法
来源：http://on.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://ol.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ri.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://pn.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://zt.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://cn.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yf.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://hd.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://it.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://zk.wgjwhj.cn

Py:   super().greet()
来源：http://mp.shtwfgs.cn

PHP:  parent::greet();
来源：http://ar.huixinmuqiang.cn

JS:   super.greet();
来源：http://dz.yuexingan06.cn

TS:   super.greet();
来源：http://oo.muxihuayi.cn

Java: super.greet();
来源：http://fd.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lt.521024.cn

Ruby: super
来源：http://gs.hnjuh.cn

C#:   base.Greet();
来源：http://rg.huixiangedu.cn

[G08] 静态方法与属性
来源：http://me.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qk.wgjwhj.cn

PHP:  public static function f() {}
来源：http://li.bjjhwx.cn

JS:   static f() {}
来源：http://yf.asd995.cn

TS:   static f(): void {}
来源：http://bk.huixiangedu.cn

Java: static void f() {}
来源：http://ta.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kp.gzmigu.cn

Ruby: def self.f; end
来源：http://jx.hahajie.cn

C#:   public static void F() {}
来源：http://sg.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://iv.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://sb.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xx.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zg.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://vz.nszjky.cn

Java: interface Shape { double area(); }
来源：http://sz.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://mj.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mw.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://xm.bjjhwx.cn

[G10] 访问控制
来源：http://yv.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://es.gzmigu.cn

PHP:  public / protected / private
来源：http://oa.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://ub.shxzskj.cn

TS:   public / protected / private
来源：http://mj.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://li.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gp.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://xm.shxzukj.cn

C#:   public / protected / private / internal
来源：http://qg.hnjuh.cn

[G11] getter / setter
来源：http://qa.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://hn.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nq.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://lm.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://pl.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://yh.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gh.9csxet.cn

Ruby: attr_accessor :name
来源：http://px.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://pz.yuexingan06.cn

[G12] 对象转字符串
来源：http://gy.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://ll.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qq.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://qc.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://ps.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://lc.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ks.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://ow.colortex.cn

C#:   public override string ToString() => Name;
来源：http://uu.nicolike.cn

[G13] 判断对象类型
来源：http://ot.asd995.cn

Py:   isinstance(u, User)
来源：http://yt.nicolike.cn

PHP:  $u instanceof User
来源：http://na.yuexingan06.cn

JS:   u instanceof User
来源：http://nn.jctech888.com.cn

TS:   u instanceof User
来源：http://ae.shxzskj.cn

Java: u instanceof User
来源：http://sh.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kq.asd995.cn

Ruby: u.is_a?(User)
来源：http://ru.colortex.cn

C#:   u is User
来源：http://ax.newstarts.cn

[G14] 数据类 / record
来源：http://rk.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qh.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://vv.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://de.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://xw.newstarts.cn

Java: record User(String name, int age) {}
来源：http://oq.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://rx.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tx.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://ow.wgjwhj.cn

[G15] 枚举
来源：http://kx.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://am.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cf.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mp.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kv.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://wp.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wg.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://fs.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lw.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://dx.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oi.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://si.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://op.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://ha.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iw.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ui.szsharing.cn

Ruby: obj.instance_variables
来源：http://vu.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://vv.asd995.cn

================================================================================
来源：http://wc.haigaiapp.cn

H. 异常与错误处理
来源：http://tr.hahajie.cn

================================================================================
来源：http://fo.hahajie.cn

[H01] try / catch 基础
来源：http://vt.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sq.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bc.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jn.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dx.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://td.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ta.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qz.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ad.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://dz.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ls.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tu.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pu.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cp.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nw.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iu.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ho.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fa.shxzukj.cn

[H03] 主动抛出异常
来源：http://zu.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://ik.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pb.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://fx.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://tp.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bd.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sp.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lt.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uc.chemitech.net.cn

[H04] 自定义异常类型
来源：http://oc.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://fj.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xq.asd995.cn

JS:   class MyError extends Error {}
来源：http://bc.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://cb.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://pv.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jc.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://qw.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://ne.9csxet.cn

[H05] 捕获特定类型
来源：http://mz.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://zu.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lr.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://wh.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://mv.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://bp.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ow.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://vc.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hf.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://rd.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://ck.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cc.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sc.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cw.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yn.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ny.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://li.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://bb.newstarts.cn

[H07] 断言
来源：http://yp.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://eh.nszjky.cn

PHP:  assert($x > 0);
来源：http://mq.521024.cn

JS:   console.assert(x > 0);
来源：http://zp.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://ss.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://yi.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ao.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wg.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://uo.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://qz.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://xe.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nw.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://sx.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ng.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ek.huixiangedu.cn

Go:   err.Error()
来源：http://un.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://lk.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://eo.shxzskj.cn

[H09] 带错误码的异常
来源：http://yo.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://au.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://et.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://al.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ul.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dc.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ct.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ct.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ua.muxihuayi.cn

[H10] 资源自动释放
来源：http://uz.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cd.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://on.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hd.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bh.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pq.jctech888.com.cn

Go:   defer f.Close()
来源：http://xd.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ea.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ku.panjiajie.cn


<!-- 参考信息 -->