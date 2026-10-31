代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oz.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cw.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://fv.huanxung.cn

[E17] 首字母大写
来源：http://bo.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oe.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ay.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zk.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hp.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lv.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ht.wgjwhj.cn

Ruby: s.capitalize
来源：http://nt.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xk.shxzukj.cn

[E18] 模板占位符替换
来源：http://fj.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qh.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://il.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mc.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tf.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dh.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ys.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fa.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rv.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://gu.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://sw.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://js.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://kt.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://wh.bookmarksfly.cn

Java: s.lines().toList()
来源：http://xn.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://zi.huixinmuqiang.cn

Ruby: s.lines
来源：http://zy.haigaiapp.cn

C#:   s.Split('\n')
来源：http://jt.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://br.szsharing.cn

Py:   if not s:
来源：http://rm.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qy.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vr.shxzskj.cn

TS:   if (s === "") {}
来源：http://bl.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://si.lnxyls.cn

Go:   if s == "" {}
来源：http://vf.yuexingan06.cn

Ruby: if s.empty?
来源：http://nr.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oa.521024.cn

[E21] 超长截断加省略号
来源：http://qe.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yg.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pn.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fz.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uh.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oe.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://jm.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://su.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eh.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://oe.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wj.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vo.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rh.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ja.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ee.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yn.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://cy.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gs.jctech888.com.cn

================================================================================
来源：http://hm.szsharing.cn

F. 文件与目录
来源：http://ay.gzmigu.cn

================================================================================
来源：http://ax.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://hs.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mw.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://ji.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fr.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ke.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qg.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wc.asd995.cn

Ruby: File.read("a.txt")
来源：http://jx.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://cm.hahajie.cn

[F02] 逐行读取文件
来源：http://hk.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hg.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ig.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://no.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://by.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kc.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://le.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bn.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rd.521024.cn

[F03] 写入文件（覆盖）
来源：http://sj.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lh.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dy.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ms.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pe.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ei.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zp.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://xg.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hd.shxzskj.cn

[F04] 追加写入文件
来源：http://ra.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vd.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://of.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xa.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ok.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jv.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uq.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mq.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dl.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://af.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://la.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://hg.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://wp.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://zi.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://we.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hy.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://zv.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://mo.hnjuh.cn

[F06] 删除文件
来源：http://aw.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://of.newstarts.cn

PHP:  unlink("a.txt");
来源：http://qt.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sk.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rr.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ny.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://yk.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://dt.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://hm.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://ce.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xh.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://at.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ip.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sw.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uy.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kn.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nt.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ma.asd995.cn

[F08] 遍历目录
来源：http://xi.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nk.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ju.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://ti.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://ql.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zo.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lh.huanxung.cn

Ruby: Dir.children("dir")
来源：http://fy.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://jf.chemitech.net.cn

[F09] 获取文件大小
来源：http://ut.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://kk.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://sa.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://xf.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://eu.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pb.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nl.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://rg.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://tp.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://gw.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fk.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lr.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zt.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://sp.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bv.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iu.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ud.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://my.chemitech.net.cn

[F11] 复制与移动文件
来源：http://yz.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jp.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ms.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ad.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cf.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ds.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ng.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ni.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wn.nicolike.cn

[F12] CSV 读写
来源：http://gj.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iu.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oo.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sb.szxytkj.cn

TS:   // 同上
来源：http://kk.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ge.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bw.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tg.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ri.nszjky.cn

================================================================================
来源：http://lp.hahajie.cn

G. 面向对象
来源：http://kd.newstarts.cn

================================================================================
来源：http://jw.asd995.cn

[G01] 定义类
来源：http://wi.gzmigu.cn

Py:   class User: pass
来源：http://ua.muxihuayi.cn

PHP:  class User {}
来源：http://lg.bookmarksfly.cn

JS:   class User {}
来源：http://bb.521024.cn

TS:   class User { name: string = ""; }
来源：http://ch.newstarts.cn

Java: class User {}
来源：http://ks.nicolike.cn

Go:   type User struct { Name string }
来源：http://lo.huixinmuqiang.cn

Ruby: class User; end
来源：http://va.haigaiapp.cn

C#:   class User {}
来源：http://wh.newstarts.cn

[G02] 构造函数
来源：http://ht.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://qc.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://pp.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://tc.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://jq.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://wx.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pz.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://bw.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://nc.gzmigu.cn

[G03] 实例属性
来源：http://mo.521024.cn

Py:   self.name = "x"
来源：http://zy.panjiajie.cn

PHP:  public string $name = "x";
来源：http://qo.jctech888.com.cn

JS:   this.name = "x";
来源：http://rm.shtwfgs.cn

TS:   name: string = "x";
来源：http://nc.nicolike.cn

Java: private String name;
来源：http://yz.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qm.yuexingan06.cn

Ruby: @name = "x"
来源：http://as.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://vp.chemitech.net.cn

[G04] 定义方法
来源：http://tj.szsharing.cn

Py:   def greet(self): return self.name
来源：http://of.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sn.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://fg.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://tn.asd995.cn

Java: String greet() { return name; }
来源：http://ys.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eb.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://uv.9csxet.cn

C#:   public string Greet() => Name;
来源：http://oc.panjiajie.cn

[G05] 继承
来源：http://lx.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ay.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://zb.shxzukj.cn

JS:   class Admin extends User {}
来源：http://qs.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://gr.huixiangedu.cn

Java: class Admin extends User {}
来源：http://mn.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mm.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://rl.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://lq.panjiajie.cn

[G06] 重写方法
来源：http://rz.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://ay.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eg.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://lo.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://cc.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://mt.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ec.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://ne.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://qa.bookmarksfly.cn

[G07] 调用父类方法
来源：http://ju.bjjhwx.cn

Py:   super().greet()
来源：http://ap.521024.cn

PHP:  parent::greet();
来源：http://lj.asd995.cn

JS:   super.greet();
来源：http://vc.shtwfgs.cn

TS:   super.greet();
来源：http://bl.lnxyls.cn

Java: super.greet();
来源：http://oe.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lb.lnxyls.cn

Ruby: super
来源：http://wz.shxzukj.cn

C#:   base.Greet();
来源：http://pi.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://sc.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ql.bjjhwx.cn

PHP:  public static function f() {}
来源：http://wm.shxzukj.cn

JS:   static f() {}
来源：http://gk.nszjky.cn

TS:   static f(): void {}
来源：http://bh.hnjuh.cn

Java: static void f() {}
来源：http://xu.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rx.muxihuayi.cn

Ruby: def self.f; end
来源：http://jh.hnjuh.cn

C#:   public static void F() {}
来源：http://jo.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://ql.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ea.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ba.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://ri.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://or.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://zq.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sd.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://aw.jianghongdianzi.cn

[G10] 访问控制
来源：http://mp.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://xi.wgjwhj.cn

PHP:  public / protected / private
来源：http://xc.521024.cn

JS:   #private 字段；其余公开
来源：http://sj.huanxung.cn

TS:   public / protected / private
来源：http://ya.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://qy.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xh.shtwfgs.cn

Ruby: public / protected / private
来源：http://zy.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://sm.huixiangedu.cn

[G11] getter / setter
来源：http://kr.hahajie.cn

Py:   @property 与 @x.setter
来源：http://mm.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wg.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://dd.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://oq.shxzskj.cn

Java: public String getName() { return name; }
来源：http://fx.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yo.shxzskj.cn

Ruby: attr_accessor :name
来源：http://wh.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://fa.shxzskj.cn

[G12] 对象转字符串
来源：http://bt.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://wf.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ev.nszjky.cn

JS:   toString() { return this.name; }
来源：http://av.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://ja.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://jm.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ni.hahajie.cn

Ruby: def to_s; @name; end
来源：http://yi.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://wd.newstarts.cn

[G13] 判断对象类型
来源：http://mp.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://lq.colortex.cn

PHP:  $u instanceof User
来源：http://od.shxzskj.cn

JS:   u instanceof User
来源：http://cv.jctech888.com.cn

TS:   u instanceof User
来源：http://ly.colortex.cn

Java: u instanceof User
来源：http://dn.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://di.9csxet.cn

Ruby: u.is_a?(User)
来源：http://oy.colortex.cn

C#:   u is User
来源：http://zn.hahajie.cn

[G14] 数据类 / record
来源：http://yn.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ng.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://ix.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gv.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://zk.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://ut.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://ll.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hk.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://he.bjjhwx.cn

[G15] 枚举
来源：http://gh.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rl.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ki.chemitech.net.cn


<!-- 参考信息 -->