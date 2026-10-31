代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sq.9csxet.cn

================================================================================
来源：http://br.yuexingan06.cn

F. 文件与目录
来源：http://ln.haigaiapp.cn

================================================================================
来源：http://st.chemitech.net.cn

[F01] 读取整个文件
来源：http://zu.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pb.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://re.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jd.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gu.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ku.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://np.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://mr.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://ax.huixiangedu.cn

[F02] 逐行读取文件
来源：http://mb.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sa.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mj.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bp.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wo.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sz.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://td.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://es.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cs.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://zr.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xj.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ia.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qo.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pg.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rb.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nq.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://la.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cm.huixiangedu.cn

[F04] 追加写入文件
来源：http://us.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yz.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tf.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fa.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ya.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cq.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cc.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oj.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ew.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://wu.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xy.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://rl.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://jx.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://al.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ey.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://on.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://mx.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://ly.huixiangedu.cn

[F06] 删除文件
来源：http://om.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://sm.asd995.cn

PHP:  unlink("a.txt");
来源：http://hb.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gm.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vt.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://my.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://hh.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://tm.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://rs.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://eu.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ct.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qg.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aq.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bl.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gz.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://su.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ux.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cg.huixiangedu.cn

[F08] 遍历目录
来源：http://at.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://we.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wg.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://wn.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://af.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rl.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qb.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://xg.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://df.shxzskj.cn

[F09] 获取文件大小
来源：http://oo.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://li.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://zb.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://ec.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://ec.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rg.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wi.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://jl.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://wf.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://kw.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kl.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://da.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rm.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://dn.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nv.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dm.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qx.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cf.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://ty.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xz.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ig.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wb.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gu.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kj.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rj.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vp.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kf.yuexingan06.cn

[F12] CSV 读写
来源：http://ye.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hj.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hp.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tb.chemitech.net.cn

TS:   // 同上
来源：http://iv.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ug.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rq.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cz.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nf.9csxet.cn

================================================================================
来源：http://hx.nicolike.cn

G. 面向对象
来源：http://ou.nszjky.cn

================================================================================
来源：http://ws.wgjwhj.cn

[G01] 定义类
来源：http://aq.huanxung.cn

Py:   class User: pass
来源：http://bt.lnxyls.cn

PHP:  class User {}
来源：http://ms.bookmarksfly.cn

JS:   class User {}
来源：http://yu.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://xf.chemitech.net.cn

Java: class User {}
来源：http://ed.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://yt.jianghongdianzi.cn

Ruby: class User; end
来源：http://hj.nicolike.cn

C#:   class User {}
来源：http://ow.asd995.cn

[G02] 构造函数
来源：http://kp.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://ns.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ta.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://ts.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://py.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://up.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ju.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://nt.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://ti.huanxung.cn

[G03] 实例属性
来源：http://hz.hahajie.cn

Py:   self.name = "x"
来源：http://hq.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://ov.gzmigu.cn

JS:   this.name = "x";
来源：http://iu.jctech888.com.cn

TS:   name: string = "x";
来源：http://qq.jctech888.com.cn

Java: private String name;
来源：http://pb.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ud.lnxyls.cn

Ruby: @name = "x"
来源：http://og.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://ri.yuexingan06.cn

[G04] 定义方法
来源：http://ag.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://zk.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yr.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://yh.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://ue.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://yx.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ux.huanxung.cn

Ruby: def greet; @name; end
来源：http://ro.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://he.nszjky.cn

[G05] 继承
来源：http://sn.hahajie.cn

Py:   class Admin(User): pass
来源：http://ct.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://nr.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://nw.panjiajie.cn

TS:   class Admin extends User {}
来源：http://fm.nszjky.cn

Java: class Admin extends User {}
来源：http://ld.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kt.hnjuh.cn

Ruby: class Admin < User; end
来源：http://vr.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://en.haigaiapp.cn

[G06] 重写方法
来源：http://cz.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ex.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tf.asd995.cn

JS:   greet() { return "admin"; }
来源：http://on.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://be.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://uc.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qj.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://yp.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://au.nicolike.cn

[G07] 调用父类方法
来源：http://ex.szsharing.cn

Py:   super().greet()
来源：http://pb.gzmigu.cn

PHP:  parent::greet();
来源：http://fl.asd995.cn

JS:   super.greet();
来源：http://rb.nszjky.cn

TS:   super.greet();
来源：http://id.wgjwhj.cn

Java: super.greet();
来源：http://oo.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iw.521024.cn

Ruby: super
来源：http://ix.szsharing.cn

C#:   base.Greet();
来源：http://ym.colortex.cn

[G08] 静态方法与属性
来源：http://wm.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mq.haigaiapp.cn

PHP:  public static function f() {}
来源：http://zo.shxzskj.cn

JS:   static f() {}
来源：http://ad.nicolike.cn

TS:   static f(): void {}
来源：http://pn.szsharing.cn

Java: static void f() {}
来源：http://hj.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nx.jctech888.com.cn

Ruby: def self.f; end
来源：http://sl.hahajie.cn

C#:   public static void F() {}
来源：http://mc.szsharing.cn

[G09] 接口 / 抽象类
来源：http://ys.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://vp.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ib.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ga.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://cb.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://dl.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://jx.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zh.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://vv.huixinmuqiang.cn

[G10] 访问控制
来源：http://nf.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://wm.gzmigu.cn

PHP:  public / protected / private
来源：http://kl.huanxung.cn

JS:   #private 字段；其余公开
来源：http://qk.shxzukj.cn

TS:   public / protected / private
来源：http://fq.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://dw.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fy.bookmarksfly.cn

Ruby: public / protected / private
来源：http://ij.hahajie.cn

C#:   public / protected / private / internal
来源：http://li.gzmigu.cn

[G11] getter / setter
来源：http://mb.newstarts.cn

Py:   @property 与 @x.setter
来源：http://py.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rq.colortex.cn

JS:   get name() { return this._name; }
来源：http://ed.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://uj.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://ou.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ju.nszjky.cn

Ruby: attr_accessor :name
来源：http://jn.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://py.gzmigu.cn

[G12] 对象转字符串
来源：http://ev.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://dj.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fd.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://wq.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://gz.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://ml.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hr.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://jq.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://es.szxytkj.cn

[G13] 判断对象类型
来源：http://iz.colortex.cn

Py:   isinstance(u, User)
来源：http://vk.shtwfgs.cn

PHP:  $u instanceof User
来源：http://kh.jctech888.com.cn

JS:   u instanceof User
来源：http://mv.nszjky.cn

TS:   u instanceof User
来源：http://ax.szsharing.cn

Java: u instanceof User
来源：http://kd.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pe.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://vt.huixiangedu.cn

C#:   u is User
来源：http://ef.shxzskj.cn

[G14] 数据类 / record
来源：http://oy.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://li.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://kj.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uq.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://sd.nszjky.cn

Java: record User(String name, int age) {}
来源：http://lf.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://dj.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ei.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://st.panjiajie.cn

[G15] 枚举
来源：http://dx.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://at.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://op.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zo.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cr.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://zm.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ll.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://qz.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ou.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://gr.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sh.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://rv.nszjky.cn

JS:   Object.entries(obj)
来源：http://lv.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://sr.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ju.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yu.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://za.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://fh.gzmigu.cn

================================================================================
来源：http://qz.colortex.cn

H. 异常与错误处理
来源：http://sg.jianghongdianzi.cn

================================================================================
来源：http://lj.shtwfgs.cn

[H01] try / catch 基础
来源：http://tq.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gy.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xs.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uj.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mm.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tj.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jg.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zo.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://un.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ys.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qz.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://af.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://su.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vj.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://be.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jn.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://is.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qw.colortex.cn

[H03] 主动抛出异常
来源：http://hm.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://gr.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vd.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://gc.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://vh.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vx.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jv.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nw.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lh.shxzskj.cn

[H04] 自定义异常类型
来源：http://ak.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://fd.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ww.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://yp.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ml.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://eo.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://us.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://vj.szsharing.cn

C#:   class MyException : Exception {}
来源：http://zg.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://zn.gzmigu.cn

Py:   except ValueError as e:
来源：http://fi.bjjhwx.cn


<!-- 参考信息 -->