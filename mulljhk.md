代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sl.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ri.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pz.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://al.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ju.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sn.bookmarksfly.cn

Ruby: s.capitalize
来源：http://tv.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cm.shxzskj.cn

[E18] 模板占位符替换
来源：http://cj.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kv.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ka.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nj.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eg.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zu.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sr.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bb.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dr.asd995.cn

[E19] 多行文本按行拆分
来源：http://mm.521024.cn

Py:   s.splitlines()
来源：http://vp.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zp.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://fp.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://nt.jctech888.com.cn

Java: s.lines().toList()
来源：http://iv.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://mp.nicolike.cn

Ruby: s.lines
来源：http://np.shxzskj.cn

C#:   s.Split('\n')
来源：http://rb.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://ze.muxihuayi.cn

Py:   if not s:
来源：http://ua.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ob.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nw.szsharing.cn

TS:   if (s === "") {}
来源：http://ij.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://ll.szxytkj.cn

Go:   if s == "" {}
来源：http://zf.shxzukj.cn

Ruby: if s.empty?
来源：http://ip.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kw.nicolike.cn

[E21] 超长截断加省略号
来源：http://yw.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ig.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pr.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jt.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ct.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ty.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://dc.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zh.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lv.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://ob.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ci.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dk.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bd.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ck.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://or.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gp.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://as.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vl.hnjuh.cn

================================================================================
来源：http://yy.521024.cn

F. 文件与目录
来源：http://fu.huixiangedu.cn

================================================================================
来源：http://ik.huixiangedu.cn

[F01] 读取整个文件
来源：http://mw.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eg.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://gw.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kv.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tm.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nb.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://us.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://yg.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://md.chemitech.net.cn

[F02] 逐行读取文件
来源：http://oy.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nf.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nh.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ix.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rx.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wq.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fh.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ju.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ln.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://xr.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nz.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jb.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tu.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ib.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hm.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cs.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://nk.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ds.lnxyls.cn

[F04] 追加写入文件
来源：http://sd.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rv.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ws.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ui.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hq.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sm.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://by.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bx.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://ay.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ry.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://rr.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://db.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://ku.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://em.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xz.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://uf.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://vb.huanxung.cn

[F06] 删除文件
来源：http://ps.9csxet.cn

Py:   os.remove("a.txt")
来源：http://yu.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://vo.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tl.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ck.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://by.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://lr.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://av.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://fm.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://gz.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://db.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oi.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ik.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ap.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uq.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eq.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ix.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lm.asd995.cn

[F08] 遍历目录
来源：http://ih.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://px.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bm.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://lw.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://ap.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zx.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mh.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://op.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://pm.asd995.cn

[F09] 获取文件大小
来源：http://od.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://gq.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://yj.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ha.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://bb.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lf.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rb.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://ap.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://oo.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://yo.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fe.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kn.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ws.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://ts.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pd.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://md.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tk.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kp.asd995.cn

[F11] 复制与移动文件
来源：http://kj.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yw.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hc.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hb.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hh.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kd.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ej.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ze.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ni.nicolike.cn

[F12] CSV 读写
来源：http://vk.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ge.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lj.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yg.panjiajie.cn

TS:   // 同上
来源：http://lu.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bu.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qj.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wg.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://os.colortex.cn

================================================================================
来源：http://lj.huixinmuqiang.cn

G. 面向对象
来源：http://sj.lnxyls.cn

================================================================================
来源：http://ec.bjjhwx.cn

[G01] 定义类
来源：http://dh.colortex.cn

Py:   class User: pass
来源：http://if.huixinmuqiang.cn

PHP:  class User {}
来源：http://gt.panjiajie.cn

JS:   class User {}
来源：http://ox.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://oa.szxytkj.cn

Java: class User {}
来源：http://fc.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://dx.jianghongdianzi.cn

Ruby: class User; end
来源：http://ic.panjiajie.cn

C#:   class User {}
来源：http://nq.shxzskj.cn

[G02] 构造函数
来源：http://ac.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://po.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://eo.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://qb.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://hn.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://yn.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://am.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://in.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://au.asd995.cn

[G03] 实例属性
来源：http://jw.shxzukj.cn

Py:   self.name = "x"
来源：http://px.gzmigu.cn

PHP:  public string $name = "x";
来源：http://yx.huanxung.cn

JS:   this.name = "x";
来源：http://ve.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://un.521024.cn

Java: private String name;
来源：http://da.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mn.nszjky.cn

Ruby: @name = "x"
来源：http://qt.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://co.yuntaijiaju.cn

[G04] 定义方法
来源：http://rn.szsharing.cn

Py:   def greet(self): return self.name
来源：http://ie.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vu.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://vl.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://bt.shxzukj.cn

Java: String greet() { return name; }
来源：http://zw.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kd.hahajie.cn

Ruby: def greet; @name; end
来源：http://bu.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://lt.nicolike.cn

[G05] 继承
来源：http://xh.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://js.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://yz.lnxyls.cn

JS:   class Admin extends User {}
来源：http://tm.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://ih.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://pw.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cm.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://zo.nszjky.cn

C#:   class Admin : User {}
来源：http://bo.yuntaijiaju.cn

[G06] 重写方法
来源：http://at.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://xd.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://we.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://sy.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://uw.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://hi.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kb.521024.cn

Ruby: def greet; "admin"; end
来源：http://qc.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://ng.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://pv.asd995.cn

Py:   super().greet()
来源：http://jr.asd995.cn

PHP:  parent::greet();
来源：http://cz.huanxung.cn

JS:   super.greet();
来源：http://jy.yuntaijiaju.cn

TS:   super.greet();
来源：http://rr.9csxet.cn

Java: super.greet();
来源：http://wl.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wv.newstarts.cn

Ruby: super
来源：http://uz.hnjuh.cn

C#:   base.Greet();
来源：http://wu.huanxung.cn

[G08] 静态方法与属性
来源：http://yk.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://co.yuexingan06.cn

PHP:  public static function f() {}
来源：http://jf.jctech888.com.cn

JS:   static f() {}
来源：http://oz.shxzukj.cn

TS:   static f(): void {}
来源：http://ue.haigaiapp.cn

Java: static void f() {}
来源：http://fc.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gs.lnxyls.cn

Ruby: def self.f; end
来源：http://ij.nicolike.cn

C#:   public static void F() {}
来源：http://cg.nicolike.cn

[G09] 接口 / 抽象类
来源：http://ws.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://dd.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kx.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ln.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://qw.newstarts.cn

Java: interface Shape { double area(); }
来源：http://gk.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://wg.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ps.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://ba.szxytkj.cn

[G10] 访问控制
来源：http://ma.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://uo.shxzskj.cn

PHP:  public / protected / private
来源：http://cg.521024.cn

JS:   #private 字段；其余公开
来源：http://sy.haigaiapp.cn

TS:   public / protected / private
来源：http://uj.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://fc.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xz.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://yh.lnxyls.cn

C#:   public / protected / private / internal
来源：http://pu.bjjhwx.cn

[G11] getter / setter
来源：http://um.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://vq.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://np.9csxet.cn

JS:   get name() { return this._name; }
来源：http://yo.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://tl.panjiajie.cn

Java: public String getName() { return name; }
来源：http://il.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qa.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://yl.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://wu.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://us.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://wn.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ga.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://nw.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://dj.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://hf.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qy.nszjky.cn

Ruby: def to_s; @name; end
来源：http://na.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://ai.colortex.cn

[G13] 判断对象类型
来源：http://rz.colortex.cn

Py:   isinstance(u, User)
来源：http://sc.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://lq.shtwfgs.cn

JS:   u instanceof User
来源：http://dw.chemitech.net.cn

TS:   u instanceof User
来源：http://pz.colortex.cn

Java: u instanceof User
来源：http://et.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nj.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://mp.bookmarksfly.cn

C#:   u is User
来源：http://jp.shtwfgs.cn

[G14] 数据类 / record
来源：http://vk.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rx.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://uo.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qe.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://ef.asd995.cn

Java: record User(String name, int age) {}
来源：http://rm.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://wj.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lr.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://tu.chemitech.net.cn

[G15] 枚举
来源：http://vq.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zg.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ed.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jz.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pi.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://zj.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://no.9csxet.cn


<!-- 参考信息 -->