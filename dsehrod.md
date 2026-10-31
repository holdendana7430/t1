代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lk.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lu.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uw.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lj.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lb.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vv.colortex.cn

[F03] 写入文件（覆盖）
来源：http://cu.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aw.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wr.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sz.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://er.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hr.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yh.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://rd.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ds.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://lv.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fu.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gs.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lj.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ld.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kj.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://us.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://de.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ra.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://ut.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wt.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://wy.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://ww.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://vi.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gu.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zd.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://ax.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://qa.szxytkj.cn

[F06] 删除文件
来源：http://gc.521024.cn

Py:   os.remove("a.txt")
来源：http://yb.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://nz.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sj.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yd.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dv.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://xp.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://as.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://qq.colortex.cn

[F07] 创建目录（含多级）
来源：http://fo.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dt.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zf.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qx.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xr.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fb.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hi.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mn.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ib.shtwfgs.cn

[F08] 遍历目录
来源：http://sk.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dt.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ng.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://qe.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://qz.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ss.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gq.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://uy.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://dl.huixiangedu.cn

[F09] 获取文件大小
来源：http://jq.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://em.hahajie.cn

PHP:  filesize("a.txt");
来源：http://nv.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://fv.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://fl.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wa.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gy.huanxung.cn

Ruby: File.size("a.txt")
来源：http://te.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://vg.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://xd.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vg.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xb.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mz.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://gl.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fi.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jw.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://um.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tw.9csxet.cn

[F11] 复制与移动文件
来源：http://az.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fl.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fw.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wv.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pz.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wx.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mn.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://db.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rx.gzmigu.cn

[F12] CSV 读写
来源：http://yc.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wm.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pg.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iu.9csxet.cn

TS:   // 同上
来源：http://eh.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qt.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lw.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iq.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cw.jianghongdianzi.cn

================================================================================
来源：http://yu.shxzukj.cn

G. 面向对象
来源：http://dk.haigaiapp.cn

================================================================================
来源：http://sh.panjiajie.cn

[G01] 定义类
来源：http://pg.hahajie.cn

Py:   class User: pass
来源：http://vb.asd995.cn

PHP:  class User {}
来源：http://kx.szxytkj.cn

JS:   class User {}
来源：http://mh.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ph.szsharing.cn

Java: class User {}
来源：http://vx.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://ll.gzmigu.cn

Ruby: class User; end
来源：http://ql.521024.cn

C#:   class User {}
来源：http://hr.szxytkj.cn

[G02] 构造函数
来源：http://vv.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://ws.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://nw.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://ke.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://pt.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://vd.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://td.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://wm.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://be.huixinmuqiang.cn

[G03] 实例属性
来源：http://ia.shxzskj.cn

Py:   self.name = "x"
来源：http://gz.shxzukj.cn

PHP:  public string $name = "x";
来源：http://fc.wgjwhj.cn

JS:   this.name = "x";
来源：http://im.szsharing.cn

TS:   name: string = "x";
来源：http://my.huixinmuqiang.cn

Java: private String name;
来源：http://li.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qb.yuexingan06.cn

Ruby: @name = "x"
来源：http://kg.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://kh.hahajie.cn

[G04] 定义方法
来源：http://kx.9csxet.cn

Py:   def greet(self): return self.name
来源：http://sb.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ox.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://vk.521024.cn

TS:   greet(): string { return this.name; }
来源：http://bh.bjjhwx.cn

Java: String greet() { return name; }
来源：http://ky.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gr.newstarts.cn

Ruby: def greet; @name; end
来源：http://qb.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://ko.huixiangedu.cn

[G05] 继承
来源：http://ec.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://hx.nszjky.cn

PHP:  class Admin extends User {}
来源：http://rw.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://qw.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://bc.wgjwhj.cn

Java: class Admin extends User {}
来源：http://bf.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mv.hahajie.cn

Ruby: class Admin < User; end
来源：http://qe.9csxet.cn

C#:   class Admin : User {}
来源：http://id.szxytkj.cn

[G06] 重写方法
来源：http://nz.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://qp.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ge.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://tn.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://hp.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://vi.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ff.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://lg.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://zn.newstarts.cn

[G07] 调用父类方法
来源：http://nn.shxzukj.cn

Py:   super().greet()
来源：http://pc.colortex.cn

PHP:  parent::greet();
来源：http://mg.szsharing.cn

JS:   super.greet();
来源：http://kp.gzmigu.cn

TS:   super.greet();
来源：http://si.lnxyls.cn

Java: super.greet();
来源：http://sc.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iq.yuntaijiaju.cn

Ruby: super
来源：http://cg.newstarts.cn

C#:   base.Greet();
来源：http://bw.newstarts.cn

[G08] 静态方法与属性
来源：http://kd.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hy.colortex.cn

PHP:  public static function f() {}
来源：http://vl.panjiajie.cn

JS:   static f() {}
来源：http://hi.huanxung.cn

TS:   static f(): void {}
来源：http://nl.szsharing.cn

Java: static void f() {}
来源：http://bg.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xm.nszjky.cn

Ruby: def self.f; end
来源：http://ni.nicolike.cn

C#:   public static void F() {}
来源：http://rl.szsharing.cn

[G09] 接口 / 抽象类
来源：http://wc.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://mw.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vr.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rm.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://zl.9csxet.cn

Java: interface Shape { double area(); }
来源：http://mk.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://mc.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ib.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://ny.haigaiapp.cn

[G10] 访问控制
来源：http://rl.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://tl.bjjhwx.cn

PHP:  public / protected / private
来源：http://ss.newstarts.cn

JS:   #private 字段；其余公开
来源：http://fe.hnjuh.cn

TS:   public / protected / private
来源：http://vc.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://tz.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://er.asd995.cn

Ruby: public / protected / private
来源：http://ge.panjiajie.cn

C#:   public / protected / private / internal
来源：http://dh.bjjhwx.cn

[G11] getter / setter
来源：http://vm.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://ln.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gp.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://ss.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://ou.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://pb.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://is.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://rv.9csxet.cn

C#:   public string Name { get; set; }
来源：http://ls.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://mf.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://gj.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vz.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://ic.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://xv.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://gn.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lx.9csxet.cn

Ruby: def to_s; @name; end
来源：http://wp.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://cw.gzmigu.cn

[G13] 判断对象类型
来源：http://hr.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://ti.yuexingan06.cn

PHP:  $u instanceof User
来源：http://bd.colortex.cn

JS:   u instanceof User
来源：http://jv.chemitech.net.cn

TS:   u instanceof User
来源：http://ty.haigaiapp.cn

Java: u instanceof User
来源：http://cw.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wm.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://xg.huixiangedu.cn

C#:   u is User
来源：http://jd.hnjuh.cn

[G14] 数据类 / record
来源：http://hv.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yl.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://uu.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ze.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://nv.newstarts.cn

Java: record User(String name, int age) {}
来源：http://cu.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://nc.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ed.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://fu.shtwfgs.cn

[G15] 枚举
来源：http://ps.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kl.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bs.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ts.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ip.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://nb.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ve.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://es.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pq.colortex.cn

[G16] 对象转数组 / 字典
来源：http://rk.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cp.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://ia.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://ka.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://tn.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fn.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bj.lnxyls.cn

Ruby: obj.instance_variables
来源：http://vm.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://pt.huixiangedu.cn

================================================================================
来源：http://lc.hahajie.cn

H. 异常与错误处理
来源：http://ed.hnjuh.cn

================================================================================
来源：http://fc.huanxung.cn

[H01] try / catch 基础
来源：http://fv.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tu.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qf.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cc.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mt.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qs.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ey.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://se.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qx.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://yr.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xo.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ra.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wm.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lx.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jz.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zu.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nd.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tw.huanxung.cn

[H03] 主动抛出异常
来源：http://ia.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://ps.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tc.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://pd.asd995.cn

TS:   throw new Error("错误信息");
来源：http://ij.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qd.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ng.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wi.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ra.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://ib.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://ru.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ga.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://yr.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://xo.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://qt.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dt.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ob.521024.cn

C#:   class MyException : Exception {}
来源：http://dk.shxzukj.cn

[H05] 捕获特定类型
来源：http://bc.lnxyls.cn

Py:   except ValueError as e:
来源：http://mh.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nd.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://hi.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://wi.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://wb.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qn.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://uy.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wg.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://zo.asd995.cn

Py:   value = d.get("k") or default
来源：http://xu.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zn.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yn.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ak.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uw.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kj.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://zp.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://vt.shxzskj.cn


<!-- 参考信息 -->