代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kn.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rg.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pm.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vc.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ru.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://ki.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://of.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qw.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ml.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xa.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nl.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jn.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://zo.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dv.bookmarksfly.cn

[F04] 追加写入文件
来源：http://ov.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ry.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rt.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ty.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nr.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ux.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ty.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xx.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jj.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://ul.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cw.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://zy.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://xc.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ht.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ox.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ak.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://jc.colortex.cn

C#:   File.Exists("a.txt")
来源：http://ni.shtwfgs.cn

[F06] 删除文件
来源：http://mv.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://md.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://fu.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tm.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vm.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nw.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://mp.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://eu.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://zw.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://sx.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rf.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rt.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eg.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pp.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uq.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yz.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dr.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uu.bjjhwx.cn

[F08] 遍历目录
来源：http://bz.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zn.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jp.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://ym.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://gp.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ux.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bl.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://an.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://wn.wgjwhj.cn

[F09] 获取文件大小
来源：http://eo.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://sq.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ft.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://rm.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://oi.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ky.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mu.hahajie.cn

Ruby: File.size("a.txt")
来源：http://vs.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://du.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://ef.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wm.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zl.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ls.521024.cn

TS:   path.extname("a.txt")
来源：http://dl.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vm.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rp.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ge.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mg.hahajie.cn

[F11] 复制与移动文件
来源：http://dm.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tl.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tg.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tb.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ey.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lw.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://np.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dq.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fk.lnxyls.cn

[F12] CSV 读写
来源：http://wy.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lx.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://va.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ke.shtwfgs.cn

TS:   // 同上
来源：http://zf.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hu.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dt.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jk.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pc.haigaiapp.cn

================================================================================
来源：http://gh.huanxung.cn

G. 面向对象
来源：http://gi.shtwfgs.cn

================================================================================
来源：http://cd.muxihuayi.cn

[G01] 定义类
来源：http://qh.gzmigu.cn

Py:   class User: pass
来源：http://pg.huixinmuqiang.cn

PHP:  class User {}
来源：http://tl.szsharing.cn

JS:   class User {}
来源：http://fg.colortex.cn

TS:   class User { name: string = ""; }
来源：http://tl.gzmigu.cn

Java: class User {}
来源：http://gd.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://yn.hnjuh.cn

Ruby: class User; end
来源：http://bw.colortex.cn

C#:   class User {}
来源：http://fh.yuntaijiaju.cn

[G02] 构造函数
来源：http://jq.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://yy.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://nf.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://gi.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://wn.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ha.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sp.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://yr.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://fo.gzmigu.cn

[G03] 实例属性
来源：http://gm.bookmarksfly.cn

Py:   self.name = "x"
来源：http://nv.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://hd.panjiajie.cn

JS:   this.name = "x";
来源：http://mv.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://if.lnxyls.cn

Java: private String name;
来源：http://hl.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ne.muxihuayi.cn

Ruby: @name = "x"
来源：http://kk.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://kq.huixiangedu.cn

[G04] 定义方法
来源：http://ww.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://xi.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ta.colortex.cn

JS:   greet() { return this.name; }
来源：http://lf.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://jm.gzmigu.cn

Java: String greet() { return name; }
来源：http://le.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bb.lnxyls.cn

Ruby: def greet; @name; end
来源：http://gd.szsharing.cn

C#:   public string Greet() => Name;
来源：http://hj.yuexingan06.cn

[G05] 继承
来源：http://ck.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://wr.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://nk.9csxet.cn

JS:   class Admin extends User {}
来源：http://bx.asd995.cn

TS:   class Admin extends User {}
来源：http://cw.shxzukj.cn

Java: class Admin extends User {}
来源：http://zc.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://we.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://jf.huixiangedu.cn

C#:   class Admin : User {}
来源：http://vk.huixiangedu.cn

[G06] 重写方法
来源：http://da.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://ec.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bh.asd995.cn

JS:   greet() { return "admin"; }
来源：http://tn.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://zk.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://zv.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gf.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://cq.521024.cn

C#:   public override string Greet() => "admin";
来源：http://ri.lnxyls.cn

[G07] 调用父类方法
来源：http://en.muxihuayi.cn

Py:   super().greet()
来源：http://kn.haigaiapp.cn

PHP:  parent::greet();
来源：http://vi.szxytkj.cn

JS:   super.greet();
来源：http://hg.bookmarksfly.cn

TS:   super.greet();
来源：http://ee.shxzukj.cn

Java: super.greet();
来源：http://xd.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kg.shxzukj.cn

Ruby: super
来源：http://eu.bookmarksfly.cn

C#:   base.Greet();
来源：http://ul.nicolike.cn

[G08] 静态方法与属性
来源：http://es.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cd.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://rd.shxzskj.cn

JS:   static f() {}
来源：http://zt.chemitech.net.cn

TS:   static f(): void {}
来源：http://gs.huixinmuqiang.cn

Java: static void f() {}
来源：http://tq.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fe.haigaiapp.cn

Ruby: def self.f; end
来源：http://vz.newstarts.cn

C#:   public static void F() {}
来源：http://tv.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://zr.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://xn.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://si.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://si.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://we.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://qw.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://zr.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qe.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://ay.bookmarksfly.cn

[G10] 访问控制
来源：http://af.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://vn.colortex.cn

PHP:  public / protected / private
来源：http://wt.nicolike.cn

JS:   #private 字段；其余公开
来源：http://oz.jctech888.com.cn

TS:   public / protected / private
来源：http://wu.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://rl.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://am.huanxung.cn

Ruby: public / protected / private
来源：http://xq.gzmigu.cn

C#:   public / protected / private / internal
来源：http://mv.chemitech.net.cn

[G11] getter / setter
来源：http://jo.nszjky.cn

Py:   @property 与 @x.setter
来源：http://xj.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dh.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://aa.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://wz.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://ue.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iu.newstarts.cn

Ruby: attr_accessor :name
来源：http://hk.521024.cn

C#:   public string Name { get; set; }
来源：http://qa.521024.cn

[G12] 对象转字符串
来源：http://ma.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://fq.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nq.hahajie.cn

JS:   toString() { return this.name; }
来源：http://oy.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://jh.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://uq.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aw.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://yn.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://om.hnjuh.cn

[G13] 判断对象类型
来源：http://yf.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://oc.asd995.cn

PHP:  $u instanceof User
来源：http://zk.shxzukj.cn

JS:   u instanceof User
来源：http://yb.szxytkj.cn

TS:   u instanceof User
来源：http://lp.huanxung.cn

Java: u instanceof User
来源：http://pg.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jq.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://dy.huanxung.cn

C#:   u is User
来源：http://md.colortex.cn

[G14] 数据类 / record
来源：http://wu.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xm.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://jg.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rr.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://yo.newstarts.cn

Java: record User(String name, int age) {}
来源：http://wr.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://dv.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rp.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://fm.yuntaijiaju.cn

[G15] 枚举
来源：http://gr.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vw.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fb.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ja.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qg.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://pz.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hw.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://dq.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ox.colortex.cn

[G16] 对象转数组 / 字典
来源：http://aa.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gb.asd995.cn

PHP:  get_object_vars($obj);
来源：http://zc.szsharing.cn

JS:   Object.entries(obj)
来源：http://ng.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://ut.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mr.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qb.shxzukj.cn

Ruby: obj.instance_variables
来源：http://wg.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://zl.asd995.cn

================================================================================
来源：http://wh.9csxet.cn

H. 异常与错误处理
来源：http://rk.yuexingan06.cn

================================================================================
来源：http://as.hahajie.cn

[H01] try / catch 基础
来源：http://mg.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ug.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ro.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bl.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pu.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bq.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zr.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xy.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lt.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://yv.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kq.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eh.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://df.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://js.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://of.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jr.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rl.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ry.huanxung.cn

[H03] 主动抛出异常
来源：http://la.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://bm.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ad.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://tg.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://cl.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bo.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bn.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fd.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://da.newstarts.cn

[H04] 自定义异常类型
来源：http://tm.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://ou.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xu.hahajie.cn

JS:   class MyError extends Error {}
来源：http://cy.521024.cn

TS:   class MyError extends Error {}
来源：http://zi.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ci.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://us.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://yk.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://tb.panjiajie.cn

[H05] 捕获特定类型
来源：http://kb.hnjuh.cn

Py:   except ValueError as e:
来源：http://qv.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ip.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://gd.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://rk.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://kq.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nd.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://qb.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pa.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://gr.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://ru.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fq.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ww.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ak.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pa.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://am.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ax.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://ab.haigaiapp.cn


<!-- 参考信息 -->