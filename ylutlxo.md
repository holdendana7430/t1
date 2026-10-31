代发 wailian999

[E18] 模板占位符替换
来源：http://eq.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zy.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qo.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://au.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ig.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dn.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hs.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ad.szsharing.cn

[E19] 多行文本按行拆分
来源：http://jd.asd995.cn

Py:   s.splitlines()
来源：http://tr.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tu.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://vk.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://wu.hnjuh.cn

Java: s.lines().toList()
来源：http://ei.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://el.hahajie.cn

Ruby: s.lines
来源：http://lf.huanxung.cn

C#:   s.Split('\n')
来源：http://vt.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://ye.gzmigu.cn

Py:   if not s:
来源：http://vk.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xm.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://we.jctech888.com.cn

TS:   if (s === "") {}
来源：http://fw.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://gb.szsharing.cn

Go:   if s == "" {}
来源：http://vl.shxzskj.cn

Ruby: if s.empty?
来源：http://kc.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yo.szxytkj.cn

[E21] 超长截断加省略号
来源：http://cm.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rz.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zq.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rd.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vd.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cg.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://fz.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wp.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mi.newstarts.cn

[E22] 字节长度与字符长度
来源：http://kd.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jl.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oq.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ka.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ce.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sa.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gf.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://pl.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mt.muxihuayi.cn

================================================================================
来源：http://eb.nicolike.cn

F. 文件与目录
来源：http://do.colortex.cn

================================================================================
来源：http://wp.szsharing.cn

[F01] 读取整个文件
来源：http://vk.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mf.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://kc.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qe.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sv.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lz.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ju.nicolike.cn

Ruby: File.read("a.txt")
来源：http://jh.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://ro.newstarts.cn

[F02] 逐行读取文件
来源：http://cz.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://if.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dc.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hv.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sx.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fh.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qv.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ue.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kg.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://ej.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pu.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bu.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yn.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ad.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ns.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wp.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://gw.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ys.yuexingan06.cn

[F04] 追加写入文件
来源：http://nx.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mb.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nh.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pl.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wr.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oe.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lg.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lv.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iq.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://mm.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ja.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://vz.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://ha.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://cm.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ji.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hn.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://hc.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://gv.haigaiapp.cn

[F06] 删除文件
来源：http://ye.9csxet.cn

Py:   os.remove("a.txt")
来源：http://fg.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://vd.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ll.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vi.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ms.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://lz.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://rp.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://ln.521024.cn

[F07] 创建目录（含多级）
来源：http://jz.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ob.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vb.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tb.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wg.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ho.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zu.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ah.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tv.9csxet.cn

[F08] 遍历目录
来源：http://pa.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jz.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://va.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://jm.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://pr.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ww.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uu.szsharing.cn

Ruby: Dir.children("dir")
来源：http://yk.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://et.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://fd.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://dh.521024.cn

PHP:  filesize("a.txt");
来源：http://ey.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ye.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://hp.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vv.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://go.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://qy.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://lz.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ea.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://au.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dq.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cg.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://cj.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://js.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mq.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ps.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ie.hnjuh.cn

[F11] 复制与移动文件
来源：http://ge.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fs.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zg.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tz.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fk.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://en.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zh.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ys.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zi.panjiajie.cn

[F12] CSV 读写
来源：http://rl.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qn.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ao.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zi.muxihuayi.cn

TS:   // 同上
来源：http://di.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tm.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ac.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bk.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cy.9csxet.cn

================================================================================
来源：http://mc.panjiajie.cn

G. 面向对象
来源：http://gl.lnxyls.cn

================================================================================
来源：http://yd.asd995.cn

[G01] 定义类
来源：http://ax.huanxung.cn

Py:   class User: pass
来源：http://id.haigaiapp.cn

PHP:  class User {}
来源：http://eo.muxihuayi.cn

JS:   class User {}
来源：http://xc.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://pw.hahajie.cn

Java: class User {}
来源：http://kf.shxzskj.cn

Go:   type User struct { Name string }
来源：http://jb.hahajie.cn

Ruby: class User; end
来源：http://cm.huixinmuqiang.cn

C#:   class User {}
来源：http://xh.huanxung.cn

[G02] 构造函数
来源：http://bf.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://sm.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://qs.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://io.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://ud.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://ph.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ui.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://iv.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://hx.colortex.cn

[G03] 实例属性
来源：http://nk.shxzukj.cn

Py:   self.name = "x"
来源：http://pt.asd995.cn

PHP:  public string $name = "x";
来源：http://ch.hnjuh.cn

JS:   this.name = "x";
来源：http://jx.newstarts.cn

TS:   name: string = "x";
来源：http://un.yuexingan06.cn

Java: private String name;
来源：http://cu.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ls.hnjuh.cn

Ruby: @name = "x"
来源：http://ub.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://tr.9csxet.cn

[G04] 定义方法
来源：http://rh.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://lm.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gd.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://yx.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://mo.hahajie.cn

Java: String greet() { return name; }
来源：http://wh.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vg.nicolike.cn

Ruby: def greet; @name; end
来源：http://kk.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://yn.haigaiapp.cn

[G05] 继承
来源：http://mg.shxzskj.cn

Py:   class Admin(User): pass
来源：http://sb.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://rl.huanxung.cn

JS:   class Admin extends User {}
来源：http://iq.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://nk.huanxung.cn

Java: class Admin extends User {}
来源：http://ii.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yt.lnxyls.cn

Ruby: class Admin < User; end
来源：http://oe.bjjhwx.cn

C#:   class Admin : User {}
来源：http://zq.huixiangedu.cn

[G06] 重写方法
来源：http://zj.asd995.cn

Py:   def greet(self): return "admin"
来源：http://gd.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ub.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://pu.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://bq.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://mi.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tz.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://qh.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://nd.nicolike.cn

[G07] 调用父类方法
来源：http://ni.huixiangedu.cn

Py:   super().greet()
来源：http://wr.haigaiapp.cn

PHP:  parent::greet();
来源：http://iv.shxzukj.cn

JS:   super.greet();
来源：http://uf.lnxyls.cn

TS:   super.greet();
来源：http://da.panjiajie.cn

Java: super.greet();
来源：http://tw.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qu.shxzskj.cn

Ruby: super
来源：http://mr.haigaiapp.cn

C#:   base.Greet();
来源：http://iy.lnxyls.cn

[G08] 静态方法与属性
来源：http://ku.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ep.9csxet.cn

PHP:  public static function f() {}
来源：http://va.9csxet.cn

JS:   static f() {}
来源：http://hr.haigaiapp.cn

TS:   static f(): void {}
来源：http://op.colortex.cn

Java: static void f() {}
来源：http://tt.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hj.hahajie.cn

Ruby: def self.f; end
来源：http://wq.nszjky.cn

C#:   public static void F() {}
来源：http://ol.hahajie.cn

[G09] 接口 / 抽象类
来源：http://cx.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://jf.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bb.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wt.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://ln.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://ov.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://al.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kg.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://pe.shxzskj.cn

[G10] 访问控制
来源：http://os.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://de.bookmarksfly.cn

PHP:  public / protected / private
来源：http://lq.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://md.shxzskj.cn

TS:   public / protected / private
来源：http://xt.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://yh.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ls.jctech888.com.cn

Ruby: public / protected / private
来源：http://zi.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://vz.jianghongdianzi.cn

[G11] getter / setter
来源：http://fy.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://zf.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jj.521024.cn

JS:   get name() { return this._name; }
来源：http://vg.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://tm.newstarts.cn

Java: public String getName() { return name; }
来源：http://in.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fz.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://qv.521024.cn

C#:   public string Name { get; set; }
来源：http://fi.haigaiapp.cn

[G12] 对象转字符串
来源：http://ze.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://kx.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fp.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://rd.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://wp.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://zb.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pj.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://kd.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://ma.9csxet.cn

[G13] 判断对象类型
来源：http://qa.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://kx.shtwfgs.cn

PHP:  $u instanceof User
来源：http://ai.huixiangedu.cn

JS:   u instanceof User
来源：http://qb.shxzskj.cn

TS:   u instanceof User
来源：http://es.muxihuayi.cn

Java: u instanceof User
来源：http://wq.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hi.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://md.colortex.cn

C#:   u is User
来源：http://fm.chemitech.net.cn

[G14] 数据类 / record
来源：http://gn.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fh.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://mr.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://id.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://tj.hahajie.cn

Java: record User(String name, int age) {}
来源：http://it.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://cr.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ko.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://yi.szsharing.cn

[G15] 枚举
来源：http://yp.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://my.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jl.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pk.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wq.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://lg.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jt.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://da.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ml.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://iu.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qu.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://ng.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://ls.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://kx.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://br.muxihuayi.cn


<!-- 参考信息 -->