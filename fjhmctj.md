代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ln.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ae.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sn.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://gl.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fb.521024.cn

================================================================================
来源：http://xy.yuexingan06.cn

F. 文件与目录
来源：http://ud.shtwfgs.cn

================================================================================
来源：http://tm.9csxet.cn

[F01] 读取整个文件
来源：http://at.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zl.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://bi.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xg.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ou.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zj.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nd.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://ix.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://if.nszjky.cn

[F02] 逐行读取文件
来源：http://kr.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uh.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ht.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cu.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ny.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://se.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vv.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hn.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lh.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://ki.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ke.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wc.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yo.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yv.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://le.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pi.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://ed.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nu.haigaiapp.cn

[F04] 追加写入文件
来源：http://xk.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pt.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xy.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oo.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hl.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dy.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iw.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ie.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bq.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://ql.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tb.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://gv.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://hr.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://xg.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sa.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rq.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://jb.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://ni.jianghongdianzi.cn

[F06] 删除文件
来源：http://hq.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://rc.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://vk.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ft.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hq.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kh.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://br.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://rm.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://zr.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://li.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://og.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tq.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://av.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jm.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tt.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ie.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fx.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cu.yuntaijiaju.cn

[F08] 遍历目录
来源：http://hf.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sa.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fm.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://ca.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://bz.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ob.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jf.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://ap.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://mm.bjjhwx.cn

[F09] 获取文件大小
来源：http://xk.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://tr.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://vl.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://xz.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://cd.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xs.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rm.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://vy.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://in.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://kg.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wa.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://no.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ja.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://nx.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vg.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qm.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ng.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yy.jctech888.com.cn

[F11] 复制与移动文件
来源：http://vk.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vw.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://da.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lo.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hq.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ff.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zb.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://um.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rl.hnjuh.cn

[F12] CSV 读写
来源：http://nu.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yl.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xp.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ps.huixiangedu.cn

TS:   // 同上
来源：http://ms.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kv.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oc.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qc.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kz.szsharing.cn

================================================================================
来源：http://qx.jctech888.com.cn

G. 面向对象
来源：http://ag.shxzukj.cn

================================================================================
来源：http://xt.hahajie.cn

[G01] 定义类
来源：http://kk.9csxet.cn

Py:   class User: pass
来源：http://lh.colortex.cn

PHP:  class User {}
来源：http://lo.colortex.cn

JS:   class User {}
来源：http://ht.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://tm.asd995.cn

Java: class User {}
来源：http://wc.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://hb.521024.cn

Ruby: class User; end
来源：http://od.jianghongdianzi.cn

C#:   class User {}
来源：http://ty.szxytkj.cn

[G02] 构造函数
来源：http://ij.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://it.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://vj.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://ur.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://na.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://rx.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pg.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://mm.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://dp.jctech888.com.cn

[G03] 实例属性
来源：http://gj.wgjwhj.cn

Py:   self.name = "x"
来源：http://fd.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://zz.bookmarksfly.cn

JS:   this.name = "x";
来源：http://is.hnjuh.cn

TS:   name: string = "x";
来源：http://at.muxihuayi.cn

Java: private String name;
来源：http://ti.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wu.shtwfgs.cn

Ruby: @name = "x"
来源：http://ns.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://yl.szxytkj.cn

[G04] 定义方法
来源：http://jy.9csxet.cn

Py:   def greet(self): return self.name
来源：http://zh.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bq.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://nc.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ir.haigaiapp.cn

Java: String greet() { return name; }
来源：http://lv.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yy.lnxyls.cn

Ruby: def greet; @name; end
来源：http://wo.9csxet.cn

C#:   public string Greet() => Name;
来源：http://bh.nszjky.cn

[G05] 继承
来源：http://vj.szxytkj.cn

Py:   class Admin(User): pass
来源：http://kc.nszjky.cn

PHP:  class Admin extends User {}
来源：http://mr.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://lv.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://zv.szxytkj.cn

Java: class Admin extends User {}
来源：http://gs.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tm.colortex.cn

Ruby: class Admin < User; end
来源：http://ks.bjjhwx.cn

C#:   class Admin : User {}
来源：http://dl.newstarts.cn

[G06] 重写方法
来源：http://kd.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://ff.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cu.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://rj.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://gr.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://qo.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vv.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://el.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://ex.521024.cn

[G07] 调用父类方法
来源：http://cn.shtwfgs.cn

Py:   super().greet()
来源：http://zx.panjiajie.cn

PHP:  parent::greet();
来源：http://nj.shxzskj.cn

JS:   super.greet();
来源：http://eh.huanxung.cn

TS:   super.greet();
来源：http://pt.shxzskj.cn

Java: super.greet();
来源：http://zf.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kf.huanxung.cn

Ruby: super
来源：http://wf.panjiajie.cn

C#:   base.Greet();
来源：http://wy.jctech888.com.cn

[G08] 静态方法与属性
来源：http://qt.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ro.colortex.cn

PHP:  public static function f() {}
来源：http://hs.szsharing.cn

JS:   static f() {}
来源：http://lw.gzmigu.cn

TS:   static f(): void {}
来源：http://sv.newstarts.cn

Java: static void f() {}
来源：http://la.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wv.colortex.cn

Ruby: def self.f; end
来源：http://nh.nicolike.cn

C#:   public static void F() {}
来源：http://ku.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://mh.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://yo.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ts.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qm.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ia.521024.cn

Java: interface Shape { double area(); }
来源：http://gq.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://dq.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ej.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://ar.huixiangedu.cn

[G10] 访问控制
来源：http://do.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://rp.nszjky.cn

PHP:  public / protected / private
来源：http://ov.hahajie.cn

JS:   #private 字段；其余公开
来源：http://fu.szsharing.cn

TS:   public / protected / private
来源：http://xs.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://xi.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fy.colortex.cn

Ruby: public / protected / private
来源：http://ip.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://yn.szsharing.cn

[G11] getter / setter
来源：http://yn.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://dd.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://up.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://ze.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://wn.lnxyls.cn

Java: public String getName() { return name; }
来源：http://wo.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wg.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://wd.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://vn.asd995.cn

[G12] 对象转字符串
来源：http://ab.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://rk.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ol.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://sc.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://fw.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://bw.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pr.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://fj.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://nd.szsharing.cn

[G13] 判断对象类型
来源：http://qt.521024.cn

Py:   isinstance(u, User)
来源：http://mm.nicolike.cn

PHP:  $u instanceof User
来源：http://kg.yuntaijiaju.cn

JS:   u instanceof User
来源：http://nq.bjjhwx.cn

TS:   u instanceof User
来源：http://wm.hnjuh.cn

Java: u instanceof User
来源：http://eq.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cp.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://hj.9csxet.cn

C#:   u is User
来源：http://lj.haigaiapp.cn

[G14] 数据类 / record
来源：http://no.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rv.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://ip.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lu.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://bd.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://oa.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://qj.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sw.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://hb.colortex.cn

[G15] 枚举
来源：http://jh.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ti.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eu.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pw.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ue.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://vj.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xv.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://mz.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://le.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://hu.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://su.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://cq.huanxung.cn

JS:   Object.entries(obj)
来源：http://sb.nszjky.cn

TS:   Object.entries(obj)
来源：http://jj.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hp.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://la.asd995.cn

Ruby: obj.instance_variables
来源：http://bf.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://zz.yuntaijiaju.cn

================================================================================
来源：http://dw.yuntaijiaju.cn

H. 异常与错误处理
来源：http://pp.gzmigu.cn

================================================================================
来源：http://ol.nszjky.cn

[H01] try / catch 基础
来源：http://rr.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cu.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yr.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mc.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ca.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ty.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ue.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ay.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oi.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://ig.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wi.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wj.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tx.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lo.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hs.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rx.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sg.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kx.9csxet.cn

[H03] 主动抛出异常
来源：http://uy.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://ca.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nl.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://dn.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://lg.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gc.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sj.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uy.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ds.nszjky.cn

[H04] 自定义异常类型
来源：http://js.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://id.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vm.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://ti.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ke.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://km.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oz.asd995.cn


<!-- 参考信息 -->