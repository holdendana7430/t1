代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ci.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fq.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://ur.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vp.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ln.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yq.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pz.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://su.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xo.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://gz.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yb.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://wj.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://an.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hk.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nw.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ov.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://df.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ae.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pz.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bt.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://zk.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://td.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://xe.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://hs.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://vt.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rb.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gn.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://or.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://hm.asd995.cn

[F06] 删除文件
来源：http://kw.asd995.cn

Py:   os.remove("a.txt")
来源：http://sc.newstarts.cn

PHP:  unlink("a.txt");
来源：http://ht.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jk.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hq.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ll.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://wf.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://gt.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://zc.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://mj.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kr.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ss.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ek.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hm.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jn.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pd.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cl.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fs.521024.cn

[F08] 遍历目录
来源：http://xp.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ly.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dv.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://tk.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://as.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rc.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vp.9csxet.cn

Ruby: Dir.children("dir")
来源：http://ms.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://ko.chemitech.net.cn

[F09] 获取文件大小
来源：http://ea.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://ti.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://wo.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://nk.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://fe.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oo.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://du.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://jw.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://uu.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://mk.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yh.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yb.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fw.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://km.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sb.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eg.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://di.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jd.jctech888.com.cn

[F11] 复制与移动文件
来源：http://rv.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gj.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://do.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ou.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vf.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uc.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jl.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://za.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hk.shxzukj.cn

[F12] CSV 读写
来源：http://rh.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bs.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://la.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ps.chemitech.net.cn

TS:   // 同上
来源：http://gu.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zb.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hj.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xs.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vh.huanxung.cn

================================================================================
来源：http://tx.huanxung.cn

G. 面向对象
来源：http://iq.asd995.cn

================================================================================
来源：http://mz.hnjuh.cn

[G01] 定义类
来源：http://kn.chemitech.net.cn

Py:   class User: pass
来源：http://qe.yuexingan06.cn

PHP:  class User {}
来源：http://hg.huanxung.cn

JS:   class User {}
来源：http://ay.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://oj.colortex.cn

Java: class User {}
来源：http://ls.lnxyls.cn

Go:   type User struct { Name string }
来源：http://ux.nszjky.cn

Ruby: class User; end
来源：http://rk.yuntaijiaju.cn

C#:   class User {}
来源：http://so.szxytkj.cn

[G02] 构造函数
来源：http://wo.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://zf.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://rk.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://jp.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://ca.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://sn.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mb.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://fe.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://rp.9csxet.cn

[G03] 实例属性
来源：http://ne.colortex.cn

Py:   self.name = "x"
来源：http://hg.huanxung.cn

PHP:  public string $name = "x";
来源：http://dd.muxihuayi.cn

JS:   this.name = "x";
来源：http://aa.panjiajie.cn

TS:   name: string = "x";
来源：http://te.nicolike.cn

Java: private String name;
来源：http://ep.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://el.szsharing.cn

Ruby: @name = "x"
来源：http://el.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://eg.jianghongdianzi.cn

[G04] 定义方法
来源：http://da.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://qm.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oz.asd995.cn

JS:   greet() { return this.name; }
来源：http://oz.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://bp.wgjwhj.cn

Java: String greet() { return name; }
来源：http://go.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zc.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://lq.nicolike.cn

C#:   public string Greet() => Name;
来源：http://gg.bjjhwx.cn

[G05] 继承
来源：http://sg.521024.cn

Py:   class Admin(User): pass
来源：http://jw.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://zz.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://lp.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://nz.shxzukj.cn

Java: class Admin extends User {}
来源：http://ce.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gk.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://vw.lnxyls.cn

C#:   class Admin : User {}
来源：http://cv.nicolike.cn

[G06] 重写方法
来源：http://oq.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://ds.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pu.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://tb.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://ma.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://hu.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wx.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://mf.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://hn.shtwfgs.cn

[G07] 调用父类方法
来源：http://ix.wgjwhj.cn

Py:   super().greet()
来源：http://av.gzmigu.cn

PHP:  parent::greet();
来源：http://yg.muxihuayi.cn

JS:   super.greet();
来源：http://lj.jctech888.com.cn

TS:   super.greet();
来源：http://cl.yuntaijiaju.cn

Java: super.greet();
来源：http://fg.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ep.yuexingan06.cn

Ruby: super
来源：http://sc.szxytkj.cn

C#:   base.Greet();
来源：http://rd.gzmigu.cn

[G08] 静态方法与属性
来源：http://sy.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jy.hnjuh.cn

PHP:  public static function f() {}
来源：http://he.szxytkj.cn

JS:   static f() {}
来源：http://zf.panjiajie.cn

TS:   static f(): void {}
来源：http://pa.nicolike.cn

Java: static void f() {}
来源：http://vn.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gf.wgjwhj.cn

Ruby: def self.f; end
来源：http://lx.szxytkj.cn

C#:   public static void F() {}
来源：http://jh.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://dz.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://qr.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xn.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yj.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://iu.hahajie.cn

Java: interface Shape { double area(); }
来源：http://ar.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ha.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ea.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://gy.panjiajie.cn

[G10] 访问控制
来源：http://cn.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://do.szxytkj.cn

PHP:  public / protected / private
来源：http://xx.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://tz.colortex.cn

TS:   public / protected / private
来源：http://tn.colortex.cn

Java: public / protected / private / 默认包级
来源：http://qo.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tf.haigaiapp.cn

Ruby: public / protected / private
来源：http://ln.9csxet.cn

C#:   public / protected / private / internal
来源：http://sh.muxihuayi.cn

[G11] getter / setter
来源：http://ec.nicolike.cn

Py:   @property 与 @x.setter
来源：http://zp.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dc.colortex.cn

JS:   get name() { return this._name; }
来源：http://kl.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://am.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://hw.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xg.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://oy.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://wi.nicolike.cn

[G12] 对象转字符串
来源：http://bc.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://xe.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qb.521024.cn

JS:   toString() { return this.name; }
来源：http://di.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://ka.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://sa.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://on.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://qp.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://wf.nszjky.cn

[G13] 判断对象类型
来源：http://rm.colortex.cn

Py:   isinstance(u, User)
来源：http://zo.hahajie.cn

PHP:  $u instanceof User
来源：http://ea.shxzskj.cn

JS:   u instanceof User
来源：http://ig.wgjwhj.cn

TS:   u instanceof User
来源：http://im.hnjuh.cn

Java: u instanceof User
来源：http://bi.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qp.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://ey.asd995.cn

C#:   u is User
来源：http://yy.jctech888.com.cn

[G14] 数据类 / record
来源：http://zc.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fj.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://vf.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dq.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://ij.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://uq.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://ej.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ch.521024.cn

C#:   record User(string Name, int Age);
来源：http://fo.lnxyls.cn

[G15] 枚举
来源：http://sc.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uv.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rc.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ca.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lj.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://rz.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ei.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://ub.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yr.colortex.cn

[G16] 对象转数组 / 字典
来源：http://dt.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vr.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://rn.9csxet.cn

JS:   Object.entries(obj)
来源：http://ln.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://ra.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gn.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jy.newstarts.cn

Ruby: obj.instance_variables
来源：http://gq.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://ps.shxzskj.cn

================================================================================
来源：http://ie.newstarts.cn

H. 异常与错误处理
来源：http://rl.huanxung.cn

================================================================================
来源：http://ss.nicolike.cn

[H01] try / catch 基础
来源：http://hk.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rp.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cl.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bq.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kr.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qe.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rf.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dj.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://au.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://dt.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kc.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nq.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gx.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ra.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bk.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dp.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lt.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xe.lnxyls.cn

[H03] 主动抛出异常
来源：http://dv.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://nh.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ds.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://mr.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://ao.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zg.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aq.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ac.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nj.szxytkj.cn

[H04] 自定义异常类型
来源：http://ov.colortex.cn

Py:   class MyError(Exception): pass
来源：http://gq.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fe.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://es.szsharing.cn

TS:   class MyError extends Error {}
来源：http://he.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://ah.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kj.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://fe.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://ol.lnxyls.cn

[H05] 捕获特定类型
来源：http://sk.shxzukj.cn

Py:   except ValueError as e:
来源：http://ps.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sz.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://yc.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ds.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://by.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fd.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://bw.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tr.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://ty.nszjky.cn

Py:   value = d.get("k") or default
来源：http://li.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xx.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mj.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://op.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fu.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://go.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://th.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://jr.bookmarksfly.cn

[H07] 断言
来源：http://fi.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://vp.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://nj.asd995.cn

JS:   console.assert(x > 0);
来源：http://vv.shxzskj.cn


<!-- 参考信息 -->