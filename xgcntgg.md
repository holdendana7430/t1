代发 wailian999

PHP:  number_format(1234567);
来源：http://uq.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ky.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zb.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lp.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qx.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xn.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://rk.521024.cn

[E17] 首字母大写
来源：http://yv.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fd.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qh.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vw.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xl.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tl.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vn.huixiangedu.cn

Ruby: s.capitalize
来源：http://ze.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ly.shxzukj.cn

[E18] 模板占位符替换
来源：http://gh.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yj.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ae.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lo.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://em.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ep.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fs.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sl.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ga.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://yh.shxzukj.cn

Py:   s.splitlines()
来源：http://np.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qx.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://qs.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://ay.shxzukj.cn

Java: s.lines().toList()
来源：http://lc.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://cn.huixiangedu.cn

Ruby: s.lines
来源：http://cw.huixiangedu.cn

C#:   s.Split('\n')
来源：http://be.nszjky.cn

[E20] 判断字符串是否为空
来源：http://sn.asd995.cn

Py:   if not s:
来源：http://cg.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qu.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gk.shtwfgs.cn

TS:   if (s === "") {}
来源：http://ct.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://fc.szxytkj.cn

Go:   if s == "" {}
来源：http://ty.nicolike.cn

Ruby: if s.empty?
来源：http://zb.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ci.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://fo.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sb.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rp.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tr.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tt.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ig.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://yt.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rx.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sn.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://vt.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lb.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pw.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gt.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://of.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://id.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aw.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://at.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sd.shtwfgs.cn

================================================================================
来源：http://uz.yuexingan06.cn

F. 文件与目录
来源：http://ml.nicolike.cn

================================================================================
来源：http://fs.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://qy.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wn.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://kj.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qb.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ef.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://au.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wi.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://an.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://sd.panjiajie.cn

[F02] 逐行读取文件
来源：http://ox.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ka.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zf.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vc.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aw.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jd.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pn.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bu.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wu.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://bi.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bq.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mu.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gb.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xy.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oj.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qg.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://sz.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tf.haigaiapp.cn

[F04] 追加写入文件
来源：http://ap.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cd.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bq.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://go.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ec.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://af.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rk.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jz.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qp.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://pc.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mz.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://sg.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://ph.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://uq.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://em.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hh.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://vz.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://ue.jianghongdianzi.cn

[F06] 删除文件
来源：http://oe.521024.cn

Py:   os.remove("a.txt")
来源：http://ia.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://va.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ar.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ez.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yi.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://ly.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://ax.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://mx.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://rz.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://md.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rb.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jn.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://no.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vk.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vp.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mw.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zx.9csxet.cn

[F08] 遍历目录
来源：http://ql.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qv.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wq.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://ag.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://xt.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://og.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://it.hahajie.cn

Ruby: Dir.children("dir")
来源：http://zr.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://ts.gzmigu.cn

[F09] 获取文件大小
来源：http://dk.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://pk.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://mi.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://sl.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://cd.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ct.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qv.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://gc.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://ev.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://jh.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://da.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ff.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ti.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://qn.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fe.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hv.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://it.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tt.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://kq.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sj.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fr.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ys.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rd.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ai.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uz.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://af.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mv.gzmigu.cn

[F12] CSV 读写
来源：http://wb.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mh.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uw.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ax.huixiangedu.cn

TS:   // 同上
来源：http://ou.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ws.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wi.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ep.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uw.bookmarksfly.cn

================================================================================
来源：http://fi.gzmigu.cn

G. 面向对象
来源：http://ou.shxzskj.cn

================================================================================
来源：http://mh.shxzskj.cn

[G01] 定义类
来源：http://qd.jianghongdianzi.cn

Py:   class User: pass
来源：http://eg.jctech888.com.cn

PHP:  class User {}
来源：http://zp.shxzskj.cn

JS:   class User {}
来源：http://kd.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://hm.szsharing.cn

Java: class User {}
来源：http://zr.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://dg.muxihuayi.cn

Ruby: class User; end
来源：http://tq.huixiangedu.cn

C#:   class User {}
来源：http://tb.bjjhwx.cn

[G02] 构造函数
来源：http://rc.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://pj.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://pv.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://fv.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://hy.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://hs.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nh.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://ae.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://wm.bjjhwx.cn

[G03] 实例属性
来源：http://eg.asd995.cn

Py:   self.name = "x"
来源：http://qv.shxzukj.cn

PHP:  public string $name = "x";
来源：http://eu.shxzskj.cn

JS:   this.name = "x";
来源：http://af.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://qi.yuexingan06.cn

Java: private String name;
来源：http://na.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gy.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://ha.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://uy.shtwfgs.cn

[G04] 定义方法
来源：http://vi.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://sk.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uk.hahajie.cn

JS:   greet() { return this.name; }
来源：http://uf.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://aj.gzmigu.cn

Java: String greet() { return name; }
来源：http://mk.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mt.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://ox.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://uw.jianghongdianzi.cn

[G05] 继承
来源：http://qc.nicolike.cn

Py:   class Admin(User): pass
来源：http://tl.asd995.cn

PHP:  class Admin extends User {}
来源：http://cd.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://pf.panjiajie.cn

TS:   class Admin extends User {}
来源：http://bh.shtwfgs.cn

Java: class Admin extends User {}
来源：http://si.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://du.colortex.cn

Ruby: class Admin < User; end
来源：http://jc.huixiangedu.cn

C#:   class Admin : User {}
来源：http://re.szxytkj.cn

[G06] 重写方法
来源：http://ku.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://vf.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bl.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://xy.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://xj.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://yn.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zl.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://so.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://et.asd995.cn

[G07] 调用父类方法
来源：http://wh.hnjuh.cn

Py:   super().greet()
来源：http://du.panjiajie.cn

PHP:  parent::greet();
来源：http://ie.colortex.cn

JS:   super.greet();
来源：http://hl.asd995.cn

TS:   super.greet();
来源：http://zu.shxzukj.cn

Java: super.greet();
来源：http://bm.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qy.hnjuh.cn

Ruby: super
来源：http://oi.hahajie.cn

C#:   base.Greet();
来源：http://we.lnxyls.cn

[G08] 静态方法与属性
来源：http://ur.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ik.panjiajie.cn

PHP:  public static function f() {}
来源：http://at.hnjuh.cn

JS:   static f() {}
来源：http://he.muxihuayi.cn

TS:   static f(): void {}
来源：http://pr.huanxung.cn

Java: static void f() {}
来源：http://bq.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tn.colortex.cn

Ruby: def self.f; end
来源：http://ky.hahajie.cn

C#:   public static void F() {}
来源：http://eq.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://ha.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://fl.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mb.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ge.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://hj.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://fd.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://ry.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ld.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://vc.colortex.cn

[G10] 访问控制
来源：http://os.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://fi.nszjky.cn

PHP:  public / protected / private
来源：http://dm.asd995.cn

JS:   #private 字段；其余公开
来源：http://ps.hnjuh.cn

TS:   public / protected / private
来源：http://wc.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://vb.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wo.gzmigu.cn

Ruby: public / protected / private
来源：http://bx.szxytkj.cn

C#:   public / protected / private / internal
来源：http://tu.nszjky.cn

[G11] getter / setter
来源：http://qm.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://cn.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ds.huanxung.cn

JS:   get name() { return this._name; }
来源：http://gx.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://cw.9csxet.cn

Java: public String getName() { return name; }
来源：http://kx.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qk.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://fz.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://zv.huanxung.cn

[G12] 对象转字符串
来源：http://pn.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://wu.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://az.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://ed.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://gr.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://ut.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qj.521024.cn

Ruby: def to_s; @name; end
来源：http://sr.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://rq.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://ep.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://gc.szxytkj.cn

PHP:  $u instanceof User
来源：http://wo.hahajie.cn

JS:   u instanceof User
来源：http://qi.panjiajie.cn

TS:   u instanceof User
来源：http://xh.huanxung.cn

Java: u instanceof User
来源：http://gm.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sz.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://co.nicolike.cn

C#:   u is User
来源：http://np.chemitech.net.cn

[G14] 数据类 / record
来源：http://th.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ou.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://uj.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yy.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://ya.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://jx.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://wv.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ld.yuexingan06.cn


<!-- 参考信息 -->