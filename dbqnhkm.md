代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ut.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dw.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wn.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wm.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gc.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jx.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://oo.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://po.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mv.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zh.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bs.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sc.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ih.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://hf.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pi.jctech888.com.cn

[F04] 追加写入文件
来源：http://fm.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ti.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vi.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bd.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yj.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oo.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dy.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iy.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vz.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://gq.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hh.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://wf.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://em.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://oe.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rv.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mo.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://ud.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://xs.chemitech.net.cn

[F06] 删除文件
来源：http://cs.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://ss.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://qm.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vy.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cf.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oa.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://vr.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://bw.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://va.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://is.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mf.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://go.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ol.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fa.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xu.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eh.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://if.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fa.shxzukj.cn

[F08] 遍历目录
来源：http://cl.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ob.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hv.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://up.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://ot.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xb.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xl.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://nh.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://nc.lnxyls.cn

[F09] 获取文件大小
来源：http://br.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://ny.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://fr.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://zy.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://zy.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pj.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ce.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://gc.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://zm.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://yd.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ez.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lq.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kh.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://th.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xu.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sy.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zl.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://he.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://ws.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dh.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bo.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ab.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gb.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zk.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gq.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kw.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sl.chemitech.net.cn

[F12] CSV 读写
来源：http://ec.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yn.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uh.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ej.asd995.cn

TS:   // 同上
来源：http://la.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ll.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hp.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nu.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ap.nicolike.cn

================================================================================
来源：http://de.jctech888.com.cn

G. 面向对象
来源：http://gr.shxzukj.cn

================================================================================
来源：http://zz.huixinmuqiang.cn

[G01] 定义类
来源：http://ht.jianghongdianzi.cn

Py:   class User: pass
来源：http://pn.bookmarksfly.cn

PHP:  class User {}
来源：http://nj.muxihuayi.cn

JS:   class User {}
来源：http://gi.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ec.jctech888.com.cn

Java: class User {}
来源：http://ej.szsharing.cn

Go:   type User struct { Name string }
来源：http://wu.haigaiapp.cn

Ruby: class User; end
来源：http://qg.chemitech.net.cn

C#:   class User {}
来源：http://yz.newstarts.cn

[G02] 构造函数
来源：http://wc.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://id.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://ww.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://mi.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://bg.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://zk.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ph.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://gv.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ri.hnjuh.cn

[G03] 实例属性
来源：http://bv.nszjky.cn

Py:   self.name = "x"
来源：http://to.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://fy.shtwfgs.cn

JS:   this.name = "x";
来源：http://zz.lnxyls.cn

TS:   name: string = "x";
来源：http://cz.colortex.cn

Java: private String name;
来源：http://gk.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://al.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://qn.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://lj.yuexingan06.cn

[G04] 定义方法
来源：http://vd.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://dp.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ng.huanxung.cn

JS:   greet() { return this.name; }
来源：http://ij.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://nk.gzmigu.cn

Java: String greet() { return name; }
来源：http://fz.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://it.newstarts.cn

Ruby: def greet; @name; end
来源：http://dx.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://qw.huixinmuqiang.cn

[G05] 继承
来源：http://ss.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://si.521024.cn

PHP:  class Admin extends User {}
来源：http://aj.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://iw.shxzskj.cn

TS:   class Admin extends User {}
来源：http://op.hahajie.cn

Java: class Admin extends User {}
来源：http://lt.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yw.nicolike.cn

Ruby: class Admin < User; end
来源：http://qs.lnxyls.cn

C#:   class Admin : User {}
来源：http://cs.huixinmuqiang.cn

[G06] 重写方法
来源：http://cc.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://xa.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rh.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://dt.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://vi.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://xe.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dl.asd995.cn

Ruby: def greet; "admin"; end
来源：http://vt.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://ue.hnjuh.cn

[G07] 调用父类方法
来源：http://eh.jctech888.com.cn

Py:   super().greet()
来源：http://zj.hahajie.cn

PHP:  parent::greet();
来源：http://pw.9csxet.cn

JS:   super.greet();
来源：http://dd.gzmigu.cn

TS:   super.greet();
来源：http://br.haigaiapp.cn

Java: super.greet();
来源：http://rc.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ia.chemitech.net.cn

Ruby: super
来源：http://co.szxytkj.cn

C#:   base.Greet();
来源：http://wx.lnxyls.cn

[G08] 静态方法与属性
来源：http://ok.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xa.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://sp.521024.cn

JS:   static f() {}
来源：http://ao.huixiangedu.cn

TS:   static f(): void {}
来源：http://qo.haigaiapp.cn

Java: static void f() {}
来源：http://lr.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mj.jctech888.com.cn

Ruby: def self.f; end
来源：http://bi.chemitech.net.cn

C#:   public static void F() {}
来源：http://vd.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://zw.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://sx.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vn.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gd.521024.cn

TS:   interface Shape { area(): number; }
来源：http://re.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://vz.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://bh.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sj.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://vm.huixinmuqiang.cn

[G10] 访问控制
来源：http://dn.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://vm.gzmigu.cn

PHP:  public / protected / private
来源：http://cz.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://tt.huanxung.cn

TS:   public / protected / private
来源：http://xk.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://wz.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ie.hahajie.cn

Ruby: public / protected / private
来源：http://nl.shxzskj.cn

C#:   public / protected / private / internal
来源：http://eg.huixinmuqiang.cn

[G11] getter / setter
来源：http://nt.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://fv.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dk.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://eo.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://fo.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://ks.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ve.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://mr.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://cx.shxzukj.cn

[G12] 对象转字符串
来源：http://ke.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://hi.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sl.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://sv.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://cp.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://dd.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hv.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://ug.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://yh.gzmigu.cn

[G13] 判断对象类型
来源：http://iy.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://mk.nicolike.cn

PHP:  $u instanceof User
来源：http://za.shxzukj.cn

JS:   u instanceof User
来源：http://yp.bookmarksfly.cn

TS:   u instanceof User
来源：http://sf.jianghongdianzi.cn

Java: u instanceof User
来源：http://xd.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hg.nszjky.cn

Ruby: u.is_a?(User)
来源：http://lt.newstarts.cn

C#:   u is User
来源：http://jj.bookmarksfly.cn

[G14] 数据类 / record
来源：http://sb.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yk.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://nv.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://od.521024.cn

TS:   type User = { name: string; age: number };
来源：http://cs.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://as.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://os.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rq.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://fm.jianghongdianzi.cn

[G15] 枚举
来源：http://mc.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ac.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vd.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tn.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oo.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://lw.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sl.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://tf.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fv.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://rl.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eg.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://ty.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://jq.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://aa.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ql.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vb.hnjuh.cn

Ruby: obj.instance_variables
来源：http://jv.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://aa.newstarts.cn

================================================================================
来源：http://ua.muxihuayi.cn

H. 异常与错误处理
来源：http://jf.huixiangedu.cn

================================================================================
来源：http://ku.521024.cn

[H01] try / catch 基础
来源：http://zl.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wj.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hb.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fg.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yy.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vl.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lk.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hv.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lv.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://gz.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://en.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ex.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oq.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dp.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lw.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dh.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tl.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fb.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://pg.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://je.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ze.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://mj.colortex.cn

TS:   throw new Error("错误信息");
来源：http://nc.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mn.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hx.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fv.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rz.huanxung.cn

[H04] 自定义异常类型
来源：http://zc.asd995.cn

Py:   class MyError(Exception): pass
来源：http://mw.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hp.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://sf.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://gj.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://zr.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ll.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://pl.szsharing.cn

C#:   class MyException : Exception {}
来源：http://wj.shtwfgs.cn

[H05] 捕获特定类型
来源：http://jg.huanxung.cn

Py:   except ValueError as e:
来源：http://ca.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://el.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://pg.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://lh.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://wv.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pi.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://bh.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mp.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://op.9csxet.cn

Py:   value = d.get("k") or default
来源：http://ev.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ri.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cq.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ph.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://id.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bw.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://td.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://vr.hahajie.cn


<!-- 参考信息 -->