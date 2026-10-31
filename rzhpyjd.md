代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ws.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://gj.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pr.szsharing.cn

[F04] 追加写入文件
来源：http://eg.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gd.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pe.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vw.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ef.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lv.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bv.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qc.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gt.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://kd.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ar.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://op.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://cn.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://qb.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vd.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wi.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://kv.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://nd.521024.cn

[F06] 删除文件
来源：http://xb.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://yh.asd995.cn

PHP:  unlink("a.txt");
来源：http://qd.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zz.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://na.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vr.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://vi.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://rs.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://ri.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://jd.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rl.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pp.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pi.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://go.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gl.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jw.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uq.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ow.shxzukj.cn

[F08] 遍历目录
来源：http://qm.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hh.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ma.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://ip.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://tw.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xe.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://po.szsharing.cn

Ruby: Dir.children("dir")
来源：http://wx.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://yq.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://kv.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://wn.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://is.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://nn.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://tl.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zj.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fz.nicolike.cn

Ruby: File.size("a.txt")
来源：http://gp.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://gc.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://we.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qs.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://px.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xi.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://fh.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ya.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ww.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wn.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nj.hahajie.cn

[F11] 复制与移动文件
来源：http://xf.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ga.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vt.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ed.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://il.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://po.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xg.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://al.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ul.bookmarksfly.cn

[F12] CSV 读写
来源：http://mm.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fb.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yp.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aq.chemitech.net.cn

TS:   // 同上
来源：http://vq.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://my.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tw.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bn.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ax.wgjwhj.cn

================================================================================
来源：http://vn.huixinmuqiang.cn

G. 面向对象
来源：http://eq.521024.cn

================================================================================
来源：http://vv.jianghongdianzi.cn

[G01] 定义类
来源：http://dy.shxzukj.cn

Py:   class User: pass
来源：http://zx.shxzskj.cn

PHP:  class User {}
来源：http://xp.jctech888.com.cn

JS:   class User {}
来源：http://ds.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://bh.jctech888.com.cn

Java: class User {}
来源：http://ja.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://fa.yuntaijiaju.cn

Ruby: class User; end
来源：http://ez.huanxung.cn

C#:   class User {}
来源：http://bm.nszjky.cn

[G02] 构造函数
来源：http://jo.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://xp.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://an.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://qj.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://np.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://li.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ou.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://lp.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://du.gzmigu.cn

[G03] 实例属性
来源：http://vo.shxzukj.cn

Py:   self.name = "x"
来源：http://yc.huanxung.cn

PHP:  public string $name = "x";
来源：http://ux.hahajie.cn

JS:   this.name = "x";
来源：http://ot.nszjky.cn

TS:   name: string = "x";
来源：http://ir.hnjuh.cn

Java: private String name;
来源：http://lw.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xh.colortex.cn

Ruby: @name = "x"
来源：http://gp.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://dj.yuntaijiaju.cn

[G04] 定义方法
来源：http://vj.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://eq.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jp.521024.cn

JS:   greet() { return this.name; }
来源：http://wr.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://fx.asd995.cn

Java: String greet() { return name; }
来源：http://gh.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://io.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://lf.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://pe.huixiangedu.cn

[G05] 继承
来源：http://db.asd995.cn

Py:   class Admin(User): pass
来源：http://jm.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://ut.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ql.hahajie.cn

TS:   class Admin extends User {}
来源：http://wa.hahajie.cn

Java: class Admin extends User {}
来源：http://cw.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fc.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://ca.9csxet.cn

C#:   class Admin : User {}
来源：http://iy.bjjhwx.cn

[G06] 重写方法
来源：http://xm.colortex.cn

Py:   def greet(self): return "admin"
来源：http://um.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qw.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://su.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ki.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://iu.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://af.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://tq.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://nx.wgjwhj.cn

[G07] 调用父类方法
来源：http://tf.huixiangedu.cn

Py:   super().greet()
来源：http://qp.szsharing.cn

PHP:  parent::greet();
来源：http://ay.muxihuayi.cn

JS:   super.greet();
来源：http://aq.bookmarksfly.cn

TS:   super.greet();
来源：http://hc.wgjwhj.cn

Java: super.greet();
来源：http://ia.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tf.haigaiapp.cn

Ruby: super
来源：http://kv.colortex.cn

C#:   base.Greet();
来源：http://xv.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://wy.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://as.muxihuayi.cn

PHP:  public static function f() {}
来源：http://mi.nszjky.cn

JS:   static f() {}
来源：http://tr.colortex.cn

TS:   static f(): void {}
来源：http://yo.muxihuayi.cn

Java: static void f() {}
来源：http://ca.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nn.lnxyls.cn

Ruby: def self.f; end
来源：http://cb.jctech888.com.cn

C#:   public static void F() {}
来源：http://wh.521024.cn

[G09] 接口 / 抽象类
来源：http://zs.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://aw.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wb.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zn.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://rt.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://eu.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://tx.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tt.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://ot.521024.cn

[G10] 访问控制
来源：http://em.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://ca.haigaiapp.cn

PHP:  public / protected / private
来源：http://td.szsharing.cn

JS:   #private 字段；其余公开
来源：http://il.jctech888.com.cn

TS:   public / protected / private
来源：http://pd.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://iy.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ww.bookmarksfly.cn

Ruby: public / protected / private
来源：http://xl.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ch.nszjky.cn

[G11] getter / setter
来源：http://yi.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://hv.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aj.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ej.521024.cn

TS:   get name(): string { return this._name; }
来源：http://ib.colortex.cn

Java: public String getName() { return name; }
来源：http://cg.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jo.colortex.cn

Ruby: attr_accessor :name
来源：http://rn.newstarts.cn

C#:   public string Name { get; set; }
来源：http://pc.521024.cn

[G12] 对象转字符串
来源：http://zr.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://yb.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dj.521024.cn

JS:   toString() { return this.name; }
来源：http://ys.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://gn.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://zl.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xw.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://qu.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://ap.nszjky.cn

[G13] 判断对象类型
来源：http://ph.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://fe.panjiajie.cn

PHP:  $u instanceof User
来源：http://vo.nszjky.cn

JS:   u instanceof User
来源：http://ds.huixiangedu.cn

TS:   u instanceof User
来源：http://hw.huixinmuqiang.cn

Java: u instanceof User
来源：http://aj.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yv.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://lm.chemitech.net.cn

C#:   u is User
来源：http://bd.9csxet.cn

[G14] 数据类 / record
来源：http://pu.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gy.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://ky.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rd.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://jv.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://xn.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://wf.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ur.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://dr.521024.cn

[G15] 枚举
来源：http://tf.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ae.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mq.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tn.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uy.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://uj.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nl.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://ld.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jl.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://wj.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ke.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://hu.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://rh.asd995.cn

TS:   Object.entries(obj)
来源：http://gq.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pu.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gh.shxzskj.cn

Ruby: obj.instance_variables
来源：http://na.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://wz.9csxet.cn

================================================================================
来源：http://gx.colortex.cn

H. 异常与错误处理
来源：http://bd.hahajie.cn

================================================================================
来源：http://ym.haigaiapp.cn

[H01] try / catch 基础
来源：http://as.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ji.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ev.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ez.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://is.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fr.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://md.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jh.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fo.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://jg.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ox.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ol.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iy.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://on.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cq.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bv.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pv.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ve.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://if.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://hv.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ei.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://fw.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://us.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ro.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mn.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ki.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ia.nicolike.cn

[H04] 自定义异常类型
来源：http://eu.asd995.cn

Py:   class MyError(Exception): pass
来源：http://fn.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hx.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://ma.hahajie.cn

TS:   class MyError extends Error {}
来源：http://me.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://ji.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://me.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://al.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://jw.huixiangedu.cn

[H05] 捕获特定类型
来源：http://pr.bjjhwx.cn

Py:   except ValueError as e:
来源：http://dl.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://av.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://av.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://to.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://xd.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hu.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://dc.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ls.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://dq.colortex.cn

Py:   value = d.get("k") or default
来源：http://nc.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zy.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ms.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vp.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tf.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fk.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://cn.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://ju.shxzukj.cn

[H07] 断言
来源：http://rw.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://xx.szsharing.cn

PHP:  assert($x > 0);
来源：http://cy.nicolike.cn

JS:   console.assert(x > 0);
来源：http://yn.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://cd.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://am.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ya.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lj.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://xh.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://ig.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://vi.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jf.szsharing.cn


<!-- 参考信息 -->