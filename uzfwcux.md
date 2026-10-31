代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vi.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://to.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://lp.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sk.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sd.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zx.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jd.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://at.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wd.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ja.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mp.shxzskj.cn

[F04] 追加写入文件
来源：http://pu.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dg.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xo.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qe.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qa.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qw.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ou.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ue.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ij.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://gi.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vh.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://gh.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://uj.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ip.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jd.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wm.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://du.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://ib.hahajie.cn

[F06] 删除文件
来源：http://po.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://gu.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://xg.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sz.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dk.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gd.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://uu.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://mr.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://us.colortex.cn

[F07] 创建目录（含多级）
来源：http://ra.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fz.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bm.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xd.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zq.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dv.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ux.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://on.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gz.9csxet.cn

[F08] 遍历目录
来源：http://il.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tp.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gs.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://jv.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://wk.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wq.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qx.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://oh.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://is.wgjwhj.cn

[F09] 获取文件大小
来源：http://sm.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://qn.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://fd.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://at.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://or.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xz.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qi.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://gk.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://lb.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://nm.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://an.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qj.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ym.colortex.cn

TS:   path.extname("a.txt")
来源：http://cs.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gm.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cq.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oo.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tq.jctech888.com.cn

[F11] 复制与移动文件
来源：http://pp.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xr.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xs.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ck.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vm.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rb.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ph.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hl.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hb.shxzskj.cn

[F12] CSV 读写
来源：http://ns.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://da.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aj.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vp.newstarts.cn

TS:   // 同上
来源：http://nk.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://an.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eb.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mk.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mq.jianghongdianzi.cn

================================================================================
来源：http://ge.newstarts.cn

G. 面向对象
来源：http://ce.szxytkj.cn

================================================================================
来源：http://kr.huanxung.cn

[G01] 定义类
来源：http://vt.yuntaijiaju.cn

Py:   class User: pass
来源：http://ma.szxytkj.cn

PHP:  class User {}
来源：http://ll.bjjhwx.cn

JS:   class User {}
来源：http://mm.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://rl.newstarts.cn

Java: class User {}
来源：http://ni.colortex.cn

Go:   type User struct { Name string }
来源：http://lr.haigaiapp.cn

Ruby: class User; end
来源：http://jb.hahajie.cn

C#:   class User {}
来源：http://ji.nicolike.cn

[G02] 构造函数
来源：http://ej.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://gq.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://uf.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://vm.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://va.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://bh.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mf.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://wi.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://iz.szsharing.cn

[G03] 实例属性
来源：http://em.huanxung.cn

Py:   self.name = "x"
来源：http://vn.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://ub.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://xu.lnxyls.cn

TS:   name: string = "x";
来源：http://sk.shxzskj.cn

Java: private String name;
来源：http://pa.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aa.asd995.cn

Ruby: @name = "x"
来源：http://nn.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://mb.asd995.cn

[G04] 定义方法
来源：http://qc.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://js.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nt.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://eh.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://kw.colortex.cn

Java: String greet() { return name; }
来源：http://ar.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fy.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://db.szsharing.cn

C#:   public string Greet() => Name;
来源：http://qa.newstarts.cn

[G05] 继承
来源：http://so.szxytkj.cn

Py:   class Admin(User): pass
来源：http://em.szsharing.cn

PHP:  class Admin extends User {}
来源：http://lz.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://eo.colortex.cn

TS:   class Admin extends User {}
来源：http://tk.wgjwhj.cn

Java: class Admin extends User {}
来源：http://je.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zt.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://be.hahajie.cn

C#:   class Admin : User {}
来源：http://iv.asd995.cn

[G06] 重写方法
来源：http://vx.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://zk.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tx.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://ol.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://kr.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://hv.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hh.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://ya.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://po.panjiajie.cn

[G07] 调用父类方法
来源：http://ld.521024.cn

Py:   super().greet()
来源：http://gk.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://ey.nszjky.cn

JS:   super.greet();
来源：http://wz.panjiajie.cn

TS:   super.greet();
来源：http://lx.chemitech.net.cn

Java: super.greet();
来源：http://ll.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mi.bjjhwx.cn

Ruby: super
来源：http://bf.szxytkj.cn

C#:   base.Greet();
来源：http://hd.shxzskj.cn

[G08] 静态方法与属性
来源：http://dh.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lc.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://rp.nszjky.cn

JS:   static f() {}
来源：http://yi.bookmarksfly.cn

TS:   static f(): void {}
来源：http://wq.521024.cn

Java: static void f() {}
来源：http://cz.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eb.hahajie.cn

Ruby: def self.f; end
来源：http://rq.colortex.cn

C#:   public static void F() {}
来源：http://lx.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://ux.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://kx.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bz.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pn.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://da.asd995.cn

Java: interface Shape { double area(); }
来源：http://kc.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://nv.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zw.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://le.chemitech.net.cn

[G10] 访问控制
来源：http://lt.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://uy.szsharing.cn

PHP:  public / protected / private
来源：http://if.szsharing.cn

JS:   #private 字段；其余公开
来源：http://fv.9csxet.cn

TS:   public / protected / private
来源：http://mu.521024.cn

Java: public / protected / private / 默认包级
来源：http://rc.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mv.asd995.cn

Ruby: public / protected / private
来源：http://eo.9csxet.cn

C#:   public / protected / private / internal
来源：http://uk.yuexingan06.cn

[G11] getter / setter
来源：http://jg.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://tu.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rc.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://fu.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://zb.hahajie.cn

Java: public String getName() { return name; }
来源：http://xp.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bz.shxzskj.cn

Ruby: attr_accessor :name
来源：http://xo.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://nw.huixiangedu.cn

[G12] 对象转字符串
来源：http://nz.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://cl.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://br.newstarts.cn

JS:   toString() { return this.name; }
来源：http://lx.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://wl.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://tc.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wb.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://dv.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://sv.nszjky.cn

[G13] 判断对象类型
来源：http://gh.newstarts.cn

Py:   isinstance(u, User)
来源：http://jz.gzmigu.cn

PHP:  $u instanceof User
来源：http://tc.wgjwhj.cn

JS:   u instanceof User
来源：http://gl.szsharing.cn

TS:   u instanceof User
来源：http://kr.bookmarksfly.cn

Java: u instanceof User
来源：http://pq.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bt.hahajie.cn

Ruby: u.is_a?(User)
来源：http://uf.hahajie.cn

C#:   u is User
来源：http://cl.muxihuayi.cn

[G14] 数据类 / record
来源：http://fl.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fe.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://pm.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ks.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://cn.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://wm.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://zc.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mp.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://xa.shxzukj.cn

[G15] 枚举
来源：http://lr.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://id.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cc.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iq.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wn.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://aw.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lr.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://jd.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aw.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://qp.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://is.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://xq.newstarts.cn

JS:   Object.entries(obj)
来源：http://lq.szxytkj.cn

TS:   Object.entries(obj)
来源：http://un.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://us.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://st.hahajie.cn

Ruby: obj.instance_variables
来源：http://st.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://jo.shtwfgs.cn

================================================================================
来源：http://ao.newstarts.cn

H. 异常与错误处理
来源：http://tm.gzmigu.cn

================================================================================
来源：http://zc.nszjky.cn

[H01] try / catch 基础
来源：http://lb.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bq.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wj.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://is.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://he.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qd.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xl.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eh.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jp.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://lc.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zm.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mi.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ig.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dq.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cz.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hg.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ea.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jl.newstarts.cn

[H03] 主动抛出异常
来源：http://bh.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://iv.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xs.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://no.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://bq.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gp.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ao.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cy.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mi.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://go.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://mh.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ws.nicolike.cn

JS:   class MyError extends Error {}
来源：http://dw.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://oq.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://kj.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pw.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://jj.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://gv.shxzukj.cn

[H05] 捕获特定类型
来源：http://fk.asd995.cn

Py:   except ValueError as e:
来源：http://zy.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://le.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://bm.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://je.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://nx.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ou.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://sw.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ep.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://kf.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://nf.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sq.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ba.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hq.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ol.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://op.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ik.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://lc.chemitech.net.cn

[H07] 断言
来源：http://ou.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://yc.huanxung.cn

PHP:  assert($x > 0);
来源：http://nt.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://gw.jianghongdianzi.cn


<!-- 参考信息 -->