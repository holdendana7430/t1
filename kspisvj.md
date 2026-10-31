代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://qx.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://dt.szxytkj.cn

Java: s.lines().toList()
来源：http://dv.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://bp.huixiangedu.cn

Ruby: s.lines
来源：http://ty.9csxet.cn

C#:   s.Split('\n')
来源：http://bv.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://fv.gzmigu.cn

Py:   if not s:
来源：http://vu.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bi.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ox.shxzukj.cn

TS:   if (s === "") {}
来源：http://df.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ly.muxihuayi.cn

Go:   if s == "" {}
来源：http://iy.haigaiapp.cn

Ruby: if s.empty?
来源：http://rl.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://br.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://um.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hp.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jk.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://db.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kb.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hy.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://ks.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pa.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tq.521024.cn

[E22] 字节长度与字符长度
来源：http://ob.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xt.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qh.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hn.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qy.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uu.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zf.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://fl.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oq.lnxyls.cn

================================================================================
来源：http://kz.jianghongdianzi.cn

F. 文件与目录
来源：http://yu.9csxet.cn

================================================================================
来源：http://ce.wgjwhj.cn

[F01] 读取整个文件
来源：http://ps.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xe.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://pm.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rt.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ww.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nk.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tj.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://zq.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ge.521024.cn

[F02] 逐行读取文件
来源：http://wt.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bm.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ml.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vp.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gb.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://it.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ki.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kr.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fm.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://zc.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wm.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iu.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bv.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://or.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jg.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yg.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://bn.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zl.haigaiapp.cn

[F04] 追加写入文件
来源：http://qo.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ka.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vv.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gn.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ek.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ln.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vj.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kx.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://or.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://wj.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hq.521024.cn

PHP:  file_exists("a.txt");
来源：http://ax.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://rl.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://qo.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dr.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dv.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://na.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://bq.yuexingan06.cn

[F06] 删除文件
来源：http://ri.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://fz.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://rl.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jj.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mh.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pn.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://yd.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://qn.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://yg.nszjky.cn

[F07] 创建目录（含多级）
来源：http://xf.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sz.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dj.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oj.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gk.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iu.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ve.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gv.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ia.jianghongdianzi.cn

[F08] 遍历目录
来源：http://jy.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mp.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vh.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://qr.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://tz.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jv.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fs.szsharing.cn

Ruby: Dir.children("dir")
来源：http://kb.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://xe.chemitech.net.cn

[F09] 获取文件大小
来源：http://uv.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://pb.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://go.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://wt.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://bv.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tr.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kn.szsharing.cn

Ruby: File.size("a.txt")
来源：http://tz.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://gk.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://at.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://di.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lr.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oh.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://yq.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tz.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dm.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sd.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yy.panjiajie.cn

[F11] 复制与移动文件
来源：http://vf.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ig.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://am.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yk.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vf.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ty.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kh.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ms.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mg.yuntaijiaju.cn

[F12] CSV 读写
来源：http://wd.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rv.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jz.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xa.shtwfgs.cn

TS:   // 同上
来源：http://op.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mm.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wb.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ca.nszjky.cn

================================================================================
来源：http://qf.hahajie.cn

G. 面向对象
来源：http://dh.bjjhwx.cn

================================================================================
来源：http://nf.shxzukj.cn

[G01] 定义类
来源：http://iz.9csxet.cn

Py:   class User: pass
来源：http://ml.huixinmuqiang.cn

PHP:  class User {}
来源：http://bk.yuexingan06.cn

JS:   class User {}
来源：http://mt.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://bx.yuexingan06.cn

Java: class User {}
来源：http://lw.521024.cn

Go:   type User struct { Name string }
来源：http://kw.lnxyls.cn

Ruby: class User; end
来源：http://ei.szsharing.cn

C#:   class User {}
来源：http://eo.chemitech.net.cn

[G02] 构造函数
来源：http://cr.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://js.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://ow.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://uj.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://ub.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://dr.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eu.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://au.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://ov.jctech888.com.cn

[G03] 实例属性
来源：http://pt.newstarts.cn

Py:   self.name = "x"
来源：http://mn.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://lz.hnjuh.cn

JS:   this.name = "x";
来源：http://sf.lnxyls.cn

TS:   name: string = "x";
来源：http://yg.huanxung.cn

Java: private String name;
来源：http://zw.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bw.szsharing.cn

Ruby: @name = "x"
来源：http://ee.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://wz.shxzskj.cn

[G04] 定义方法
来源：http://ge.521024.cn

Py:   def greet(self): return self.name
来源：http://nt.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xo.newstarts.cn

JS:   greet() { return this.name; }
来源：http://wb.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://zk.lnxyls.cn

Java: String greet() { return name; }
来源：http://ri.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xn.huanxung.cn

Ruby: def greet; @name; end
来源：http://ah.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://db.szxytkj.cn

[G05] 继承
来源：http://ob.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ik.9csxet.cn

PHP:  class Admin extends User {}
来源：http://kq.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://wh.lnxyls.cn

TS:   class Admin extends User {}
来源：http://qk.jctech888.com.cn

Java: class Admin extends User {}
来源：http://uy.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://np.nszjky.cn

Ruby: class Admin < User; end
来源：http://wy.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://xw.colortex.cn

[G06] 重写方法
来源：http://nx.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://ih.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dn.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://qa.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://vh.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://da.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sn.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://ou.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://el.hnjuh.cn

[G07] 调用父类方法
来源：http://ne.huixinmuqiang.cn

Py:   super().greet()
来源：http://da.newstarts.cn

PHP:  parent::greet();
来源：http://ik.panjiajie.cn

JS:   super.greet();
来源：http://sz.hnjuh.cn

TS:   super.greet();
来源：http://ei.colortex.cn

Java: super.greet();
来源：http://wm.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kw.haigaiapp.cn

Ruby: super
来源：http://cm.asd995.cn

C#:   base.Greet();
来源：http://nq.9csxet.cn

[G08] 静态方法与属性
来源：http://bx.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dx.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://uu.huixinmuqiang.cn

JS:   static f() {}
来源：http://mw.jctech888.com.cn

TS:   static f(): void {}
来源：http://my.huixiangedu.cn

Java: static void f() {}
来源：http://aa.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://og.chemitech.net.cn

Ruby: def self.f; end
来源：http://uy.haigaiapp.cn

C#:   public static void F() {}
来源：http://it.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://wo.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://lx.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hv.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wn.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://la.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://nt.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://yg.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oe.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://sa.521024.cn

[G10] 访问控制
来源：http://mb.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://qz.521024.cn

PHP:  public / protected / private
来源：http://rh.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://vy.haigaiapp.cn

TS:   public / protected / private
来源：http://vk.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://qn.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xw.shtwfgs.cn

Ruby: public / protected / private
来源：http://fd.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://kl.newstarts.cn

[G11] getter / setter
来源：http://ue.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://vq.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yn.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://de.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ig.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://sk.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://se.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://bh.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://cj.muxihuayi.cn

[G12] 对象转字符串
来源：http://yk.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://jw.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hx.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://jf.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://ip.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://wj.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wp.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://ay.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://nn.lnxyls.cn

[G13] 判断对象类型
来源：http://ni.colortex.cn

Py:   isinstance(u, User)
来源：http://fa.521024.cn

PHP:  $u instanceof User
来源：http://dw.chemitech.net.cn

JS:   u instanceof User
来源：http://kw.shxzukj.cn

TS:   u instanceof User
来源：http://wv.hahajie.cn

Java: u instanceof User
来源：http://is.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cl.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://dp.9csxet.cn

C#:   u is User
来源：http://gt.colortex.cn

[G14] 数据类 / record
来源：http://lj.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lh.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://iw.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tn.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://ic.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://gi.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://wg.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ta.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://lf.9csxet.cn

[G15] 枚举
来源：http://im.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zm.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cz.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ic.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gg.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://vc.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ln.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://on.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tr.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://pk.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kl.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://li.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://ft.nicolike.cn

TS:   Object.entries(obj)
来源：http://ec.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qw.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://me.hnjuh.cn

Ruby: obj.instance_variables
来源：http://pe.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pf.colortex.cn

================================================================================
来源：http://jz.wgjwhj.cn

H. 异常与错误处理
来源：http://es.shxzskj.cn

================================================================================
来源：http://jz.asd995.cn

[H01] try / catch 基础
来源：http://gm.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xf.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://do.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tb.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xr.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nv.szsharing.cn


<!-- 参考信息 -->