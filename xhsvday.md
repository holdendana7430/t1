代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://qd.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ps.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tn.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://um.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gd.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://hs.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://hw.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pq.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://si.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://kr.jctech888.com.cn

Java: s.lines().toList()
来源：http://am.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://wm.hahajie.cn

Ruby: s.lines
来源：http://fd.hahajie.cn

C#:   s.Split('\n')
来源：http://xi.nszjky.cn

[E20] 判断字符串是否为空
来源：http://lj.nszjky.cn

Py:   if not s:
来源：http://yr.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rs.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zb.panjiajie.cn

TS:   if (s === "") {}
来源：http://ww.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://zs.521024.cn

Go:   if s == "" {}
来源：http://xz.nszjky.cn

Ruby: if s.empty?
来源：http://cj.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kf.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://qx.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dz.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wi.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://js.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://of.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rt.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://ij.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yv.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oy.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://bq.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nb.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bc.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xx.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sr.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pw.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ft.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://fw.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wo.nszjky.cn

================================================================================
来源：http://qn.yuntaijiaju.cn

F. 文件与目录
来源：http://rh.9csxet.cn

================================================================================
来源：http://nr.szxytkj.cn

[F01] 读取整个文件
来源：http://pp.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nm.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://ea.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cw.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://na.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oz.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wk.nicolike.cn

Ruby: File.read("a.txt")
来源：http://ic.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://xc.hahajie.cn

[F02] 逐行读取文件
来源：http://xh.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xb.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zd.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qy.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://it.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mw.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ad.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lr.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iq.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://rx.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ou.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://up.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ez.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xa.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yd.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gi.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://ea.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lr.huixiangedu.cn

[F04] 追加写入文件
来源：http://ct.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iw.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://og.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bq.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pb.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qx.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rr.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bb.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kw.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://tp.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qw.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://al.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://av.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://lf.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xo.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tl.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://lh.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://yh.yuexingan06.cn

[F06] 删除文件
来源：http://is.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://dr.nszjky.cn

PHP:  unlink("a.txt");
来源：http://sg.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jf.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lv.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pu.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://wq.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://cl.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://yg.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://ob.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qg.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fz.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dg.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ho.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mc.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lz.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pc.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fq.bookmarksfly.cn

[F08] 遍历目录
来源：http://fh.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rq.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xr.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://ov.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://uo.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lw.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nz.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://oy.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://vz.jctech888.com.cn

[F09] 获取文件大小
来源：http://hb.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://oz.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://sq.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://dn.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://hf.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kd.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mn.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://pz.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://mj.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://xk.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vz.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://et.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mq.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://lz.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xm.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lo.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ud.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ja.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://mg.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dh.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hi.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://su.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gi.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fj.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ou.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zb.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mh.hnjuh.cn

[F12] CSV 读写
来源：http://jh.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ry.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pu.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nq.huanxung.cn

TS:   // 同上
来源：http://uo.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mj.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ta.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fr.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fs.huanxung.cn

================================================================================
来源：http://uj.shxzukj.cn

G. 面向对象
来源：http://gr.shxzukj.cn

================================================================================
来源：http://qg.newstarts.cn

[G01] 定义类
来源：http://xe.hnjuh.cn

Py:   class User: pass
来源：http://fi.gzmigu.cn

PHP:  class User {}
来源：http://lr.szsharing.cn

JS:   class User {}
来源：http://zn.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://tt.szsharing.cn

Java: class User {}
来源：http://rq.hahajie.cn

Go:   type User struct { Name string }
来源：http://na.hahajie.cn

Ruby: class User; end
来源：http://zr.szxytkj.cn

C#:   class User {}
来源：http://vn.shxzukj.cn

[G02] 构造函数
来源：http://cn.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://qu.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://mt.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://lz.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://zq.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://su.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gh.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://ii.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://ms.szsharing.cn

[G03] 实例属性
来源：http://kt.colortex.cn

Py:   self.name = "x"
来源：http://zd.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://ci.newstarts.cn

JS:   this.name = "x";
来源：http://ht.huixiangedu.cn

TS:   name: string = "x";
来源：http://ol.521024.cn

Java: private String name;
来源：http://nt.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://op.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://ax.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ko.shxzukj.cn

[G04] 定义方法
来源：http://rr.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://if.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ny.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://tq.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ir.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://dg.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iq.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://kj.asd995.cn

C#:   public string Greet() => Name;
来源：http://ke.huixiangedu.cn

[G05] 继承
来源：http://yy.panjiajie.cn

Py:   class Admin(User): pass
来源：http://vj.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://wp.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://tx.shxzukj.cn

TS:   class Admin extends User {}
来源：http://nv.asd995.cn

Java: class Admin extends User {}
来源：http://ti.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://we.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://qv.shtwfgs.cn

C#:   class Admin : User {}
来源：http://wi.gzmigu.cn

[G06] 重写方法
来源：http://yw.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://rr.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pp.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://km.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://xm.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://mr.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pc.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://zz.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://ob.haigaiapp.cn

[G07] 调用父类方法
来源：http://uu.chemitech.net.cn

Py:   super().greet()
来源：http://pk.colortex.cn

PHP:  parent::greet();
来源：http://rg.9csxet.cn

JS:   super.greet();
来源：http://fh.shxzskj.cn

TS:   super.greet();
来源：http://iu.gzmigu.cn

Java: super.greet();
来源：http://fn.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cv.szxytkj.cn

Ruby: super
来源：http://mw.huixiangedu.cn

C#:   base.Greet();
来源：http://ey.chemitech.net.cn

[G08] 静态方法与属性
来源：http://ah.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hh.chemitech.net.cn

PHP:  public static function f() {}
来源：http://zb.yuexingan06.cn

JS:   static f() {}
来源：http://pg.panjiajie.cn

TS:   static f(): void {}
来源：http://wn.bookmarksfly.cn

Java: static void f() {}
来源：http://gf.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wh.szsharing.cn

Ruby: def self.f; end
来源：http://xd.huixiangedu.cn

C#:   public static void F() {}
来源：http://ms.521024.cn

[G09] 接口 / 抽象类
来源：http://wu.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://we.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nd.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://in.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://gv.szsharing.cn

Java: interface Shape { double area(); }
来源：http://ff.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://ib.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cd.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://ea.hnjuh.cn

[G10] 访问控制
来源：http://rq.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://qa.muxihuayi.cn

PHP:  public / protected / private
来源：http://kh.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://jr.chemitech.net.cn

TS:   public / protected / private
来源：http://et.colortex.cn

Java: public / protected / private / 默认包级
来源：http://af.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jd.yuexingan06.cn

Ruby: public / protected / private
来源：http://lg.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://lj.panjiajie.cn

[G11] getter / setter
来源：http://om.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://gs.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zn.nicolike.cn

JS:   get name() { return this._name; }
来源：http://mb.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://cf.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://xm.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bo.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://ku.colortex.cn

C#:   public string Name { get; set; }
来源：http://rd.lnxyls.cn

[G12] 对象转字符串
来源：http://ra.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://yy.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ks.huanxung.cn

JS:   toString() { return this.name; }
来源：http://hf.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://et.521024.cn

Java: @Override public String toString() { return name; }
来源：http://fa.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://at.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://pk.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://uk.yuexingan06.cn

[G13] 判断对象类型
来源：http://gt.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://cc.wgjwhj.cn

PHP:  $u instanceof User
来源：http://jf.jianghongdianzi.cn

JS:   u instanceof User
来源：http://ud.yuntaijiaju.cn

TS:   u instanceof User
来源：http://fq.chemitech.net.cn

Java: u instanceof User
来源：http://kp.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yi.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://ax.hahajie.cn

C#:   u is User
来源：http://af.9csxet.cn

[G14] 数据类 / record
来源：http://zv.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sw.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://aq.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dy.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://yv.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://tk.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://jn.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://by.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://dn.gzmigu.cn

[G15] 枚举
来源：http://xb.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vj.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ds.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gc.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ob.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://vu.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pv.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://yp.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wj.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://si.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dc.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://bm.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://te.shxzukj.cn

TS:   Object.entries(obj)
来源：http://dt.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://se.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xh.panjiajie.cn

Ruby: obj.instance_variables
来源：http://eh.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ww.bjjhwx.cn

================================================================================
来源：http://os.panjiajie.cn


<!-- 参考信息 -->