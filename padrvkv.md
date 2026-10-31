代发 wailian999

PHP:  number_format(1234567);
来源：http://bn.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kt.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dm.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kc.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tj.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bj.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://ax.bjjhwx.cn

[E17] 首字母大写
来源：http://dx.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://db.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yp.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hg.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rj.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fa.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lk.nicolike.cn

Ruby: s.capitalize
来源：http://kd.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jy.asd995.cn

[E18] 模板占位符替换
来源：http://ai.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ol.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mz.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ht.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dp.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rc.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yx.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tq.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wo.colortex.cn

[E19] 多行文本按行拆分
来源：http://zf.9csxet.cn

Py:   s.splitlines()
来源：http://ur.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lg.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://za.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://eo.nszjky.cn

Java: s.lines().toList()
来源：http://ju.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://nv.shxzskj.cn

Ruby: s.lines
来源：http://kp.gzmigu.cn

C#:   s.Split('\n')
来源：http://fr.nszjky.cn

[E20] 判断字符串是否为空
来源：http://qy.wgjwhj.cn

Py:   if not s:
来源：http://qf.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sj.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nt.gzmigu.cn

TS:   if (s === "") {}
来源：http://jl.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://ul.jctech888.com.cn

Go:   if s == "" {}
来源：http://ax.nicolike.cn

Ruby: if s.empty?
来源：http://lg.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lr.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://qi.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://od.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oi.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://af.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ci.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jz.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://jk.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://je.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ig.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://cf.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zg.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kw.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vv.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mk.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ub.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yt.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://dp.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oe.nszjky.cn

================================================================================
来源：http://je.nicolike.cn

F. 文件与目录
来源：http://oy.9csxet.cn

================================================================================
来源：http://nu.lnxyls.cn

[F01] 读取整个文件
来源：http://ua.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mf.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://ma.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kc.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yr.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://po.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://he.521024.cn

Ruby: File.read("a.txt")
来源：http://mf.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://yv.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://cp.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nc.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dz.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ue.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yr.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sz.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wy.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://id.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uk.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://nd.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sf.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yj.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tl.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hp.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kg.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tj.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://jg.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ol.521024.cn

[F04] 追加写入文件
来源：http://kc.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pl.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qk.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wx.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eh.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wn.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ch.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hs.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pk.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://gh.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ux.colortex.cn

PHP:  file_exists("a.txt");
来源：http://mf.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://gi.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://uu.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pg.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qk.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://kk.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://xk.wgjwhj.cn

[F06] 删除文件
来源：http://bs.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://og.szsharing.cn

PHP:  unlink("a.txt");
来源：http://kp.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ff.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lp.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vg.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://um.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://tj.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ej.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://mt.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sq.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://re.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qe.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pk.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zn.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bd.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zd.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oo.bjjhwx.cn

[F08] 遍历目录
来源：http://pw.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yw.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pi.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://zi.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://mv.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ue.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wu.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://wg.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://jo.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://kx.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://jv.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://re.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://oi.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://ly.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://if.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hm.9csxet.cn

Ruby: File.size("a.txt")
来源：http://sn.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://fq.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://ct.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yi.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ue.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ub.nicolike.cn

TS:   path.extname("a.txt")
来源：http://jf.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nc.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nk.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wv.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hp.hahajie.cn

[F11] 复制与移动文件
来源：http://te.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gp.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ge.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ir.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pk.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rr.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yt.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zl.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://su.bjjhwx.cn

[F12] CSV 读写
来源：http://ca.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sw.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fw.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dd.gzmigu.cn

TS:   // 同上
来源：http://zd.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ee.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://es.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ka.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oi.yuexingan06.cn

================================================================================
来源：http://ee.shtwfgs.cn

G. 面向对象
来源：http://st.chemitech.net.cn

================================================================================
来源：http://il.asd995.cn

[G01] 定义类
来源：http://wy.jctech888.com.cn

Py:   class User: pass
来源：http://rg.9csxet.cn

PHP:  class User {}
来源：http://gi.shxzukj.cn

JS:   class User {}
来源：http://ju.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://fa.newstarts.cn

Java: class User {}
来源：http://fd.521024.cn

Go:   type User struct { Name string }
来源：http://yl.jianghongdianzi.cn

Ruby: class User; end
来源：http://go.haigaiapp.cn

C#:   class User {}
来源：http://ih.muxihuayi.cn

[G02] 构造函数
来源：http://gw.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ht.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://ow.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ae.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://hi.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://dk.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ac.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://mc.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://yk.bookmarksfly.cn

[G03] 实例属性
来源：http://ba.huanxung.cn

Py:   self.name = "x"
来源：http://ra.huanxung.cn

PHP:  public string $name = "x";
来源：http://jt.muxihuayi.cn

JS:   this.name = "x";
来源：http://fk.bookmarksfly.cn

TS:   name: string = "x";
来源：http://mf.haigaiapp.cn

Java: private String name;
来源：http://gh.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dj.hahajie.cn

Ruby: @name = "x"
来源：http://of.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://uf.lnxyls.cn

[G04] 定义方法
来源：http://eb.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://qy.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hg.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://pd.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://bs.huixiangedu.cn

Java: String greet() { return name; }
来源：http://gt.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sn.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://ru.asd995.cn

C#:   public string Greet() => Name;
来源：http://de.panjiajie.cn

[G05] 继承
来源：http://fy.colortex.cn

Py:   class Admin(User): pass
来源：http://wr.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://za.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ys.asd995.cn

TS:   class Admin extends User {}
来源：http://rd.9csxet.cn

Java: class Admin extends User {}
来源：http://pf.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xr.szsharing.cn

Ruby: class Admin < User; end
来源：http://un.nicolike.cn

C#:   class Admin : User {}
来源：http://pw.newstarts.cn

[G06] 重写方法
来源：http://cc.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://ab.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nh.colortex.cn

JS:   greet() { return "admin"; }
来源：http://in.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://eb.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://go.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lj.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://tn.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://uy.huixiangedu.cn

[G07] 调用父类方法
来源：http://vi.bjjhwx.cn

Py:   super().greet()
来源：http://bi.hahajie.cn

PHP:  parent::greet();
来源：http://im.chemitech.net.cn

JS:   super.greet();
来源：http://kw.nszjky.cn

TS:   super.greet();
来源：http://ef.gzmigu.cn

Java: super.greet();
来源：http://gu.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uh.newstarts.cn

Ruby: super
来源：http://na.wgjwhj.cn

C#:   base.Greet();
来源：http://xt.lnxyls.cn

[G08] 静态方法与属性
来源：http://ud.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kr.panjiajie.cn

PHP:  public static function f() {}
来源：http://av.hahajie.cn

JS:   static f() {}
来源：http://kv.szsharing.cn

TS:   static f(): void {}
来源：http://lu.shxzskj.cn

Java: static void f() {}
来源：http://zf.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wy.hnjuh.cn

Ruby: def self.f; end
来源：http://xn.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://bc.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://wc.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://tj.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rt.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tw.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://kk.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://wj.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ba.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zn.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://wb.chemitech.net.cn

[G10] 访问控制
来源：http://qi.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://vb.shxzukj.cn

PHP:  public / protected / private
来源：http://nc.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://ap.szsharing.cn

TS:   public / protected / private
来源：http://ai.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://ce.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vb.9csxet.cn

Ruby: public / protected / private
来源：http://po.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://ln.shtwfgs.cn

[G11] getter / setter
来源：http://ne.9csxet.cn

Py:   @property 与 @x.setter
来源：http://bv.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ld.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://gu.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://kd.colortex.cn

Java: public String getName() { return name; }
来源：http://ef.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vx.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://lx.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://hz.muxihuayi.cn

[G12] 对象转字符串
来源：http://ha.521024.cn

Py:   def __str__(self): return self.name
来源：http://qg.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vm.nszjky.cn

JS:   toString() { return this.name; }
来源：http://hk.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://oh.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://ob.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://so.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://nd.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://kf.asd995.cn

[G13] 判断对象类型
来源：http://qt.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://ii.jctech888.com.cn

PHP:  $u instanceof User
来源：http://ch.muxihuayi.cn

JS:   u instanceof User
来源：http://lx.jctech888.com.cn

TS:   u instanceof User
来源：http://lw.huanxung.cn

Java: u instanceof User
来源：http://rn.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mj.9csxet.cn

Ruby: u.is_a?(User)
来源：http://gj.asd995.cn

C#:   u is User
来源：http://fd.bjjhwx.cn

[G14] 数据类 / record
来源：http://lk.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pa.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://sh.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pp.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://ij.nicolike.cn

Java: record User(String name, int age) {}
来源：http://by.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://vu.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nq.szsharing.cn


<!-- 参考信息 -->