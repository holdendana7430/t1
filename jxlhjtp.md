代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cw.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jk.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://em.bookmarksfly.cn

[E17] 首字母大写
来源：http://rx.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ax.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qg.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dn.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ap.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vp.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mw.shtwfgs.cn

Ruby: s.capitalize
来源：http://bx.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ll.haigaiapp.cn

[E18] 模板占位符替换
来源：http://vx.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ee.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cb.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cx.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hc.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xi.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://de.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mv.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://er.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://xq.asd995.cn

Py:   s.splitlines()
来源：http://ki.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xd.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://hh.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://sg.szsharing.cn

Java: s.lines().toList()
来源：http://kw.521024.cn

Go:   strings.Split(s, "\n")
来源：http://gg.hnjuh.cn

Ruby: s.lines
来源：http://ez.nszjky.cn

C#:   s.Split('\n')
来源：http://gh.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://lq.huixinmuqiang.cn

Py:   if not s:
来源：http://iw.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rj.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qj.9csxet.cn

TS:   if (s === "") {}
来源：http://my.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://wg.wgjwhj.cn

Go:   if s == "" {}
来源：http://du.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://ow.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pk.nszjky.cn

[E21] 超长截断加省略号
来源：http://nt.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://on.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rw.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://li.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wt.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ck.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://lu.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ux.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uf.newstarts.cn

[E22] 字节长度与字符长度
来源：http://of.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fy.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fi.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wy.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ml.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gy.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wa.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://pt.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zr.gzmigu.cn

================================================================================
来源：http://nz.9csxet.cn

F. 文件与目录
来源：http://lx.gzmigu.cn

================================================================================
来源：http://sl.521024.cn

[F01] 读取整个文件
来源：http://zc.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wa.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://el.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dc.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ha.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yw.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ju.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://wv.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://zn.szsharing.cn

[F02] 逐行读取文件
来源：http://pv.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dh.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uv.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nv.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fx.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jc.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cr.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zd.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fy.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://ps.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ut.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ki.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kw.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bp.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ju.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://di.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://ie.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hv.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://gg.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ce.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sp.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xr.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ee.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sq.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hn.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rt.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yb.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://lf.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xv.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://ri.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://sd.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://yc.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bv.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ta.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://nm.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://np.shxzukj.cn

[F06] 删除文件
来源：http://ot.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://tw.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://oi.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ae.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://te.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ls.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://sa.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://rk.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://cs.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://de.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rm.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://my.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ly.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mx.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pq.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nf.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ta.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jz.colortex.cn

[F08] 遍历目录
来源：http://pi.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dq.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sj.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://jy.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://xs.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nl.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kq.asd995.cn

Ruby: Dir.children("dir")
来源：http://ig.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://kj.nicolike.cn

[F09] 获取文件大小
来源：http://ra.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://rt.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://va.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://rw.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ud.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ns.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aw.hahajie.cn

Ruby: File.size("a.txt")
来源：http://rp.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://il.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://zo.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://au.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qb.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uz.colortex.cn

TS:   path.extname("a.txt")
来源：http://fy.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pz.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://na.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://he.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fe.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://gv.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bm.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ln.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nz.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uk.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fy.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zw.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jf.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dr.yuntaijiaju.cn

[F12] CSV 读写
来源：http://cg.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fj.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://br.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tc.wgjwhj.cn

TS:   // 同上
来源：http://sw.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cl.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fw.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ef.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pl.szxytkj.cn

================================================================================
来源：http://qo.hahajie.cn

G. 面向对象
来源：http://bg.huanxung.cn

================================================================================
来源：http://ah.shxzskj.cn

[G01] 定义类
来源：http://wi.jctech888.com.cn

Py:   class User: pass
来源：http://fc.shxzskj.cn

PHP:  class User {}
来源：http://we.bjjhwx.cn

JS:   class User {}
来源：http://me.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ba.nicolike.cn

Java: class User {}
来源：http://ih.panjiajie.cn

Go:   type User struct { Name string }
来源：http://on.nszjky.cn

Ruby: class User; end
来源：http://cl.wgjwhj.cn

C#:   class User {}
来源：http://fj.szsharing.cn

[G02] 构造函数
来源：http://jb.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://vm.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://my.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://al.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://tc.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://ts.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ec.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://zu.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://ot.asd995.cn

[G03] 实例属性
来源：http://ji.hahajie.cn

Py:   self.name = "x"
来源：http://di.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://dt.huanxung.cn

JS:   this.name = "x";
来源：http://dz.asd995.cn

TS:   name: string = "x";
来源：http://cw.huanxung.cn

Java: private String name;
来源：http://px.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tc.shtwfgs.cn

Ruby: @name = "x"
来源：http://ag.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://tr.wgjwhj.cn

[G04] 定义方法
来源：http://na.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://ir.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mv.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://vp.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://er.bjjhwx.cn

Java: String greet() { return name; }
来源：http://ys.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bt.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://be.hahajie.cn

C#:   public string Greet() => Name;
来源：http://sx.yuexingan06.cn

[G05] 继承
来源：http://xv.521024.cn

Py:   class Admin(User): pass
来源：http://nc.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://qc.nicolike.cn

JS:   class Admin extends User {}
来源：http://gq.hahajie.cn

TS:   class Admin extends User {}
来源：http://yy.chemitech.net.cn

Java: class Admin extends User {}
来源：http://rg.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://px.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://ra.panjiajie.cn

C#:   class Admin : User {}
来源：http://mi.nszjky.cn

[G06] 重写方法
来源：http://wg.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://ll.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kp.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://zk.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://tt.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://rj.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oo.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://ni.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://gi.panjiajie.cn

[G07] 调用父类方法
来源：http://aa.asd995.cn

Py:   super().greet()
来源：http://fr.shxzukj.cn

PHP:  parent::greet();
来源：http://tl.shxzskj.cn

JS:   super.greet();
来源：http://da.asd995.cn

TS:   super.greet();
来源：http://ut.newstarts.cn

Java: super.greet();
来源：http://cn.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://au.nicolike.cn

Ruby: super
来源：http://zn.bookmarksfly.cn

C#:   base.Greet();
来源：http://qy.newstarts.cn

[G08] 静态方法与属性
来源：http://yj.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ot.szsharing.cn

PHP:  public static function f() {}
来源：http://ja.shtwfgs.cn

JS:   static f() {}
来源：http://wm.szsharing.cn

TS:   static f(): void {}
来源：http://cg.nszjky.cn

Java: static void f() {}
来源：http://id.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kf.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://gb.bookmarksfly.cn

C#:   public static void F() {}
来源：http://hu.nicolike.cn

[G09] 接口 / 抽象类
来源：http://ah.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://zj.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fh.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sx.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://ov.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://ue.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ex.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ne.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://nu.asd995.cn

[G10] 访问控制
来源：http://el.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://fq.yuexingan06.cn

PHP:  public / protected / private
来源：http://nq.nszjky.cn

JS:   #private 字段；其余公开
来源：http://pr.chemitech.net.cn

TS:   public / protected / private
来源：http://ii.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://dy.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rl.shxzskj.cn

Ruby: public / protected / private
来源：http://ke.lnxyls.cn

C#:   public / protected / private / internal
来源：http://ge.9csxet.cn

[G11] getter / setter
来源：http://sw.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://gq.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qg.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://ea.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://yi.9csxet.cn

Java: public String getName() { return name; }
来源：http://xn.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cy.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://sx.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://hb.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://op.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ux.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lw.szsharing.cn

JS:   toString() { return this.name; }
来源：http://ev.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://zq.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://py.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qf.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://uq.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://xo.nszjky.cn

[G13] 判断对象类型
来源：http://ld.colortex.cn

Py:   isinstance(u, User)
来源：http://vq.colortex.cn

PHP:  $u instanceof User
来源：http://fv.colortex.cn

JS:   u instanceof User
来源：http://ar.lnxyls.cn

TS:   u instanceof User
来源：http://qs.asd995.cn

Java: u instanceof User
来源：http://ju.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pn.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://lt.newstarts.cn

C#:   u is User
来源：http://ck.jctech888.com.cn

[G14] 数据类 / record
来源：http://wq.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cp.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://wz.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gz.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://yr.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://ey.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://vv.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ow.521024.cn

C#:   record User(string Name, int Age);
来源：http://ms.9csxet.cn

[G15] 枚举
来源：http://yb.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bp.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://td.yuntaijiaju.cn


<!-- 参考信息 -->