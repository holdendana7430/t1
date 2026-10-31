代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rg.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ge.lnxyls.cn

Ruby: s.capitalize
来源：http://ol.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uh.nicolike.cn

[E18] 模板占位符替换
来源：http://wh.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cl.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cw.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nu.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uo.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://as.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eu.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lu.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bc.nicolike.cn

[E19] 多行文本按行拆分
来源：http://bt.gzmigu.cn

Py:   s.splitlines()
来源：http://ly.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ag.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://mt.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://jk.szsharing.cn

Java: s.lines().toList()
来源：http://my.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://ie.bjjhwx.cn

Ruby: s.lines
来源：http://xr.9csxet.cn

C#:   s.Split('\n')
来源：http://tq.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://ja.gzmigu.cn

Py:   if not s:
来源：http://uo.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jf.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sr.huanxung.cn

TS:   if (s === "") {}
来源：http://kt.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://qm.newstarts.cn

Go:   if s == "" {}
来源：http://sc.huanxung.cn

Ruby: if s.empty?
来源：http://ft.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oj.colortex.cn

[E21] 超长截断加省略号
来源：http://nh.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wa.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kk.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tg.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uo.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ac.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://nb.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gl.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ts.newstarts.cn

[E22] 字节长度与字符长度
来源：http://bn.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nx.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ln.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ff.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ob.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rn.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cv.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://el.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mq.colortex.cn

================================================================================
来源：http://hl.yuexingan06.cn

F. 文件与目录
来源：http://ke.panjiajie.cn

================================================================================
来源：http://qi.muxihuayi.cn

[F01] 读取整个文件
来源：http://qz.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zj.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://wf.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dv.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oz.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fx.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pn.hahajie.cn

Ruby: File.read("a.txt")
来源：http://of.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://pw.huanxung.cn

[F02] 逐行读取文件
来源：http://ce.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ps.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ft.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xy.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bc.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eg.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yz.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nb.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://uh.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xr.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ay.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ot.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qd.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zo.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ie.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://sm.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nb.bjjhwx.cn

[F04] 追加写入文件
来源：http://sv.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://py.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yr.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://km.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lb.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zx.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pq.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hd.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ol.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://lb.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://og.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://bt.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://vf.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://qj.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://go.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nd.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ge.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://kp.colortex.cn

[F06] 删除文件
来源：http://pr.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://ea.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://yv.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://li.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nk.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jj.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://ya.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://xm.521024.cn

C#:   File.Delete("a.txt");
来源：http://rs.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://su.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ya.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://im.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://da.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ks.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vz.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fh.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qh.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pt.jctech888.com.cn

[F08] 遍历目录
来源：http://ya.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ah.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gn.521024.cn

JS:   fs.readdirSync("dir")
来源：http://ca.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://no.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rk.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ew.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://vg.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://no.asd995.cn

[F09] 获取文件大小
来源：http://wq.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://cw.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://wp.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://iy.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://jt.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eq.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xr.nszjky.cn

Ruby: File.size("a.txt")
来源：http://aq.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://sj.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://pl.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bt.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xz.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ds.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://ll.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nk.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zs.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ne.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://to.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://tu.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bn.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ik.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jk.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lp.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ws.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mt.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://er.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://de.nszjky.cn

[F12] CSV 读写
来源：http://il.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fq.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fu.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qs.hahajie.cn

TS:   // 同上
来源：http://fy.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jh.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oc.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://su.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ac.haigaiapp.cn

================================================================================
来源：http://eu.shxzskj.cn

G. 面向对象
来源：http://ew.9csxet.cn

================================================================================
来源：http://nx.szsharing.cn

[G01] 定义类
来源：http://gm.jianghongdianzi.cn

Py:   class User: pass
来源：http://iu.lnxyls.cn

PHP:  class User {}
来源：http://fb.lnxyls.cn

JS:   class User {}
来源：http://oa.asd995.cn

TS:   class User { name: string = ""; }
来源：http://ma.9csxet.cn

Java: class User {}
来源：http://hx.colortex.cn

Go:   type User struct { Name string }
来源：http://gj.panjiajie.cn

Ruby: class User; end
来源：http://ys.shxzukj.cn

C#:   class User {}
来源：http://ew.asd995.cn

[G02] 构造函数
来源：http://qr.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://gy.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://wv.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://qh.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://bt.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://om.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jh.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://xx.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://ec.shxzukj.cn

[G03] 实例属性
来源：http://ku.panjiajie.cn

Py:   self.name = "x"
来源：http://ps.szsharing.cn

PHP:  public string $name = "x";
来源：http://bm.nszjky.cn

JS:   this.name = "x";
来源：http://cg.asd995.cn

TS:   name: string = "x";
来源：http://ft.szsharing.cn

Java: private String name;
来源：http://bs.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://am.muxihuayi.cn

Ruby: @name = "x"
来源：http://lc.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://oz.shtwfgs.cn

[G04] 定义方法
来源：http://rx.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://fx.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gt.nicolike.cn

JS:   greet() { return this.name; }
来源：http://zx.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://bp.haigaiapp.cn

Java: String greet() { return name; }
来源：http://fy.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bt.panjiajie.cn

Ruby: def greet; @name; end
来源：http://uy.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://dz.wgjwhj.cn

[G05] 继承
来源：http://pu.szsharing.cn

Py:   class Admin(User): pass
来源：http://lb.colortex.cn

PHP:  class Admin extends User {}
来源：http://ae.shxzskj.cn

JS:   class Admin extends User {}
来源：http://vl.shxzukj.cn

TS:   class Admin extends User {}
来源：http://nk.huixiangedu.cn

Java: class Admin extends User {}
来源：http://jq.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fl.panjiajie.cn

Ruby: class Admin < User; end
来源：http://aq.wgjwhj.cn

C#:   class Admin : User {}
来源：http://hz.9csxet.cn

[G06] 重写方法
来源：http://zh.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://qa.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mr.asd995.cn

JS:   greet() { return "admin"; }
来源：http://be.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://sj.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://kt.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rf.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://nt.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://gl.nszjky.cn

[G07] 调用父类方法
来源：http://ab.colortex.cn

Py:   super().greet()
来源：http://gv.panjiajie.cn

PHP:  parent::greet();
来源：http://kc.bjjhwx.cn

JS:   super.greet();
来源：http://oy.huixiangedu.cn

TS:   super.greet();
来源：http://db.newstarts.cn

Java: super.greet();
来源：http://ja.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fa.huixinmuqiang.cn

Ruby: super
来源：http://zc.9csxet.cn

C#:   base.Greet();
来源：http://vs.gzmigu.cn

[G08] 静态方法与属性
来源：http://dt.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sm.muxihuayi.cn

PHP:  public static function f() {}
来源：http://iv.jctech888.com.cn

JS:   static f() {}
来源：http://ya.newstarts.cn

TS:   static f(): void {}
来源：http://mv.yuntaijiaju.cn

Java: static void f() {}
来源：http://az.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bx.szxytkj.cn

Ruby: def self.f; end
来源：http://sb.hahajie.cn

C#:   public static void F() {}
来源：http://xh.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://jo.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://yk.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dd.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qr.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://yc.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://ti.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://jk.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gg.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://mf.chemitech.net.cn

[G10] 访问控制
来源：http://ni.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://wy.shxzskj.cn

PHP:  public / protected / private
来源：http://ob.9csxet.cn

JS:   #private 字段；其余公开
来源：http://nv.szxytkj.cn

TS:   public / protected / private
来源：http://cp.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://bc.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qq.hahajie.cn

Ruby: public / protected / private
来源：http://fl.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://xu.yuexingan06.cn

[G11] getter / setter
来源：http://la.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://op.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qj.521024.cn

JS:   get name() { return this._name; }
来源：http://gl.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://db.huanxung.cn

Java: public String getName() { return name; }
来源：http://lg.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://we.gzmigu.cn

Ruby: attr_accessor :name
来源：http://tr.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://rq.bjjhwx.cn

[G12] 对象转字符串
来源：http://fb.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://fp.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jv.hahajie.cn

JS:   toString() { return this.name; }
来源：http://hc.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://pj.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://oh.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rl.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://qs.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://vc.bookmarksfly.cn

[G13] 判断对象类型
来源：http://cy.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://lp.colortex.cn

PHP:  $u instanceof User
来源：http://dm.muxihuayi.cn

JS:   u instanceof User
来源：http://ip.jianghongdianzi.cn

TS:   u instanceof User
来源：http://hk.wgjwhj.cn

Java: u instanceof User
来源：http://my.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ux.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://gn.jianghongdianzi.cn

C#:   u is User
来源：http://ve.colortex.cn

[G14] 数据类 / record
来源：http://gu.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://be.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://gq.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ee.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://tb.521024.cn

Java: record User(String name, int age) {}
来源：http://ai.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://no.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jf.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://us.521024.cn

[G15] 枚举
来源：http://xk.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fe.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hb.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wy.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vo.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://pz.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pd.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://dg.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yx.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://cp.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iu.huixiangedu.cn


<!-- 参考信息 -->