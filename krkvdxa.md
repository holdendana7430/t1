代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wa.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jz.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lw.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jw.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gh.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://os.huanxung.cn

Ruby: s.capitalize
来源：http://bh.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ma.haigaiapp.cn

[E18] 模板占位符替换
来源：http://ws.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hq.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bf.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kb.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tt.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ae.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nj.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ot.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gf.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://cd.huanxung.cn

Py:   s.splitlines()
来源：http://yr.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vu.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://bn.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://fd.szxytkj.cn

Java: s.lines().toList()
来源：http://jr.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://wh.hahajie.cn

Ruby: s.lines
来源：http://fo.szxytkj.cn

C#:   s.Split('\n')
来源：http://xl.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://os.shxzskj.cn

Py:   if not s:
来源：http://ek.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://np.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lr.gzmigu.cn

TS:   if (s === "") {}
来源：http://np.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://tx.gzmigu.cn

Go:   if s == "" {}
来源：http://az.bjjhwx.cn

Ruby: if s.empty?
来源：http://xe.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tf.huanxung.cn

[E21] 超长截断加省略号
来源：http://nd.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tb.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://va.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bf.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hl.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ve.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://cf.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gj.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fz.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://gt.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yk.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eg.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ui.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iq.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jk.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ew.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://zr.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sd.jctech888.com.cn

================================================================================
来源：http://qn.jctech888.com.cn

F. 文件与目录
来源：http://ds.szsharing.cn

================================================================================
来源：http://gr.521024.cn

[F01] 读取整个文件
来源：http://ag.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ao.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://yw.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iu.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fm.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cq.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eq.521024.cn

Ruby: File.read("a.txt")
来源：http://sx.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://ru.huanxung.cn

[F02] 逐行读取文件
来源：http://ml.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uy.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xz.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kb.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ue.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uf.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pr.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cl.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lq.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://fo.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wg.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://af.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fp.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ec.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dc.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eb.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://wj.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zs.shxzskj.cn

[F04] 追加写入文件
来源：http://at.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yy.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vc.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mu.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ww.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jw.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wl.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rs.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mr.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://lm.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kk.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://et.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://ac.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://uf.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hm.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mx.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://to.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://kw.shtwfgs.cn

[F06] 删除文件
来源：http://ta.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://ev.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://zt.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://af.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uf.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eb.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ws.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://oa.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://bx.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://zm.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hd.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uo.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cx.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wa.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ms.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ny.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tw.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rp.521024.cn

[F08] 遍历目录
来源：http://ix.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vp.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pd.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://af.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://eu.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tu.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cv.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://sl.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://hg.newstarts.cn

[F09] 获取文件大小
来源：http://ol.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://ss.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ca.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://ee.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://oe.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lw.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xn.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://ga.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://sw.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://ab.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mh.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wm.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kh.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://ba.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eq.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xh.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tx.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vt.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://xw.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rk.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tk.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ep.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kb.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zu.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://br.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vz.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pi.shxzukj.cn

[F12] CSV 读写
来源：http://ol.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gy.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zu.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ie.huixiangedu.cn

TS:   // 同上
来源：http://so.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fu.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jl.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ax.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dd.hnjuh.cn

================================================================================
来源：http://ib.szxytkj.cn

G. 面向对象
来源：http://ck.szxytkj.cn

================================================================================
来源：http://we.colortex.cn

[G01] 定义类
来源：http://iz.gzmigu.cn

Py:   class User: pass
来源：http://qk.jianghongdianzi.cn

PHP:  class User {}
来源：http://zu.nszjky.cn

JS:   class User {}
来源：http://tu.colortex.cn

TS:   class User { name: string = ""; }
来源：http://ai.szxytkj.cn

Java: class User {}
来源：http://ao.shxzukj.cn

Go:   type User struct { Name string }
来源：http://jd.bookmarksfly.cn

Ruby: class User; end
来源：http://sm.shxzskj.cn

C#:   class User {}
来源：http://lx.lnxyls.cn

[G02] 构造函数
来源：http://ey.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://jv.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://vp.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://qj.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://ri.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://ph.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ha.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://cu.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://kr.nszjky.cn

[G03] 实例属性
来源：http://aq.huanxung.cn

Py:   self.name = "x"
来源：http://us.szxytkj.cn

PHP:  public string $name = "x";
来源：http://xu.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://tn.muxihuayi.cn

TS:   name: string = "x";
来源：http://lg.bookmarksfly.cn

Java: private String name;
来源：http://jz.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kx.shxzskj.cn

Ruby: @name = "x"
来源：http://do.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://as.hahajie.cn

[G04] 定义方法
来源：http://bo.9csxet.cn

Py:   def greet(self): return self.name
来源：http://lt.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pc.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://sl.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://tp.panjiajie.cn

Java: String greet() { return name; }
来源：http://pr.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qa.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://pj.nszjky.cn

C#:   public string Greet() => Name;
来源：http://id.shxzskj.cn

[G05] 继承
来源：http://kj.nszjky.cn

Py:   class Admin(User): pass
来源：http://fy.nszjky.cn

PHP:  class Admin extends User {}
来源：http://ne.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://qd.huanxung.cn

TS:   class Admin extends User {}
来源：http://nk.hahajie.cn

Java: class Admin extends User {}
来源：http://oh.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xy.szsharing.cn

Ruby: class Admin < User; end
来源：http://zl.huanxung.cn

C#:   class Admin : User {}
来源：http://uz.9csxet.cn

[G06] 重写方法
来源：http://io.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://hc.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yq.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://ub.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://nx.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://rt.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ug.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://lh.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://fu.hahajie.cn

[G07] 调用父类方法
来源：http://oh.lnxyls.cn

Py:   super().greet()
来源：http://ud.hnjuh.cn

PHP:  parent::greet();
来源：http://lz.bookmarksfly.cn

JS:   super.greet();
来源：http://jw.huixinmuqiang.cn

TS:   super.greet();
来源：http://fa.wgjwhj.cn

Java: super.greet();
来源：http://gp.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ez.shxzskj.cn

Ruby: super
来源：http://ht.asd995.cn

C#:   base.Greet();
来源：http://zf.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://bb.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://to.lnxyls.cn

PHP:  public static function f() {}
来源：http://st.haigaiapp.cn

JS:   static f() {}
来源：http://bo.asd995.cn

TS:   static f(): void {}
来源：http://ji.huixiangedu.cn

Java: static void f() {}
来源：http://io.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fk.asd995.cn

Ruby: def self.f; end
来源：http://iq.shxzskj.cn

C#:   public static void F() {}
来源：http://sz.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://mm.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://fx.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hl.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xn.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://qt.521024.cn

Java: interface Shape { double area(); }
来源：http://ky.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ih.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jp.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://uj.hahajie.cn

[G10] 访问控制
来源：http://pt.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://gv.shxzskj.cn

PHP:  public / protected / private
来源：http://tz.521024.cn

JS:   #private 字段；其余公开
来源：http://bk.panjiajie.cn

TS:   public / protected / private
来源：http://ra.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://kz.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ec.colortex.cn

Ruby: public / protected / private
来源：http://ax.521024.cn

C#:   public / protected / private / internal
来源：http://bl.shtwfgs.cn

[G11] getter / setter
来源：http://um.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://ic.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oc.asd995.cn

JS:   get name() { return this._name; }
来源：http://vw.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://xf.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://qa.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hb.szxytkj.cn

Ruby: attr_accessor :name
来源：http://xk.521024.cn

C#:   public string Name { get; set; }
来源：http://xt.nicolike.cn

[G12] 对象转字符串
来源：http://ut.asd995.cn

Py:   def __str__(self): return self.name
来源：http://ea.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mp.newstarts.cn

JS:   toString() { return this.name; }
来源：http://tw.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://jk.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://vx.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vf.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://lp.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://wo.huixiangedu.cn

[G13] 判断对象类型
来源：http://ia.nicolike.cn

Py:   isinstance(u, User)
来源：http://cl.hnjuh.cn

PHP:  $u instanceof User
来源：http://wq.huanxung.cn

JS:   u instanceof User
来源：http://pk.huixiangedu.cn

TS:   u instanceof User
来源：http://kx.szsharing.cn

Java: u instanceof User
来源：http://sq.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pp.asd995.cn

Ruby: u.is_a?(User)
来源：http://kq.shxzskj.cn

C#:   u is User
来源：http://zh.yuexingan06.cn

[G14] 数据类 / record
来源：http://hn.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hj.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://jf.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xk.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://ll.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://jz.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://uz.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gh.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://fl.wgjwhj.cn

[G15] 枚举
来源：http://ek.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vp.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dm.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://to.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fw.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://wr.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kk.bjjhwx.cn


<!-- 参考信息 -->