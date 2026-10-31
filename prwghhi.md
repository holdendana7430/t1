代发 wailian999

Ruby: s.lines
来源：http://yp.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://qs.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://sp.lnxyls.cn

Py:   if not s:
来源：http://jz.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pb.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vu.wgjwhj.cn

TS:   if (s === "") {}
来源：http://qa.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://zb.huanxung.cn

Go:   if s == "" {}
来源：http://lv.9csxet.cn

Ruby: if s.empty?
来源：http://si.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fw.hahajie.cn

[E21] 超长截断加省略号
来源：http://pq.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jf.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fb.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gy.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lg.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ho.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ne.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pj.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zj.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://bt.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bg.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kd.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pe.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lm.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://db.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ih.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ij.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pc.newstarts.cn

================================================================================
来源：http://en.bjjhwx.cn

F. 文件与目录
来源：http://ld.newstarts.cn

================================================================================
来源：http://xx.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://ft.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zm.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://wg.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qh.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fc.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://aj.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uz.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://qx.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://xe.gzmigu.cn

[F02] 逐行读取文件
来源：http://dg.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mm.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pr.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hv.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qk.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hk.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ts.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tz.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bz.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://xf.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ro.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cv.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://re.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fj.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cr.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://di.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://ev.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ks.nicolike.cn

[F04] 追加写入文件
来源：http://pt.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wu.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gx.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yx.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gw.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hy.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wn.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mc.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sl.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://to.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xz.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://kg.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://zg.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://yf.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yf.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tq.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://yt.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://jn.nszjky.cn

[F06] 删除文件
来源：http://ei.asd995.cn

Py:   os.remove("a.txt")
来源：http://ha.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://ad.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dr.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cy.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ea.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://ka.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://gc.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://jl.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://tb.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mr.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ee.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jg.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pp.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ze.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eh.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ib.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bc.gzmigu.cn

[F08] 遍历目录
来源：http://vy.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sp.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nc.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://wb.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://qp.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pt.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ut.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://wq.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://hk.shxzukj.cn

[F09] 获取文件大小
来源：http://nt.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://nn.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ky.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://zu.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://hl.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://de.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://he.asd995.cn

Ruby: File.size("a.txt")
来源：http://xf.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://wc.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://xe.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mb.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tk.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aw.hahajie.cn

TS:   path.extname("a.txt")
来源：http://pu.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://md.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vj.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xd.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qc.muxihuayi.cn

[F11] 复制与移动文件
来源：http://da.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ex.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uw.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dw.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rs.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mn.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lx.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://me.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lu.521024.cn

[F12] CSV 读写
来源：http://ew.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qh.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yw.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mm.9csxet.cn

TS:   // 同上
来源：http://xt.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ha.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dk.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hf.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wy.haigaiapp.cn

================================================================================
来源：http://zb.szxytkj.cn

G. 面向对象
来源：http://et.shxzukj.cn

================================================================================
来源：http://gd.bookmarksfly.cn

[G01] 定义类
来源：http://yc.hnjuh.cn

Py:   class User: pass
来源：http://fc.wgjwhj.cn

PHP:  class User {}
来源：http://wn.jianghongdianzi.cn

JS:   class User {}
来源：http://gd.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://cr.shxzskj.cn

Java: class User {}
来源：http://fq.hahajie.cn

Go:   type User struct { Name string }
来源：http://te.hahajie.cn

Ruby: class User; end
来源：http://tj.lnxyls.cn

C#:   class User {}
来源：http://ba.muxihuayi.cn

[G02] 构造函数
来源：http://sw.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://bj.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://yu.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://mp.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://ba.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://im.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bc.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://rs.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://mm.huixinmuqiang.cn

[G03] 实例属性
来源：http://pz.asd995.cn

Py:   self.name = "x"
来源：http://om.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://cn.jctech888.com.cn

JS:   this.name = "x";
来源：http://qt.yuexingan06.cn

TS:   name: string = "x";
来源：http://mr.shxzukj.cn

Java: private String name;
来源：http://tq.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ki.yuexingan06.cn

Ruby: @name = "x"
来源：http://qd.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://kb.hnjuh.cn

[G04] 定义方法
来源：http://ko.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://dy.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ku.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://dc.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://gs.szsharing.cn

Java: String greet() { return name; }
来源：http://qu.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fl.hahajie.cn

Ruby: def greet; @name; end
来源：http://uw.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://eo.szxytkj.cn

[G05] 继承
来源：http://df.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://ss.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://an.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://vt.shxzskj.cn

TS:   class Admin extends User {}
来源：http://dx.newstarts.cn

Java: class Admin extends User {}
来源：http://jc.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tg.nicolike.cn

Ruby: class Admin < User; end
来源：http://gx.muxihuayi.cn

C#:   class Admin : User {}
来源：http://bm.hnjuh.cn

[G06] 重写方法
来源：http://ss.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://wz.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nk.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://ze.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://oh.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://ks.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zw.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://is.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://hi.muxihuayi.cn

[G07] 调用父类方法
来源：http://id.9csxet.cn

Py:   super().greet()
来源：http://az.haigaiapp.cn

PHP:  parent::greet();
来源：http://vk.shxzskj.cn

JS:   super.greet();
来源：http://wi.yuexingan06.cn

TS:   super.greet();
来源：http://dc.bjjhwx.cn

Java: super.greet();
来源：http://ep.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bi.shxzukj.cn

Ruby: super
来源：http://lq.muxihuayi.cn

C#:   base.Greet();
来源：http://kb.shxzskj.cn

[G08] 静态方法与属性
来源：http://ua.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ai.nszjky.cn

PHP:  public static function f() {}
来源：http://ek.haigaiapp.cn

JS:   static f() {}
来源：http://fi.jctech888.com.cn

TS:   static f(): void {}
来源：http://bs.huanxung.cn

Java: static void f() {}
来源：http://id.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jb.muxihuayi.cn

Ruby: def self.f; end
来源：http://qb.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://bi.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://jv.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://zo.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://li.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ok.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://rf.hahajie.cn

Java: interface Shape { double area(); }
来源：http://cn.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://lh.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oz.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://kd.chemitech.net.cn

[G10] 访问控制
来源：http://ek.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://jk.bookmarksfly.cn

PHP:  public / protected / private
来源：http://dj.colortex.cn

JS:   #private 字段；其余公开
来源：http://iq.yuntaijiaju.cn

TS:   public / protected / private
来源：http://rl.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://pn.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aa.colortex.cn

Ruby: public / protected / private
来源：http://qb.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://hz.jctech888.com.cn

[G11] getter / setter
来源：http://pd.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://yw.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ue.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://bu.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://lw.lnxyls.cn

Java: public String getName() { return name; }
来源：http://kd.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ns.shxzskj.cn

Ruby: attr_accessor :name
来源：http://dt.9csxet.cn

C#:   public string Name { get; set; }
来源：http://tm.hnjuh.cn

[G12] 对象转字符串
来源：http://gv.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://mr.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eb.asd995.cn

JS:   toString() { return this.name; }
来源：http://ln.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://an.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://gi.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iz.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://jh.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://uu.panjiajie.cn

[G13] 判断对象类型
来源：http://wh.asd995.cn

Py:   isinstance(u, User)
来源：http://vj.haigaiapp.cn

PHP:  $u instanceof User
来源：http://my.bjjhwx.cn

JS:   u instanceof User
来源：http://uw.shxzskj.cn

TS:   u instanceof User
来源：http://ct.asd995.cn

Java: u instanceof User
来源：http://rr.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wk.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://rq.muxihuayi.cn

C#:   u is User
来源：http://cg.bookmarksfly.cn

[G14] 数据类 / record
来源：http://zq.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://by.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://it.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cn.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://xw.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://ep.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://vk.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yw.asd995.cn

C#:   record User(string Name, int Age);
来源：http://zy.hnjuh.cn

[G15] 枚举
来源：http://zv.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hn.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pb.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iy.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rc.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://ru.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wv.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://wx.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ir.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://wl.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://af.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://ra.521024.cn

JS:   Object.entries(obj)
来源：http://az.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://dz.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sz.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rn.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://ig.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://qw.huanxung.cn

================================================================================
来源：http://qg.shxzskj.cn

H. 异常与错误处理
来源：http://qh.lnxyls.cn

================================================================================
来源：http://ts.szxytkj.cn

[H01] try / catch 基础
来源：http://yc.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cc.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yk.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dq.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wg.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yx.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yp.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vm.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zy.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://ck.9csxet.cn


<!-- 参考信息 -->