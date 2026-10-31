代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://il.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yn.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://va.chemitech.net.cn

[E17] 首字母大写
来源：http://cl.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xt.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gg.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qs.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fh.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vt.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://my.yuexingan06.cn

Ruby: s.capitalize
来源：http://to.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vg.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://jd.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qg.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://my.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zq.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rc.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vr.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://af.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lw.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hv.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://cm.gzmigu.cn

Py:   s.splitlines()
来源：http://cz.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bn.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://mf.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://wv.bookmarksfly.cn

Java: s.lines().toList()
来源：http://wz.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://ox.yuexingan06.cn

Ruby: s.lines
来源：http://up.shxzskj.cn

C#:   s.Split('\n')
来源：http://ng.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://bb.huanxung.cn

Py:   if not s:
来源：http://qj.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pc.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ma.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://sw.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://ce.9csxet.cn

Go:   if s == "" {}
来源：http://ny.jctech888.com.cn

Ruby: if s.empty?
来源：http://sp.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xn.nszjky.cn

[E21] 超长截断加省略号
来源：http://es.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://of.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://om.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jf.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jl.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pq.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://ew.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fm.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yn.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://it.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yf.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hr.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://po.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rh.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uf.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jo.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://qw.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jc.lnxyls.cn

================================================================================
来源：http://oy.huanxung.cn

F. 文件与目录
来源：http://yg.huixiangedu.cn

================================================================================
来源：http://dh.lnxyls.cn

[F01] 读取整个文件
来源：http://aa.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uy.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://yu.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kg.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gw.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sj.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wu.colortex.cn

Ruby: File.read("a.txt")
来源：http://pw.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://zg.nicolike.cn

[F02] 逐行读取文件
来源：http://ti.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gs.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hp.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pt.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://de.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sc.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jg.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://on.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://vs.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ml.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jt.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vz.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lx.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yl.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kx.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ld.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fe.hnjuh.cn

[F04] 追加写入文件
来源：http://oo.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xx.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pu.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qp.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://af.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rt.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://le.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kk.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vm.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://au.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tq.521024.cn

PHP:  file_exists("a.txt");
来源：http://nh.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://tu.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://pm.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wc.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mb.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ge.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ng.hahajie.cn

[F06] 删除文件
来源：http://ot.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://is.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://fd.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ah.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ae.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oa.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://nu.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://hy.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://gy.nicolike.cn

[F07] 创建目录（含多级）
来源：http://vw.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sy.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ot.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tn.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iz.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ty.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ov.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rt.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fq.shxzskj.cn

[F08] 遍历目录
来源：http://tk.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wk.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://av.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://ht.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://kh.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sw.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qa.szsharing.cn

Ruby: Dir.children("dir")
来源：http://vi.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://gc.haigaiapp.cn

[F09] 获取文件大小
来源：http://ux.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://pn.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://dc.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://kj.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://wb.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ud.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hl.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://gn.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://hv.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://bh.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://my.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uc.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zz.szsharing.cn

TS:   path.extname("a.txt")
来源：http://pa.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bh.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ad.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zs.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vw.chemitech.net.cn

[F11] 复制与移动文件
来源：http://pz.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sk.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vr.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eg.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rp.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oj.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vy.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ce.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hs.huixiangedu.cn

[F12] CSV 读写
来源：http://kz.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kw.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tz.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ba.yuntaijiaju.cn

TS:   // 同上
来源：http://ow.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://un.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cs.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zt.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://le.jctech888.com.cn

================================================================================
来源：http://tg.nszjky.cn

G. 面向对象
来源：http://qr.shxzskj.cn

================================================================================
来源：http://xh.hnjuh.cn

[G01] 定义类
来源：http://ja.9csxet.cn

Py:   class User: pass
来源：http://xg.hahajie.cn

PHP:  class User {}
来源：http://uf.hnjuh.cn

JS:   class User {}
来源：http://ue.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://tt.hahajie.cn

Java: class User {}
来源：http://hd.szxytkj.cn

Go:   type User struct { Name string }
来源：http://qw.haigaiapp.cn

Ruby: class User; end
来源：http://ya.chemitech.net.cn

C#:   class User {}
来源：http://hu.521024.cn

[G02] 构造函数
来源：http://nv.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://pp.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://sz.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://xe.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://bb.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://za.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gf.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://xw.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://xx.panjiajie.cn

[G03] 实例属性
来源：http://pv.hnjuh.cn

Py:   self.name = "x"
来源：http://bw.nszjky.cn

PHP:  public string $name = "x";
来源：http://bh.szsharing.cn

JS:   this.name = "x";
来源：http://mt.hnjuh.cn

TS:   name: string = "x";
来源：http://ht.wgjwhj.cn

Java: private String name;
来源：http://kk.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sb.huanxung.cn

Ruby: @name = "x"
来源：http://cw.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ir.yuexingan06.cn

[G04] 定义方法
来源：http://hc.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://yq.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xc.newstarts.cn

JS:   greet() { return this.name; }
来源：http://bg.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://dw.newstarts.cn

Java: String greet() { return name; }
来源：http://yh.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jy.hahajie.cn

Ruby: def greet; @name; end
来源：http://xl.521024.cn

C#:   public string Greet() => Name;
来源：http://wb.bjjhwx.cn

[G05] 继承
来源：http://pr.newstarts.cn

Py:   class Admin(User): pass
来源：http://se.hahajie.cn

PHP:  class Admin extends User {}
来源：http://yl.nicolike.cn

JS:   class Admin extends User {}
来源：http://xl.shxzskj.cn

TS:   class Admin extends User {}
来源：http://ma.huanxung.cn

Java: class Admin extends User {}
来源：http://rq.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xo.shxzskj.cn

Ruby: class Admin < User; end
来源：http://ob.521024.cn

C#:   class Admin : User {}
来源：http://yc.hahajie.cn

[G06] 重写方法
来源：http://cd.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://hf.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ip.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ig.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://bq.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://iv.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cu.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://hp.521024.cn

C#:   public override string Greet() => "admin";
来源：http://gg.wgjwhj.cn

[G07] 调用父类方法
来源：http://df.hahajie.cn

Py:   super().greet()
来源：http://da.nicolike.cn

PHP:  parent::greet();
来源：http://wo.lnxyls.cn

JS:   super.greet();
来源：http://ga.jianghongdianzi.cn

TS:   super.greet();
来源：http://ss.9csxet.cn

Java: super.greet();
来源：http://bi.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tz.gzmigu.cn

Ruby: super
来源：http://dg.haigaiapp.cn

C#:   base.Greet();
来源：http://un.nicolike.cn

[G08] 静态方法与属性
来源：http://zi.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nr.huanxung.cn

PHP:  public static function f() {}
来源：http://fl.chemitech.net.cn

JS:   static f() {}
来源：http://wp.huixiangedu.cn

TS:   static f(): void {}
来源：http://dw.chemitech.net.cn

Java: static void f() {}
来源：http://qw.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ul.newstarts.cn

Ruby: def self.f; end
来源：http://va.hahajie.cn

C#:   public static void F() {}
来源：http://kw.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://uf.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://yq.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ng.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ef.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://ye.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://ug.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://up.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rx.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://hi.chemitech.net.cn

[G10] 访问控制
来源：http://jl.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://gc.asd995.cn

PHP:  public / protected / private
来源：http://lo.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://ky.shtwfgs.cn

TS:   public / protected / private
来源：http://jx.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://ns.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nk.gzmigu.cn

Ruby: public / protected / private
来源：http://zj.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://mt.muxihuayi.cn

[G11] getter / setter
来源：http://yq.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://yy.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nj.hahajie.cn

JS:   get name() { return this._name; }
来源：http://qf.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://ft.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://ab.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nb.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://qn.szsharing.cn

C#:   public string Name { get; set; }
来源：http://tb.colortex.cn

[G12] 对象转字符串
来源：http://ww.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://tw.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fg.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://kf.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://xh.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://ys.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://du.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://kg.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://xb.szsharing.cn

[G13] 判断对象类型
来源：http://hv.huanxung.cn

Py:   isinstance(u, User)
来源：http://vi.haigaiapp.cn

PHP:  $u instanceof User
来源：http://yx.wgjwhj.cn

JS:   u instanceof User
来源：http://si.chemitech.net.cn

TS:   u instanceof User
来源：http://ar.huixinmuqiang.cn

Java: u instanceof User
来源：http://fq.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qu.huanxung.cn

Ruby: u.is_a?(User)
来源：http://xc.asd995.cn

C#:   u is User
来源：http://uw.yuexingan06.cn

[G14] 数据类 / record
来源：http://ar.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cm.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://qn.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ql.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://ov.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://pv.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://fe.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mj.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://ck.colortex.cn

[G15] 枚举
来源：http://kj.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ij.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yp.huixinmuqiang.cn


<!-- 参考信息 -->