代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tb.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bx.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dh.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://de.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eb.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vp.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jd.yuntaijiaju.cn

[F08] 遍历目录
来源：http://np.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xo.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rk.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://bv.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://it.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oy.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://po.newstarts.cn

Ruby: Dir.children("dir")
来源：http://el.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://nt.hahajie.cn

[F09] 获取文件大小
来源：http://sy.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://vj.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://yn.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://sj.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://un.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eh.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jh.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://mt.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://bz.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://wy.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yk.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mo.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cd.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://ae.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eu.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ey.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lz.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xl.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://iv.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rs.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ta.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lm.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dw.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wf.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vp.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://av.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yc.wgjwhj.cn

[F12] CSV 读写
来源：http://sv.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ks.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sa.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cg.shxzukj.cn

TS:   // 同上
来源：http://hw.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lm.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mr.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ob.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rd.panjiajie.cn

================================================================================
来源：http://rv.bookmarksfly.cn

G. 面向对象
来源：http://xg.nszjky.cn

================================================================================
来源：http://du.bookmarksfly.cn

[G01] 定义类
来源：http://yt.jianghongdianzi.cn

Py:   class User: pass
来源：http://xp.521024.cn

PHP:  class User {}
来源：http://pf.jianghongdianzi.cn

JS:   class User {}
来源：http://rs.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://ew.bjjhwx.cn

Java: class User {}
来源：http://ky.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://wt.asd995.cn

Ruby: class User; end
来源：http://xm.muxihuayi.cn

C#:   class User {}
来源：http://lz.yuntaijiaju.cn

[G02] 构造函数
来源：http://dk.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://vc.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://vy.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://kf.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://bq.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://zw.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pq.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://om.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://dm.hnjuh.cn

[G03] 实例属性
来源：http://cy.nszjky.cn

Py:   self.name = "x"
来源：http://xe.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://xq.9csxet.cn

JS:   this.name = "x";
来源：http://ph.huixiangedu.cn

TS:   name: string = "x";
来源：http://pb.521024.cn

Java: private String name;
来源：http://vq.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lp.huanxung.cn

Ruby: @name = "x"
来源：http://eb.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://fc.jctech888.com.cn

[G04] 定义方法
来源：http://dr.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://ob.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ks.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://hf.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://nh.nicolike.cn

Java: String greet() { return name; }
来源：http://qn.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tw.nicolike.cn

Ruby: def greet; @name; end
来源：http://rq.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://ib.szsharing.cn

[G05] 继承
来源：http://am.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://jh.szsharing.cn

PHP:  class Admin extends User {}
来源：http://bx.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://ke.panjiajie.cn

TS:   class Admin extends User {}
来源：http://th.nicolike.cn

Java: class Admin extends User {}
来源：http://ri.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nu.gzmigu.cn

Ruby: class Admin < User; end
来源：http://si.muxihuayi.cn

C#:   class Admin : User {}
来源：http://ha.panjiajie.cn

[G06] 重写方法
来源：http://ae.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://yk.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ob.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://ig.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://bz.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://jh.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kw.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://uw.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://iq.huixiangedu.cn

[G07] 调用父类方法
来源：http://cm.lnxyls.cn

Py:   super().greet()
来源：http://sp.chemitech.net.cn

PHP:  parent::greet();
来源：http://hb.yuexingan06.cn

JS:   super.greet();
来源：http://tv.jianghongdianzi.cn

TS:   super.greet();
来源：http://fe.jctech888.com.cn

Java: super.greet();
来源：http://lt.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vd.shxzskj.cn

Ruby: super
来源：http://ae.lnxyls.cn

C#:   base.Greet();
来源：http://po.shtwfgs.cn

[G08] 静态方法与属性
来源：http://xo.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wh.chemitech.net.cn

PHP:  public static function f() {}
来源：http://jo.szsharing.cn

JS:   static f() {}
来源：http://nw.huixiangedu.cn

TS:   static f(): void {}
来源：http://eo.huanxung.cn

Java: static void f() {}
来源：http://dj.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://in.hnjuh.cn

Ruby: def self.f; end
来源：http://xa.szsharing.cn

C#:   public static void F() {}
来源：http://cg.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://ox.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://sy.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kn.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gf.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://gi.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://oh.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://xz.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://st.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://fk.9csxet.cn

[G10] 访问控制
来源：http://vp.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://az.szxytkj.cn

PHP:  public / protected / private
来源：http://ky.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://tn.asd995.cn

TS:   public / protected / private
来源：http://vc.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://mf.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vi.shxzukj.cn

Ruby: public / protected / private
来源：http://lh.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://wx.shxzukj.cn

[G11] getter / setter
来源：http://ib.huanxung.cn

Py:   @property 与 @x.setter
来源：http://sc.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ba.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://eg.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://gc.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://xq.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://br.szxytkj.cn

Ruby: attr_accessor :name
来源：http://da.szsharing.cn

C#:   public string Name { get; set; }
来源：http://vh.hnjuh.cn

[G12] 对象转字符串
来源：http://ef.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://gm.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ph.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://wr.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://sf.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://ze.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gy.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://qb.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://zg.nicolike.cn

[G13] 判断对象类型
来源：http://lq.nicolike.cn

Py:   isinstance(u, User)
来源：http://fn.nszjky.cn

PHP:  $u instanceof User
来源：http://zn.szsharing.cn

JS:   u instanceof User
来源：http://gy.chemitech.net.cn

TS:   u instanceof User
来源：http://km.szsharing.cn

Java: u instanceof User
来源：http://iq.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yg.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://xs.nszjky.cn

C#:   u is User
来源：http://cb.9csxet.cn

[G14] 数据类 / record
来源：http://ss.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ch.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://fq.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lg.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://eu.szsharing.cn

Java: record User(String name, int age) {}
来源：http://dh.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://up.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iz.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://sv.bookmarksfly.cn

[G15] 枚举
来源：http://mn.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zq.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ib.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gx.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tc.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://gn.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hc.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ok.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dr.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://zr.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hv.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://wz.szsharing.cn

JS:   Object.entries(obj)
来源：http://ia.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://un.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xu.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ya.gzmigu.cn

Ruby: obj.instance_variables
来源：http://zm.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ws.huixiangedu.cn

================================================================================
来源：http://yq.szxytkj.cn

H. 异常与错误处理
来源：http://mv.wgjwhj.cn

================================================================================
来源：http://bh.9csxet.cn

[H01] try / catch 基础
来源：http://oc.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dg.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lu.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gh.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ic.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qw.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eb.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tf.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hn.colortex.cn

[H02] finally / ensure 收尾
来源：http://kn.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gk.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kf.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ep.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://th.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rn.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rz.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yk.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dx.huanxung.cn

[H03] 主动抛出异常
来源：http://yy.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://uu.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://od.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://tg.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://un.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ef.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mp.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cf.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ek.haigaiapp.cn

[H04] 自定义异常类型
来源：http://gw.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://ss.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ga.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://on.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://au.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://ub.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jk.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://eb.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://if.haigaiapp.cn

[H05] 捕获特定类型
来源：http://so.shxzskj.cn

Py:   except ValueError as e:
来源：http://rd.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ac.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://jw.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://oz.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://bs.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://he.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://cv.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kb.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://hc.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://cu.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jn.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cf.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qm.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vf.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gf.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://up.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://nl.asd995.cn

[H07] 断言
来源：http://vn.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://pb.newstarts.cn

PHP:  assert($x > 0);
来源：http://rc.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://ei.hahajie.cn

TS:   console.assert(x > 0);
来源：http://lu.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://qq.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vz.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qg.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://gl.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://ms.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ca.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sl.lnxyls.cn

JS:   e.message;  e.stack
来源：http://mf.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qw.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vu.szxytkj.cn

Go:   err.Error()
来源：http://go.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://eg.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://tt.szsharing.cn

[H09] 带错误码的异常
来源：http://ai.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lg.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ir.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://se.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://br.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://va.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ek.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nx.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pk.nszjky.cn

[H10] 资源自动释放
来源：http://vv.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jg.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qe.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://we.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wa.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oa.huixiangedu.cn

Go:   defer f.Close()
来源：http://hq.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gq.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hh.bookmarksfly.cn

================================================================================
来源：http://ar.yuexingan06.cn

I. 正则表达式
来源：http://dh.huixinmuqiang.cn

================================================================================
来源：http://qk.hahajie.cn

[I01] 判断是否匹配
来源：http://kt.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ek.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jz.asd995.cn

JS:   /\d+/.test(s)
来源：http://lc.szsharing.cn

TS:   /\d+/.test(s)
来源：http://za.jctech888.com.cn


<!-- 参考信息 -->