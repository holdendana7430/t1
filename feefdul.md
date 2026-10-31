代发 wailian999

PHP:  number_format(1234567);
来源：http://do.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kx.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dj.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mi.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tp.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xi.asd995.cn

C#:   1234567.ToString("N0")
来源：http://ty.nicolike.cn

[E17] 首字母大写
来源：http://cb.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dz.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bw.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lq.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yv.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://um.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tg.bjjhwx.cn

Ruby: s.capitalize
来源：http://vp.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gw.jctech888.com.cn

[E18] 模板占位符替换
来源：http://vi.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kt.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qs.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sv.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wu.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cr.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ur.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://je.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bx.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://rn.huixiangedu.cn

Py:   s.splitlines()
来源：http://em.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gz.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://xd.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://di.nszjky.cn

Java: s.lines().toList()
来源：http://kf.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://tb.yuntaijiaju.cn

Ruby: s.lines
来源：http://qu.wgjwhj.cn

C#:   s.Split('\n')
来源：http://nx.nicolike.cn

[E20] 判断字符串是否为空
来源：http://bt.bjjhwx.cn

Py:   if not s:
来源：http://mh.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rn.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ap.521024.cn

TS:   if (s === "") {}
来源：http://zw.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://ju.yuexingan06.cn

Go:   if s == "" {}
来源：http://xs.jctech888.com.cn

Ruby: if s.empty?
来源：http://cu.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pc.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://da.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qq.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rm.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qu.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ey.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cd.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://cg.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nr.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fp.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://ea.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zl.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ye.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ne.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jw.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wc.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bb.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://jo.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zs.szsharing.cn

================================================================================
来源：http://xp.panjiajie.cn

F. 文件与目录
来源：http://dr.huanxung.cn

================================================================================
来源：http://lt.chemitech.net.cn

[F01] 读取整个文件
来源：http://qy.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xg.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://vl.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mx.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ir.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ba.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sc.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://jt.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://bf.lnxyls.cn

[F02] 逐行读取文件
来源：http://xu.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pu.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bw.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pa.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gw.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://as.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ei.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dr.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://os.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://km.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gc.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://be.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zv.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ac.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fw.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rt.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://rn.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tm.gzmigu.cn

[F04] 追加写入文件
来源：http://ob.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ua.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uz.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nd.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wj.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lz.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zc.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ac.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bq.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://mp.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ed.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://nk.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://fx.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://xl.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gl.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kw.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://ts.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://vr.colortex.cn

[F06] 删除文件
来源：http://pf.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://qu.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://ip.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zy.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://po.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zv.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://le.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://ym.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://kp.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://op.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tb.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tk.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rk.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lu.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hc.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oc.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yn.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mi.nszjky.cn

[F08] 遍历目录
来源：http://ei.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jk.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://as.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://ie.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://hm.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xk.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://do.hahajie.cn

Ruby: Dir.children("dir")
来源：http://eu.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://du.bjjhwx.cn

[F09] 获取文件大小
来源：http://na.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://ot.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://xx.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://si.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://pa.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://es.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jy.asd995.cn

Ruby: File.size("a.txt")
来源：http://cy.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://tn.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://lz.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ur.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ua.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hf.nszjky.cn

TS:   path.extname("a.txt")
来源：http://iy.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gf.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zc.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ka.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sp.huixiangedu.cn

[F11] 复制与移动文件
来源：http://yq.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ai.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gx.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ts.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wz.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ga.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ll.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xo.huanxung.cn

[F12] CSV 读写
来源：http://xw.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kl.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hh.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zh.jianghongdianzi.cn

TS:   // 同上
来源：http://fd.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://at.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uf.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gf.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vr.9csxet.cn

================================================================================
来源：http://al.lnxyls.cn

G. 面向对象
来源：http://gv.newstarts.cn

================================================================================
来源：http://vs.huanxung.cn

[G01] 定义类
来源：http://ez.chemitech.net.cn

Py:   class User: pass
来源：http://xn.hnjuh.cn

PHP:  class User {}
来源：http://jv.panjiajie.cn

JS:   class User {}
来源：http://lz.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://qo.jianghongdianzi.cn

Java: class User {}
来源：http://nl.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://jq.hnjuh.cn

Ruby: class User; end
来源：http://zw.huixinmuqiang.cn

C#:   class User {}
来源：http://bq.gzmigu.cn

[G02] 构造函数
来源：http://an.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://xh.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://cg.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://wf.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://rr.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://nb.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://md.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://tf.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://zs.chemitech.net.cn

[G03] 实例属性
来源：http://kz.nicolike.cn

Py:   self.name = "x"
来源：http://zu.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://lr.bookmarksfly.cn

JS:   this.name = "x";
来源：http://an.shxzskj.cn

TS:   name: string = "x";
来源：http://gq.colortex.cn

Java: private String name;
来源：http://ah.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ui.jctech888.com.cn

Ruby: @name = "x"
来源：http://kl.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://bn.nszjky.cn

[G04] 定义方法
来源：http://ix.huanxung.cn

Py:   def greet(self): return self.name
来源：http://xy.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pp.521024.cn

JS:   greet() { return this.name; }
来源：http://oq.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://lf.gzmigu.cn

Java: String greet() { return name; }
来源：http://dt.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rc.lnxyls.cn

Ruby: def greet; @name; end
来源：http://vs.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://qy.chemitech.net.cn

[G05] 继承
来源：http://tc.hahajie.cn

Py:   class Admin(User): pass
来源：http://iw.521024.cn

PHP:  class Admin extends User {}
来源：http://pt.szxytkj.cn

JS:   class Admin extends User {}
来源：http://na.9csxet.cn

TS:   class Admin extends User {}
来源：http://mu.yuexingan06.cn

Java: class Admin extends User {}
来源：http://dx.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xm.hnjuh.cn

Ruby: class Admin < User; end
来源：http://ox.asd995.cn

C#:   class Admin : User {}
来源：http://nz.shtwfgs.cn

[G06] 重写方法
来源：http://xp.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://jx.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xm.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://uv.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://bb.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://ep.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fg.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://du.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://qn.bookmarksfly.cn

[G07] 调用父类方法
来源：http://ok.wgjwhj.cn

Py:   super().greet()
来源：http://xa.panjiajie.cn

PHP:  parent::greet();
来源：http://sj.hahajie.cn

JS:   super.greet();
来源：http://zk.nicolike.cn

TS:   super.greet();
来源：http://db.huixinmuqiang.cn

Java: super.greet();
来源：http://dm.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wr.wgjwhj.cn

Ruby: super
来源：http://nx.colortex.cn

C#:   base.Greet();
来源：http://wf.haigaiapp.cn

[G08] 静态方法与属性
来源：http://it.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wa.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://tu.huixinmuqiang.cn

JS:   static f() {}
来源：http://mj.gzmigu.cn

TS:   static f(): void {}
来源：http://he.yuntaijiaju.cn

Java: static void f() {}
来源：http://uo.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hq.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://kv.hahajie.cn

C#:   public static void F() {}
来源：http://km.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://nb.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://sm.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zx.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zh.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://fb.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://vd.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://eb.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wu.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://ay.nszjky.cn

[G10] 访问控制
来源：http://pg.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://px.asd995.cn

PHP:  public / protected / private
来源：http://ra.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://lf.bookmarksfly.cn

TS:   public / protected / private
来源：http://ry.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://ls.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gi.nicolike.cn

Ruby: public / protected / private
来源：http://mr.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://ou.bjjhwx.cn

[G11] getter / setter
来源：http://ke.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://uu.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wx.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://ck.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://vn.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://jb.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dt.panjiajie.cn

Ruby: attr_accessor :name
来源：http://wj.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://os.szxytkj.cn

[G12] 对象转字符串
来源：http://zg.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://vs.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://es.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://lj.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://mm.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://it.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nk.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://pg.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://io.wgjwhj.cn

[G13] 判断对象类型
来源：http://jn.gzmigu.cn

Py:   isinstance(u, User)
来源：http://yf.chemitech.net.cn

PHP:  $u instanceof User
来源：http://lc.9csxet.cn

JS:   u instanceof User
来源：http://ye.bjjhwx.cn

TS:   u instanceof User
来源：http://jv.hahajie.cn

Java: u instanceof User
来源：http://is.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mj.asd995.cn

Ruby: u.is_a?(User)
来源：http://bl.bookmarksfly.cn

C#:   u is User
来源：http://ae.521024.cn

[G14] 数据类 / record
来源：http://sf.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mx.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://tq.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cb.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://hq.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://cs.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://la.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dj.huanxung.cn


<!-- 参考信息 -->