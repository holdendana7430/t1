代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dp.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://st.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zh.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://dx.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dx.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yu.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oz.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mb.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tg.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bm.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ti.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gv.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://xs.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ql.colortex.cn

PHP:  file_exists("a.txt");
来源：http://ju.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://wq.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ms.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zm.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ag.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://gj.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://lw.9csxet.cn

[F06] 删除文件
来源：http://xj.szsharing.cn

Py:   os.remove("a.txt")
来源：http://az.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://uw.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ec.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vx.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ea.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://kr.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://vm.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://uz.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://ac.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cz.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ic.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hr.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ll.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iy.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ul.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yb.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://te.haigaiapp.cn

[F08] 遍历目录
来源：http://fe.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kq.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eg.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://gg.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://jx.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zm.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bb.colortex.cn

Ruby: Dir.children("dir")
来源：http://im.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://cx.haigaiapp.cn

[F09] 获取文件大小
来源：http://wc.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://gn.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://ga.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://ac.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://iz.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kp.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ot.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://dq.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://cr.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://zm.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tc.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oj.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ob.colortex.cn

TS:   path.extname("a.txt")
来源：http://lf.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sp.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wk.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://le.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://an.lnxyls.cn

[F11] 复制与移动文件
来源：http://vl.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ec.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://in.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sf.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wx.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xf.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cw.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kk.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://at.jctech888.com.cn

[F12] CSV 读写
来源：http://ta.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://as.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ri.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rw.haigaiapp.cn

TS:   // 同上
来源：http://en.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eu.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wy.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gf.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qm.chemitech.net.cn

================================================================================
来源：http://kl.colortex.cn

G. 面向对象
来源：http://eg.huixinmuqiang.cn

================================================================================
来源：http://zq.szxytkj.cn

[G01] 定义类
来源：http://gn.newstarts.cn

Py:   class User: pass
来源：http://kw.lnxyls.cn

PHP:  class User {}
来源：http://ys.521024.cn

JS:   class User {}
来源：http://ep.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://el.gzmigu.cn

Java: class User {}
来源：http://uc.nszjky.cn

Go:   type User struct { Name string }
来源：http://uz.9csxet.cn

Ruby: class User; end
来源：http://yi.haigaiapp.cn

C#:   class User {}
来源：http://ea.chemitech.net.cn

[G02] 构造函数
来源：http://wg.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://gz.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://rz.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://ps.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://ih.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://yv.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ww.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://tv.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://fb.hahajie.cn

[G03] 实例属性
来源：http://de.bjjhwx.cn

Py:   self.name = "x"
来源：http://hq.shxzskj.cn

PHP:  public string $name = "x";
来源：http://zk.wgjwhj.cn

JS:   this.name = "x";
来源：http://oc.hahajie.cn

TS:   name: string = "x";
来源：http://rv.9csxet.cn

Java: private String name;
来源：http://aa.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nj.muxihuayi.cn

Ruby: @name = "x"
来源：http://jz.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://kd.muxihuayi.cn

[G04] 定义方法
来源：http://nr.szsharing.cn

Py:   def greet(self): return self.name
来源：http://wt.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ll.szsharing.cn

JS:   greet() { return this.name; }
来源：http://bp.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://sf.huixiangedu.cn

Java: String greet() { return name; }
来源：http://tt.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fb.panjiajie.cn

Ruby: def greet; @name; end
来源：http://at.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://vc.huanxung.cn

[G05] 继承
来源：http://xn.gzmigu.cn

Py:   class Admin(User): pass
来源：http://rl.9csxet.cn

PHP:  class Admin extends User {}
来源：http://as.shxzukj.cn

JS:   class Admin extends User {}
来源：http://dh.gzmigu.cn

TS:   class Admin extends User {}
来源：http://dp.huanxung.cn

Java: class Admin extends User {}
来源：http://bw.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ev.panjiajie.cn

Ruby: class Admin < User; end
来源：http://pa.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://yb.shxzskj.cn

[G06] 重写方法
来源：http://ez.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://az.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xp.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://bu.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://re.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://wp.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hf.colortex.cn

Ruby: def greet; "admin"; end
来源：http://lf.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://yi.shtwfgs.cn

[G07] 调用父类方法
来源：http://bw.shxzskj.cn

Py:   super().greet()
来源：http://yh.wgjwhj.cn

PHP:  parent::greet();
来源：http://dk.haigaiapp.cn

JS:   super.greet();
来源：http://ot.shxzukj.cn

TS:   super.greet();
来源：http://kd.jianghongdianzi.cn

Java: super.greet();
来源：http://qx.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tc.gzmigu.cn

Ruby: super
来源：http://zg.bookmarksfly.cn

C#:   base.Greet();
来源：http://rz.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://nx.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://js.szxytkj.cn

PHP:  public static function f() {}
来源：http://qi.muxihuayi.cn

JS:   static f() {}
来源：http://vk.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://ch.huixiangedu.cn

Java: static void f() {}
来源：http://dv.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dp.hahajie.cn

Ruby: def self.f; end
来源：http://mt.huanxung.cn

C#:   public static void F() {}
来源：http://rs.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://fo.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://kt.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://be.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bx.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://zz.huanxung.cn

Java: interface Shape { double area(); }
来源：http://fo.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://cq.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pi.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://cz.muxihuayi.cn

[G10] 访问控制
来源：http://oh.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://yf.muxihuayi.cn

PHP:  public / protected / private
来源：http://ci.colortex.cn

JS:   #private 字段；其余公开
来源：http://ed.szsharing.cn

TS:   public / protected / private
来源：http://kn.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://lp.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tf.yuexingan06.cn

Ruby: public / protected / private
来源：http://ot.szxytkj.cn

C#:   public / protected / private / internal
来源：http://gx.huanxung.cn

[G11] getter / setter
来源：http://sp.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://in.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dh.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://ku.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://ae.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://ln.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://np.nicolike.cn

Ruby: attr_accessor :name
来源：http://dz.hahajie.cn

C#:   public string Name { get; set; }
来源：http://uk.yuexingan06.cn

[G12] 对象转字符串
来源：http://be.colortex.cn

Py:   def __str__(self): return self.name
来源：http://cb.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ci.colortex.cn

JS:   toString() { return this.name; }
来源：http://nh.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://cv.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://ox.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xj.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://uu.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://ex.bjjhwx.cn

[G13] 判断对象类型
来源：http://nd.gzmigu.cn

Py:   isinstance(u, User)
来源：http://ug.521024.cn

PHP:  $u instanceof User
来源：http://ia.szsharing.cn

JS:   u instanceof User
来源：http://yp.nszjky.cn

TS:   u instanceof User
来源：http://wp.huixiangedu.cn

Java: u instanceof User
来源：http://os.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ej.asd995.cn

Ruby: u.is_a?(User)
来源：http://ku.newstarts.cn

C#:   u is User
来源：http://oi.szsharing.cn

[G14] 数据类 / record
来源：http://nw.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ir.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ua.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ea.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://mu.newstarts.cn

Java: record User(String name, int age) {}
来源：http://xn.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://oe.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kv.asd995.cn

C#:   record User(string Name, int Age);
来源：http://kx.521024.cn

[G15] 枚举
来源：http://kz.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ks.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ww.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hh.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qb.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://ri.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jr.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://hg.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cn.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://gs.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yl.colortex.cn

PHP:  get_object_vars($obj);
来源：http://tt.gzmigu.cn

JS:   Object.entries(obj)
来源：http://fz.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://na.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lz.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rw.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://nb.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://zv.haigaiapp.cn

================================================================================
来源：http://qh.asd995.cn

H. 异常与错误处理
来源：http://fb.bookmarksfly.cn

================================================================================
来源：http://np.haigaiapp.cn

[H01] try / catch 基础
来源：http://fe.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xe.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sw.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rz.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qg.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vz.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yv.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gi.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fr.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://tp.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://og.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fh.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sx.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eg.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://js.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://us.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jr.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ga.chemitech.net.cn

[H03] 主动抛出异常
来源：http://bf.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://pg.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cg.colortex.cn

JS:   throw new Error("错误信息");
来源：http://qb.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://hu.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zl.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gh.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tu.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pv.colortex.cn

[H04] 自定义异常类型
来源：http://xu.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://co.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://il.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://uq.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://jv.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://sm.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xr.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://en.9csxet.cn

C#:   class MyException : Exception {}
来源：http://bp.521024.cn

[H05] 捕获特定类型
来源：http://gi.szsharing.cn

Py:   except ValueError as e:
来源：http://kf.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xc.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://gf.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ds.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://fv.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ga.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://pq.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://go.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://cp.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://rw.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mu.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lz.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qi.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iq.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rk.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://bk.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://id.9csxet.cn

[H07] 断言
来源：http://mk.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://kn.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://hx.asd995.cn

JS:   console.assert(x > 0);
来源：http://bu.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://wu.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://zf.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sc.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dx.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://pw.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://qs.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://rn.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kb.huixinmuqiang.cn


<!-- 参考信息 -->