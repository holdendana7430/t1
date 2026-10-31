代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uj.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sm.lnxyls.cn

Ruby: s.capitalize
来源：http://uq.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rd.9csxet.cn

[E18] 模板占位符替换
来源：http://vd.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uo.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mt.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uj.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hp.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kw.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mi.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://un.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oq.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://dv.asd995.cn

Py:   s.splitlines()
来源：http://rz.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ea.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://to.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://et.muxihuayi.cn

Java: s.lines().toList()
来源：http://ys.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://ld.colortex.cn

Ruby: s.lines
来源：http://la.hahajie.cn

C#:   s.Split('\n')
来源：http://qc.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://po.newstarts.cn

Py:   if not s:
来源：http://ef.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rk.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zp.haigaiapp.cn

TS:   if (s === "") {}
来源：http://uv.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://lk.haigaiapp.cn

Go:   if s == "" {}
来源：http://le.shtwfgs.cn

Ruby: if s.empty?
来源：http://hj.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ns.9csxet.cn

[E21] 超长截断加省略号
来源：http://rj.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jq.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://po.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yu.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cd.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qp.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://uj.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://go.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uk.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://xc.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gz.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hj.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://up.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://em.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mu.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vg.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://vb.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wj.yuntaijiaju.cn

================================================================================
来源：http://zm.newstarts.cn

F. 文件与目录
来源：http://hl.panjiajie.cn

================================================================================
来源：http://ep.nszjky.cn

[F01] 读取整个文件
来源：http://vn.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bh.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://qi.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jw.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fv.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rq.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mm.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://em.chemitech.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://bu.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://xz.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bo.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xi.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://os.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fl.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ji.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jc.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gb.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gj.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://uw.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dm.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ml.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vl.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ic.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ub.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cl.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://bp.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pf.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://wb.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kk.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aw.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ah.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dw.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bi.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ur.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tp.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hn.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://ig.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mx.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://li.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://nq.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://yd.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vw.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://do.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://iy.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://fi.nszjky.cn

[F06] 删除文件
来源：http://qt.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://vz.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://yo.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bg.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ql.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zy.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://xk.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://mb.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://si.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://qj.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jo.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lf.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bw.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qh.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mv.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fk.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iv.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ie.shxzukj.cn

[F08] 遍历目录
来源：http://vq.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oi.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ah.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://uy.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://zl.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yb.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aw.asd995.cn

Ruby: Dir.children("dir")
来源：http://rr.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://yu.shtwfgs.cn

[F09] 获取文件大小
来源：http://ou.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://wd.huanxung.cn

PHP:  filesize("a.txt");
来源：http://eh.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://vo.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://rm.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vz.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ok.huanxung.cn

Ruby: File.size("a.txt")
来源：http://en.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://qm.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ka.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gf.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ca.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yp.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://ya.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ug.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tb.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sw.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jr.huixiangedu.cn

[F11] 复制与移动文件
来源：http://qy.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vd.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fc.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ny.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vt.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fn.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hb.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://he.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://md.huanxung.cn

[F12] CSV 读写
来源：http://il.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://in.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ed.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ku.hahajie.cn

TS:   // 同上
来源：http://ct.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yo.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nf.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fl.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ps.lnxyls.cn

================================================================================
来源：http://ok.shxzskj.cn

G. 面向对象
来源：http://fm.asd995.cn

================================================================================
来源：http://mw.huixinmuqiang.cn

[G01] 定义类
来源：http://bu.szxytkj.cn

Py:   class User: pass
来源：http://zd.nicolike.cn

PHP:  class User {}
来源：http://mo.szsharing.cn

JS:   class User {}
来源：http://lg.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://dh.wgjwhj.cn

Java: class User {}
来源：http://by.nszjky.cn

Go:   type User struct { Name string }
来源：http://as.newstarts.cn

Ruby: class User; end
来源：http://jt.colortex.cn

C#:   class User {}
来源：http://kw.shxzukj.cn

[G02] 构造函数
来源：http://kx.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://eo.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://kp.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://jw.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://uw.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://mz.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rh.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://in.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://tw.bookmarksfly.cn

[G03] 实例属性
来源：http://mt.colortex.cn

Py:   self.name = "x"
来源：http://gf.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://bn.9csxet.cn

JS:   this.name = "x";
来源：http://ml.521024.cn

TS:   name: string = "x";
来源：http://wt.huanxung.cn

Java: private String name;
来源：http://jx.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vu.muxihuayi.cn

Ruby: @name = "x"
来源：http://wm.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://be.shtwfgs.cn

[G04] 定义方法
来源：http://da.521024.cn

Py:   def greet(self): return self.name
来源：http://dw.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ce.huanxung.cn

JS:   greet() { return this.name; }
来源：http://jq.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://hv.shxzskj.cn

Java: String greet() { return name; }
来源：http://wj.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zn.521024.cn

Ruby: def greet; @name; end
来源：http://zx.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://zs.szxytkj.cn

[G05] 继承
来源：http://ob.gzmigu.cn

Py:   class Admin(User): pass
来源：http://cy.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://ge.hahajie.cn

JS:   class Admin extends User {}
来源：http://bo.szxytkj.cn

TS:   class Admin extends User {}
来源：http://fx.huixiangedu.cn

Java: class Admin extends User {}
来源：http://wj.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ea.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://qc.9csxet.cn

C#:   class Admin : User {}
来源：http://jq.gzmigu.cn

[G06] 重写方法
来源：http://mi.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://kl.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iq.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://wt.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://hj.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://hg.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ko.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://el.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://up.nszjky.cn

[G07] 调用父类方法
来源：http://ea.panjiajie.cn

Py:   super().greet()
来源：http://kk.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://kk.nszjky.cn

JS:   super.greet();
来源：http://bs.jianghongdianzi.cn

TS:   super.greet();
来源：http://xb.yuexingan06.cn

Java: super.greet();
来源：http://sw.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qb.bookmarksfly.cn

Ruby: super
来源：http://hs.shxzukj.cn

C#:   base.Greet();
来源：http://mp.hahajie.cn

[G08] 静态方法与属性
来源：http://kn.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cc.szsharing.cn

PHP:  public static function f() {}
来源：http://tq.muxihuayi.cn

JS:   static f() {}
来源：http://kq.szxytkj.cn

TS:   static f(): void {}
来源：http://wt.521024.cn

Java: static void f() {}
来源：http://yn.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jj.jctech888.com.cn

Ruby: def self.f; end
来源：http://xp.huanxung.cn

C#:   public static void F() {}
来源：http://tf.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://mo.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://ui.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rr.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nm.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://kp.asd995.cn

Java: interface Shape { double area(); }
来源：http://wo.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://sr.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://za.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://go.jianghongdianzi.cn

[G10] 访问控制
来源：http://rq.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://ac.bjjhwx.cn

PHP:  public / protected / private
来源：http://kh.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://fj.lnxyls.cn

TS:   public / protected / private
来源：http://bl.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://qw.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dq.colortex.cn

Ruby: public / protected / private
来源：http://mk.lnxyls.cn

C#:   public / protected / private / internal
来源：http://ml.hahajie.cn

[G11] getter / setter
来源：http://lb.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://xb.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mh.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://iv.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ib.nicolike.cn

Java: public String getName() { return name; }
来源：http://an.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dx.asd995.cn

Ruby: attr_accessor :name
来源：http://fe.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://pg.hahajie.cn

[G12] 对象转字符串
来源：http://yw.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://ks.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://td.nicolike.cn

JS:   toString() { return this.name; }
来源：http://pn.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://gh.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://cq.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jb.nszjky.cn

Ruby: def to_s; @name; end
来源：http://tl.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://kx.nicolike.cn

[G13] 判断对象类型
来源：http://rk.521024.cn

Py:   isinstance(u, User)
来源：http://fz.shxzskj.cn

PHP:  $u instanceof User
来源：http://vl.huixinmuqiang.cn

JS:   u instanceof User
来源：http://cm.jctech888.com.cn

TS:   u instanceof User
来源：http://mj.haigaiapp.cn

Java: u instanceof User
来源：http://th.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rq.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://yk.szxytkj.cn

C#:   u is User
来源：http://ct.bookmarksfly.cn

[G14] 数据类 / record
来源：http://fr.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ky.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://vw.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fx.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://mf.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://by.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://gf.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vu.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://ak.chemitech.net.cn

[G15] 枚举
来源：http://re.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wn.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ff.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://js.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rw.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://pk.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dw.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://pa.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dz.asd995.cn

[G16] 对象转数组 / 字典
来源：http://vy.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wn.nszjky.cn


<!-- 参考信息 -->