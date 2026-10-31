代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://vh.9csxet.cn

[F02] 逐行读取文件
来源：http://by.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hw.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kg.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kx.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xx.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cf.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kt.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://io.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yy.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://lb.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fd.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lo.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gk.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lu.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cg.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yt.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://rm.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fw.wgjwhj.cn

[F04] 追加写入文件
来源：http://at.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wk.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ya.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iv.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vt.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tk.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xj.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ks.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cj.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://jg.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zr.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://se.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://iw.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://cz.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hf.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ja.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://kn.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://jy.wgjwhj.cn

[F06] 删除文件
来源：http://dy.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://am.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://bx.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eo.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jr.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kd.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://lx.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://zz.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://ig.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://sn.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ca.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uo.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ri.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zo.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kk.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kh.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://br.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kc.jianghongdianzi.cn

[F08] 遍历目录
来源：http://pt.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ec.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uf.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://mw.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://ny.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nb.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jt.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://js.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://cj.colortex.cn

[F09] 获取文件大小
来源：http://cb.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://mm.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://dm.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://mv.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://xq.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ob.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nx.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://mb.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://iy.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://rn.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cv.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ih.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qb.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://vx.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cu.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://np.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jm.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ci.yuexingan06.cn

[F11] 复制与移动文件
来源：http://ig.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ds.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ge.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://at.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wj.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bs.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ni.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xc.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oq.shxzskj.cn

[F12] CSV 读写
来源：http://sd.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zh.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ec.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kt.panjiajie.cn

TS:   // 同上
来源：http://xn.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://by.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nt.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oo.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://at.nicolike.cn

================================================================================
来源：http://jr.szxytkj.cn

G. 面向对象
来源：http://we.nszjky.cn

================================================================================
来源：http://sh.bjjhwx.cn

[G01] 定义类
来源：http://ek.colortex.cn

Py:   class User: pass
来源：http://zb.haigaiapp.cn

PHP:  class User {}
来源：http://po.yuntaijiaju.cn

JS:   class User {}
来源：http://of.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://yd.szsharing.cn

Java: class User {}
来源：http://ew.hnjuh.cn

Go:   type User struct { Name string }
来源：http://pb.hahajie.cn

Ruby: class User; end
来源：http://qh.shtwfgs.cn

C#:   class User {}
来源：http://ol.yuntaijiaju.cn

[G02] 构造函数
来源：http://cb.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://hy.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://zj.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://ui.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://gq.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://ax.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zz.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://vd.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://tq.jianghongdianzi.cn

[G03] 实例属性
来源：http://vi.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://nm.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://yf.wgjwhj.cn

JS:   this.name = "x";
来源：http://bh.wgjwhj.cn

TS:   name: string = "x";
来源：http://sr.lnxyls.cn

Java: private String name;
来源：http://az.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ao.huixiangedu.cn

Ruby: @name = "x"
来源：http://hu.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://md.muxihuayi.cn

[G04] 定义方法
来源：http://vv.nszjky.cn

Py:   def greet(self): return self.name
来源：http://br.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ia.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://gp.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://gp.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://sl.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rk.panjiajie.cn

Ruby: def greet; @name; end
来源：http://ys.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://qu.huixinmuqiang.cn

[G05] 继承
来源：http://ci.gzmigu.cn

Py:   class Admin(User): pass
来源：http://yc.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://bf.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://vg.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://jl.nicolike.cn

Java: class Admin extends User {}
来源：http://lv.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gv.hnjuh.cn

Ruby: class Admin < User; end
来源：http://qj.bjjhwx.cn

C#:   class Admin : User {}
来源：http://fe.huixiangedu.cn

[G06] 重写方法
来源：http://zg.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://rs.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zo.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://fo.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://ab.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://cg.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cv.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://xp.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://ql.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://qu.jctech888.com.cn

Py:   super().greet()
来源：http://io.hnjuh.cn

PHP:  parent::greet();
来源：http://zc.huixiangedu.cn

JS:   super.greet();
来源：http://bd.gzmigu.cn

TS:   super.greet();
来源：http://yi.yuexingan06.cn

Java: super.greet();
来源：http://aj.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mh.chemitech.net.cn

Ruby: super
来源：http://rd.nicolike.cn

C#:   base.Greet();
来源：http://qc.gzmigu.cn

[G08] 静态方法与属性
来源：http://ug.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cx.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://fu.9csxet.cn

JS:   static f() {}
来源：http://ho.panjiajie.cn

TS:   static f(): void {}
来源：http://eu.asd995.cn

Java: static void f() {}
来源：http://gq.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vw.jctech888.com.cn

Ruby: def self.f; end
来源：http://qp.szxytkj.cn

C#:   public static void F() {}
来源：http://vt.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://qn.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://ui.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bp.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pz.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://ym.9csxet.cn

Java: interface Shape { double area(); }
来源：http://bu.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://vb.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ce.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://ex.hahajie.cn

[G10] 访问控制
来源：http://cz.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://wi.9csxet.cn

PHP:  public / protected / private
来源：http://qr.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://do.huixiangedu.cn

TS:   public / protected / private
来源：http://ch.asd995.cn

Java: public / protected / private / 默认包级
来源：http://qf.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ms.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://in.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://cl.wgjwhj.cn

[G11] getter / setter
来源：http://ai.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://bz.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xb.colortex.cn

JS:   get name() { return this._name; }
来源：http://da.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://je.panjiajie.cn

Java: public String getName() { return name; }
来源：http://oa.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ho.521024.cn

Ruby: attr_accessor :name
来源：http://fr.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://zu.shxzukj.cn

[G12] 对象转字符串
来源：http://nx.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://is.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vx.nicolike.cn

JS:   toString() { return this.name; }
来源：http://pg.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://hf.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://az.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bh.nicolike.cn

Ruby: def to_s; @name; end
来源：http://xe.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://na.shxzukj.cn

[G13] 判断对象类型
来源：http://uz.nszjky.cn

Py:   isinstance(u, User)
来源：http://pe.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://ht.shtwfgs.cn

JS:   u instanceof User
来源：http://pu.muxihuayi.cn

TS:   u instanceof User
来源：http://on.lnxyls.cn

Java: u instanceof User
来源：http://lr.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hg.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://hr.gzmigu.cn

C#:   u is User
来源：http://fb.shxzskj.cn

[G14] 数据类 / record
来源：http://jg.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ix.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://fa.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ul.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://so.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://cf.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://rd.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yy.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://sg.gzmigu.cn

[G15] 枚举
来源：http://zk.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cn.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://df.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oc.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jb.521024.cn

Java: enum Color { RED, GREEN }
来源：http://dn.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xv.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://el.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sy.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://zo.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zo.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://cj.521024.cn

JS:   Object.entries(obj)
来源：http://id.521024.cn

TS:   Object.entries(obj)
来源：http://jm.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pa.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dn.lnxyls.cn

Ruby: obj.instance_variables
来源：http://ue.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://qf.chemitech.net.cn

================================================================================
来源：http://hj.szxytkj.cn

H. 异常与错误处理
来源：http://ja.szsharing.cn

================================================================================
来源：http://iq.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://as.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ha.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cg.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://je.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lh.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dt.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uv.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://su.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zz.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://nl.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hk.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://il.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ro.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rm.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bb.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mk.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oo.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vl.hahajie.cn

[H03] 主动抛出异常
来源：http://sv.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://dj.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sv.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://my.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://ja.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lz.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://os.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eb.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gl.hnjuh.cn

[H04] 自定义异常类型
来源：http://fy.521024.cn

Py:   class MyError(Exception): pass
来源：http://dv.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://po.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://sf.nszjky.cn

TS:   class MyError extends Error {}
来源：http://kz.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://di.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fb.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://bo.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://ra.huanxung.cn

[H05] 捕获特定类型
来源：http://jl.huanxung.cn

Py:   except ValueError as e:
来源：http://ff.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ry.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://qq.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://kt.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://ec.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oq.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://sa.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ye.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://jd.521024.cn

Py:   value = d.get("k") or default
来源：http://le.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eq.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://af.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://po.bjjhwx.cn


<!-- 参考信息 -->