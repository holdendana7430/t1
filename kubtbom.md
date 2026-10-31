代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://vy.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vn.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lw.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://zx.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://rl.wgjwhj.cn

[F06] 删除文件
来源：http://hf.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://gg.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://fq.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eq.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hm.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qa.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://bk.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://ln.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://aq.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://ml.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rm.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://es.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://en.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hl.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cs.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lq.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pa.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://no.colortex.cn

[F08] 遍历目录
来源：http://rf.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pr.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nu.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://bk.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://kj.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nv.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ht.colortex.cn

Ruby: Dir.children("dir")
来源：http://es.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://vg.huixiangedu.cn

[F09] 获取文件大小
来源：http://zu.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://bm.nicolike.cn

PHP:  filesize("a.txt");
来源：http://pe.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://di.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://oz.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vb.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rc.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://jt.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://zs.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://oq.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zj.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dw.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fv.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://bg.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jc.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yp.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qk.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ds.chemitech.net.cn

[F11] 复制与移动文件
来源：http://sv.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sn.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wg.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jw.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mf.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bt.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wf.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dy.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uu.newstarts.cn

[F12] CSV 读写
来源：http://la.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ns.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ef.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nx.szsharing.cn

TS:   // 同上
来源：http://ir.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fc.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pn.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ho.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qr.jctech888.com.cn

================================================================================
来源：http://ex.yuntaijiaju.cn

G. 面向对象
来源：http://ml.shxzskj.cn

================================================================================
来源：http://ga.bookmarksfly.cn

[G01] 定义类
来源：http://ex.gzmigu.cn

Py:   class User: pass
来源：http://sn.szsharing.cn

PHP:  class User {}
来源：http://vf.huanxung.cn

JS:   class User {}
来源：http://hc.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://ir.521024.cn

Java: class User {}
来源：http://bo.hahajie.cn

Go:   type User struct { Name string }
来源：http://ch.colortex.cn

Ruby: class User; end
来源：http://lj.panjiajie.cn

C#:   class User {}
来源：http://qm.nszjky.cn

[G02] 构造函数
来源：http://zy.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://um.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://zw.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://iz.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://zt.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://wu.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rd.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://cj.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://yq.chemitech.net.cn

[G03] 实例属性
来源：http://kq.bookmarksfly.cn

Py:   self.name = "x"
来源：http://nv.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://ou.shxzukj.cn

JS:   this.name = "x";
来源：http://sg.asd995.cn

TS:   name: string = "x";
来源：http://yi.shxzskj.cn

Java: private String name;
来源：http://wi.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shxzskj.cn

Ruby: @name = "x"
来源：http://qa.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://di.szsharing.cn

[G04] 定义方法
来源：http://qz.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://eq.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xk.nicolike.cn

JS:   greet() { return this.name; }
来源：http://zu.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://nc.521024.cn

Java: String greet() { return name; }
来源：http://rn.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hf.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://wu.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://lp.hnjuh.cn

[G05] 继承
来源：http://ni.lnxyls.cn

Py:   class Admin(User): pass
来源：http://mj.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://ww.colortex.cn

JS:   class Admin extends User {}
来源：http://rv.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://hj.wgjwhj.cn

Java: class Admin extends User {}
来源：http://ga.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ds.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://pf.lnxyls.cn

C#:   class Admin : User {}
来源：http://oj.chemitech.net.cn

[G06] 重写方法
来源：http://fp.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://hh.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ua.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://xn.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://nm.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://bh.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ds.colortex.cn

Ruby: def greet; "admin"; end
来源：http://qa.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://mb.huixiangedu.cn

[G07] 调用父类方法
来源：http://vm.nicolike.cn

Py:   super().greet()
来源：http://mk.9csxet.cn

PHP:  parent::greet();
来源：http://pc.newstarts.cn

JS:   super.greet();
来源：http://vr.yuntaijiaju.cn

TS:   super.greet();
来源：http://yy.nicolike.cn

Java: super.greet();
来源：http://yp.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dy.shtwfgs.cn

Ruby: super
来源：http://zy.haigaiapp.cn

C#:   base.Greet();
来源：http://qr.newstarts.cn

[G08] 静态方法与属性
来源：http://pd.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mf.szxytkj.cn

PHP:  public static function f() {}
来源：http://fy.chemitech.net.cn

JS:   static f() {}
来源：http://yp.huixiangedu.cn

TS:   static f(): void {}
来源：http://sn.521024.cn

Java: static void f() {}
来源：http://jo.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qy.bjjhwx.cn

Ruby: def self.f; end
来源：http://lb.shtwfgs.cn

C#:   public static void F() {}
来源：http://so.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://xm.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://iw.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sh.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ti.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://kp.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://jt.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://pp.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xn.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://nr.haigaiapp.cn

[G10] 访问控制
来源：http://cj.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://bs.521024.cn

PHP:  public / protected / private
来源：http://ht.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://lq.hnjuh.cn

TS:   public / protected / private
来源：http://tg.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://wa.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ox.muxihuayi.cn

Ruby: public / protected / private
来源：http://mw.huanxung.cn

C#:   public / protected / private / internal
来源：http://yr.chemitech.net.cn

[G11] getter / setter
来源：http://hb.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://io.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://od.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://eg.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://zo.colortex.cn

Java: public String getName() { return name; }
来源：http://go.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vc.hnjuh.cn

Ruby: attr_accessor :name
来源：http://za.newstarts.cn

C#:   public string Name { get; set; }
来源：http://py.9csxet.cn

[G12] 对象转字符串
来源：http://wr.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://an.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gg.hahajie.cn

JS:   toString() { return this.name; }
来源：http://pn.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://bn.521024.cn

Java: @Override public String toString() { return name; }
来源：http://rh.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jo.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://cj.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://uk.newstarts.cn

[G13] 判断对象类型
来源：http://bf.nszjky.cn

Py:   isinstance(u, User)
来源：http://mn.colortex.cn

PHP:  $u instanceof User
来源：http://ph.yuntaijiaju.cn

JS:   u instanceof User
来源：http://wh.hnjuh.cn

TS:   u instanceof User
来源：http://yc.yuexingan06.cn

Java: u instanceof User
来源：http://yq.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mx.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ph.huixinmuqiang.cn

C#:   u is User
来源：http://zc.huanxung.cn

[G14] 数据类 / record
来源：http://su.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vp.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://qf.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yo.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://hf.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://nh.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://ng.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bj.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://zs.muxihuayi.cn

[G15] 枚举
来源：http://xy.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vj.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sg.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ln.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cq.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://zr.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yg.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://yy.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://il.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://jw.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hd.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://wd.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://cv.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://rf.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xd.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bb.hahajie.cn

Ruby: obj.instance_variables
来源：http://or.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://lx.wgjwhj.cn

================================================================================
来源：http://tk.wgjwhj.cn

H. 异常与错误处理
来源：http://hw.yuexingan06.cn

================================================================================
来源：http://cw.hnjuh.cn

[H01] try / catch 基础
来源：http://ci.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uk.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nq.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ns.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://po.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://du.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://po.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fz.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xv.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://fo.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qe.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ik.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://af.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://st.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kr.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bi.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kw.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mo.bjjhwx.cn

[H03] 主动抛出异常
来源：http://vm.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://nm.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lt.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://zn.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://uk.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wi.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sy.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xq.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kf.panjiajie.cn

[H04] 自定义异常类型
来源：http://zg.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://iu.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ho.nicolike.cn

JS:   class MyError extends Error {}
来源：http://um.szsharing.cn

TS:   class MyError extends Error {}
来源：http://bj.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://jk.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qi.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ft.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://lh.muxihuayi.cn

[H05] 捕获特定类型
来源：http://mb.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://em.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gt.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://xq.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://is.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://th.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mh.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://hv.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eh.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://bx.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://rn.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vb.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pd.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gf.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bf.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kj.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://nm.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://co.szxytkj.cn

[H07] 断言
来源：http://ck.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://fl.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://qg.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://lk.521024.cn

TS:   console.assert(x > 0);
来源：http://ng.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://wz.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bz.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bt.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://ad.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://yt.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://uc.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ar.gzmigu.cn

JS:   e.message;  e.stack
来源：http://zv.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oz.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ts.szxytkj.cn

Go:   err.Error()
来源：http://tx.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://hh.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://ai.hnjuh.cn

[H09] 带错误码的异常
来源：http://up.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kb.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jt.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://na.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pw.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cr.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sy.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tu.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yh.gzmigu.cn

[H10] 资源自动释放
来源：http://ih.yuexingan06.cn


<!-- 参考信息 -->