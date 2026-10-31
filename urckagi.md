代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://sr.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pr.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://io.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xb.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tm.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://nl.hahajie.cn

Py:   s.splitlines()
来源：http://ti.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zg.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://cx.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://gq.nszjky.cn

Java: s.lines().toList()
来源：http://xb.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://ig.wgjwhj.cn

Ruby: s.lines
来源：http://nh.nszjky.cn

C#:   s.Split('\n')
来源：http://lr.hahajie.cn

[E20] 判断字符串是否为空
来源：http://gj.szxytkj.cn

Py:   if not s:
来源：http://lu.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vx.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dd.haigaiapp.cn

TS:   if (s === "") {}
来源：http://ib.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://nm.9csxet.cn

Go:   if s == "" {}
来源：http://ji.yuexingan06.cn

Ruby: if s.empty?
来源：http://ey.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://is.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://up.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cg.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cr.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iy.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ty.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vd.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://ox.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ou.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gq.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://tq.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zv.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ct.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xs.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iw.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://md.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xp.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://ee.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vk.jianghongdianzi.cn

================================================================================
来源：http://ur.yuntaijiaju.cn

F. 文件与目录
来源：http://ip.nicolike.cn

================================================================================
来源：http://yu.bjjhwx.cn

[F01] 读取整个文件
来源：http://wd.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jq.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://yf.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fz.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xo.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://co.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zi.nszjky.cn

Ruby: File.read("a.txt")
来源：http://jg.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://qi.hahajie.cn

[F02] 逐行读取文件
来源：http://wv.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wr.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mk.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gz.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nd.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vc.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bj.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lk.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://so.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://xq.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qs.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xq.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ov.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://un.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://do.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sg.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://mn.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fh.9csxet.cn

[F04] 追加写入文件
来源：http://xp.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pl.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tf.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ml.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dv.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fw.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://id.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jl.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vf.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://eu.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://dw.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://uh.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://fy.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fc.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qf.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://kr.asd995.cn

C#:   File.Exists("a.txt")
来源：http://nw.huixinmuqiang.cn

[F06] 删除文件
来源：http://fu.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://fh.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://oz.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sf.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hs.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gt.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://mp.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://uq.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://wd.szsharing.cn

[F07] 创建目录（含多级）
来源：http://zl.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rd.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yu.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rn.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wu.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tv.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sl.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iu.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uu.gzmigu.cn

[F08] 遍历目录
来源：http://hu.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ab.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gp.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://hw.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://xe.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uw.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pb.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://ic.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://pk.hnjuh.cn

[F09] 获取文件大小
来源：http://jv.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://st.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://oa.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://rb.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://ye.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ek.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tf.521024.cn

Ruby: File.size("a.txt")
来源：http://dp.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://sd.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://lw.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zp.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://of.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wr.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://ty.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://we.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yp.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ae.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cw.shtwfgs.cn

[F11] 复制与移动文件
来源：http://dw.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zb.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aa.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fu.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://re.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jy.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ap.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://co.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vf.521024.cn

[F12] CSV 读写
来源：http://qt.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ib.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ip.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sn.newstarts.cn

TS:   // 同上
来源：http://xt.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bg.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ym.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hh.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wd.nszjky.cn

================================================================================
来源：http://mm.asd995.cn

G. 面向对象
来源：http://ap.bookmarksfly.cn

================================================================================
来源：http://pd.jctech888.com.cn

[G01] 定义类
来源：http://am.huanxung.cn

Py:   class User: pass
来源：http://ef.huanxung.cn

PHP:  class User {}
来源：http://px.yuexingan06.cn

JS:   class User {}
来源：http://xp.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://bo.szsharing.cn

Java: class User {}
来源：http://to.asd995.cn

Go:   type User struct { Name string }
来源：http://do.yuexingan06.cn

Ruby: class User; end
来源：http://bm.wgjwhj.cn

C#:   class User {}
来源：http://zd.9csxet.cn

[G02] 构造函数
来源：http://zr.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://mx.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://mc.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://af.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://aq.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://sp.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://er.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://bn.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://kv.colortex.cn

[G03] 实例属性
来源：http://sj.jctech888.com.cn

Py:   self.name = "x"
来源：http://px.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://nx.shtwfgs.cn

JS:   this.name = "x";
来源：http://ov.9csxet.cn

TS:   name: string = "x";
来源：http://rp.huixiangedu.cn

Java: private String name;
来源：http://pi.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zg.hnjuh.cn

Ruby: @name = "x"
来源：http://fr.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://wy.nicolike.cn

[G04] 定义方法
来源：http://rt.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://vb.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yr.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://md.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://oj.gzmigu.cn

Java: String greet() { return name; }
来源：http://cg.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jk.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://ig.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://uy.yuntaijiaju.cn

[G05] 继承
来源：http://ip.huanxung.cn

Py:   class Admin(User): pass
来源：http://hr.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://qd.shxzukj.cn

JS:   class Admin extends User {}
来源：http://tx.newstarts.cn

TS:   class Admin extends User {}
来源：http://gt.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://zt.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pg.gzmigu.cn

Ruby: class Admin < User; end
来源：http://qh.hahajie.cn

C#:   class Admin : User {}
来源：http://zg.huanxung.cn

[G06] 重写方法
来源：http://bq.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://sj.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gk.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://tt.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://gk.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://tg.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oa.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://aq.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://ha.muxihuayi.cn

[G07] 调用父类方法
来源：http://du.colortex.cn

Py:   super().greet()
来源：http://nd.haigaiapp.cn

PHP:  parent::greet();
来源：http://jb.gzmigu.cn

JS:   super.greet();
来源：http://xz.colortex.cn

TS:   super.greet();
来源：http://dr.gzmigu.cn

Java: super.greet();
来源：http://rm.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xl.szsharing.cn

Ruby: super
来源：http://ht.asd995.cn

C#:   base.Greet();
来源：http://cf.asd995.cn

[G08] 静态方法与属性
来源：http://iz.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ff.jctech888.com.cn

PHP:  public static function f() {}
来源：http://fa.huanxung.cn

JS:   static f() {}
来源：http://jc.hahajie.cn

TS:   static f(): void {}
来源：http://jk.gzmigu.cn

Java: static void f() {}
来源：http://rg.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wa.huixiangedu.cn

Ruby: def self.f; end
来源：http://im.jctech888.com.cn

C#:   public static void F() {}
来源：http://jq.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://ce.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://fq.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zq.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cv.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://ds.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://ux.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://vu.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lw.521024.cn

C#:   interface IShape { double Area(); }
来源：http://ci.wgjwhj.cn

[G10] 访问控制
来源：http://zc.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://af.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://za.nszjky.cn

JS:   #private 字段；其余公开
来源：http://vi.huanxung.cn

TS:   public / protected / private
来源：http://gw.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://gg.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ia.hahajie.cn

Ruby: public / protected / private
来源：http://yj.9csxet.cn

C#:   public / protected / private / internal
来源：http://kd.jianghongdianzi.cn

[G11] getter / setter
来源：http://jh.newstarts.cn

Py:   @property 与 @x.setter
来源：http://cn.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fg.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://qq.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://kg.szxytkj.cn

Java: public String getName() { return name; }
来源：http://fm.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vl.lnxyls.cn

Ruby: attr_accessor :name
来源：http://up.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://lc.hnjuh.cn

[G12] 对象转字符串
来源：http://zs.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://mq.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vg.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://kh.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://vb.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://cw.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sj.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://nv.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://uu.panjiajie.cn

[G13] 判断对象类型
来源：http://sj.hahajie.cn

Py:   isinstance(u, User)
来源：http://ns.shxzukj.cn

PHP:  $u instanceof User
来源：http://mq.nicolike.cn

JS:   u instanceof User
来源：http://dr.shxzukj.cn

TS:   u instanceof User
来源：http://gc.9csxet.cn

Java: u instanceof User
来源：http://rh.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gn.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ii.9csxet.cn

C#:   u is User
来源：http://dz.521024.cn

[G14] 数据类 / record
来源：http://sm.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rg.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://gu.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ed.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://xn.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://zo.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://kb.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lt.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://wx.wgjwhj.cn

[G15] 枚举
来源：http://nj.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://he.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pz.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fv.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iq.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://ub.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ir.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://un.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gn.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://tm.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hx.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://dt.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://iw.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://ur.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://em.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ei.hahajie.cn

Ruby: obj.instance_variables
来源：http://cm.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://pg.521024.cn

================================================================================
来源：http://ce.yuexingan06.cn


<!-- 参考信息 -->