代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://ay.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nb.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ni.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lb.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ru.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://bl.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ub.bookmarksfly.cn

[F04] 追加写入文件
来源：http://ec.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vv.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pj.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nj.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ej.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ia.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gd.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nb.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jq.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://sb.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oe.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://fp.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://sd.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://tq.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vb.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ml.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://kp.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://hp.wgjwhj.cn

[F06] 删除文件
来源：http://ai.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://dj.521024.cn

PHP:  unlink("a.txt");
来源：http://ow.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pe.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cj.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jl.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://gi.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://oj.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://bs.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://uj.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rv.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fn.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rt.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qr.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qa.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://it.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oi.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mn.haigaiapp.cn

[F08] 遍历目录
来源：http://il.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eg.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tn.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://kq.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://pk.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gj.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://et.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://xk.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://zk.nszjky.cn

[F09] 获取文件大小
来源：http://zd.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://wf.nszjky.cn

PHP:  filesize("a.txt");
来源：http://nt.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://mh.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://ce.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aj.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zi.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://gm.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://sm.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://su.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kd.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://py.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ve.9csxet.cn

TS:   path.extname("a.txt")
来源：http://uk.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pt.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vx.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xq.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://in.szxytkj.cn

[F11] 复制与移动文件
来源：http://xg.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cn.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lz.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tq.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yk.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dt.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yt.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fk.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ln.gzmigu.cn

[F12] CSV 读写
来源：http://mq.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bt.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pd.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wv.gzmigu.cn

TS:   // 同上
来源：http://ih.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ck.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ed.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://em.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tb.szxytkj.cn

================================================================================
来源：http://ts.9csxet.cn

G. 面向对象
来源：http://sf.asd995.cn

================================================================================
来源：http://dt.newstarts.cn

[G01] 定义类
来源：http://np.nszjky.cn

Py:   class User: pass
来源：http://ny.nicolike.cn

PHP:  class User {}
来源：http://ai.szxytkj.cn

JS:   class User {}
来源：http://yy.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://qq.muxihuayi.cn

Java: class User {}
来源：http://mx.panjiajie.cn

Go:   type User struct { Name string }
来源：http://hp.9csxet.cn

Ruby: class User; end
来源：http://ot.yuntaijiaju.cn

C#:   class User {}
来源：http://qq.nszjky.cn

[G02] 构造函数
来源：http://xy.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://mt.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://qo.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://es.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://lm.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://lx.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wi.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ht.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://dl.huixinmuqiang.cn

[G03] 实例属性
来源：http://yn.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://zd.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://ml.huanxung.cn

JS:   this.name = "x";
来源：http://rf.hnjuh.cn

TS:   name: string = "x";
来源：http://rs.nszjky.cn

Java: private String name;
来源：http://et.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ck.chemitech.net.cn

Ruby: @name = "x"
来源：http://hb.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://nz.huixiangedu.cn

[G04] 定义方法
来源：http://dm.nicolike.cn

Py:   def greet(self): return self.name
来源：http://vf.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kd.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://kx.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://vk.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://fo.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uw.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://xs.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://bf.haigaiapp.cn

[G05] 继承
来源：http://po.szxytkj.cn

Py:   class Admin(User): pass
来源：http://vq.9csxet.cn

PHP:  class Admin extends User {}
来源：http://su.lnxyls.cn

JS:   class Admin extends User {}
来源：http://hw.szsharing.cn

TS:   class Admin extends User {}
来源：http://ap.huanxung.cn

Java: class Admin extends User {}
来源：http://xh.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rd.shxzskj.cn

Ruby: class Admin < User; end
来源：http://lp.szxytkj.cn

C#:   class Admin : User {}
来源：http://ay.wgjwhj.cn

[G06] 重写方法
来源：http://th.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://tp.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://im.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://bh.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ep.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://gm.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ia.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://tc.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://cz.hahajie.cn

[G07] 调用父类方法
来源：http://li.shxzukj.cn

Py:   super().greet()
来源：http://jf.hahajie.cn

PHP:  parent::greet();
来源：http://uh.jianghongdianzi.cn

JS:   super.greet();
来源：http://is.jianghongdianzi.cn

TS:   super.greet();
来源：http://jc.huanxung.cn

Java: super.greet();
来源：http://rj.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qj.yuexingan06.cn

Ruby: super
来源：http://di.yuexingan06.cn

C#:   base.Greet();
来源：http://rd.panjiajie.cn

[G08] 静态方法与属性
来源：http://vs.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tt.asd995.cn

PHP:  public static function f() {}
来源：http://jy.shxzskj.cn

JS:   static f() {}
来源：http://wz.9csxet.cn

TS:   static f(): void {}
来源：http://fe.wgjwhj.cn

Java: static void f() {}
来源：http://rt.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ru.yuexingan06.cn

Ruby: def self.f; end
来源：http://tn.szxytkj.cn

C#:   public static void F() {}
来源：http://dp.nszjky.cn

[G09] 接口 / 抽象类
来源：http://aj.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://ir.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xc.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xe.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://ft.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://ea.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://nc.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xi.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://sr.huixiangedu.cn

[G10] 访问控制
来源：http://vm.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://qi.muxihuayi.cn

PHP:  public / protected / private
来源：http://oz.huanxung.cn

JS:   #private 字段；其余公开
来源：http://az.wgjwhj.cn

TS:   public / protected / private
来源：http://zb.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://dc.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://go.szxytkj.cn

Ruby: public / protected / private
来源：http://va.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://ht.huixiangedu.cn

[G11] getter / setter
来源：http://uv.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://nf.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qi.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://hh.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://qy.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://fl.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zr.colortex.cn

Ruby: attr_accessor :name
来源：http://vj.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://by.huixiangedu.cn

[G12] 对象转字符串
来源：http://el.asd995.cn

Py:   def __str__(self): return self.name
来源：http://fl.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mu.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://wj.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://rc.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://rj.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bx.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://kg.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://dp.chemitech.net.cn

[G13] 判断对象类型
来源：http://ax.shxzskj.cn

Py:   isinstance(u, User)
来源：http://gu.lnxyls.cn

PHP:  $u instanceof User
来源：http://ja.gzmigu.cn

JS:   u instanceof User
来源：http://gg.521024.cn

TS:   u instanceof User
来源：http://no.asd995.cn

Java: u instanceof User
来源：http://ry.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ys.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://xg.asd995.cn

C#:   u is User
来源：http://xl.haigaiapp.cn

[G14] 数据类 / record
来源：http://pc.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yl.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://sr.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sp.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://rj.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://lh.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://lp.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yn.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://nj.shtwfgs.cn

[G15] 枚举
来源：http://ip.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nc.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qb.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bz.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qu.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://nl.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ew.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://rm.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nb.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://xh.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uw.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://ww.huanxung.cn

JS:   Object.entries(obj)
来源：http://cy.asd995.cn

TS:   Object.entries(obj)
来源：http://fd.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mw.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://un.521024.cn

Ruby: obj.instance_variables
来源：http://xa.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://sa.wgjwhj.cn

================================================================================
来源：http://rn.gzmigu.cn

H. 异常与错误处理
来源：http://ns.haigaiapp.cn

================================================================================
来源：http://uk.szsharing.cn

[H01] try / catch 基础
来源：http://kf.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gd.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kl.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ps.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://es.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ly.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://be.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://im.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ho.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://jr.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://by.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ps.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bz.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pj.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ov.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nq.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qe.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qp.hnjuh.cn

[H03] 主动抛出异常
来源：http://uz.521024.cn

Py:   raise ValueError("错误信息")
来源：http://ea.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://su.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://as.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://br.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ix.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ad.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bq.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ch.shtwfgs.cn

[H04] 自定义异常类型
来源：http://wi.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://ml.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ju.521024.cn

JS:   class MyError extends Error {}
来源：http://qe.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://vo.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://ze.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vu.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://fb.asd995.cn

C#:   class MyException : Exception {}
来源：http://ec.9csxet.cn

[H05] 捕获特定类型
来源：http://pr.haigaiapp.cn

Py:   except ValueError as e:
来源：http://oc.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kl.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://gy.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://eg.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://bd.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wm.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://xt.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uu.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ax.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://sx.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sg.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qc.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ft.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hj.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iv.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://wn.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://ev.9csxet.cn

[H07] 断言
来源：http://zs.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://ln.9csxet.cn

PHP:  assert($x > 0);
来源：http://cx.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://vg.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://xx.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://iu.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fx.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zi.colortex.cn


<!-- 参考信息 -->