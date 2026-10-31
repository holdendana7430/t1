代发 wailian999

Go:   if s == "" {}
来源：http://yb.colortex.cn

Ruby: if s.empty?
来源：http://ry.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gj.9csxet.cn

[E21] 超长截断加省略号
来源：http://cm.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yr.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bt.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xs.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fr.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yx.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://je.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hh.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cs.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://cp.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gk.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jn.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cx.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lp.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://on.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yv.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://br.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hf.wgjwhj.cn

================================================================================
来源：http://bq.panjiajie.cn

F. 文件与目录
来源：http://vf.panjiajie.cn

================================================================================
来源：http://yu.gzmigu.cn

[F01] 读取整个文件
来源：http://ps.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dg.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://et.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fo.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zy.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kv.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ia.nszjky.cn

Ruby: File.read("a.txt")
来源：http://zq.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://pz.haigaiapp.cn

[F02] 逐行读取文件
来源：http://qx.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wj.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sq.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oa.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dl.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://it.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gf.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bp.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zc.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://zj.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dm.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lf.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dk.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sg.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vw.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ti.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://xc.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ud.colortex.cn

[F04] 追加写入文件
来源：http://hw.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://st.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ri.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tf.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vb.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://di.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fl.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qa.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nb.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://bm.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yk.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://np.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://ok.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://pn.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hg.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://au.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://jp.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://mt.yuexingan06.cn

[F06] 删除文件
来源：http://he.521024.cn

Py:   os.remove("a.txt")
来源：http://xq.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://wk.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vd.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ho.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gv.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://de.colortex.cn

Ruby: File.delete("a.txt")
来源：http://fp.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://xd.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://qn.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ei.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jz.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vf.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ue.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qk.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aw.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pz.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ij.huixinmuqiang.cn

[F08] 遍历目录
来源：http://iu.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ou.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gq.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://rv.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://jm.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jz.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mc.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://kb.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://xe.szsharing.cn

[F09] 获取文件大小
来源：http://gj.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://cr.asd995.cn

PHP:  filesize("a.txt");
来源：http://ns.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://wy.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://zj.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vz.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xw.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://by.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://xh.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ci.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nb.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nz.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vk.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://yi.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ui.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zg.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tc.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gs.panjiajie.cn

[F11] 复制与移动文件
来源：http://jr.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lk.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uz.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ep.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dn.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ss.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cp.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jh.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ey.bjjhwx.cn

[F12] CSV 读写
来源：http://iv.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://le.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fy.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yl.nicolike.cn

TS:   // 同上
来源：http://nz.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sh.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qm.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uk.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://on.huixinmuqiang.cn

================================================================================
来源：http://qa.huanxung.cn

G. 面向对象
来源：http://av.newstarts.cn

================================================================================
来源：http://pf.szsharing.cn

[G01] 定义类
来源：http://wt.yuntaijiaju.cn

Py:   class User: pass
来源：http://do.panjiajie.cn

PHP:  class User {}
来源：http://tt.chemitech.net.cn

JS:   class User {}
来源：http://kn.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://ts.colortex.cn

Java: class User {}
来源：http://gv.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://bw.9csxet.cn

Ruby: class User; end
来源：http://bz.szsharing.cn

C#:   class User {}
来源：http://ef.bookmarksfly.cn

[G02] 构造函数
来源：http://cx.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://bx.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://jv.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://xj.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://or.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://rj.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ja.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://ko.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://qk.huixiangedu.cn

[G03] 实例属性
来源：http://vh.wgjwhj.cn

Py:   self.name = "x"
来源：http://ou.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://oh.shtwfgs.cn

JS:   this.name = "x";
来源：http://ue.nicolike.cn

TS:   name: string = "x";
来源：http://nr.shxzskj.cn

Java: private String name;
来源：http://xw.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xp.gzmigu.cn

Ruby: @name = "x"
来源：http://fy.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://yz.colortex.cn

[G04] 定义方法
来源：http://ax.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://wm.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cq.nicolike.cn

JS:   greet() { return this.name; }
来源：http://lt.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://bc.jctech888.com.cn

Java: String greet() { return name; }
来源：http://lv.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://it.szsharing.cn

Ruby: def greet; @name; end
来源：http://wz.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://nt.huixinmuqiang.cn

[G05] 继承
来源：http://co.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://ab.9csxet.cn

PHP:  class Admin extends User {}
来源：http://eu.szxytkj.cn

JS:   class Admin extends User {}
来源：http://oj.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://ue.shxzskj.cn

Java: class Admin extends User {}
来源：http://za.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ze.9csxet.cn

Ruby: class Admin < User; end
来源：http://yk.shxzskj.cn

C#:   class Admin : User {}
来源：http://kz.bjjhwx.cn

[G06] 重写方法
来源：http://na.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://pq.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tk.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://jk.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://dz.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://cq.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://md.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://wz.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://hi.asd995.cn

[G07] 调用父类方法
来源：http://lz.newstarts.cn

Py:   super().greet()
来源：http://dx.huixiangedu.cn

PHP:  parent::greet();
来源：http://qo.hnjuh.cn

JS:   super.greet();
来源：http://ku.chemitech.net.cn

TS:   super.greet();
来源：http://dz.muxihuayi.cn

Java: super.greet();
来源：http://xp.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://id.shxzskj.cn

Ruby: super
来源：http://gh.shtwfgs.cn

C#:   base.Greet();
来源：http://nn.asd995.cn

[G08] 静态方法与属性
来源：http://mx.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wr.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://ys.lnxyls.cn

JS:   static f() {}
来源：http://hr.hnjuh.cn

TS:   static f(): void {}
来源：http://mv.bookmarksfly.cn

Java: static void f() {}
来源：http://sm.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ql.chemitech.net.cn

Ruby: def self.f; end
来源：http://jl.szsharing.cn

C#:   public static void F() {}
来源：http://ww.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://gm.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://xe.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ft.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ua.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://oc.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://ed.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://uc.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pi.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://cp.colortex.cn

[G10] 访问控制
来源：http://cb.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://tx.hahajie.cn

PHP:  public / protected / private
来源：http://zb.huanxung.cn

JS:   #private 字段；其余公开
来源：http://hy.shxzukj.cn

TS:   public / protected / private
来源：http://qo.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://vq.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hq.chemitech.net.cn

Ruby: public / protected / private
来源：http://hb.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://an.panjiajie.cn

[G11] getter / setter
来源：http://bj.colortex.cn

Py:   @property 与 @x.setter
来源：http://mr.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tv.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://kv.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://hn.newstarts.cn

Java: public String getName() { return name; }
来源：http://qd.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xy.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://og.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://sc.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://rl.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://ba.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uz.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://oe.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://ke.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://xb.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lc.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://mz.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://fu.lnxyls.cn

[G13] 判断对象类型
来源：http://es.szxytkj.cn

Py:   isinstance(u, User)
来源：http://qn.huanxung.cn

PHP:  $u instanceof User
来源：http://gy.shtwfgs.cn

JS:   u instanceof User
来源：http://fl.haigaiapp.cn

TS:   u instanceof User
来源：http://dp.521024.cn

Java: u instanceof User
来源：http://jr.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ar.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ip.shtwfgs.cn

C#:   u is User
来源：http://tq.shxzskj.cn

[G14] 数据类 / record
来源：http://fn.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rb.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://tf.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qi.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://vj.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://eu.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://mj.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sw.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://ru.lnxyls.cn

[G15] 枚举
来源：http://xa.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://be.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://le.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dp.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ca.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://tq.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vi.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://rs.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vv.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://yh.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hb.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://hi.colortex.cn

JS:   Object.entries(obj)
来源：http://ld.newstarts.cn

TS:   Object.entries(obj)
来源：http://cw.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kl.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ad.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://ma.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://pq.newstarts.cn

================================================================================
来源：http://xd.yuexingan06.cn

H. 异常与错误处理
来源：http://ye.bjjhwx.cn

================================================================================
来源：http://ac.shxzukj.cn

[H01] try / catch 基础
来源：http://ku.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qx.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://do.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fi.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bh.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mu.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uk.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wr.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iv.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ta.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uk.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ed.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vn.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hm.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cw.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yb.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zu.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vb.gzmigu.cn


<!-- 参考信息 -->