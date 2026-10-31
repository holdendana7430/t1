代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sy.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://uu.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bu.shxzukj.cn

[F04] 追加写入文件
来源：http://bj.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vj.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yj.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qr.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jo.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hh.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lc.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ue.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yq.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://zq.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dq.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://vd.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://lj.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://tj.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mm.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tv.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://tp.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://if.nszjky.cn

[F06] 删除文件
来源：http://gf.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://kt.asd995.cn

PHP:  unlink("a.txt");
来源：http://ve.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xc.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hi.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fc.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://zs.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://bl.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://hk.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ot.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ln.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oh.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pf.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://df.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fq.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://al.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qv.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ln.jianghongdianzi.cn

[F08] 遍历目录
来源：http://ov.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xe.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ph.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://bo.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://eq.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ki.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ta.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://ui.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://ux.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://vf.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ok.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://oi.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://fm.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://hi.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://go.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kt.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://pk.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ih.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://yv.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hq.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sk.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rj.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://tt.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jg.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bk.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ee.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ic.hahajie.cn

[F11] 复制与移动文件
来源：http://zu.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ba.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://et.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wc.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://za.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ex.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ux.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fs.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://te.huanxung.cn

[F12] CSV 读写
来源：http://ah.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ru.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bl.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tg.gzmigu.cn

TS:   // 同上
来源：http://mp.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hp.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qm.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lq.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kj.yuntaijiaju.cn

================================================================================
来源：http://nr.huixinmuqiang.cn

G. 面向对象
来源：http://lh.gzmigu.cn

================================================================================
来源：http://bn.gzmigu.cn

[G01] 定义类
来源：http://wq.yuntaijiaju.cn

Py:   class User: pass
来源：http://ha.gzmigu.cn

PHP:  class User {}
来源：http://uo.asd995.cn

JS:   class User {}
来源：http://bz.asd995.cn

TS:   class User { name: string = ""; }
来源：http://sk.gzmigu.cn

Java: class User {}
来源：http://sp.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://iy.asd995.cn

Ruby: class User; end
来源：http://bc.hnjuh.cn

C#:   class User {}
来源：http://st.muxihuayi.cn

[G02] 构造函数
来源：http://pu.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://fl.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://wi.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://xe.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://ft.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://wl.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uv.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ra.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://zo.bookmarksfly.cn

[G03] 实例属性
来源：http://kz.bookmarksfly.cn

Py:   self.name = "x"
来源：http://rc.9csxet.cn

PHP:  public string $name = "x";
来源：http://rt.huanxung.cn

JS:   this.name = "x";
来源：http://jg.nszjky.cn

TS:   name: string = "x";
来源：http://wp.szxytkj.cn

Java: private String name;
来源：http://sa.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qq.nszjky.cn

Ruby: @name = "x"
来源：http://iz.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://zu.9csxet.cn

[G04] 定义方法
来源：http://xw.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://xg.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cg.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://ni.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://jc.colortex.cn

Java: String greet() { return name; }
来源：http://ir.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ab.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://lk.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://sn.shxzukj.cn

[G05] 继承
来源：http://qs.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://sj.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://if.521024.cn

JS:   class Admin extends User {}
来源：http://ht.nicolike.cn

TS:   class Admin extends User {}
来源：http://bw.huixiangedu.cn

Java: class Admin extends User {}
来源：http://fl.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vo.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://yl.asd995.cn

C#:   class Admin : User {}
来源：http://wl.colortex.cn

[G06] 重写方法
来源：http://bk.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://az.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dh.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://xt.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://gm.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://hf.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ke.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://os.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://iu.muxihuayi.cn

[G07] 调用父类方法
来源：http://zi.bjjhwx.cn

Py:   super().greet()
来源：http://ye.newstarts.cn

PHP:  parent::greet();
来源：http://xn.jctech888.com.cn

JS:   super.greet();
来源：http://br.shtwfgs.cn

TS:   super.greet();
来源：http://yg.newstarts.cn

Java: super.greet();
来源：http://wd.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oc.newstarts.cn

Ruby: super
来源：http://ws.szxytkj.cn

C#:   base.Greet();
来源：http://vc.yuexingan06.cn

[G08] 静态方法与属性
来源：http://yj.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bq.nicolike.cn

PHP:  public static function f() {}
来源：http://sb.hahajie.cn

JS:   static f() {}
来源：http://mo.wgjwhj.cn

TS:   static f(): void {}
来源：http://wo.yuexingan06.cn

Java: static void f() {}
来源：http://fb.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kh.9csxet.cn

Ruby: def self.f; end
来源：http://kq.panjiajie.cn

C#:   public static void F() {}
来源：http://lj.colortex.cn

[G09] 接口 / 抽象类
来源：http://rm.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://jo.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xk.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jv.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://eh.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://qq.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://yw.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://de.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://uk.yuntaijiaju.cn

[G10] 访问控制
来源：http://fj.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://tc.lnxyls.cn

PHP:  public / protected / private
来源：http://bx.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://dg.nicolike.cn

TS:   public / protected / private
来源：http://qi.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://yu.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sz.asd995.cn

Ruby: public / protected / private
来源：http://zd.nszjky.cn

C#:   public / protected / private / internal
来源：http://wf.shtwfgs.cn

[G11] getter / setter
来源：http://tu.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://fy.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oq.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://gl.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://ct.nszjky.cn

Java: public String getName() { return name; }
来源：http://wr.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nl.521024.cn

Ruby: attr_accessor :name
来源：http://tc.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://cu.nicolike.cn

[G12] 对象转字符串
来源：http://wy.colortex.cn

Py:   def __str__(self): return self.name
来源：http://ms.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kl.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://pp.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://me.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://ov.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kz.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://yj.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://fy.9csxet.cn

[G13] 判断对象类型
来源：http://oj.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://wm.lnxyls.cn

PHP:  $u instanceof User
来源：http://ho.panjiajie.cn

JS:   u instanceof User
来源：http://vl.chemitech.net.cn

TS:   u instanceof User
来源：http://dh.521024.cn

Java: u instanceof User
来源：http://im.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ln.huanxung.cn

Ruby: u.is_a?(User)
来源：http://zy.bookmarksfly.cn

C#:   u is User
来源：http://fm.shxzukj.cn

[G14] 数据类 / record
来源：http://xe.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ej.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://xv.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qk.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://rg.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://sn.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://yi.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kk.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://ka.muxihuayi.cn

[G15] 枚举
来源：http://wr.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://do.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zq.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rf.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pt.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://yg.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sy.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://rk.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oy.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://lh.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dz.521024.cn

PHP:  get_object_vars($obj);
来源：http://uk.lnxyls.cn

JS:   Object.entries(obj)
来源：http://df.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://gj.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ex.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rg.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://pi.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://on.hahajie.cn

================================================================================
来源：http://ix.colortex.cn

H. 异常与错误处理
来源：http://ms.nszjky.cn

================================================================================
来源：http://pu.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://na.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jj.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mf.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wl.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xk.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fj.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nn.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://im.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kc.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://ak.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tc.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wh.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cr.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zv.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jy.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dz.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oe.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://et.asd995.cn

[H03] 主动抛出异常
来源：http://nc.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ot.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://be.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://ia.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://zp.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pg.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ou.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qy.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xj.colortex.cn

[H04] 自定义异常类型
来源：http://qa.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://dx.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cf.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://fw.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://hi.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://sl.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mr.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://oe.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://vk.lnxyls.cn

[H05] 捕获特定类型
来源：http://qc.muxihuayi.cn

Py:   except ValueError as e:
来源：http://ku.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uo.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://zx.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://lx.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://ua.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kz.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://no.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zs.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://jc.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://qd.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pa.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sh.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zk.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nz.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wc.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://gu.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://tf.jianghongdianzi.cn

[H07] 断言
来源：http://vw.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://hw.szsharing.cn

PHP:  assert($x > 0);
来源：http://sp.colortex.cn

JS:   console.assert(x > 0);
来源：http://ua.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://vp.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://of.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://um.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ui.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://sx.521024.cn

[H08] 获取错误信息与堆栈
来源：http://pf.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://st.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yx.chemitech.net.cn


<!-- 参考信息 -->