代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yu.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mk.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ig.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fo.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ur.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vu.jctech888.com.cn

Ruby: s.capitalize
来源：http://el.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oh.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ao.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pg.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cy.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cn.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mg.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xf.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sf.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://da.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pa.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://ov.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://mx.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gp.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://yf.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://uu.huixiangedu.cn

Java: s.lines().toList()
来源：http://lf.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://rt.shxzukj.cn

Ruby: s.lines
来源：http://av.nicolike.cn

C#:   s.Split('\n')
来源：http://sw.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://iu.colortex.cn

Py:   if not s:
来源：http://ga.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hs.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xz.wgjwhj.cn

TS:   if (s === "") {}
来源：http://ok.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://ws.asd995.cn

Go:   if s == "" {}
来源：http://ln.haigaiapp.cn

Ruby: if s.empty?
来源：http://xv.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dw.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://xi.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ni.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ir.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hm.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pt.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xg.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://wc.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://si.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rj.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://ot.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nq.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mu.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sd.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://en.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pr.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wu.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://uo.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uo.nicolike.cn

================================================================================
来源：http://dc.szsharing.cn

F. 文件与目录
来源：http://lh.shxzukj.cn

================================================================================
来源：http://jc.chemitech.net.cn

[F01] 读取整个文件
来源：http://vw.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jn.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://tk.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mf.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lx.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qy.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nq.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://qd.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://fc.szsharing.cn

[F02] 逐行读取文件
来源：http://zo.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://di.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cr.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://by.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ld.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zm.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ds.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ro.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yu.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://ki.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rk.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yq.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://py.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ly.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lo.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sn.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://es.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://va.gzmigu.cn

[F04] 追加写入文件
来源：http://no.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ol.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sk.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oy.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lb.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ro.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iz.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lg.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://if.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://mh.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xv.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://yk.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://vr.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://ne.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fx.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fe.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://hd.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://na.colortex.cn

[F06] 删除文件
来源：http://cf.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://vr.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://ax.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xr.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ax.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zu.asd995.cn

Go:   os.Remove("a.txt")
来源：http://mz.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://jl.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://qu.nicolike.cn

[F07] 创建目录（含多级）
来源：http://gs.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ij.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ip.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mt.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wr.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uy.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nn.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mn.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://th.szsharing.cn

[F08] 遍历目录
来源：http://fy.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zj.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ox.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://dh.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://mj.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dm.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://os.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://sn.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://vc.panjiajie.cn

[F09] 获取文件大小
来源：http://vj.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://jw.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://ih.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://he.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://wz.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lk.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pi.nicolike.cn

Ruby: File.size("a.txt")
来源：http://rs.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://mm.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://qb.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rk.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tu.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lx.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://jz.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yn.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xp.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ln.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ut.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://lr.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ui.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://le.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://po.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xd.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xv.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xo.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vz.yuntaijiaju.cn

[F12] CSV 读写
来源：http://cp.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ll.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cm.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ng.yuexingan06.cn

TS:   // 同上
来源：http://yl.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ka.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aw.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gk.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://td.gzmigu.cn

================================================================================
来源：http://ri.panjiajie.cn

G. 面向对象
来源：http://gh.gzmigu.cn

================================================================================
来源：http://yr.panjiajie.cn

[G01] 定义类
来源：http://jx.szxytkj.cn

Py:   class User: pass
来源：http://gl.shtwfgs.cn

PHP:  class User {}
来源：http://eb.muxihuayi.cn

JS:   class User {}
来源：http://ls.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://sz.asd995.cn

Java: class User {}
来源：http://fk.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://rz.nszjky.cn

Ruby: class User; end
来源：http://au.hnjuh.cn

C#:   class User {}
来源：http://zh.hahajie.cn

[G02] 构造函数
来源：http://la.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://wd.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://uv.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://cz.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://mf.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://rs.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ls.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://gx.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://wf.asd995.cn

[G03] 实例属性
来源：http://rd.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://fz.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://jd.asd995.cn

JS:   this.name = "x";
来源：http://us.nszjky.cn

TS:   name: string = "x";
来源：http://cb.hahajie.cn

Java: private String name;
来源：http://be.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ik.521024.cn

Ruby: @name = "x"
来源：http://ag.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://zs.nszjky.cn

[G04] 定义方法
来源：http://sh.nicolike.cn

Py:   def greet(self): return self.name
来源：http://oq.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mc.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://kb.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://ij.huixiangedu.cn

Java: String greet() { return name; }
来源：http://ke.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://za.szsharing.cn

Ruby: def greet; @name; end
来源：http://qj.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://cm.jctech888.com.cn

[G05] 继承
来源：http://dv.gzmigu.cn

Py:   class Admin(User): pass
来源：http://hc.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://yi.521024.cn

JS:   class Admin extends User {}
来源：http://lp.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://ki.nicolike.cn

Java: class Admin extends User {}
来源：http://jk.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wi.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://ge.colortex.cn

C#:   class Admin : User {}
来源：http://qx.lnxyls.cn

[G06] 重写方法
来源：http://gh.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://hj.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xu.asd995.cn

JS:   greet() { return "admin"; }
来源：http://se.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://ju.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://gq.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zq.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://vw.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ic.panjiajie.cn

[G07] 调用父类方法
来源：http://nh.huanxung.cn

Py:   super().greet()
来源：http://kw.bookmarksfly.cn

PHP:  parent::greet();
来源：http://in.huixinmuqiang.cn

JS:   super.greet();
来源：http://le.nszjky.cn

TS:   super.greet();
来源：http://ma.huanxung.cn

Java: super.greet();
来源：http://rp.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hy.wgjwhj.cn

Ruby: super
来源：http://jd.asd995.cn

C#:   base.Greet();
来源：http://be.colortex.cn

[G08] 静态方法与属性
来源：http://rf.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mi.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://xk.asd995.cn

JS:   static f() {}
来源：http://yw.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://pd.9csxet.cn

Java: static void f() {}
来源：http://xl.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iy.panjiajie.cn

Ruby: def self.f; end
来源：http://sf.bookmarksfly.cn

C#:   public static void F() {}
来源：http://xx.huanxung.cn

[G09] 接口 / 抽象类
来源：http://ne.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://kj.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ix.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zu.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://aw.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://qj.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://yu.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ho.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://dw.9csxet.cn

[G10] 访问控制
来源：http://dy.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://pv.gzmigu.cn

PHP:  public / protected / private
来源：http://ns.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://zt.hahajie.cn

TS:   public / protected / private
来源：http://jn.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://mk.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bv.panjiajie.cn

Ruby: public / protected / private
来源：http://ej.newstarts.cn

C#:   public / protected / private / internal
来源：http://vc.szsharing.cn

[G11] getter / setter
来源：http://ul.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://wu.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qi.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://bl.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://yg.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://eg.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://dg.asd995.cn

C#:   public string Name { get; set; }
来源：http://tp.asd995.cn

[G12] 对象转字符串
来源：http://hn.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://fg.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ro.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://vz.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://ew.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://ib.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rf.asd995.cn

Ruby: def to_s; @name; end
来源：http://xe.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://aw.gzmigu.cn

[G13] 判断对象类型
来源：http://vv.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://le.szsharing.cn

PHP:  $u instanceof User
来源：http://ck.huixiangedu.cn

JS:   u instanceof User
来源：http://ls.szxytkj.cn

TS:   u instanceof User
来源：http://lt.nicolike.cn

Java: u instanceof User
来源：http://fz.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sb.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://vq.huixiangedu.cn

C#:   u is User
来源：http://ou.muxihuayi.cn

[G14] 数据类 / record
来源：http://dy.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xh.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://wm.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ai.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://bt.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://tu.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://sz.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://me.colortex.cn

C#:   record User(string Name, int Age);
来源：http://mu.gzmigu.cn

[G15] 枚举
来源：http://lb.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nl.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gj.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cf.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vj.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://vh.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qc.huixiangedu.cn


<!-- 参考信息 -->