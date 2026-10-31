代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uo.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://cs.shxzskj.cn

Py:   s.splitlines()
来源：http://om.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vk.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://og.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://zn.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://nd.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://gk.haigaiapp.cn

Ruby: s.lines
来源：http://ic.hahajie.cn

C#:   s.Split('\n')
来源：http://lm.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://ba.shxzskj.cn

Py:   if not s:
来源：http://bq.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xl.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://il.huixiangedu.cn

TS:   if (s === "") {}
来源：http://lt.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://be.nszjky.cn

Go:   if s == "" {}
来源：http://uo.szsharing.cn

Ruby: if s.empty?
来源：http://ec.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ri.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://uy.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vd.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tw.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jp.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ik.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lr.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://lr.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ru.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wu.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://zk.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://li.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xa.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rn.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ay.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ia.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zs.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://md.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tv.yuntaijiaju.cn

================================================================================
来源：http://vl.hahajie.cn

F. 文件与目录
来源：http://sd.huixinmuqiang.cn

================================================================================
来源：http://jk.colortex.cn

[F01] 读取整个文件
来源：http://dg.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mm.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://op.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ui.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://us.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zo.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ny.nicolike.cn

Ruby: File.read("a.txt")
来源：http://gk.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ot.nicolike.cn

[F02] 逐行读取文件
来源：http://fx.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jx.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kj.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ox.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pd.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ab.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rf.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wu.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cf.asd995.cn

[F03] 写入文件（覆盖）
来源：http://gz.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uz.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ua.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fm.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wj.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ok.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ss.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://dc.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wj.nicolike.cn

[F04] 追加写入文件
来源：http://ua.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://za.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rd.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fc.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nq.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ud.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xq.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zu.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://yo.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://hm.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://rz.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://mi.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oa.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rs.521024.cn

Ruby: File.exist?("a.txt")
来源：http://ug.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://hd.szxytkj.cn

[F06] 删除文件
来源：http://io.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://ks.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://fw.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ux.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hn.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zu.colortex.cn

Go:   os.Remove("a.txt")
来源：http://qz.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://mv.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://is.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://st.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hb.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://do.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zy.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zq.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ls.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lg.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ft.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ri.szsharing.cn

[F08] 遍历目录
来源：http://jm.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nf.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bt.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://kt.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://yu.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://om.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qa.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://vi.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://ap.hnjuh.cn

[F09] 获取文件大小
来源：http://pr.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://qi.newstarts.cn

PHP:  filesize("a.txt");
来源：http://ug.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://qb.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://et.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ro.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yq.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://dd.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://hw.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://ia.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kt.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gy.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://va.nszjky.cn

TS:   path.extname("a.txt")
来源：http://pb.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hx.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rk.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://he.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kk.yuexingan06.cn

[F11] 复制与移动文件
来源：http://dj.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wx.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ue.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://de.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ke.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://my.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://br.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ms.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mi.lnxyls.cn

[F12] CSV 读写
来源：http://jy.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sr.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nq.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dv.shxzskj.cn

TS:   // 同上
来源：http://in.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://do.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xt.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mp.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bl.szsharing.cn

================================================================================
来源：http://xv.colortex.cn

G. 面向对象
来源：http://qq.asd995.cn

================================================================================
来源：http://wq.hahajie.cn

[G01] 定义类
来源：http://wx.muxihuayi.cn

Py:   class User: pass
来源：http://si.yuntaijiaju.cn

PHP:  class User {}
来源：http://xp.chemitech.net.cn

JS:   class User {}
来源：http://ix.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://ox.yuexingan06.cn

Java: class User {}
来源：http://hk.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://va.521024.cn

Ruby: class User; end
来源：http://vz.colortex.cn

C#:   class User {}
来源：http://mq.szxytkj.cn

[G02] 构造函数
来源：http://wu.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://ht.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://tl.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://sv.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://gx.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://sx.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yf.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://gi.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://ct.szsharing.cn

[G03] 实例属性
来源：http://kf.newstarts.cn

Py:   self.name = "x"
来源：http://xz.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://dg.muxihuayi.cn

JS:   this.name = "x";
来源：http://dz.shxzskj.cn

TS:   name: string = "x";
来源：http://fk.bookmarksfly.cn

Java: private String name;
来源：http://lz.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jg.chemitech.net.cn

Ruby: @name = "x"
来源：http://dm.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://qx.nicolike.cn

[G04] 定义方法
来源：http://pw.521024.cn

Py:   def greet(self): return self.name
来源：http://in.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xn.szsharing.cn

JS:   greet() { return this.name; }
来源：http://pu.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://qd.asd995.cn

Java: String greet() { return name; }
来源：http://ol.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://za.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://jp.asd995.cn

C#:   public string Greet() => Name;
来源：http://jm.hnjuh.cn

[G05] 继承
来源：http://py.nszjky.cn

Py:   class Admin(User): pass
来源：http://bb.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://ee.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://qw.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://ty.shxzukj.cn

Java: class Admin extends User {}
来源：http://zn.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vl.521024.cn

Ruby: class Admin < User; end
来源：http://sq.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ik.huixiangedu.cn

[G06] 重写方法
来源：http://jt.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://wa.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://de.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://wn.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://tr.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://bi.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yf.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://iq.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://ea.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://sm.hahajie.cn

Py:   super().greet()
来源：http://bg.yuexingan06.cn

PHP:  parent::greet();
来源：http://lc.nszjky.cn

JS:   super.greet();
来源：http://kb.chemitech.net.cn

TS:   super.greet();
来源：http://ow.muxihuayi.cn

Java: super.greet();
来源：http://pr.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sv.9csxet.cn

Ruby: super
来源：http://ru.huixiangedu.cn

C#:   base.Greet();
来源：http://lq.hnjuh.cn

[G08] 静态方法与属性
来源：http://ti.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://am.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://gd.wgjwhj.cn

JS:   static f() {}
来源：http://ai.nicolike.cn

TS:   static f(): void {}
来源：http://iq.huixiangedu.cn

Java: static void f() {}
来源：http://cy.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://em.shxzukj.cn

Ruby: def self.f; end
来源：http://wk.yuexingan06.cn

C#:   public static void F() {}
来源：http://kv.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://li.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://vt.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bj.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nn.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://fg.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://sp.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://om.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zk.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://mc.yuexingan06.cn

[G10] 访问控制
来源：http://yz.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://cj.521024.cn

PHP:  public / protected / private
来源：http://rh.szsharing.cn

JS:   #private 字段；其余公开
来源：http://cf.shxzskj.cn

TS:   public / protected / private
来源：http://my.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://ne.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://il.521024.cn

Ruby: public / protected / private
来源：http://zj.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://sh.gzmigu.cn

[G11] getter / setter
来源：http://ie.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://ej.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ou.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://dz.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://oa.szxytkj.cn

Java: public String getName() { return name; }
来源：http://bc.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oq.9csxet.cn

Ruby: attr_accessor :name
来源：http://xr.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://yt.521024.cn

[G12] 对象转字符串
来源：http://by.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://sq.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ri.huanxung.cn

JS:   toString() { return this.name; }
来源：http://jj.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://tv.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://vf.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qa.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://iy.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://xt.jctech888.com.cn

[G13] 判断对象类型
来源：http://dr.gzmigu.cn

Py:   isinstance(u, User)
来源：http://fn.chemitech.net.cn

PHP:  $u instanceof User
来源：http://ke.chemitech.net.cn

JS:   u instanceof User
来源：http://ka.colortex.cn

TS:   u instanceof User
来源：http://jb.colortex.cn

Java: u instanceof User
来源：http://dp.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://je.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://ff.shxzskj.cn

C#:   u is User
来源：http://ck.muxihuayi.cn

[G14] 数据类 / record
来源：http://hx.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://es.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://jx.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eq.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://vl.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://st.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://dy.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gd.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://nl.wgjwhj.cn

[G15] 枚举
来源：http://yk.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mj.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zf.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uc.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mm.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://vz.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oe.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://nj.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://js.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://lo.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mq.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://md.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://dz.nszjky.cn

TS:   Object.entries(obj)
来源：http://ht.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zt.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wu.huanxung.cn

Ruby: obj.instance_variables
来源：http://ca.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://oo.muxihuayi.cn

================================================================================
来源：http://tv.gzmigu.cn

H. 异常与错误处理
来源：http://re.huixiangedu.cn

================================================================================
来源：http://xt.shxzskj.cn

[H01] try / catch 基础
来源：http://vq.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://im.jctech888.com.cn


<!-- 参考信息 -->