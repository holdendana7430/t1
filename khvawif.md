代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tt.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jr.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://in.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zj.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://si.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://al.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://mi.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://sp.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://qi.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://db.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wa.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://ez.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://wa.colortex.cn

[F06] 删除文件
来源：http://fg.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://lc.hahajie.cn

PHP:  unlink("a.txt");
来源：http://us.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jw.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jq.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sz.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://od.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://ss.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://nv.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://xi.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qr.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fl.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://st.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wu.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qa.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sl.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iy.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yr.muxihuayi.cn

[F08] 遍历目录
来源：http://cv.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wx.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sw.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://tc.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://zt.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zr.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qj.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://gs.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://bi.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://ln.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ma.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://ry.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://rk.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://oe.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ap.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ex.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://in.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://se.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://rn.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jn.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jb.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ob.hahajie.cn

TS:   path.extname("a.txt")
来源：http://kl.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uz.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ym.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ud.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gh.newstarts.cn

[F11] 复制与移动文件
来源：http://pk.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://el.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kf.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ss.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qf.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fj.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xa.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pw.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wd.huixiangedu.cn

[F12] CSV 读写
来源：http://ks.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ja.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bx.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gs.muxihuayi.cn

TS:   // 同上
来源：http://bv.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xe.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ft.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vp.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ke.521024.cn

================================================================================
来源：http://ew.gzmigu.cn

G. 面向对象
来源：http://at.haigaiapp.cn

================================================================================
来源：http://co.jctech888.com.cn

[G01] 定义类
来源：http://dy.bookmarksfly.cn

Py:   class User: pass
来源：http://ms.jianghongdianzi.cn

PHP:  class User {}
来源：http://tw.panjiajie.cn

JS:   class User {}
来源：http://wg.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://em.shxzskj.cn

Java: class User {}
来源：http://va.shxzukj.cn

Go:   type User struct { Name string }
来源：http://kg.wgjwhj.cn

Ruby: class User; end
来源：http://qg.muxihuayi.cn

C#:   class User {}
来源：http://uy.nicolike.cn

[G02] 构造函数
来源：http://fa.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://il.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://uo.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://np.colortex.cn

TS:   constructor(public name: string) {}
来源：http://iw.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://os.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qw.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://bw.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://dw.asd995.cn

[G03] 实例属性
来源：http://xa.huanxung.cn

Py:   self.name = "x"
来源：http://oh.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://sj.huixiangedu.cn

JS:   this.name = "x";
来源：http://rm.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://na.chemitech.net.cn

Java: private String name;
来源：http://qq.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ck.szsharing.cn

Ruby: @name = "x"
来源：http://ra.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://tz.szxytkj.cn

[G04] 定义方法
来源：http://gy.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://zp.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fx.nicolike.cn

JS:   greet() { return this.name; }
来源：http://oz.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://gi.bjjhwx.cn

Java: String greet() { return name; }
来源：http://at.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eg.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://jz.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://re.colortex.cn

[G05] 继承
来源：http://dq.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://no.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://gv.szsharing.cn

JS:   class Admin extends User {}
来源：http://wu.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://nc.szsharing.cn

Java: class Admin extends User {}
来源：http://fr.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nt.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://aq.hnjuh.cn

C#:   class Admin : User {}
来源：http://gm.9csxet.cn

[G06] 重写方法
来源：http://mq.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://zd.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mj.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://wb.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://xo.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://su.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wp.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://mw.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://do.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://zb.panjiajie.cn

Py:   super().greet()
来源：http://hs.hahajie.cn

PHP:  parent::greet();
来源：http://fj.shtwfgs.cn

JS:   super.greet();
来源：http://nh.szxytkj.cn

TS:   super.greet();
来源：http://zs.nszjky.cn

Java: super.greet();
来源：http://qz.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ah.huixinmuqiang.cn

Ruby: super
来源：http://bk.yuntaijiaju.cn

C#:   base.Greet();
来源：http://hx.asd995.cn

[G08] 静态方法与属性
来源：http://ba.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dr.szsharing.cn

PHP:  public static function f() {}
来源：http://qb.bjjhwx.cn

JS:   static f() {}
来源：http://jt.shtwfgs.cn

TS:   static f(): void {}
来源：http://ev.chemitech.net.cn

Java: static void f() {}
来源：http://ar.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kd.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://sg.shxzukj.cn

C#:   public static void F() {}
来源：http://ej.szsharing.cn

[G09] 接口 / 抽象类
来源：http://ss.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://cq.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://em.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cz.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://hh.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://tp.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://go.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gc.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://az.colortex.cn

[G10] 访问控制
来源：http://vg.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://vc.huixiangedu.cn

PHP:  public / protected / private
来源：http://ij.nszjky.cn

JS:   #private 字段；其余公开
来源：http://rs.wgjwhj.cn

TS:   public / protected / private
来源：http://ut.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://yx.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wt.muxihuayi.cn

Ruby: public / protected / private
来源：http://dq.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://wf.haigaiapp.cn

[G11] getter / setter
来源：http://vm.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://tk.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zf.hahajie.cn

JS:   get name() { return this._name; }
来源：http://mv.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://wx.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://lv.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hm.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://dc.asd995.cn

C#:   public string Name { get; set; }
来源：http://nm.wgjwhj.cn

[G12] 对象转字符串
来源：http://nc.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://bi.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sh.colortex.cn

JS:   toString() { return this.name; }
来源：http://yy.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://nz.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://xs.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mq.huanxung.cn

Ruby: def to_s; @name; end
来源：http://ju.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://kq.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://xv.szxytkj.cn

Py:   isinstance(u, User)
来源：http://pw.panjiajie.cn

PHP:  $u instanceof User
来源：http://rr.yuexingan06.cn

JS:   u instanceof User
来源：http://rw.newstarts.cn

TS:   u instanceof User
来源：http://rl.hnjuh.cn

Java: u instanceof User
来源：http://en.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yi.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://zw.nszjky.cn

C#:   u is User
来源：http://by.hnjuh.cn

[G14] 数据类 / record
来源：http://gg.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fi.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://jg.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rh.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://du.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://kf.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://wi.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://it.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ca.huixinmuqiang.cn

[G15] 枚举
来源：http://og.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pf.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mp.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yt.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vc.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ww.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ki.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://fu.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ie.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://xp.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pu.colortex.cn

PHP:  get_object_vars($obj);
来源：http://rv.huanxung.cn

JS:   Object.entries(obj)
来源：http://lh.szxytkj.cn

TS:   Object.entries(obj)
来源：http://fx.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vy.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bc.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://px.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://vx.gzmigu.cn

================================================================================
来源：http://il.jctech888.com.cn

H. 异常与错误处理
来源：http://ux.huixiangedu.cn

================================================================================
来源：http://ha.9csxet.cn

[H01] try / catch 基础
来源：http://vm.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dz.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ka.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nj.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kq.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zh.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rs.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kt.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://id.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://cj.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://un.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ao.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mc.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ay.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gf.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mn.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bm.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yh.gzmigu.cn

[H03] 主动抛出异常
来源：http://nv.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ss.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ue.colortex.cn

JS:   throw new Error("错误信息");
来源：http://do.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://rx.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://od.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ck.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://au.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tc.chemitech.net.cn

[H04] 自定义异常类型
来源：http://ox.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://vi.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cq.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://au.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://nk.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://mk.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ri.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://td.nicolike.cn

C#:   class MyException : Exception {}
来源：http://wn.hnjuh.cn

[H05] 捕获特定类型
来源：http://hg.szxytkj.cn

Py:   except ValueError as e:
来源：http://if.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tv.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://sw.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://hi.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://uh.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nv.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://jr.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xp.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://qd.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://ok.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gx.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oe.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ne.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qp.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://no.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ka.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://ct.szxytkj.cn

[H07] 断言
来源：http://vf.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://pi.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://ia.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://oi.szsharing.cn

TS:   console.assert(x > 0);
来源：http://xq.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://vw.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ia.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fy.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ef.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://hm.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://tc.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fb.asd995.cn

JS:   e.message;  e.stack
来源：http://gk.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kb.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xc.hnjuh.cn

Go:   err.Error()
来源：http://ch.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://pb.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://ff.shtwfgs.cn

[H09] 带错误码的异常
来源：http://tz.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zg.haigaiapp.cn


<!-- 参考信息 -->