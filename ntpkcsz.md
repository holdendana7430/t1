代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bw.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yq.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xu.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ms.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bq.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xv.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uv.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hb.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://at.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://so.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://gy.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://tf.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://zn.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qc.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ls.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://fr.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://ch.bookmarksfly.cn

[F06] 删除文件
来源：http://xn.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://wl.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://kz.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gt.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rs.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kq.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://mp.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://ca.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://rt.nszjky.cn

[F07] 创建目录（含多级）
来源：http://ut.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mo.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bx.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cx.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mv.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sh.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qu.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ap.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bb.shtwfgs.cn

[F08] 遍历目录
来源：http://ru.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tc.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dv.521024.cn

JS:   fs.readdirSync("dir")
来源：http://mh.521024.cn

TS:   fs.readdirSync("dir")
来源：http://jm.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ji.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ej.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://wo.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ry.nszjky.cn

[F09] 获取文件大小
来源：http://xq.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://gy.huanxung.cn

PHP:  filesize("a.txt");
来源：http://fi.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://yw.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://hh.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yn.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vl.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://qr.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://aq.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://tk.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vc.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oh.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://st.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://se.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fg.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rd.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fb.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zc.shtwfgs.cn

[F11] 复制与移动文件
来源：http://kk.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mu.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xd.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nn.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tn.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nr.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pk.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mb.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nz.chemitech.net.cn

[F12] CSV 读写
来源：http://wa.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wn.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uw.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ai.huanxung.cn

TS:   // 同上
来源：http://tq.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ht.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sy.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kb.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xt.jctech888.com.cn

================================================================================
来源：http://mg.colortex.cn

G. 面向对象
来源：http://mh.szxytkj.cn

================================================================================
来源：http://rt.chemitech.net.cn

[G01] 定义类
来源：http://hz.szxytkj.cn

Py:   class User: pass
来源：http://wl.hahajie.cn

PHP:  class User {}
来源：http://va.lnxyls.cn

JS:   class User {}
来源：http://fo.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://wz.yuntaijiaju.cn

Java: class User {}
来源：http://zb.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://wq.haigaiapp.cn

Ruby: class User; end
来源：http://lq.yuexingan06.cn

C#:   class User {}
来源：http://vo.huanxung.cn

[G02] 构造函数
来源：http://gb.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://jn.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://sg.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ce.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://cp.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://qw.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ue.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://ti.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://rt.huanxung.cn

[G03] 实例属性
来源：http://xp.shtwfgs.cn

Py:   self.name = "x"
来源：http://jo.colortex.cn

PHP:  public string $name = "x";
来源：http://ci.newstarts.cn

JS:   this.name = "x";
来源：http://ka.muxihuayi.cn

TS:   name: string = "x";
来源：http://xl.yuexingan06.cn

Java: private String name;
来源：http://wd.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kk.lnxyls.cn

Ruby: @name = "x"
来源：http://sv.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://uz.haigaiapp.cn

[G04] 定义方法
来源：http://dj.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://mh.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tl.nicolike.cn

JS:   greet() { return this.name; }
来源：http://ax.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://xx.colortex.cn

Java: String greet() { return name; }
来源：http://ij.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dc.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://xo.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://ig.shxzukj.cn

[G05] 继承
来源：http://nf.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://xc.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://wr.asd995.cn

JS:   class Admin extends User {}
来源：http://as.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://oo.colortex.cn

Java: class Admin extends User {}
来源：http://ka.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xk.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://nj.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://re.huixiangedu.cn

[G06] 重写方法
来源：http://hi.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://ji.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rb.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://fh.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://qs.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://sf.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lm.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://ri.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://oa.szsharing.cn

[G07] 调用父类方法
来源：http://wi.haigaiapp.cn

Py:   super().greet()
来源：http://bh.wgjwhj.cn

PHP:  parent::greet();
来源：http://mp.muxihuayi.cn

JS:   super.greet();
来源：http://nj.asd995.cn

TS:   super.greet();
来源：http://sx.szsharing.cn

Java: super.greet();
来源：http://op.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://od.colortex.cn

Ruby: super
来源：http://xc.hahajie.cn

C#:   base.Greet();
来源：http://gn.bjjhwx.cn

[G08] 静态方法与属性
来源：http://uq.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hy.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://wo.shxzukj.cn

JS:   static f() {}
来源：http://od.hahajie.cn

TS:   static f(): void {}
来源：http://ye.asd995.cn

Java: static void f() {}
来源：http://wg.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jf.gzmigu.cn

Ruby: def self.f; end
来源：http://ey.newstarts.cn

C#:   public static void F() {}
来源：http://we.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://vw.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ej.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aj.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gd.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://cc.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://dl.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://da.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zf.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://zr.bookmarksfly.cn

[G10] 访问控制
来源：http://fa.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://df.shtwfgs.cn

PHP:  public / protected / private
来源：http://rz.colortex.cn

JS:   #private 字段；其余公开
来源：http://ic.gzmigu.cn

TS:   public / protected / private
来源：http://jp.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://eq.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://li.yuexingan06.cn

Ruby: public / protected / private
来源：http://ba.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://yb.haigaiapp.cn

[G11] getter / setter
来源：http://kb.huanxung.cn

Py:   @property 与 @x.setter
来源：http://zm.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ld.nicolike.cn

JS:   get name() { return this._name; }
来源：http://ul.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://yi.huanxung.cn

Java: public String getName() { return name; }
来源：http://zy.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ho.huanxung.cn

Ruby: attr_accessor :name
来源：http://ib.521024.cn

C#:   public string Name { get; set; }
来源：http://yy.newstarts.cn

[G12] 对象转字符串
来源：http://hv.521024.cn

Py:   def __str__(self): return self.name
来源：http://vh.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pr.hahajie.cn

JS:   toString() { return this.name; }
来源：http://qu.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://nq.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://th.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ml.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://yv.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://ji.huixiangedu.cn

[G13] 判断对象类型
来源：http://qw.huanxung.cn

Py:   isinstance(u, User)
来源：http://ug.521024.cn

PHP:  $u instanceof User
来源：http://lu.szsharing.cn

JS:   u instanceof User
来源：http://yo.yuntaijiaju.cn

TS:   u instanceof User
来源：http://gt.9csxet.cn

Java: u instanceof User
来源：http://uh.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sm.colortex.cn

Ruby: u.is_a?(User)
来源：http://ep.huixinmuqiang.cn

C#:   u is User
来源：http://rq.jctech888.com.cn

[G14] 数据类 / record
来源：http://xa.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sg.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://bw.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ls.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://tx.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://hz.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://bk.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nh.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://sh.colortex.cn

[G15] 枚举
来源：http://mc.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mi.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rg.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kl.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dd.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://vs.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vu.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://xf.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gf.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://dx.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://db.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://xl.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://pf.colortex.cn

TS:   Object.entries(obj)
来源：http://fg.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ie.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://na.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://mq.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://xv.szxytkj.cn

================================================================================
来源：http://hn.nszjky.cn

H. 异常与错误处理
来源：http://kw.szxytkj.cn

================================================================================
来源：http://ev.huanxung.cn

[H01] try / catch 基础
来源：http://wo.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lv.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nb.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://av.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mf.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ot.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sy.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://th.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vf.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ju.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ss.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ix.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mp.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yu.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ti.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tx.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gv.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lq.haigaiapp.cn

[H03] 主动抛出异常
来源：http://vi.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://wa.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xg.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://do.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://jk.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://az.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pt.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://np.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gs.9csxet.cn

[H04] 自定义异常类型
来源：http://xx.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://il.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dh.szsharing.cn

JS:   class MyError extends Error {}
来源：http://mn.nicolike.cn

TS:   class MyError extends Error {}
来源：http://gj.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://mt.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hk.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://ar.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://tz.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://yv.nszjky.cn

Py:   except ValueError as e:
来源：http://lj.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eq.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://dt.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://vd.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://cm.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rb.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://rf.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ap.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://xu.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://sr.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sm.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jq.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://df.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cs.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://po.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://ce.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://ud.chemitech.net.cn

[H07] 断言
来源：http://tb.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ri.hnjuh.cn

PHP:  assert($x > 0);
来源：http://nb.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://ko.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://lv.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://cr.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tf.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jf.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://fi.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://gp.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://et.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zv.hahajie.cn

JS:   e.message;  e.stack
来源：http://vi.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dh.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nu.colortex.cn

Go:   err.Error()
来源：http://wn.jianghongdianzi.cn


<!-- 参考信息 -->