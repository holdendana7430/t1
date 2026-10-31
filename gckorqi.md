代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://ga.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hr.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pp.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vp.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ey.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://dh.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yk.jctech888.com.cn

[F04] 追加写入文件
来源：http://jr.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://db.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://um.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://va.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yn.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zd.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ma.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hq.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sb.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://di.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ak.colortex.cn

PHP:  file_exists("a.txt");
来源：http://dm.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ga.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://lo.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ah.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mh.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://vu.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://oc.shxzskj.cn

[F06] 删除文件
来源：http://bx.asd995.cn

Py:   os.remove("a.txt")
来源：http://qr.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://up.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zo.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wj.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ql.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://yv.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://ql.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://lq.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://lp.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fw.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aw.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xe.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ep.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vi.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hl.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zb.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kp.jctech888.com.cn

[F08] 遍历目录
来源：http://vf.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://it.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://so.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://dg.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://vu.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zc.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lu.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://bl.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://xt.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://oo.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://ss.colortex.cn

PHP:  filesize("a.txt");
来源：http://kk.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://td.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://ja.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yx.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tk.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://de.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://tv.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://qn.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xm.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cu.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iy.asd995.cn

TS:   path.extname("a.txt")
来源：http://nv.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tk.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mc.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fd.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://de.muxihuayi.cn

[F11] 复制与移动文件
来源：http://za.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ld.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hd.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jy.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ey.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xx.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ud.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lm.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bc.yuexingan06.cn

[F12] CSV 读写
来源：http://hc.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uc.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xp.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ub.bookmarksfly.cn

TS:   // 同上
来源：http://zb.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jy.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vc.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cd.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eq.newstarts.cn

================================================================================
来源：http://sz.jianghongdianzi.cn

G. 面向对象
来源：http://jc.huanxung.cn

================================================================================
来源：http://ip.lnxyls.cn

[G01] 定义类
来源：http://nu.bjjhwx.cn

Py:   class User: pass
来源：http://lv.jctech888.com.cn

PHP:  class User {}
来源：http://yk.hahajie.cn

JS:   class User {}
来源：http://ol.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://fz.lnxyls.cn

Java: class User {}
来源：http://iz.hahajie.cn

Go:   type User struct { Name string }
来源：http://hv.jctech888.com.cn

Ruby: class User; end
来源：http://ux.jctech888.com.cn

C#:   class User {}
来源：http://gz.bookmarksfly.cn

[G02] 构造函数
来源：http://ab.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://rz.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ch.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://ns.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://qn.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://ko.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://od.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://bf.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://hq.shxzskj.cn

[G03] 实例属性
来源：http://io.shtwfgs.cn

Py:   self.name = "x"
来源：http://cd.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://ie.9csxet.cn

JS:   this.name = "x";
来源：http://ik.huixiangedu.cn

TS:   name: string = "x";
来源：http://so.hnjuh.cn

Java: private String name;
来源：http://yw.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pc.huixiangedu.cn

Ruby: @name = "x"
来源：http://ay.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://vb.huixinmuqiang.cn

[G04] 定义方法
来源：http://mv.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://jg.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fa.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://nh.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://hi.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://am.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pu.hnjuh.cn

Ruby: def greet; @name; end
来源：http://cr.szsharing.cn

C#:   public string Greet() => Name;
来源：http://sw.jctech888.com.cn

[G05] 继承
来源：http://jq.huanxung.cn

Py:   class Admin(User): pass
来源：http://jz.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://hy.lnxyls.cn

JS:   class Admin extends User {}
来源：http://ol.shxzskj.cn

TS:   class Admin extends User {}
来源：http://nm.newstarts.cn

Java: class Admin extends User {}
来源：http://xp.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wi.colortex.cn

Ruby: class Admin < User; end
来源：http://bv.hahajie.cn

C#:   class Admin : User {}
来源：http://rf.huanxung.cn

[G06] 重写方法
来源：http://nk.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://ap.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ss.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://ln.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://wq.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://sd.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://he.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://xq.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://sw.shxzskj.cn

[G07] 调用父类方法
来源：http://dt.shxzukj.cn

Py:   super().greet()
来源：http://hy.chemitech.net.cn

PHP:  parent::greet();
来源：http://pl.hahajie.cn

JS:   super.greet();
来源：http://mm.521024.cn

TS:   super.greet();
来源：http://cx.szsharing.cn

Java: super.greet();
来源：http://gz.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cx.huixiangedu.cn

Ruby: super
来源：http://kx.newstarts.cn

C#:   base.Greet();
来源：http://pb.muxihuayi.cn

[G08] 静态方法与属性
来源：http://tx.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://be.szxytkj.cn

PHP:  public static function f() {}
来源：http://xi.bookmarksfly.cn

JS:   static f() {}
来源：http://oy.huanxung.cn

TS:   static f(): void {}
来源：http://nf.lnxyls.cn

Java: static void f() {}
来源：http://bo.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://og.yuexingan06.cn

Ruby: def self.f; end
来源：http://sq.jctech888.com.cn

C#:   public static void F() {}
来源：http://iw.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://ui.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://gu.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fu.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mq.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://pr.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://rt.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ln.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qg.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://dp.jctech888.com.cn

[G10] 访问控制
来源：http://fg.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://pu.szxytkj.cn

PHP:  public / protected / private
来源：http://nc.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://vj.wgjwhj.cn

TS:   public / protected / private
来源：http://zm.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://yp.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://to.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://ju.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://rf.hnjuh.cn

[G11] getter / setter
来源：http://di.szsharing.cn

Py:   @property 与 @x.setter
来源：http://nv.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wa.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://zu.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://xg.szsharing.cn

Java: public String getName() { return name; }
来源：http://fo.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pq.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://qv.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://bx.yuexingan06.cn

[G12] 对象转字符串
来源：http://yi.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://pk.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://is.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://bv.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://kt.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://wb.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rq.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://nu.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://ra.yuexingan06.cn

[G13] 判断对象类型
来源：http://lg.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://ka.colortex.cn

PHP:  $u instanceof User
来源：http://jh.shxzskj.cn

JS:   u instanceof User
来源：http://cf.9csxet.cn

TS:   u instanceof User
来源：http://hj.huanxung.cn

Java: u instanceof User
来源：http://hw.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vp.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://im.hnjuh.cn

C#:   u is User
来源：http://ab.nicolike.cn

[G14] 数据类 / record
来源：http://kb.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lu.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://qa.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mo.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://pl.nicolike.cn

Java: record User(String name, int age) {}
来源：http://mi.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://zd.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jc.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://zg.bjjhwx.cn

[G15] 枚举
来源：http://dm.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pe.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hu.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ll.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nb.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://gd.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yi.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://he.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lv.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://fe.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://am.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ea.huanxung.cn

JS:   Object.entries(obj)
来源：http://hx.nicolike.cn

TS:   Object.entries(obj)
来源：http://pm.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vk.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jz.panjiajie.cn

Ruby: obj.instance_variables
来源：http://yk.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://qf.huixiangedu.cn

================================================================================
来源：http://bg.chemitech.net.cn

H. 异常与错误处理
来源：http://xv.chemitech.net.cn

================================================================================
来源：http://na.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://nq.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jl.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nr.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zr.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pm.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jx.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ac.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sp.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gd.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://wy.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zc.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://em.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ss.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jj.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fk.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zs.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dp.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pa.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://dc.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://iu.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ac.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://pr.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://cs.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://re.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mj.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xo.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yz.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://wh.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://rj.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nt.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://wc.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://ge.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://qh.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ej.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://po.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://hk.nszjky.cn

[H05] 捕获特定类型
来源：http://zm.szsharing.cn

Py:   except ValueError as e:
来源：http://ko.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fi.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://as.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://dd.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://fd.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dj.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://fl.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ff.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://zt.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://gf.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mf.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://os.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ei.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rm.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uz.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://gj.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://zh.wgjwhj.cn

[H07] 断言
来源：http://we.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://yp.hahajie.cn

PHP:  assert($x > 0);
来源：http://dq.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://cz.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://se.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://eh.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mb.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tk.jianghongdianzi.cn


<!-- 参考信息 -->