代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ay.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://if.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ro.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ah.huanxung.cn

Go:   if s == "" {}
来源：http://hw.shxzukj.cn

Ruby: if s.empty?
来源：http://gb.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tn.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://de.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vq.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kl.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ou.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ve.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lc.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://ra.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oh.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ir.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://zn.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vh.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bb.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://so.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ga.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ik.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mz.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://gw.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ox.asd995.cn

================================================================================
来源：http://yo.wgjwhj.cn

F. 文件与目录
来源：http://gg.panjiajie.cn

================================================================================
来源：http://nl.shxzskj.cn

[F01] 读取整个文件
来源：http://xv.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ib.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://dt.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uj.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nh.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hf.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ld.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://bo.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://ze.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://rs.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ec.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yt.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sh.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hq.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pv.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sh.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cn.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ep.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://nw.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://px.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ou.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lo.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kv.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tv.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kn.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://zx.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yx.hnjuh.cn

[F04] 追加写入文件
来源：http://do.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rx.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mx.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ky.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gc.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ru.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ma.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zl.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ci.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://kf.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xl.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://ip.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://nd.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://np.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ek.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qh.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://um.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://mx.gzmigu.cn

[F06] 删除文件
来源：http://xi.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://qe.521024.cn

PHP:  unlink("a.txt");
来源：http://fs.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ja.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gy.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fj.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://kx.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://nb.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://ck.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://mq.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pe.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gz.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://he.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ks.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nz.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://un.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ut.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://st.nicolike.cn

[F08] 遍历目录
来源：http://wk.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vp.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ge.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://al.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://ir.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wi.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nz.hahajie.cn

Ruby: Dir.children("dir")
来源：http://he.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://cu.hahajie.cn

[F09] 获取文件大小
来源：http://uf.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://av.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://ga.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://nv.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ve.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ki.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xk.9csxet.cn

Ruby: File.size("a.txt")
来源：http://os.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://en.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://nw.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hq.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ep.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cc.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://xv.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ou.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://to.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://td.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vr.chemitech.net.cn

[F11] 复制与移动文件
来源：http://rr.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xr.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vm.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kf.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uf.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fn.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://at.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jm.jianghongdianzi.cn

[F12] CSV 读写
来源：http://ze.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://av.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://of.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gw.shtwfgs.cn

TS:   // 同上
来源：http://us.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cq.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oi.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nj.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lh.panjiajie.cn

================================================================================
来源：http://oj.nicolike.cn

G. 面向对象
来源：http://uw.panjiajie.cn

================================================================================
来源：http://xf.asd995.cn

[G01] 定义类
来源：http://lr.huanxung.cn

Py:   class User: pass
来源：http://iz.bjjhwx.cn

PHP:  class User {}
来源：http://qa.panjiajie.cn

JS:   class User {}
来源：http://tu.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://vk.yuntaijiaju.cn

Java: class User {}
来源：http://db.panjiajie.cn

Go:   type User struct { Name string }
来源：http://ln.lnxyls.cn

Ruby: class User; end
来源：http://xz.jctech888.com.cn

C#:   class User {}
来源：http://yh.huanxung.cn

[G02] 构造函数
来源：http://vs.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://ji.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://su.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ig.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://me.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://fe.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rb.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://dv.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://zt.gzmigu.cn

[G03] 实例属性
来源：http://ba.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://gv.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://iu.nszjky.cn

JS:   this.name = "x";
来源：http://ja.9csxet.cn

TS:   name: string = "x";
来源：http://vy.521024.cn

Java: private String name;
来源：http://cu.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dm.huixiangedu.cn

Ruby: @name = "x"
来源：http://bt.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ig.nszjky.cn

[G04] 定义方法
来源：http://ij.colortex.cn

Py:   def greet(self): return self.name
来源：http://zj.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xo.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://nf.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://yf.jctech888.com.cn

Java: String greet() { return name; }
来源：http://pe.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ie.shxzukj.cn

Ruby: def greet; @name; end
来源：http://oa.521024.cn

C#:   public string Greet() => Name;
来源：http://un.haigaiapp.cn

[G05] 继承
来源：http://av.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://zz.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://er.panjiajie.cn

JS:   class Admin extends User {}
来源：http://jc.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://tg.nszjky.cn

Java: class Admin extends User {}
来源：http://aa.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ju.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://nt.muxihuayi.cn

C#:   class Admin : User {}
来源：http://ax.hahajie.cn

[G06] 重写方法
来源：http://re.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://qp.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ec.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://fr.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://gt.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://bw.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xm.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://at.521024.cn

C#:   public override string Greet() => "admin";
来源：http://fh.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://sy.bjjhwx.cn

Py:   super().greet()
来源：http://ap.panjiajie.cn

PHP:  parent::greet();
来源：http://no.colortex.cn

JS:   super.greet();
来源：http://fx.huanxung.cn

TS:   super.greet();
来源：http://qj.newstarts.cn

Java: super.greet();
来源：http://ws.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://px.huixiangedu.cn

Ruby: super
来源：http://sm.bookmarksfly.cn

C#:   base.Greet();
来源：http://zr.colortex.cn

[G08] 静态方法与属性
来源：http://lt.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xt.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://tj.9csxet.cn

JS:   static f() {}
来源：http://nn.colortex.cn

TS:   static f(): void {}
来源：http://ec.muxihuayi.cn

Java: static void f() {}
来源：http://wj.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ul.asd995.cn

Ruby: def self.f; end
来源：http://nf.panjiajie.cn

C#:   public static void F() {}
来源：http://wf.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://lt.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://dj.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wl.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ou.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://ze.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://sm.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://bg.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://om.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://dl.jianghongdianzi.cn

[G10] 访问控制
来源：http://oc.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://hh.9csxet.cn

PHP:  public / protected / private
来源：http://qb.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://lf.gzmigu.cn

TS:   public / protected / private
来源：http://dj.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://er.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xz.gzmigu.cn

Ruby: public / protected / private
来源：http://zd.newstarts.cn

C#:   public / protected / private / internal
来源：http://uf.jianghongdianzi.cn

[G11] getter / setter
来源：http://xe.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://nj.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ar.521024.cn

JS:   get name() { return this._name; }
来源：http://hr.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://lh.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ob.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jo.colortex.cn

Ruby: attr_accessor :name
来源：http://zx.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://hw.shtwfgs.cn

[G12] 对象转字符串
来源：http://rg.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://nv.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ye.nszjky.cn

JS:   toString() { return this.name; }
来源：http://he.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://sa.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://zu.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wh.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ex.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://pu.9csxet.cn

[G13] 判断对象类型
来源：http://xn.gzmigu.cn

Py:   isinstance(u, User)
来源：http://yt.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://tu.huixiangedu.cn

JS:   u instanceof User
来源：http://lp.bjjhwx.cn

TS:   u instanceof User
来源：http://mu.wgjwhj.cn

Java: u instanceof User
来源：http://gt.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kp.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://cb.lnxyls.cn

C#:   u is User
来源：http://tb.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://qz.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://by.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://mj.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tc.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://go.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://ii.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://bq.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wp.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://wz.yuntaijiaju.cn

[G15] 枚举
来源：http://xr.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ry.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kp.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://il.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zh.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://py.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cm.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://tf.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://el.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://ps.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ea.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://ta.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://kb.newstarts.cn

TS:   Object.entries(obj)
来源：http://zv.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eo.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oz.colortex.cn

Ruby: obj.instance_variables
来源：http://gq.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://vm.521024.cn

================================================================================
来源：http://gl.nicolike.cn

H. 异常与错误处理
来源：http://pq.muxihuayi.cn

================================================================================
来源：http://pd.huixiangedu.cn

[H01] try / catch 基础
来源：http://pb.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mw.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dx.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ba.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wd.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zz.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yv.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nn.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bs.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://yd.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rc.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zf.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cq.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://md.chemitech.net.cn


<!-- 参考信息 -->