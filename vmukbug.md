代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rm.haigaiapp.cn

================================================================================
来源：http://pe.huixiangedu.cn

F. 文件与目录
来源：http://rq.shtwfgs.cn

================================================================================
来源：http://eg.huanxung.cn

[F01] 读取整个文件
来源：http://gz.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jr.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://oh.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nb.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fs.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ig.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bt.hahajie.cn

Ruby: File.read("a.txt")
来源：http://rg.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://xr.newstarts.cn

[F02] 逐行读取文件
来源：http://eo.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dl.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://st.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hv.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ad.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ph.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vt.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rb.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ov.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://bt.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qb.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nt.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ot.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cm.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fg.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kz.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ue.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zn.hahajie.cn

[F04] 追加写入文件
来源：http://lj.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rf.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xz.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nh.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zb.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ie.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ch.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://po.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gk.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://sm.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gs.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://tk.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ct.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://in.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ww.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sz.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://vk.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://nl.gzmigu.cn

[F06] 删除文件
来源：http://jv.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://dd.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://xn.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://df.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jh.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gq.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://rc.521024.cn

Ruby: File.delete("a.txt")
来源：http://ly.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://rd.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://ex.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fp.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qt.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cm.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cm.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ic.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kr.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://us.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qp.lnxyls.cn

[F08] 遍历目录
来源：http://ri.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://me.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rh.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://ga.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://jg.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ph.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zd.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://vf.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://bf.muxihuayi.cn

[F09] 获取文件大小
来源：http://cj.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://yh.newstarts.cn

PHP:  filesize("a.txt");
来源：http://hr.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://if.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://ja.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xi.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mc.nicolike.cn

Ruby: File.size("a.txt")
来源：http://nd.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://bf.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://yn.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tj.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ai.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://at.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://jh.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zs.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yt.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cy.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ab.wgjwhj.cn

[F11] 复制与移动文件
来源：http://vt.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tl.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ia.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ce.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eh.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qr.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lb.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uk.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bk.lnxyls.cn

[F12] CSV 读写
来源：http://wu.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wr.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ks.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qc.nicolike.cn

TS:   // 同上
来源：http://ne.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cs.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mf.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://do.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yc.shxzskj.cn

================================================================================
来源：http://tx.yuexingan06.cn

G. 面向对象
来源：http://dj.szxytkj.cn

================================================================================
来源：http://td.hnjuh.cn

[G01] 定义类
来源：http://gt.lnxyls.cn

Py:   class User: pass
来源：http://zt.huixiangedu.cn

PHP:  class User {}
来源：http://zy.jctech888.com.cn

JS:   class User {}
来源：http://rp.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://hc.huixiangedu.cn

Java: class User {}
来源：http://fz.colortex.cn

Go:   type User struct { Name string }
来源：http://ah.panjiajie.cn

Ruby: class User; end
来源：http://vq.nszjky.cn

C#:   class User {}
来源：http://hx.huanxung.cn

[G02] 构造函数
来源：http://wl.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://fg.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://in.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://su.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://be.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://pf.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pi.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://vg.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://ag.szxytkj.cn

[G03] 实例属性
来源：http://gw.huanxung.cn

Py:   self.name = "x"
来源：http://mg.asd995.cn

PHP:  public string $name = "x";
来源：http://ua.521024.cn

JS:   this.name = "x";
来源：http://bd.shxzskj.cn

TS:   name: string = "x";
来源：http://ha.hnjuh.cn

Java: private String name;
来源：http://ws.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rd.newstarts.cn

Ruby: @name = "x"
来源：http://or.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://tw.9csxet.cn

[G04] 定义方法
来源：http://yq.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://wj.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iv.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://ot.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://wn.haigaiapp.cn

Java: String greet() { return name; }
来源：http://kt.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mm.panjiajie.cn

Ruby: def greet; @name; end
来源：http://qo.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://mq.szxytkj.cn

[G05] 继承
来源：http://wn.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://hb.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://eg.nicolike.cn

JS:   class Admin extends User {}
来源：http://zi.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://ht.muxihuayi.cn

Java: class Admin extends User {}
来源：http://zt.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wb.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://uq.chemitech.net.cn

C#:   class Admin : User {}
来源：http://km.haigaiapp.cn

[G06] 重写方法
来源：http://sj.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://ca.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zj.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://tu.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://vg.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://vz.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pd.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://mo.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ed.haigaiapp.cn

[G07] 调用父类方法
来源：http://ls.bjjhwx.cn

Py:   super().greet()
来源：http://xu.gzmigu.cn

PHP:  parent::greet();
来源：http://vq.yuexingan06.cn

JS:   super.greet();
来源：http://eq.hnjuh.cn

TS:   super.greet();
来源：http://kl.yuexingan06.cn

Java: super.greet();
来源：http://cb.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fo.chemitech.net.cn

Ruby: super
来源：http://qg.hnjuh.cn

C#:   base.Greet();
来源：http://pr.521024.cn

[G08] 静态方法与属性
来源：http://wr.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qh.muxihuayi.cn

PHP:  public static function f() {}
来源：http://md.wgjwhj.cn

JS:   static f() {}
来源：http://dz.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://oi.yuexingan06.cn

Java: static void f() {}
来源：http://vk.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zq.lnxyls.cn

Ruby: def self.f; end
来源：http://tz.huixiangedu.cn

C#:   public static void F() {}
来源：http://rn.huanxung.cn

[G09] 接口 / 抽象类
来源：http://em.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://yi.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kz.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wt.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://fv.colortex.cn

Java: interface Shape { double area(); }
来源：http://lf.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://mm.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xq.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://md.wgjwhj.cn

[G10] 访问控制
来源：http://wi.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://uu.nszjky.cn

PHP:  public / protected / private
来源：http://se.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://pa.szxytkj.cn

TS:   public / protected / private
来源：http://lp.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://tl.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jg.shxzskj.cn

Ruby: public / protected / private
来源：http://fu.szsharing.cn

C#:   public / protected / private / internal
来源：http://tq.asd995.cn

[G11] getter / setter
来源：http://cn.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://ha.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vi.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://mv.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://lp.szxytkj.cn

Java: public String getName() { return name; }
来源：http://jo.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hi.asd995.cn

Ruby: attr_accessor :name
来源：http://zi.9csxet.cn

C#:   public string Name { get; set; }
来源：http://jn.9csxet.cn

[G12] 对象转字符串
来源：http://qv.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://ct.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wr.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://ey.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://zf.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://jd.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ip.asd995.cn

Ruby: def to_s; @name; end
来源：http://gp.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://xi.shxzskj.cn

[G13] 判断对象类型
来源：http://hg.shxzskj.cn

Py:   isinstance(u, User)
来源：http://ce.wgjwhj.cn

PHP:  $u instanceof User
来源：http://gb.szsharing.cn

JS:   u instanceof User
来源：http://go.asd995.cn

TS:   u instanceof User
来源：http://gr.lnxyls.cn

Java: u instanceof User
来源：http://wm.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wk.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://fn.newstarts.cn

C#:   u is User
来源：http://xt.nszjky.cn

[G14] 数据类 / record
来源：http://go.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://io.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://wb.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fu.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://db.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://pr.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://rx.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qh.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://mn.szxytkj.cn

[G15] 枚举
来源：http://jp.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yy.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sw.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kb.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hy.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://ek.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bx.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://sy.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mm.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://xv.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pt.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://fx.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://eo.hnjuh.cn

TS:   Object.entries(obj)
来源：http://eh.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zt.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rx.hnjuh.cn

Ruby: obj.instance_variables
来源：http://io.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://xq.shxzskj.cn

================================================================================
来源：http://qe.shxzskj.cn

H. 异常与错误处理
来源：http://mp.asd995.cn

================================================================================
来源：http://pp.9csxet.cn

[H01] try / catch 基础
来源：http://un.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vi.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wc.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ag.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ot.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sy.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yz.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hh.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ci.huanxung.cn

[H02] finally / ensure 收尾
来源：http://my.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aw.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pe.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qm.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ce.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qn.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uy.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mm.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sv.haigaiapp.cn

[H03] 主动抛出异常
来源：http://vs.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://ag.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iy.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://pn.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://gf.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ot.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jn.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xi.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wq.521024.cn

[H04] 自定义异常类型
来源：http://rd.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://ih.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fq.nszjky.cn

JS:   class MyError extends Error {}
来源：http://ug.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://qo.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://sp.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://md.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://iw.huanxung.cn

C#:   class MyException : Exception {}
来源：http://jp.521024.cn

[H05] 捕获特定类型
来源：http://wh.huanxung.cn

Py:   except ValueError as e:
来源：http://au.hnjuh.cn


<!-- 参考信息 -->