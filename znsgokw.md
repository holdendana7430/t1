代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://ss.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://rb.521024.cn

Java: s.lines().toList()
来源：http://qy.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://dc.muxihuayi.cn

Ruby: s.lines
来源：http://mp.colortex.cn

C#:   s.Split('\n')
来源：http://px.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://fn.wgjwhj.cn

Py:   if not s:
来源：http://ko.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tr.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ho.muxihuayi.cn

TS:   if (s === "") {}
来源：http://qr.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://oy.shtwfgs.cn

Go:   if s == "" {}
来源：http://la.colortex.cn

Ruby: if s.empty?
来源：http://vk.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ky.szsharing.cn

[E21] 超长截断加省略号
来源：http://pe.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://er.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://es.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wc.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gv.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vj.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://wx.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ti.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xu.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://fq.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ay.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gm.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://li.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://er.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vs.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cz.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://kh.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://io.haigaiapp.cn

================================================================================
来源：http://kl.muxihuayi.cn

F. 文件与目录
来源：http://ew.colortex.cn

================================================================================
来源：http://nc.colortex.cn

[F01] 读取整个文件
来源：http://fk.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ml.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://iq.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lp.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nb.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bb.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://un.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://sb.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://jk.shxzukj.cn

[F02] 逐行读取文件
来源：http://ia.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ci.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gn.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qj.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fk.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ei.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nl.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nz.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cm.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://zt.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dn.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rr.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pv.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ua.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qb.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://js.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://xl.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mv.muxihuayi.cn

[F04] 追加写入文件
来源：http://sp.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yy.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dp.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://td.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ij.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aw.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dj.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ha.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wg.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://zu.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ag.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://fc.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://hf.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://qv.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uv.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zo.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://vg.colortex.cn

C#:   File.Exists("a.txt")
来源：http://vh.hnjuh.cn

[F06] 删除文件
来源：http://jp.nicolike.cn

Py:   os.remove("a.txt")
来源：http://mn.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://fy.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jf.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ty.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iq.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://pw.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://jm.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://pd.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://fb.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hb.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mn.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://me.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ul.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qq.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yo.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://te.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wu.shxzukj.cn

[F08] 遍历目录
来源：http://kk.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://by.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rn.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://ad.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://lq.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ct.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yp.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://pz.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://fp.muxihuayi.cn

[F09] 获取文件大小
来源：http://mc.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://ym.szsharing.cn

PHP:  filesize("a.txt");
来源：http://ra.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://ts.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://nl.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xl.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fd.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://oz.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://ys.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://rs.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ie.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nd.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://me.newstarts.cn

TS:   path.extname("a.txt")
来源：http://ua.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ns.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ce.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ic.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xl.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://sl.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gk.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qn.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://po.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ui.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yp.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fw.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pw.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zi.gzmigu.cn

[F12] CSV 读写
来源：http://aw.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ue.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vu.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://os.nicolike.cn

TS:   // 同上
来源：http://cy.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eg.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oz.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xd.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nf.shxzskj.cn

================================================================================
来源：http://hm.shxzukj.cn

G. 面向对象
来源：http://gk.shxzskj.cn

================================================================================
来源：http://ie.hnjuh.cn

[G01] 定义类
来源：http://rz.shxzukj.cn

Py:   class User: pass
来源：http://ms.nicolike.cn

PHP:  class User {}
来源：http://zu.szsharing.cn

JS:   class User {}
来源：http://mz.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://ub.nszjky.cn

Java: class User {}
来源：http://gg.shxzskj.cn

Go:   type User struct { Name string }
来源：http://nn.nicolike.cn

Ruby: class User; end
来源：http://dj.muxihuayi.cn

C#:   class User {}
来源：http://ch.hnjuh.cn

[G02] 构造函数
来源：http://ww.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://xq.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://uv.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://ql.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://iu.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://ts.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cl.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://oe.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://hk.jianghongdianzi.cn

[G03] 实例属性
来源：http://jv.shtwfgs.cn

Py:   self.name = "x"
来源：http://in.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://qw.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://uj.521024.cn

TS:   name: string = "x";
来源：http://at.hahajie.cn

Java: private String name;
来源：http://rp.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pt.chemitech.net.cn

Ruby: @name = "x"
来源：http://pc.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://gy.yuntaijiaju.cn

[G04] 定义方法
来源：http://ez.colortex.cn

Py:   def greet(self): return self.name
来源：http://il.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rz.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://sm.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://tm.gzmigu.cn

Java: String greet() { return name; }
来源：http://qd.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ds.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://mo.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://ac.asd995.cn

[G05] 继承
来源：http://np.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://fh.nszjky.cn

PHP:  class Admin extends User {}
来源：http://ce.asd995.cn

JS:   class Admin extends User {}
来源：http://tw.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://os.nicolike.cn

Java: class Admin extends User {}
来源：http://wh.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ik.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://jj.bjjhwx.cn

C#:   class Admin : User {}
来源：http://rs.yuntaijiaju.cn

[G06] 重写方法
来源：http://ye.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://qq.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jp.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://dg.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://ji.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://le.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oq.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://yg.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://vm.panjiajie.cn

[G07] 调用父类方法
来源：http://nn.wgjwhj.cn

Py:   super().greet()
来源：http://jf.haigaiapp.cn

PHP:  parent::greet();
来源：http://kt.521024.cn

JS:   super.greet();
来源：http://kk.nicolike.cn

TS:   super.greet();
来源：http://jb.asd995.cn

Java: super.greet();
来源：http://kc.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ie.haigaiapp.cn

Ruby: super
来源：http://xv.jianghongdianzi.cn

C#:   base.Greet();
来源：http://ej.nicolike.cn

[G08] 静态方法与属性
来源：http://yg.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ux.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://vc.panjiajie.cn

JS:   static f() {}
来源：http://qn.asd995.cn

TS:   static f(): void {}
来源：http://tz.asd995.cn

Java: static void f() {}
来源：http://tf.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fb.szxytkj.cn

Ruby: def self.f; end
来源：http://on.asd995.cn

C#:   public static void F() {}
来源：http://za.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://sl.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://tc.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qm.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tf.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://jc.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://qk.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://bg.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hl.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://ik.nicolike.cn

[G10] 访问控制
来源：http://yt.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://ba.szsharing.cn

PHP:  public / protected / private
来源：http://jt.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://rq.haigaiapp.cn

TS:   public / protected / private
来源：http://ah.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://jq.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://co.9csxet.cn

Ruby: public / protected / private
来源：http://mo.lnxyls.cn

C#:   public / protected / private / internal
来源：http://st.bookmarksfly.cn

[G11] getter / setter
来源：http://nl.huanxung.cn

Py:   @property 与 @x.setter
来源：http://fm.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://is.huanxung.cn

JS:   get name() { return this._name; }
来源：http://fa.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://mm.521024.cn

Java: public String getName() { return name; }
来源：http://fb.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://op.shxzukj.cn

Ruby: attr_accessor :name
来源：http://se.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://hy.newstarts.cn

[G12] 对象转字符串
来源：http://ku.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://qu.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cu.huanxung.cn

JS:   toString() { return this.name; }
来源：http://os.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://hb.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://nm.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rb.hahajie.cn

Ruby: def to_s; @name; end
来源：http://fw.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://er.panjiajie.cn

[G13] 判断对象类型
来源：http://yw.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://wy.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://xe.nszjky.cn

JS:   u instanceof User
来源：http://ns.9csxet.cn

TS:   u instanceof User
来源：http://ep.nszjky.cn

Java: u instanceof User
来源：http://hw.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bt.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://sa.hnjuh.cn

C#:   u is User
来源：http://bz.shxzskj.cn

[G14] 数据类 / record
来源：http://dy.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nm.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://zj.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://al.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://op.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://vp.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://wr.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vc.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://ld.nszjky.cn

[G15] 枚举
来源：http://eq.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qu.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yd.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ei.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yz.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://ch.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uh.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://nc.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lh.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://yw.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xo.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://so.huanxung.cn

JS:   Object.entries(obj)
来源：http://ri.colortex.cn

TS:   Object.entries(obj)
来源：http://jt.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://or.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://na.colortex.cn

Ruby: obj.instance_variables
来源：http://ol.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://gi.lnxyls.cn

================================================================================
来源：http://mk.huanxung.cn

H. 异常与错误处理
来源：http://wd.huixiangedu.cn

================================================================================
来源：http://ip.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://bj.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ao.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nz.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pa.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://is.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uw.newstarts.cn


<!-- 参考信息 -->