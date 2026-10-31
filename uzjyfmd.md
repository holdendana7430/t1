代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://td.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bk.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://vk.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cc.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pi.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gw.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lj.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hu.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gb.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ah.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://me.bjjhwx.cn

[F04] 追加写入文件
来源：http://cx.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kz.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kx.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://op.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yg.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sl.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dk.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cb.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rj.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://cb.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bk.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://vj.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://rp.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://ga.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tl.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pz.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ws.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://sm.bjjhwx.cn

[F06] 删除文件
来源：http://iu.asd995.cn

Py:   os.remove("a.txt")
来源：http://uj.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://fj.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yz.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nr.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mw.colortex.cn

Go:   os.Remove("a.txt")
来源：http://wf.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://mm.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://yz.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://hb.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vm.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xj.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ow.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kx.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ms.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zn.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lw.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aa.huixiangedu.cn

[F08] 遍历目录
来源：http://zh.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tu.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pz.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://jz.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://if.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xo.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ad.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://zk.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://mw.muxihuayi.cn

[F09] 获取文件大小
来源：http://nl.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://te.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://yo.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://fn.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://cz.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tc.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zk.huanxung.cn

Ruby: File.size("a.txt")
来源：http://we.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://hq.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://lg.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hs.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ge.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hv.asd995.cn

TS:   path.extname("a.txt")
来源：http://kc.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://id.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ud.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://om.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ja.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://jh.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zg.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ej.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qt.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kk.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tv.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bk.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mz.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jp.szsharing.cn

[F12] CSV 读写
来源：http://ye.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ch.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bo.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ft.jianghongdianzi.cn

TS:   // 同上
来源：http://cr.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lk.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fl.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vx.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bw.nicolike.cn

================================================================================
来源：http://ak.bookmarksfly.cn

G. 面向对象
来源：http://dq.hahajie.cn

================================================================================
来源：http://kk.bookmarksfly.cn

[G01] 定义类
来源：http://yp.lnxyls.cn

Py:   class User: pass
来源：http://jg.shtwfgs.cn

PHP:  class User {}
来源：http://ne.colortex.cn

JS:   class User {}
来源：http://xd.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://mf.hahajie.cn

Java: class User {}
来源：http://wp.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://mi.nicolike.cn

Ruby: class User; end
来源：http://tt.shxzskj.cn

C#:   class User {}
来源：http://og.9csxet.cn

[G02] 构造函数
来源：http://vy.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ze.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://us.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://zt.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://km.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://me.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kj.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://py.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://gm.huanxung.cn

[G03] 实例属性
来源：http://ah.gzmigu.cn

Py:   self.name = "x"
来源：http://ox.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://ny.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://fp.haigaiapp.cn

TS:   name: string = "x";
来源：http://fi.shxzskj.cn

Java: private String name;
来源：http://od.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://np.bjjhwx.cn

Ruby: @name = "x"
来源：http://ua.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://uq.521024.cn

[G04] 定义方法
来源：http://tr.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://sk.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uh.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://lb.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://sh.shxzukj.cn

Java: String greet() { return name; }
来源：http://kx.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ge.szxytkj.cn

Ruby: def greet; @name; end
来源：http://ww.521024.cn

C#:   public string Greet() => Name;
来源：http://aa.bjjhwx.cn

[G05] 继承
来源：http://sj.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://gk.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://ld.lnxyls.cn

JS:   class Admin extends User {}
来源：http://af.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://qz.huixiangedu.cn

Java: class Admin extends User {}
来源：http://cg.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lp.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://xa.shxzskj.cn

C#:   class Admin : User {}
来源：http://yd.shxzukj.cn

[G06] 重写方法
来源：http://ra.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://su.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ot.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://ve.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://dq.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://ij.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fg.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://do.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://ma.shtwfgs.cn

[G07] 调用父类方法
来源：http://vy.asd995.cn

Py:   super().greet()
来源：http://cz.521024.cn

PHP:  parent::greet();
来源：http://ut.yuexingan06.cn

JS:   super.greet();
来源：http://ti.panjiajie.cn

TS:   super.greet();
来源：http://nl.yuexingan06.cn

Java: super.greet();
来源：http://tf.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nj.jianghongdianzi.cn

Ruby: super
来源：http://ks.chemitech.net.cn

C#:   base.Greet();
来源：http://bq.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://rd.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wg.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://yn.hnjuh.cn

JS:   static f() {}
来源：http://fd.huixiangedu.cn

TS:   static f(): void {}
来源：http://cq.yuntaijiaju.cn

Java: static void f() {}
来源：http://dx.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cl.lnxyls.cn

Ruby: def self.f; end
来源：http://gl.gzmigu.cn

C#:   public static void F() {}
来源：http://om.nicolike.cn

[G09] 接口 / 抽象类
来源：http://rn.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://jn.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://it.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cn.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://er.asd995.cn

Java: interface Shape { double area(); }
来源：http://tc.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://uf.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gp.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://ev.newstarts.cn

[G10] 访问控制
来源：http://nj.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://iw.shxzskj.cn

PHP:  public / protected / private
来源：http://ai.colortex.cn

JS:   #private 字段；其余公开
来源：http://tv.szxytkj.cn

TS:   public / protected / private
来源：http://da.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://wt.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://to.nszjky.cn

Ruby: public / protected / private
来源：http://ab.9csxet.cn

C#:   public / protected / private / internal
来源：http://xm.huanxung.cn

[G11] getter / setter
来源：http://rp.9csxet.cn

Py:   @property 与 @x.setter
来源：http://ec.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tf.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://xc.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ji.newstarts.cn

Java: public String getName() { return name; }
来源：http://kr.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hl.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://uo.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://xe.hahajie.cn

[G12] 对象转字符串
来源：http://wx.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://dj.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uq.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://eq.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://zu.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://zp.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sj.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://wz.colortex.cn

C#:   public override string ToString() => Name;
来源：http://nj.lnxyls.cn

[G13] 判断对象类型
来源：http://ts.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://uy.szsharing.cn

PHP:  $u instanceof User
来源：http://ze.shxzukj.cn

JS:   u instanceof User
来源：http://zu.yuntaijiaju.cn

TS:   u instanceof User
来源：http://mx.muxihuayi.cn

Java: u instanceof User
来源：http://oi.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jm.hahajie.cn

Ruby: u.is_a?(User)
来源：http://qu.hnjuh.cn

C#:   u is User
来源：http://jf.hnjuh.cn

[G14] 数据类 / record
来源：http://zz.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rd.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://du.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rq.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://us.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://ve.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://ki.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tl.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://wy.huixinmuqiang.cn

[G15] 枚举
来源：http://dm.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vl.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cd.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uk.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ja.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://at.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ge.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://yf.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rt.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://of.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://io.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://uw.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://vw.521024.cn

TS:   Object.entries(obj)
来源：http://eb.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zy.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dr.huanxung.cn

Ruby: obj.instance_variables
来源：http://in.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://pm.chemitech.net.cn

================================================================================
来源：http://wr.huixiangedu.cn

H. 异常与错误处理
来源：http://ye.wgjwhj.cn

================================================================================
来源：http://uk.9csxet.cn

[H01] try / catch 基础
来源：http://iq.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://el.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gq.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://db.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xn.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tz.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nx.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zy.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qq.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://rp.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lt.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mr.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lh.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tw.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cz.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qe.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cz.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://st.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://sf.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://vi.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://db.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://sv.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://cr.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lz.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vf.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://py.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ee.huanxung.cn

[H04] 自定义异常类型
来源：http://sk.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://xh.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wk.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://ij.nicolike.cn

TS:   class MyError extends Error {}
来源：http://xl.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://um.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ds.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://wa.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://nj.haigaiapp.cn

[H05] 捕获特定类型
来源：http://bf.lnxyls.cn

Py:   except ValueError as e:
来源：http://pg.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pp.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ox.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ve.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://gq.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ln.521024.cn

Ruby: rescue ArgumentError => e
来源：http://kp.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://io.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://cn.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://kh.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pk.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dn.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tx.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vi.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hc.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://gz.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://ax.panjiajie.cn

[H07] 断言
来源：http://dn.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://oq.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://zr.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://aj.gzmigu.cn


<!-- 参考信息 -->