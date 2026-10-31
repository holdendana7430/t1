代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vn.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ee.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tv.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ob.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hp.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zd.gzmigu.cn

Ruby: s.capitalize
来源：http://rb.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tu.9csxet.cn

[E18] 模板占位符替换
来源：http://fw.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xn.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hc.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ko.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zr.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mw.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wp.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://op.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sc.nszjky.cn

[E19] 多行文本按行拆分
来源：http://ed.nicolike.cn

Py:   s.splitlines()
来源：http://qw.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kq.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://yi.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://vo.wgjwhj.cn

Java: s.lines().toList()
来源：http://gs.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://vi.huanxung.cn

Ruby: s.lines
来源：http://cl.bjjhwx.cn

C#:   s.Split('\n')
来源：http://hz.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://kf.yuntaijiaju.cn

Py:   if not s:
来源：http://is.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://al.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xf.chemitech.net.cn

TS:   if (s === "") {}
来源：http://ij.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://cz.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://fa.shtwfgs.cn

Ruby: if s.empty?
来源：http://xl.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rp.gzmigu.cn

[E21] 超长截断加省略号
来源：http://au.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zy.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wj.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xw.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://is.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mz.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://iv.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dy.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ae.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://yf.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cy.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://la.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ig.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ap.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cl.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://so.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://qu.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fq.colortex.cn

================================================================================
来源：http://vx.nszjky.cn

F. 文件与目录
来源：http://vw.huanxung.cn

================================================================================
来源：http://nj.panjiajie.cn

[F01] 读取整个文件
来源：http://yt.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ll.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://wl.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dc.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ev.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://at.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vf.colortex.cn

Ruby: File.read("a.txt")
来源：http://cx.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ve.shtwfgs.cn

[F02] 逐行读取文件
来源：http://hj.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wy.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wo.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oq.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yb.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wn.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dr.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vw.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yq.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://tl.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tq.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fh.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://br.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ju.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pc.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://au.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://oo.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ch.jctech888.com.cn

[F04] 追加写入文件
来源：http://qg.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pr.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tv.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xt.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lr.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ih.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gg.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://di.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cu.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://la.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pq.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://of.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://kc.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://ic.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eb.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hp.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://vj.colortex.cn

C#:   File.Exists("a.txt")
来源：http://vc.jianghongdianzi.cn

[F06] 删除文件
来源：http://rh.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://he.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://sp.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tg.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jc.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pq.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://kl.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://ip.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://uy.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://cm.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ny.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ii.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cw.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kb.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wp.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gs.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rr.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iu.shxzskj.cn

[F08] 遍历目录
来源：http://cj.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yf.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bx.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://ln.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://xc.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ck.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yu.szsharing.cn

Ruby: Dir.children("dir")
来源：http://ug.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://vw.newstarts.cn

[F09] 获取文件大小
来源：http://ww.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://jz.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://jl.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://cl.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://hv.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qw.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ad.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://gb.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ez.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://yb.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fg.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zn.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ds.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://hr.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lc.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://io.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dq.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kw.colortex.cn

[F11] 复制与移动文件
来源：http://hi.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tu.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wm.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nn.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fa.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ad.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sm.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ga.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kz.lnxyls.cn

[F12] CSV 读写
来源：http://cm.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gt.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://od.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bt.bjjhwx.cn

TS:   // 同上
来源：http://ww.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://as.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xp.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mh.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nb.huixinmuqiang.cn

================================================================================
来源：http://ep.521024.cn

G. 面向对象
来源：http://he.haigaiapp.cn

================================================================================
来源：http://ph.bjjhwx.cn

[G01] 定义类
来源：http://tc.asd995.cn

Py:   class User: pass
来源：http://nh.panjiajie.cn

PHP:  class User {}
来源：http://xm.newstarts.cn

JS:   class User {}
来源：http://hw.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://vo.huixiangedu.cn

Java: class User {}
来源：http://id.shxzukj.cn

Go:   type User struct { Name string }
来源：http://no.panjiajie.cn

Ruby: class User; end
来源：http://zr.colortex.cn

C#:   class User {}
来源：http://yc.szxytkj.cn

[G02] 构造函数
来源：http://ts.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://gg.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://zt.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://gj.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://pa.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://qp.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://in.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://xm.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://gb.colortex.cn

[G03] 实例属性
来源：http://bd.gzmigu.cn

Py:   self.name = "x"
来源：http://zv.521024.cn

PHP:  public string $name = "x";
来源：http://kf.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://rb.asd995.cn

TS:   name: string = "x";
来源：http://bh.bjjhwx.cn

Java: private String name;
来源：http://rw.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wv.yuexingan06.cn

Ruby: @name = "x"
来源：http://qd.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://bu.haigaiapp.cn

[G04] 定义方法
来源：http://uw.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://ys.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nx.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://eb.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://ek.haigaiapp.cn

Java: String greet() { return name; }
来源：http://oy.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fs.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://fu.nszjky.cn

C#:   public string Greet() => Name;
来源：http://qa.huanxung.cn

[G05] 继承
来源：http://ep.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://jq.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://bs.asd995.cn

JS:   class Admin extends User {}
来源：http://nw.huanxung.cn

TS:   class Admin extends User {}
来源：http://bk.gzmigu.cn

Java: class Admin extends User {}
来源：http://ld.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ka.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://vs.nicolike.cn

C#:   class Admin : User {}
来源：http://bc.9csxet.cn

[G06] 重写方法
来源：http://oc.521024.cn

Py:   def greet(self): return "admin"
来源：http://tc.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ge.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://zq.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://mf.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://ut.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nm.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://yv.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://ka.colortex.cn

[G07] 调用父类方法
来源：http://ck.huixiangedu.cn

Py:   super().greet()
来源：http://zp.haigaiapp.cn

PHP:  parent::greet();
来源：http://es.jianghongdianzi.cn

JS:   super.greet();
来源：http://au.jianghongdianzi.cn

TS:   super.greet();
来源：http://sg.muxihuayi.cn

Java: super.greet();
来源：http://tn.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gy.jianghongdianzi.cn

Ruby: super
来源：http://dt.bookmarksfly.cn

C#:   base.Greet();
来源：http://if.huixiangedu.cn

[G08] 静态方法与属性
来源：http://kf.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jy.hahajie.cn

PHP:  public static function f() {}
来源：http://cw.chemitech.net.cn

JS:   static f() {}
来源：http://xx.shtwfgs.cn

TS:   static f(): void {}
来源：http://vr.bookmarksfly.cn

Java: static void f() {}
来源：http://cw.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rw.huixiangedu.cn

Ruby: def self.f; end
来源：http://ru.wgjwhj.cn

C#:   public static void F() {}
来源：http://fj.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://sm.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://zu.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eb.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nk.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://hv.szsharing.cn

Java: interface Shape { double area(); }
来源：http://hq.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://xx.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ta.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://hs.huixiangedu.cn

[G10] 访问控制
来源：http://il.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://tj.521024.cn

PHP:  public / protected / private
来源：http://ja.nicolike.cn

JS:   #private 字段；其余公开
来源：http://lp.huanxung.cn

TS:   public / protected / private
来源：http://ba.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://uw.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dt.shxzskj.cn

Ruby: public / protected / private
来源：http://tp.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://dp.nszjky.cn

[G11] getter / setter
来源：http://il.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://le.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://az.asd995.cn

JS:   get name() { return this._name; }
来源：http://gq.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://pg.hnjuh.cn

Java: public String getName() { return name; }
来源：http://ro.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gl.nszjky.cn

Ruby: attr_accessor :name
来源：http://gg.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ac.9csxet.cn

[G12] 对象转字符串
来源：http://rz.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ip.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nc.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://wk.521024.cn

TS:   toString(): string { return this.name; }
来源：http://wm.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://kh.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zv.nszjky.cn

Ruby: def to_s; @name; end
来源：http://ea.521024.cn

C#:   public override string ToString() => Name;
来源：http://ch.newstarts.cn

[G13] 判断对象类型
来源：http://rv.szsharing.cn

Py:   isinstance(u, User)
来源：http://za.shxzskj.cn

PHP:  $u instanceof User
来源：http://zz.nszjky.cn

JS:   u instanceof User
来源：http://ge.shtwfgs.cn

TS:   u instanceof User
来源：http://su.szxytkj.cn

Java: u instanceof User
来源：http://rd.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ma.hahajie.cn

Ruby: u.is_a?(User)
来源：http://ka.jctech888.com.cn

C#:   u is User
来源：http://jk.shtwfgs.cn

[G14] 数据类 / record
来源：http://bi.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ay.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://zs.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ou.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://ny.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://we.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://lj.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ru.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://bg.chemitech.net.cn

[G15] 枚举
来源：http://tq.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://it.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hw.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://un.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hu.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://ei.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ej.haigaiapp.cn


<!-- 参考信息 -->