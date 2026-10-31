代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sc.huixinmuqiang.cn

================================================================================
来源：http://ba.newstarts.cn

F. 文件与目录
来源：http://zg.gzmigu.cn

================================================================================
来源：http://wu.huanxung.cn

[F01] 读取整个文件
来源：http://bn.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fg.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://aq.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://li.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lf.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uy.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ar.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://kb.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://dn.nszjky.cn

[F02] 逐行读取文件
来源：http://uo.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fe.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hf.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xl.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ho.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gz.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aw.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qs.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ug.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ja.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hp.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dn.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ys.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ri.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yt.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ha.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://wo.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sj.9csxet.cn

[F04] 追加写入文件
来源：http://ux.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wc.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ii.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mq.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ak.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yb.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gc.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lz.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yo.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://jr.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pc.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://ax.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://gu.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://rg.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hs.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bu.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://st.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://fh.bookmarksfly.cn

[F06] 删除文件
来源：http://xy.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://ii.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://pj.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tc.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://km.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vx.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://eq.asd995.cn

Ruby: File.delete("a.txt")
来源：http://ph.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://pm.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://wq.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qh.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zn.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tj.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yf.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dy.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://iq.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cv.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ip.nicolike.cn

[F08] 遍历目录
来源：http://sm.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zp.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ek.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://uw.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://tn.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wi.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gf.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://yk.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://by.chemitech.net.cn

[F09] 获取文件大小
来源：http://tw.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ux.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://tl.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://do.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://or.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vz.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zz.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://dh.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://hr.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://dc.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vl.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://si.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kq.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://id.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ef.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kt.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ea.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dx.haigaiapp.cn

[F11] 复制与移动文件
来源：http://nl.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aw.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://au.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://on.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ae.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cs.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lf.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fa.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fp.shxzukj.cn

[F12] CSV 读写
来源：http://kw.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sc.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://at.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uj.hnjuh.cn

TS:   // 同上
来源：http://zw.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gg.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mf.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fl.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vu.shxzukj.cn

================================================================================
来源：http://of.chemitech.net.cn

G. 面向对象
来源：http://dt.bookmarksfly.cn

================================================================================
来源：http://ph.szsharing.cn

[G01] 定义类
来源：http://tf.521024.cn

Py:   class User: pass
来源：http://nn.szxytkj.cn

PHP:  class User {}
来源：http://qx.newstarts.cn

JS:   class User {}
来源：http://je.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://pp.haigaiapp.cn

Java: class User {}
来源：http://fv.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://pn.shtwfgs.cn

Ruby: class User; end
来源：http://lv.shxzskj.cn

C#:   class User {}
来源：http://ce.jianghongdianzi.cn

[G02] 构造函数
来源：http://wp.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://ot.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ds.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://ht.asd995.cn

TS:   constructor(public name: string) {}
来源：http://ht.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://om.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yv.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://zj.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://kc.9csxet.cn

[G03] 实例属性
来源：http://xf.newstarts.cn

Py:   self.name = "x"
来源：http://hj.gzmigu.cn

PHP:  public string $name = "x";
来源：http://gg.lnxyls.cn

JS:   this.name = "x";
来源：http://uv.chemitech.net.cn

TS:   name: string = "x";
来源：http://tk.wgjwhj.cn

Java: private String name;
来源：http://cn.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rj.asd995.cn

Ruby: @name = "x"
来源：http://nl.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://zl.jctech888.com.cn

[G04] 定义方法
来源：http://gw.hahajie.cn

Py:   def greet(self): return self.name
来源：http://kn.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ri.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://rd.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://ya.huanxung.cn

Java: String greet() { return name; }
来源：http://vq.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wc.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://ky.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://fi.jctech888.com.cn

[G05] 继承
来源：http://zd.hahajie.cn

Py:   class Admin(User): pass
来源：http://rb.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://ce.newstarts.cn

JS:   class Admin extends User {}
来源：http://xv.szsharing.cn

TS:   class Admin extends User {}
来源：http://ql.hnjuh.cn

Java: class Admin extends User {}
来源：http://pd.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hl.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://dz.shxzukj.cn

C#:   class Admin : User {}
来源：http://ql.huixiangedu.cn

[G06] 重写方法
来源：http://yo.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://om.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ow.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://fk.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://kd.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://nx.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ha.asd995.cn

Ruby: def greet; "admin"; end
来源：http://lh.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://gx.shxzukj.cn

[G07] 调用父类方法
来源：http://sc.muxihuayi.cn

Py:   super().greet()
来源：http://he.bookmarksfly.cn

PHP:  parent::greet();
来源：http://hv.yuntaijiaju.cn

JS:   super.greet();
来源：http://yl.newstarts.cn

TS:   super.greet();
来源：http://gc.huanxung.cn

Java: super.greet();
来源：http://pv.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kn.huixinmuqiang.cn

Ruby: super
来源：http://lw.huanxung.cn

C#:   base.Greet();
来源：http://bu.shxzukj.cn

[G08] 静态方法与属性
来源：http://bk.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ed.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://gt.shtwfgs.cn

JS:   static f() {}
来源：http://ot.shxzukj.cn

TS:   static f(): void {}
来源：http://dt.hnjuh.cn

Java: static void f() {}
来源：http://jz.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nm.521024.cn

Ruby: def self.f; end
来源：http://jv.panjiajie.cn

C#:   public static void F() {}
来源：http://hp.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://ft.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://zn.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rs.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tz.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://bi.521024.cn

Java: interface Shape { double area(); }
来源：http://mv.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://qx.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qu.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://ae.muxihuayi.cn

[G10] 访问控制
来源：http://jd.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://ck.newstarts.cn

PHP:  public / protected / private
来源：http://ja.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://bw.hahajie.cn

TS:   public / protected / private
来源：http://rg.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://ko.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xk.gzmigu.cn

Ruby: public / protected / private
来源：http://jy.gzmigu.cn

C#:   public / protected / private / internal
来源：http://bq.jianghongdianzi.cn

[G11] getter / setter
来源：http://gl.521024.cn

Py:   @property 与 @x.setter
来源：http://ok.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xx.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://oj.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://sw.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://oe.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://to.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://hs.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://rg.hnjuh.cn

[G12] 对象转字符串
来源：http://jf.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://en.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ws.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://bb.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://ju.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://np.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pf.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://ey.521024.cn

C#:   public override string ToString() => Name;
来源：http://qw.521024.cn

[G13] 判断对象类型
来源：http://kz.newstarts.cn

Py:   isinstance(u, User)
来源：http://my.9csxet.cn

PHP:  $u instanceof User
来源：http://cg.shxzukj.cn

JS:   u instanceof User
来源：http://lq.muxihuayi.cn

TS:   u instanceof User
来源：http://ro.szxytkj.cn

Java: u instanceof User
来源：http://sl.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hp.szsharing.cn

Ruby: u.is_a?(User)
来源：http://kl.colortex.cn

C#:   u is User
来源：http://xp.shxzukj.cn

[G14] 数据类 / record
来源：http://oe.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ap.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://wn.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://my.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://ee.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://nl.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://nl.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yx.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://tr.nicolike.cn

[G15] 枚举
来源：http://sb.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xu.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qi.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bp.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tb.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://lu.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://df.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://wl.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gc.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://ms.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sc.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://lh.9csxet.cn

JS:   Object.entries(obj)
来源：http://fb.nicolike.cn

TS:   Object.entries(obj)
来源：http://gy.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ag.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rn.nicolike.cn

Ruby: obj.instance_variables
来源：http://ha.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://uq.yuexingan06.cn

================================================================================
来源：http://am.bookmarksfly.cn

H. 异常与错误处理
来源：http://ua.521024.cn

================================================================================
来源：http://qo.asd995.cn

[H01] try / catch 基础
来源：http://fg.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pa.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ut.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nq.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bu.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dd.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uu.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://da.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mq.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://lq.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iv.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hc.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uu.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kg.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qq.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gl.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wj.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ra.shxzskj.cn

[H03] 主动抛出异常
来源：http://lj.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://sy.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cq.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://ni.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://av.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qd.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aa.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://py.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pl.shtwfgs.cn

[H04] 自定义异常类型
来源：http://gr.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://oa.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rh.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://py.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ip.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://tc.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nt.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://zy.hahajie.cn

C#:   class MyException : Exception {}
来源：http://ri.yuexingan06.cn

[H05] 捕获特定类型
来源：http://hr.panjiajie.cn

Py:   except ValueError as e:
来源：http://te.chemitech.net.cn


<!-- 参考信息 -->