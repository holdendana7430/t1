代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://om.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://po.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://op.shxzukj.cn

[E17] 首字母大写
来源：http://hx.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bo.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bo.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dz.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://il.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gg.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zd.muxihuayi.cn

Ruby: s.capitalize
来源：http://rm.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bl.lnxyls.cn

[E18] 模板占位符替换
来源：http://sc.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ks.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ob.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jy.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ll.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yc.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uu.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jw.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lm.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://cq.521024.cn

Py:   s.splitlines()
来源：http://zi.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tn.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://fi.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://hw.shxzskj.cn

Java: s.lines().toList()
来源：http://hn.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://az.gzmigu.cn

Ruby: s.lines
来源：http://eg.szsharing.cn

C#:   s.Split('\n')
来源：http://kp.huanxung.cn

[E20] 判断字符串是否为空
来源：http://cs.yuntaijiaju.cn

Py:   if not s:
来源：http://lf.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jj.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://no.huanxung.cn

TS:   if (s === "") {}
来源：http://pn.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://db.gzmigu.cn

Go:   if s == "" {}
来源：http://sr.asd995.cn

Ruby: if s.empty?
来源：http://ey.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qq.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://ma.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wr.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jy.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bn.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hj.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jd.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://bp.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uw.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ce.nicolike.cn

[E22] 字节长度与字符长度
来源：http://ip.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://my.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ch.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tn.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://di.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ck.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qk.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://co.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kp.hahajie.cn

================================================================================
来源：http://ve.lnxyls.cn

F. 文件与目录
来源：http://ac.panjiajie.cn

================================================================================
来源：http://av.yuexingan06.cn

[F01] 读取整个文件
来源：http://ax.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ap.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://dt.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rf.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://at.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oh.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fn.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://ge.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://my.nszjky.cn

[F02] 逐行读取文件
来源：http://ym.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uk.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xu.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://as.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cx.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hj.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jj.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rm.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dy.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://xu.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ml.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bm.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jp.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gu.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://su.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vp.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://rz.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ah.huanxung.cn

[F04] 追加写入文件
来源：http://ot.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yr.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sg.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sc.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qr.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uc.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ox.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sw.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jb.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://sy.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yf.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://fj.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://vo.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://qq.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bz.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ip.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://bw.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://yb.haigaiapp.cn

[F06] 删除文件
来源：http://af.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://dr.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://su.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dk.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zz.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yy.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://yd.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://iv.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://vk.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://cz.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wq.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yf.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pg.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qt.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iu.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bh.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wk.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cq.gzmigu.cn

[F08] 遍历目录
来源：http://hi.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qh.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hc.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://sd.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://ks.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mz.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yh.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://pa.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://fb.shxzskj.cn

[F09] 获取文件大小
来源：http://lr.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://el.szsharing.cn

PHP:  filesize("a.txt");
来源：http://ij.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://qg.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://zp.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://se.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dg.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://pi.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://zp.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://jd.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qn.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ia.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ps.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://vs.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hn.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yu.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qx.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://po.521024.cn

[F11] 复制与移动文件
来源：http://cn.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zx.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kc.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bj.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zw.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bx.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tx.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fe.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mb.hahajie.cn

[F12] CSV 读写
来源：http://nl.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uf.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bi.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ed.panjiajie.cn

TS:   // 同上
来源：http://jc.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://je.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xv.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ct.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ti.szsharing.cn

================================================================================
来源：http://ci.yuntaijiaju.cn

G. 面向对象
来源：http://wx.jctech888.com.cn

================================================================================
来源：http://yq.wgjwhj.cn

[G01] 定义类
来源：http://yy.shxzukj.cn

Py:   class User: pass
来源：http://qf.shxzskj.cn

PHP:  class User {}
来源：http://ki.shtwfgs.cn

JS:   class User {}
来源：http://zc.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://qr.shxzukj.cn

Java: class User {}
来源：http://mf.hahajie.cn

Go:   type User struct { Name string }
来源：http://iw.huanxung.cn

Ruby: class User; end
来源：http://yo.szsharing.cn

C#:   class User {}
来源：http://yk.szsharing.cn

[G02] 构造函数
来源：http://iu.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://ds.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://xs.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://xm.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://fu.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://fc.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iq.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://nj.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://oz.chemitech.net.cn

[G03] 实例属性
来源：http://nb.521024.cn

Py:   self.name = "x"
来源：http://lt.szxytkj.cn

PHP:  public string $name = "x";
来源：http://vk.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://ko.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://jc.shxzskj.cn

Java: private String name;
来源：http://rw.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fr.lnxyls.cn

Ruby: @name = "x"
来源：http://md.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://wr.hnjuh.cn

[G04] 定义方法
来源：http://ju.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://mb.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lz.9csxet.cn

JS:   greet() { return this.name; }
来源：http://oo.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://dp.shtwfgs.cn

Java: String greet() { return name; }
来源：http://rv.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ze.shxzukj.cn

Ruby: def greet; @name; end
来源：http://pw.colortex.cn

C#:   public string Greet() => Name;
来源：http://hx.szsharing.cn

[G05] 继承
来源：http://mc.asd995.cn

Py:   class Admin(User): pass
来源：http://ga.9csxet.cn

PHP:  class Admin extends User {}
来源：http://sy.shxzskj.cn

JS:   class Admin extends User {}
来源：http://qj.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://kc.huanxung.cn

Java: class Admin extends User {}
来源：http://xm.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://db.szsharing.cn

Ruby: class Admin < User; end
来源：http://eo.jctech888.com.cn

C#:   class Admin : User {}
来源：http://yj.huixiangedu.cn

[G06] 重写方法
来源：http://rn.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://oo.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ld.asd995.cn

JS:   greet() { return "admin"; }
来源：http://on.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://an.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ag.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jz.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://ad.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://wu.shtwfgs.cn

[G07] 调用父类方法
来源：http://vd.9csxet.cn

Py:   super().greet()
来源：http://yo.szxytkj.cn

PHP:  parent::greet();
来源：http://pu.shtwfgs.cn

JS:   super.greet();
来源：http://jy.hnjuh.cn

TS:   super.greet();
来源：http://yh.yuntaijiaju.cn

Java: super.greet();
来源：http://pk.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jp.shxzukj.cn

Ruby: super
来源：http://gj.nicolike.cn

C#:   base.Greet();
来源：http://dm.huanxung.cn

[G08] 静态方法与属性
来源：http://tx.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sn.shxzukj.cn

PHP:  public static function f() {}
来源：http://pa.yuexingan06.cn

JS:   static f() {}
来源：http://fw.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://rw.huixiangedu.cn

Java: static void f() {}
来源：http://yq.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zm.haigaiapp.cn

Ruby: def self.f; end
来源：http://ep.huanxung.cn

C#:   public static void F() {}
来源：http://hd.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://vj.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://ah.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hf.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ud.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://dl.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://xd.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://zs.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yk.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://ho.shxzukj.cn

[G10] 访问控制
来源：http://qz.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://wo.szsharing.cn

PHP:  public / protected / private
来源：http://fk.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://mq.shtwfgs.cn

TS:   public / protected / private
来源：http://gm.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://lk.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gm.haigaiapp.cn

Ruby: public / protected / private
来源：http://ui.hnjuh.cn

C#:   public / protected / private / internal
来源：http://os.yuexingan06.cn

[G11] getter / setter
来源：http://bl.hahajie.cn

Py:   @property 与 @x.setter
来源：http://ip.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ac.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://wp.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://gr.hahajie.cn

Java: public String getName() { return name; }
来源：http://gl.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://su.hahajie.cn

Ruby: attr_accessor :name
来源：http://xo.newstarts.cn

C#:   public string Name { get; set; }
来源：http://ms.szxytkj.cn

[G12] 对象转字符串
来源：http://uw.colortex.cn

Py:   def __str__(self): return self.name
来源：http://il.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zp.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://ox.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://zu.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://og.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://je.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://rr.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://yy.521024.cn

[G13] 判断对象类型
来源：http://nr.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://kq.wgjwhj.cn

PHP:  $u instanceof User
来源：http://gi.huixinmuqiang.cn

JS:   u instanceof User
来源：http://nu.panjiajie.cn

TS:   u instanceof User
来源：http://us.bjjhwx.cn

Java: u instanceof User
来源：http://en.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gi.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://vc.jianghongdianzi.cn

C#:   u is User
来源：http://mf.shtwfgs.cn

[G14] 数据类 / record
来源：http://vi.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qk.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://xt.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aq.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://pu.szsharing.cn

Java: record User(String name, int age) {}
来源：http://qr.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://mb.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://el.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://dd.9csxet.cn

[G15] 枚举
来源：http://ru.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cm.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://da.newstarts.cn


<!-- 参考信息 -->