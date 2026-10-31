代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hu.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sg.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gl.hahajie.cn

Ruby: File.read("a.txt")
来源：http://cr.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://hd.shxzskj.cn

[F02] 逐行读取文件
来源：http://lg.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tz.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gx.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oy.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xf.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qn.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://it.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qy.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fx.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://is.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ln.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ao.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aa.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bt.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cu.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qk.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://oy.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mz.yuexingan06.cn

[F04] 追加写入文件
来源：http://kd.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yb.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ww.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mz.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jk.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qe.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mx.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fw.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://da.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://nh.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gr.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://at.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://hf.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://jx.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gm.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ex.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://sz.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://lh.yuntaijiaju.cn

[F06] 删除文件
来源：http://uj.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://yk.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://mg.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jj.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pd.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ky.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://as.asd995.cn

Ruby: File.delete("a.txt")
来源：http://yy.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ck.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://zr.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jd.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jq.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cx.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xk.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pj.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xz.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ud.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tr.521024.cn

[F08] 遍历目录
来源：http://xj.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rd.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xl.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://ob.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://xn.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ej.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bo.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://qe.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://uk.szxytkj.cn

[F09] 获取文件大小
来源：http://au.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://po.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://kc.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://py.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://cj.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qs.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mj.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://nn.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://xy.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://cg.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kg.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://po.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bb.hahajie.cn

TS:   path.extname("a.txt")
来源：http://jk.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mu.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cg.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iy.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ep.szxytkj.cn

[F11] 复制与移动文件
来源：http://uv.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lp.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dz.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cg.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qm.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fq.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bb.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ts.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vg.colortex.cn

[F12] CSV 读写
来源：http://rf.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tm.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kz.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://es.huixiangedu.cn

TS:   // 同上
来源：http://bp.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ye.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dw.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zf.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ui.hahajie.cn

================================================================================
来源：http://xf.lnxyls.cn

G. 面向对象
来源：http://rd.yuexingan06.cn

================================================================================
来源：http://nk.hahajie.cn

[G01] 定义类
来源：http://up.yuntaijiaju.cn

Py:   class User: pass
来源：http://ru.yuntaijiaju.cn

PHP:  class User {}
来源：http://vq.colortex.cn

JS:   class User {}
来源：http://up.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://kg.colortex.cn

Java: class User {}
来源：http://yd.hahajie.cn

Go:   type User struct { Name string }
来源：http://wh.hnjuh.cn

Ruby: class User; end
来源：http://kz.jianghongdianzi.cn

C#:   class User {}
来源：http://jm.asd995.cn

[G02] 构造函数
来源：http://zn.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://ip.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ps.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://ag.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://le.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://vz.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ae.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://xd.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://me.nicolike.cn

[G03] 实例属性
来源：http://ic.chemitech.net.cn

Py:   self.name = "x"
来源：http://kn.hahajie.cn

PHP:  public string $name = "x";
来源：http://ls.lnxyls.cn

JS:   this.name = "x";
来源：http://jh.chemitech.net.cn

TS:   name: string = "x";
来源：http://ed.jianghongdianzi.cn

Java: private String name;
来源：http://ty.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ak.panjiajie.cn

Ruby: @name = "x"
来源：http://qs.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://xe.bjjhwx.cn

[G04] 定义方法
来源：http://nk.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://do.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tn.newstarts.cn

JS:   greet() { return this.name; }
来源：http://xd.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://wn.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://xi.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://as.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://qr.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://ry.huixinmuqiang.cn

[G05] 继承
来源：http://na.shxzukj.cn

Py:   class Admin(User): pass
来源：http://bn.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://dn.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://zt.huanxung.cn

TS:   class Admin extends User {}
来源：http://kk.newstarts.cn

Java: class Admin extends User {}
来源：http://qq.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nq.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://zr.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://ug.chemitech.net.cn

[G06] 重写方法
来源：http://fm.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://bv.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://it.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ql.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://ld.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://el.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wg.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://ld.521024.cn

C#:   public override string Greet() => "admin";
来源：http://tq.shxzskj.cn

[G07] 调用父类方法
来源：http://cg.asd995.cn

Py:   super().greet()
来源：http://hg.bjjhwx.cn

PHP:  parent::greet();
来源：http://xq.szsharing.cn

JS:   super.greet();
来源：http://gv.yuntaijiaju.cn

TS:   super.greet();
来源：http://mp.gzmigu.cn

Java: super.greet();
来源：http://db.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tw.newstarts.cn

Ruby: super
来源：http://hf.lnxyls.cn

C#:   base.Greet();
来源：http://vl.nicolike.cn

[G08] 静态方法与属性
来源：http://xa.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ap.521024.cn

PHP:  public static function f() {}
来源：http://vd.shxzukj.cn

JS:   static f() {}
来源：http://zd.shxzskj.cn

TS:   static f(): void {}
来源：http://da.jianghongdianzi.cn

Java: static void f() {}
来源：http://vj.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ww.lnxyls.cn

Ruby: def self.f; end
来源：http://ly.haigaiapp.cn

C#:   public static void F() {}
来源：http://dp.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://pu.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://in.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jj.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sr.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://hq.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://oc.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://ii.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yq.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://yb.chemitech.net.cn

[G10] 访问控制
来源：http://do.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://vs.lnxyls.cn

PHP:  public / protected / private
来源：http://mx.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://pz.bjjhwx.cn

TS:   public / protected / private
来源：http://qf.asd995.cn

Java: public / protected / private / 默认包级
来源：http://go.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tw.hnjuh.cn

Ruby: public / protected / private
来源：http://uq.newstarts.cn

C#:   public / protected / private / internal
来源：http://tf.bookmarksfly.cn

[G11] getter / setter
来源：http://yb.asd995.cn

Py:   @property 与 @x.setter
来源：http://wo.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wy.colortex.cn

JS:   get name() { return this._name; }
来源：http://de.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://rl.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://bv.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jv.lnxyls.cn

Ruby: attr_accessor :name
来源：http://my.9csxet.cn

C#:   public string Name { get; set; }
来源：http://qc.shxzukj.cn

[G12] 对象转字符串
来源：http://ek.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://ac.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lj.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://qn.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://ab.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://ud.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lq.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://du.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://kz.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://ws.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://gs.asd995.cn

PHP:  $u instanceof User
来源：http://eg.shtwfgs.cn

JS:   u instanceof User
来源：http://se.chemitech.net.cn

TS:   u instanceof User
来源：http://aw.shxzukj.cn

Java: u instanceof User
来源：http://vx.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hs.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://vi.bjjhwx.cn

C#:   u is User
来源：http://qf.shxzskj.cn

[G14] 数据类 / record
来源：http://eh.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ru.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://hz.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vj.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://be.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://iz.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://lg.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ug.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://cr.yuntaijiaju.cn

[G15] 枚举
来源：http://lv.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sa.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://su.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cn.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dp.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://xs.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rb.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://fq.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ly.521024.cn

[G16] 对象转数组 / 字典
来源：http://dq.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://du.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://xh.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://wa.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://hf.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zr.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bs.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://ag.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://yi.jctech888.com.cn

================================================================================
来源：http://eu.hnjuh.cn

H. 异常与错误处理
来源：http://hd.huixinmuqiang.cn

================================================================================
来源：http://ur.nicolike.cn

[H01] try / catch 基础
来源：http://hf.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pc.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wv.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ec.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hr.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ks.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nm.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lq.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pz.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://jf.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://np.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tu.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dj.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tr.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vp.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://au.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eu.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sm.9csxet.cn

[H03] 主动抛出异常
来源：http://df.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://sf.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oq.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ih.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://nk.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jg.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tu.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dv.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ii.9csxet.cn

[H04] 自定义异常类型
来源：http://gm.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://tg.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vt.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://qh.colortex.cn

TS:   class MyError extends Error {}
来源：http://ha.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://dp.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xo.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://lw.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://px.muxihuayi.cn

[H05] 捕获特定类型
来源：http://xd.panjiajie.cn

Py:   except ValueError as e:
来源：http://xk.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hk.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://yp.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://hq.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://wm.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://um.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://gh.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nt.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://nk.jctech888.com.cn


<!-- 参考信息 -->