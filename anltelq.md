代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lj.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bp.shtwfgs.cn

TS:   if (s === "") {}
来源：http://vu.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://ap.jctech888.com.cn

Go:   if s == "" {}
来源：http://id.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://ml.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://th.szxytkj.cn

[E21] 超长截断加省略号
来源：http://on.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mu.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zi.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pa.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nq.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://as.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://jy.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rb.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zj.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://en.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jz.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lp.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vv.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://us.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fk.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pi.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://zz.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oc.chemitech.net.cn

================================================================================
来源：http://he.shtwfgs.cn

F. 文件与目录
来源：http://rr.yuntaijiaju.cn

================================================================================
来源：http://us.9csxet.cn

[F01] 读取整个文件
来源：http://vr.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ei.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://wu.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cz.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://by.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lt.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uu.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://ss.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://kt.gzmigu.cn

[F02] 逐行读取文件
来源：http://sg.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bp.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://px.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ch.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://il.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cv.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pn.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gs.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bo.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://er.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iy.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bb.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ip.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://db.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pm.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ds.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://kd.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pd.hahajie.cn

[F04] 追加写入文件
来源：http://sm.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://do.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tf.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sv.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://el.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://on.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xl.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://li.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ox.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://ga.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uh.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://fq.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://ws.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://ly.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kj.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sn.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://vn.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://ug.huixinmuqiang.cn

[F06] 删除文件
来源：http://sn.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://ux.9csxet.cn

PHP:  unlink("a.txt");
来源：http://zf.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kv.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hz.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wr.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://fh.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://ro.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://cb.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://gy.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rk.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oi.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://go.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pr.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kj.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cf.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://em.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://as.shxzukj.cn

[F08] 遍历目录
来源：http://ha.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ni.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ct.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://yl.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://oi.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zh.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lu.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://ny.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://lp.nszjky.cn

[F09] 获取文件大小
来源：http://pz.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://if.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://an.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://lv.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://jn.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://av.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qk.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://xd.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://rb.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://rf.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qn.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ud.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vz.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://tk.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dd.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pt.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fx.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uq.gzmigu.cn

[F11] 复制与移动文件
来源：http://vo.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sp.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uk.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hu.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ci.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iy.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qs.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cc.shxzukj.cn

[F12] CSV 读写
来源：http://fl.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://in.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jj.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cg.szxytkj.cn

TS:   // 同上
来源：http://hs.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bj.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qn.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qi.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ya.jctech888.com.cn

================================================================================
来源：http://gl.szsharing.cn

G. 面向对象
来源：http://hn.haigaiapp.cn

================================================================================
来源：http://or.huixiangedu.cn

[G01] 定义类
来源：http://yt.shxzukj.cn

Py:   class User: pass
来源：http://xl.nszjky.cn

PHP:  class User {}
来源：http://iv.huixinmuqiang.cn

JS:   class User {}
来源：http://bq.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://jq.colortex.cn

Java: class User {}
来源：http://ee.hahajie.cn

Go:   type User struct { Name string }
来源：http://nt.9csxet.cn

Ruby: class User; end
来源：http://in.shtwfgs.cn

C#:   class User {}
来源：http://on.bookmarksfly.cn

[G02] 构造函数
来源：http://ed.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://qk.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://yl.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://az.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://rw.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://ij.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yz.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://rv.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://kv.szsharing.cn

[G03] 实例属性
来源：http://mp.hahajie.cn

Py:   self.name = "x"
来源：http://yg.asd995.cn

PHP:  public string $name = "x";
来源：http://qp.chemitech.net.cn

JS:   this.name = "x";
来源：http://zp.yuexingan06.cn

TS:   name: string = "x";
来源：http://rp.muxihuayi.cn

Java: private String name;
来源：http://oi.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ea.wgjwhj.cn

Ruby: @name = "x"
来源：http://wa.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://px.wgjwhj.cn

[G04] 定义方法
来源：http://ku.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://lo.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oi.9csxet.cn

JS:   greet() { return this.name; }
来源：http://kh.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://wb.huixiangedu.cn

Java: String greet() { return name; }
来源：http://ek.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ty.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://df.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://fa.panjiajie.cn

[G05] 继承
来源：http://fb.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://iq.colortex.cn

PHP:  class Admin extends User {}
来源：http://xx.521024.cn

JS:   class Admin extends User {}
来源：http://ag.lnxyls.cn

TS:   class Admin extends User {}
来源：http://rx.hnjuh.cn

Java: class Admin extends User {}
来源：http://sl.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ax.colortex.cn

Ruby: class Admin < User; end
来源：http://oi.shtwfgs.cn

C#:   class Admin : User {}
来源：http://hw.huanxung.cn

[G06] 重写方法
来源：http://au.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://oq.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ln.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ln.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://ah.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://dc.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wh.asd995.cn

Ruby: def greet; "admin"; end
来源：http://yt.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://lg.asd995.cn

[G07] 调用父类方法
来源：http://tz.nicolike.cn

Py:   super().greet()
来源：http://aw.nicolike.cn

PHP:  parent::greet();
来源：http://fq.9csxet.cn

JS:   super.greet();
来源：http://rd.jianghongdianzi.cn

TS:   super.greet();
来源：http://bi.jctech888.com.cn

Java: super.greet();
来源：http://rp.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qi.gzmigu.cn

Ruby: super
来源：http://yn.bookmarksfly.cn

C#:   base.Greet();
来源：http://rf.haigaiapp.cn

[G08] 静态方法与属性
来源：http://ew.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ai.bjjhwx.cn

PHP:  public static function f() {}
来源：http://hz.shtwfgs.cn

JS:   static f() {}
来源：http://bq.huixiangedu.cn

TS:   static f(): void {}
来源：http://id.muxihuayi.cn

Java: static void f() {}
来源：http://ci.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lp.newstarts.cn

Ruby: def self.f; end
来源：http://mx.521024.cn

C#:   public static void F() {}
来源：http://ku.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://kk.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ia.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vk.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hy.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://eh.huanxung.cn

Java: interface Shape { double area(); }
来源：http://fv.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://kr.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yr.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://xm.shxzskj.cn

[G10] 访问控制
来源：http://rs.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://vx.shxzukj.cn

PHP:  public / protected / private
来源：http://on.nszjky.cn

JS:   #private 字段；其余公开
来源：http://bg.asd995.cn

TS:   public / protected / private
来源：http://vq.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://yw.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cj.jctech888.com.cn

Ruby: public / protected / private
来源：http://mq.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://wv.wgjwhj.cn

[G11] getter / setter
来源：http://jq.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://rp.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mw.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://qe.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://cn.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://cl.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ac.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://pn.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://va.nszjky.cn

[G12] 对象转字符串
来源：http://wo.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://mz.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vc.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://xj.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://mx.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://aw.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pk.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://tx.colortex.cn

C#:   public override string ToString() => Name;
来源：http://eb.shtwfgs.cn

[G13] 判断对象类型
来源：http://ot.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://ls.chemitech.net.cn

PHP:  $u instanceof User
来源：http://ax.chemitech.net.cn

JS:   u instanceof User
来源：http://qq.asd995.cn

TS:   u instanceof User
来源：http://ex.colortex.cn

Java: u instanceof User
来源：http://sa.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://km.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://zy.newstarts.cn

C#:   u is User
来源：http://mr.nicolike.cn

[G14] 数据类 / record
来源：http://ss.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tj.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ke.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cq.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://ns.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://ci.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://xy.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jn.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://rg.haigaiapp.cn

[G15] 枚举
来源：http://jy.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://or.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ss.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vw.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qo.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://mp.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dn.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://dg.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cf.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://zu.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xh.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://fx.hnjuh.cn

JS:   Object.entries(obj)
来源：http://kf.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://im.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ed.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ke.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://yk.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://dd.bjjhwx.cn

================================================================================
来源：http://us.shtwfgs.cn

H. 异常与错误处理
来源：http://ua.szxytkj.cn

================================================================================
来源：http://bx.bookmarksfly.cn

[H01] try / catch 基础
来源：http://cl.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kc.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pu.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://li.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ff.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://td.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yv.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://os.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ap.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://ct.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://js.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vz.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oq.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://by.colortex.cn


<!-- 参考信息 -->