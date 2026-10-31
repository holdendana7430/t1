代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hw.jctech888.com.cn

[F02] 逐行读取文件
来源：http://qk.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ch.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ms.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://in.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zw.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ah.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ux.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fi.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kk.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://cn.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ja.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://np.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://df.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ur.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hk.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qk.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://wz.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ja.shxzukj.cn

[F04] 追加写入文件
来源：http://ey.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bw.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vu.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wz.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://me.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qe.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ur.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ij.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vt.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://pg.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oo.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://xn.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://ax.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://wu.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kh.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kl.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://ah.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://qz.521024.cn

[F06] 删除文件
来源：http://hc.huanxung.cn

Py:   os.remove("a.txt")
来源：http://rr.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://th.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tj.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kj.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://re.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://ec.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://om.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ua.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://nr.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zp.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xw.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gq.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vs.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bh.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jo.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wa.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ui.haigaiapp.cn

[F08] 遍历目录
来源：http://il.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uj.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cw.521024.cn

JS:   fs.readdirSync("dir")
来源：http://el.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://bp.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nk.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ij.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://wy.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://xd.panjiajie.cn

[F09] 获取文件大小
来源：http://pa.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://pw.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://hv.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://mu.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://rb.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mm.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://li.huanxung.cn

Ruby: File.size("a.txt")
来源：http://ha.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://hh.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://ii.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ku.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qt.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yx.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://mm.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ll.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qa.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nq.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lw.newstarts.cn

[F11] 复制与移动文件
来源：http://fl.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kn.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jx.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lp.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bh.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fp.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lv.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wi.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uq.yuexingan06.cn

[F12] CSV 读写
来源：http://kj.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kt.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rb.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yi.gzmigu.cn

TS:   // 同上
来源：http://ni.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pj.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rk.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://um.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wd.huanxung.cn

================================================================================
来源：http://vk.bjjhwx.cn

G. 面向对象
来源：http://vz.bjjhwx.cn

================================================================================
来源：http://ca.bjjhwx.cn

[G01] 定义类
来源：http://er.bjjhwx.cn

Py:   class User: pass
来源：http://tl.bookmarksfly.cn

PHP:  class User {}
来源：http://gp.huanxung.cn

JS:   class User {}
来源：http://ka.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://sf.lnxyls.cn

Java: class User {}
来源：http://ck.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://rz.shtwfgs.cn

Ruby: class User; end
来源：http://ef.bookmarksfly.cn

C#:   class User {}
来源：http://st.shxzskj.cn

[G02] 构造函数
来源：http://xr.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://tp.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://ka.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://uq.asd995.cn

TS:   constructor(public name: string) {}
来源：http://ve.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://fz.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qr.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://xp.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://uz.nszjky.cn

[G03] 实例属性
来源：http://ol.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://uj.huanxung.cn

PHP:  public string $name = "x";
来源：http://ky.szsharing.cn

JS:   this.name = "x";
来源：http://ne.muxihuayi.cn

TS:   name: string = "x";
来源：http://ys.shxzskj.cn

Java: private String name;
来源：http://il.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vv.newstarts.cn

Ruby: @name = "x"
来源：http://wk.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://cu.colortex.cn

[G04] 定义方法
来源：http://qf.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://am.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jp.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://ml.521024.cn

TS:   greet(): string { return this.name; }
来源：http://fm.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://sb.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qr.shxzskj.cn

Ruby: def greet; @name; end
来源：http://zh.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://vq.nszjky.cn

[G05] 继承
来源：http://lw.asd995.cn

Py:   class Admin(User): pass
来源：http://mi.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://rl.newstarts.cn

JS:   class Admin extends User {}
来源：http://iy.hahajie.cn

TS:   class Admin extends User {}
来源：http://fu.szsharing.cn

Java: class Admin extends User {}
来源：http://io.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xb.lnxyls.cn

Ruby: class Admin < User; end
来源：http://ik.szsharing.cn

C#:   class Admin : User {}
来源：http://cn.bjjhwx.cn

[G06] 重写方法
来源：http://pd.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://gp.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://am.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ty.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://hj.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://uy.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qs.colortex.cn

Ruby: def greet; "admin"; end
来源：http://oa.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://fs.haigaiapp.cn

[G07] 调用父类方法
来源：http://pw.colortex.cn

Py:   super().greet()
来源：http://zs.wgjwhj.cn

PHP:  parent::greet();
来源：http://rd.bookmarksfly.cn

JS:   super.greet();
来源：http://he.gzmigu.cn

TS:   super.greet();
来源：http://et.yuexingan06.cn

Java: super.greet();
来源：http://cj.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lo.9csxet.cn

Ruby: super
来源：http://vh.colortex.cn

C#:   base.Greet();
来源：http://lr.asd995.cn

[G08] 静态方法与属性
来源：http://ay.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://im.bjjhwx.cn

PHP:  public static function f() {}
来源：http://uf.muxihuayi.cn

JS:   static f() {}
来源：http://zd.yuexingan06.cn

TS:   static f(): void {}
来源：http://vw.shxzukj.cn

Java: static void f() {}
来源：http://pp.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ts.lnxyls.cn

Ruby: def self.f; end
来源：http://rr.jctech888.com.cn

C#:   public static void F() {}
来源：http://vb.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://uf.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://yd.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xw.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ua.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://tv.colortex.cn

Java: interface Shape { double area(); }
来源：http://wm.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://rx.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ov.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://nr.gzmigu.cn

[G10] 访问控制
来源：http://wz.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://cb.chemitech.net.cn

PHP:  public / protected / private
来源：http://nb.nicolike.cn

JS:   #private 字段；其余公开
来源：http://lz.huanxung.cn

TS:   public / protected / private
来源：http://fh.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://qm.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ic.haigaiapp.cn

Ruby: public / protected / private
来源：http://nn.lnxyls.cn

C#:   public / protected / private / internal
来源：http://or.jctech888.com.cn

[G11] getter / setter
来源：http://rv.nszjky.cn

Py:   @property 与 @x.setter
来源：http://fq.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rj.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://gy.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://hp.szxytkj.cn

Java: public String getName() { return name; }
来源：http://ti.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ug.colortex.cn

Ruby: attr_accessor :name
来源：http://vv.newstarts.cn

C#:   public string Name { get; set; }
来源：http://kz.newstarts.cn

[G12] 对象转字符串
来源：http://vl.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://sh.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hx.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://ql.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://fu.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://gv.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cs.521024.cn

Ruby: def to_s; @name; end
来源：http://ut.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://zb.asd995.cn

[G13] 判断对象类型
来源：http://wz.hnjuh.cn

Py:   isinstance(u, User)
来源：http://sh.gzmigu.cn

PHP:  $u instanceof User
来源：http://iw.huixinmuqiang.cn

JS:   u instanceof User
来源：http://uy.szsharing.cn

TS:   u instanceof User
来源：http://ba.colortex.cn

Java: u instanceof User
来源：http://pj.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bq.colortex.cn

Ruby: u.is_a?(User)
来源：http://lq.asd995.cn

C#:   u is User
来源：http://oz.521024.cn

[G14] 数据类 / record
来源：http://zd.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jt.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://ue.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://se.521024.cn

TS:   type User = { name: string; age: number };
来源：http://cb.colortex.cn

Java: record User(String name, int age) {}
来源：http://ew.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://um.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kh.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://zl.hahajie.cn

[G15] 枚举
来源：http://xt.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lb.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kb.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cz.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ky.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://ub.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ci.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://ot.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eg.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://he.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yw.colortex.cn

PHP:  get_object_vars($obj);
来源：http://vf.gzmigu.cn

JS:   Object.entries(obj)
来源：http://xu.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://pg.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tr.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fw.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://ly.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://gu.nszjky.cn

================================================================================
来源：http://xo.jianghongdianzi.cn

H. 异常与错误处理
来源：http://hi.9csxet.cn

================================================================================
来源：http://fx.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://gm.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://om.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hp.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ww.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yv.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yl.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fg.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aj.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lc.asd995.cn

[H02] finally / ensure 收尾
来源：http://yp.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sj.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nd.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ge.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://va.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sq.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pl.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xc.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ly.szxytkj.cn

[H03] 主动抛出异常
来源：http://rq.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://we.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cx.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://xn.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://mq.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uh.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ub.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mq.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dt.hahajie.cn

[H04] 自定义异常类型
来源：http://jl.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://vm.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yj.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://ff.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://qc.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://gr.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lp.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://st.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://pk.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://wi.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://dy.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nt.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://ky.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://gg.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://px.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mo.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://jf.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ku.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://ko.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://un.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ta.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jy.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dx.asd995.cn


<!-- 参考信息 -->