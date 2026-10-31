代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cc.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sm.huixiangedu.cn

TS:   if (s === "") {}
来源：http://jy.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://rh.panjiajie.cn

Go:   if s == "" {}
来源：http://lg.nicolike.cn

Ruby: if s.empty?
来源：http://cm.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://si.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://lu.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mz.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xc.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sx.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ia.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bl.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://si.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nb.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ac.9csxet.cn

[E22] 字节长度与字符长度
来源：http://gl.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zb.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ty.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://my.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ci.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yo.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wj.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://qm.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dj.lnxyls.cn

================================================================================
来源：http://kp.huanxung.cn

F. 文件与目录
来源：http://wz.muxihuayi.cn

================================================================================
来源：http://jz.huanxung.cn

[F01] 读取整个文件
来源：http://ee.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vm.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://oj.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iq.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ek.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bl.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cz.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://er.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://on.jctech888.com.cn

[F02] 逐行读取文件
来源：http://ej.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mg.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ds.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://on.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jd.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zv.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wa.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gb.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tu.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://lm.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lf.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tj.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ns.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yh.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kj.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://in.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://jd.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://za.bookmarksfly.cn

[F04] 追加写入文件
来源：http://wl.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aj.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fa.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wq.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tj.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yx.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://br.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qr.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ym.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://ku.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jw.colortex.cn

PHP:  file_exists("a.txt");
来源：http://jm.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://hf.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://sg.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rw.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uz.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://of.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://kb.chemitech.net.cn

[F06] 删除文件
来源：http://rk.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://vq.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://bz.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wh.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bz.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yv.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://yr.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://bq.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://ua.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://ab.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rn.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tx.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gx.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vi.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cz.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vy.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aj.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rf.shxzukj.cn

[F08] 遍历目录
来源：http://vn.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ir.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xp.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://cc.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://ab.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gn.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bh.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://ww.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://sx.panjiajie.cn

[F09] 获取文件大小
来源：http://wc.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://eo.newstarts.cn

PHP:  filesize("a.txt");
来源：http://pf.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://zt.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://qw.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lz.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xr.colortex.cn

Ruby: File.size("a.txt")
来源：http://ux.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://et.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://kc.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qp.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oz.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jo.hahajie.cn

TS:   path.extname("a.txt")
来源：http://ye.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sx.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ji.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vh.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nl.nicolike.cn

[F11] 复制与移动文件
来源：http://wr.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xz.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://os.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ua.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hi.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hq.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xb.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://px.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nu.jianghongdianzi.cn

[F12] CSV 读写
来源：http://qy.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fl.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sp.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://th.hahajie.cn

TS:   // 同上
来源：http://ry.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pl.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ut.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jh.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://id.hahajie.cn

================================================================================
来源：http://ew.muxihuayi.cn

G. 面向对象
来源：http://xv.nszjky.cn

================================================================================
来源：http://wj.wgjwhj.cn

[G01] 定义类
来源：http://vw.chemitech.net.cn

Py:   class User: pass
来源：http://bj.shxzukj.cn

PHP:  class User {}
来源：http://tp.huixiangedu.cn

JS:   class User {}
来源：http://in.asd995.cn

TS:   class User { name: string = ""; }
来源：http://ah.521024.cn

Java: class User {}
来源：http://vn.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://fj.wgjwhj.cn

Ruby: class User; end
来源：http://by.521024.cn

C#:   class User {}
来源：http://qe.nicolike.cn

[G02] 构造函数
来源：http://kx.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://ax.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hi.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://df.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://vq.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://np.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hv.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ic.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://xe.shtwfgs.cn

[G03] 实例属性
来源：http://ht.huixiangedu.cn

Py:   self.name = "x"
来源：http://dp.szsharing.cn

PHP:  public string $name = "x";
来源：http://sd.szxytkj.cn

JS:   this.name = "x";
来源：http://ug.szxytkj.cn

TS:   name: string = "x";
来源：http://lp.yuntaijiaju.cn

Java: private String name;
来源：http://fb.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vy.yuexingan06.cn

Ruby: @name = "x"
来源：http://xu.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://og.muxihuayi.cn

[G04] 定义方法
来源：http://py.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://zq.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vv.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://zm.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://zk.huixiangedu.cn

Java: String greet() { return name; }
来源：http://tk.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jd.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://hl.colortex.cn

C#:   public string Greet() => Name;
来源：http://wd.shxzukj.cn

[G05] 继承
来源：http://mm.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://ko.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://tk.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://vv.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://gc.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://du.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ph.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://ea.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://zk.haigaiapp.cn

[G06] 重写方法
来源：http://gx.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://hu.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gm.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://ik.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://lp.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://uu.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kc.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://dx.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://pd.hnjuh.cn

[G07] 调用父类方法
来源：http://uq.huixiangedu.cn

Py:   super().greet()
来源：http://hs.9csxet.cn

PHP:  parent::greet();
来源：http://uq.shxzukj.cn

JS:   super.greet();
来源：http://qe.muxihuayi.cn

TS:   super.greet();
来源：http://dd.shtwfgs.cn

Java: super.greet();
来源：http://hj.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hf.nicolike.cn

Ruby: super
来源：http://pv.colortex.cn

C#:   base.Greet();
来源：http://je.panjiajie.cn

[G08] 静态方法与属性
来源：http://ob.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sg.521024.cn

PHP:  public static function f() {}
来源：http://ct.jianghongdianzi.cn

JS:   static f() {}
来源：http://ob.yuexingan06.cn

TS:   static f(): void {}
来源：http://jk.haigaiapp.cn

Java: static void f() {}
来源：http://jr.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rl.szxytkj.cn

Ruby: def self.f; end
来源：http://re.bookmarksfly.cn

C#:   public static void F() {}
来源：http://lx.hahajie.cn

[G09] 接口 / 抽象类
来源：http://fx.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://jf.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xa.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cl.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://rg.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://rb.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://ia.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nj.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://tb.szxytkj.cn

[G10] 访问控制
来源：http://em.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://sp.huanxung.cn

PHP:  public / protected / private
来源：http://ld.newstarts.cn

JS:   #private 字段；其余公开
来源：http://cg.jctech888.com.cn

TS:   public / protected / private
来源：http://ng.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://kh.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eh.bjjhwx.cn

Ruby: public / protected / private
来源：http://xy.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://bk.nicolike.cn

[G11] getter / setter
来源：http://em.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://xh.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gh.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://er.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://iq.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://wy.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hn.nicolike.cn

Ruby: attr_accessor :name
来源：http://yx.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://cj.newstarts.cn

[G12] 对象转字符串
来源：http://wn.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://za.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zw.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://qp.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://si.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://rx.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://za.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://ln.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://dn.szxytkj.cn

[G13] 判断对象类型
来源：http://gt.521024.cn

Py:   isinstance(u, User)
来源：http://rx.chemitech.net.cn

PHP:  $u instanceof User
来源：http://qs.bookmarksfly.cn

JS:   u instanceof User
来源：http://nw.yuexingan06.cn

TS:   u instanceof User
来源：http://yn.wgjwhj.cn

Java: u instanceof User
来源：http://hy.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://db.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://sv.newstarts.cn

C#:   u is User
来源：http://mc.521024.cn

[G14] 数据类 / record
来源：http://hy.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vp.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://pi.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fh.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://gc.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://yc.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://kb.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xo.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://oy.gzmigu.cn

[G15] 枚举
来源：http://an.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ea.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://by.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ng.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wu.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://og.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://be.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://fr.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yf.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://ba.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tt.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://hv.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://oc.szxytkj.cn

TS:   Object.entries(obj)
来源：http://zt.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pc.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mp.shxzukj.cn

Ruby: obj.instance_variables
来源：http://fa.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://ei.newstarts.cn

================================================================================
来源：http://jv.newstarts.cn

H. 异常与错误处理
来源：http://fj.colortex.cn

================================================================================
来源：http://id.panjiajie.cn

[H01] try / catch 基础
来源：http://gz.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qj.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://da.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gi.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lf.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xy.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gz.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ew.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xh.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://cz.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pi.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bu.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ha.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ae.nszjky.cn


<!-- 参考信息 -->