代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wy.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kd.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://pz.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kd.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rs.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jd.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://up.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jn.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nm.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://xd.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ja.muxihuayi.cn

[F04] 追加写入文件
来源：http://ru.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cu.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fe.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eu.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zs.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eo.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gu.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ks.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sz.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://zs.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uf.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://zu.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://np.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://in.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nw.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://va.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://np.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://ch.shtwfgs.cn

[F06] 删除文件
来源：http://mp.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://qa.9csxet.cn

PHP:  unlink("a.txt");
来源：http://vh.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yp.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fq.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mp.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://qx.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://ks.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://dd.nszjky.cn

[F07] 创建目录（含多级）
来源：http://hl.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qu.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ti.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yc.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wt.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zx.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oc.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xx.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://no.hnjuh.cn

[F08] 遍历目录
来源：http://th.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ln.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://su.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://vn.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://sp.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lg.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yj.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://ds.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://rx.lnxyls.cn

[F09] 获取文件大小
来源：http://re.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://ih.asd995.cn

PHP:  filesize("a.txt");
来源：http://iu.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://rf.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://fh.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iv.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fs.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://it.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://yk.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://ix.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://so.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://to.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ei.nicolike.cn

TS:   path.extname("a.txt")
来源：http://yy.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://df.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hb.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jw.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ok.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://ib.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bk.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eh.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mj.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://en.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oq.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gr.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gf.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ms.szsharing.cn

[F12] CSV 读写
来源：http://az.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mp.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gm.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wv.jctech888.com.cn

TS:   // 同上
来源：http://pb.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jr.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tm.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sx.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sr.colortex.cn

================================================================================
来源：http://yr.bookmarksfly.cn

G. 面向对象
来源：http://dc.jianghongdianzi.cn

================================================================================
来源：http://dz.yuexingan06.cn

[G01] 定义类
来源：http://qg.bookmarksfly.cn

Py:   class User: pass
来源：http://bq.9csxet.cn

PHP:  class User {}
来源：http://pz.asd995.cn

JS:   class User {}
来源：http://tq.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://qd.yuntaijiaju.cn

Java: class User {}
来源：http://gm.szxytkj.cn

Go:   type User struct { Name string }
来源：http://wn.nicolike.cn

Ruby: class User; end
来源：http://qg.muxihuayi.cn

C#:   class User {}
来源：http://os.panjiajie.cn

[G02] 构造函数
来源：http://xd.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://es.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://ff.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://rc.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://lm.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://dv.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fe.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://lc.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://zz.hnjuh.cn

[G03] 实例属性
来源：http://px.yuexingan06.cn

Py:   self.name = "x"
来源：http://gj.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://hk.nszjky.cn

JS:   this.name = "x";
来源：http://jo.nicolike.cn

TS:   name: string = "x";
来源：http://fy.jctech888.com.cn

Java: private String name;
来源：http://hm.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ph.shxzskj.cn

Ruby: @name = "x"
来源：http://ye.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://xq.521024.cn

[G04] 定义方法
来源：http://bs.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://lw.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tv.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://mk.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://pd.shxzukj.cn

Java: String greet() { return name; }
来源：http://on.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://no.lnxyls.cn

Ruby: def greet; @name; end
来源：http://hx.hahajie.cn

C#:   public string Greet() => Name;
来源：http://de.nszjky.cn

[G05] 继承
来源：http://qy.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://vx.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://sk.szxytkj.cn

JS:   class Admin extends User {}
来源：http://cd.huanxung.cn

TS:   class Admin extends User {}
来源：http://qz.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ju.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nh.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://tm.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://ov.huanxung.cn

[G06] 重写方法
来源：http://gv.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://gc.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ud.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://sw.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://wc.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ph.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ic.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://nv.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://un.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://im.panjiajie.cn

Py:   super().greet()
来源：http://hl.asd995.cn

PHP:  parent::greet();
来源：http://rs.gzmigu.cn

JS:   super.greet();
来源：http://eu.szxytkj.cn

TS:   super.greet();
来源：http://wo.shxzskj.cn

Java: super.greet();
来源：http://wy.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vc.bookmarksfly.cn

Ruby: super
来源：http://ev.huanxung.cn

C#:   base.Greet();
来源：http://lu.haigaiapp.cn

[G08] 静态方法与属性
来源：http://ih.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rz.yuexingan06.cn

PHP:  public static function f() {}
来源：http://kt.asd995.cn

JS:   static f() {}
来源：http://sr.lnxyls.cn

TS:   static f(): void {}
来源：http://ui.wgjwhj.cn

Java: static void f() {}
来源：http://ig.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rg.shxzukj.cn

Ruby: def self.f; end
来源：http://ow.nszjky.cn

C#:   public static void F() {}
来源：http://db.nszjky.cn

[G09] 接口 / 抽象类
来源：http://wt.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://lr.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mn.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vm.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://cs.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://mp.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://qp.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lj.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://vd.huanxung.cn

[G10] 访问控制
来源：http://fq.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://di.haigaiapp.cn

PHP:  public / protected / private
来源：http://hp.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://fy.huixinmuqiang.cn

TS:   public / protected / private
来源：http://ld.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://pa.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gj.bookmarksfly.cn

Ruby: public / protected / private
来源：http://yb.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://zf.jctech888.com.cn

[G11] getter / setter
来源：http://rb.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://mp.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bw.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ue.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://pr.panjiajie.cn

Java: public String getName() { return name; }
来源：http://sk.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xw.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://ul.521024.cn

C#:   public string Name { get; set; }
来源：http://ep.colortex.cn

[G12] 对象转字符串
来源：http://mf.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://mw.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dl.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://id.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://uj.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://sb.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nv.nicolike.cn

Ruby: def to_s; @name; end
来源：http://ad.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://iu.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://fj.9csxet.cn

Py:   isinstance(u, User)
来源：http://od.9csxet.cn

PHP:  $u instanceof User
来源：http://fv.huixinmuqiang.cn

JS:   u instanceof User
来源：http://rx.bookmarksfly.cn

TS:   u instanceof User
来源：http://ug.yuntaijiaju.cn

Java: u instanceof User
来源：http://uq.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jt.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://sj.jctech888.com.cn

C#:   u is User
来源：http://hb.wgjwhj.cn

[G14] 数据类 / record
来源：http://hh.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://os.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://il.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nt.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://tj.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://sj.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://rf.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ve.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://ug.hahajie.cn

[G15] 枚举
来源：http://yn.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fw.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zq.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hm.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kv.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://kg.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zl.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://rr.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ho.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://bj.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gw.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://ws.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ej.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://fj.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kh.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tt.colortex.cn

Ruby: obj.instance_variables
来源：http://xx.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://hv.szxytkj.cn

================================================================================
来源：http://vu.521024.cn

H. 异常与错误处理
来源：http://cz.huixinmuqiang.cn

================================================================================
来源：http://rt.haigaiapp.cn

[H01] try / catch 基础
来源：http://kj.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ri.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jx.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vb.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rt.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fu.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ps.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dv.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dw.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://ae.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ec.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fh.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gl.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sy.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bq.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ji.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ro.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zm.szsharing.cn

[H03] 主动抛出异常
来源：http://dj.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://lc.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ya.asd995.cn

JS:   throw new Error("错误信息");
来源：http://mo.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://cc.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ox.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wm.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xp.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fd.chemitech.net.cn

[H04] 自定义异常类型
来源：http://kt.asd995.cn

Py:   class MyError(Exception): pass
来源：http://nj.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xq.huanxung.cn

JS:   class MyError extends Error {}
来源：http://is.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://mk.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://uh.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nh.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://ty.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://mj.huixiangedu.cn

[H05] 捕获特定类型
来源：http://ko.szxytkj.cn

Py:   except ValueError as e:
来源：http://sy.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uo.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://xy.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://tv.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://yq.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://en.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://fw.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qt.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://ae.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://tx.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://az.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kb.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vh.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sd.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hf.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://do.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://ve.asd995.cn

[H07] 断言
来源：http://is.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://gv.shxzukj.cn

PHP:  assert($x > 0);
来源：http://sh.newstarts.cn

JS:   console.assert(x > 0);
来源：http://kf.wgjwhj.cn


<!-- 参考信息 -->