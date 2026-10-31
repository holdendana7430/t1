代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gp.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tv.colortex.cn

Ruby: s.capitalize
来源：http://yp.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://em.huixiangedu.cn

[E18] 模板占位符替换
来源：http://wt.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ra.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tk.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xs.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ui.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nn.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rl.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yv.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nh.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://vj.colortex.cn

Py:   s.splitlines()
来源：http://fc.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ld.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://jn.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://oq.newstarts.cn

Java: s.lines().toList()
来源：http://xe.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://ec.shxzskj.cn

Ruby: s.lines
来源：http://dy.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://qx.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://dq.muxihuayi.cn

Py:   if not s:
来源：http://hg.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mb.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tq.hahajie.cn

TS:   if (s === "") {}
来源：http://ye.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://bj.haigaiapp.cn

Go:   if s == "" {}
来源：http://jd.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://aj.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bz.9csxet.cn

[E21] 超长截断加省略号
来源：http://zw.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ky.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ik.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rm.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xs.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qx.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://by.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nc.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vl.9csxet.cn

[E22] 字节长度与字符长度
来源：http://ln.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qs.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zj.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://et.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lz.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yq.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vt.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://ia.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jc.colortex.cn

================================================================================
来源：http://ji.521024.cn

F. 文件与目录
来源：http://ws.huanxung.cn

================================================================================
来源：http://re.shxzukj.cn

[F01] 读取整个文件
来源：http://xg.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rg.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://zu.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gn.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://li.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yd.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yi.nicolike.cn

Ruby: File.read("a.txt")
来源：http://km.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ld.nicolike.cn

[F02] 逐行读取文件
来源：http://tk.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fe.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tn.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xr.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xy.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ob.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gj.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gu.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ue.colortex.cn

[F03] 写入文件（覆盖）
来源：http://qz.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rd.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ye.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lu.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://it.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rs.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aj.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://ce.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gt.szsharing.cn

[F04] 追加写入文件
来源：http://fh.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fl.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vs.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zy.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lk.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eq.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kb.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ym.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ha.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://mo.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zv.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://ye.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://vw.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://xs.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cj.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gs.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://hf.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://js.szsharing.cn

[F06] 删除文件
来源：http://wc.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://xl.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://mt.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ie.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nd.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vg.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://ld.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://vs.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://yk.szsharing.cn

[F07] 创建目录（含多级）
来源：http://ms.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kc.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kh.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dw.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jo.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hv.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pu.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://su.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vc.asd995.cn

[F08] 遍历目录
来源：http://la.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yk.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gg.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://oc.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://lg.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qh.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ji.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://gq.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://az.hahajie.cn

[F09] 获取文件大小
来源：http://ax.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://qm.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://hs.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://zv.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://hc.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pl.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ot.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://ze.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://zc.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://vy.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ew.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nf.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yh.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://sb.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ks.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ol.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vx.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ko.nszjky.cn

[F11] 复制与移动文件
来源：http://py.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kb.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ho.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ht.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kz.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aa.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kj.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yd.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nm.wgjwhj.cn

[F12] CSV 读写
来源：http://lx.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ds.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://af.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lb.huanxung.cn

TS:   // 同上
来源：http://gu.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tz.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://se.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ko.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cp.gzmigu.cn

================================================================================
来源：http://sw.shxzukj.cn

G. 面向对象
来源：http://cg.muxihuayi.cn

================================================================================
来源：http://nb.9csxet.cn

[G01] 定义类
来源：http://wg.panjiajie.cn

Py:   class User: pass
来源：http://xi.yuexingan06.cn

PHP:  class User {}
来源：http://po.lnxyls.cn

JS:   class User {}
来源：http://mj.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://pk.huanxung.cn

Java: class User {}
来源：http://pz.shxzskj.cn

Go:   type User struct { Name string }
来源：http://uh.chemitech.net.cn

Ruby: class User; end
来源：http://hm.shxzskj.cn

C#:   class User {}
来源：http://xf.newstarts.cn

[G02] 构造函数
来源：http://qn.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://tv.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://di.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://zn.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://td.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://ly.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ul.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://ah.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://gd.panjiajie.cn

[G03] 实例属性
来源：http://kq.bjjhwx.cn

Py:   self.name = "x"
来源：http://vf.newstarts.cn

PHP:  public string $name = "x";
来源：http://ra.shtwfgs.cn

JS:   this.name = "x";
来源：http://gp.panjiajie.cn

TS:   name: string = "x";
来源：http://hu.bjjhwx.cn

Java: private String name;
来源：http://gp.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jg.lnxyls.cn

Ruby: @name = "x"
来源：http://sc.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ge.huixinmuqiang.cn

[G04] 定义方法
来源：http://ze.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://kk.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mi.colortex.cn

JS:   greet() { return this.name; }
来源：http://oa.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://fs.chemitech.net.cn

Java: String greet() { return name; }
来源：http://vl.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vy.colortex.cn

Ruby: def greet; @name; end
来源：http://pc.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://qo.colortex.cn

[G05] 继承
来源：http://yn.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://eo.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://as.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://om.newstarts.cn

TS:   class Admin extends User {}
来源：http://xd.szxytkj.cn

Java: class Admin extends User {}
来源：http://fy.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kn.lnxyls.cn

Ruby: class Admin < User; end
来源：http://fa.muxihuayi.cn

C#:   class Admin : User {}
来源：http://sx.jianghongdianzi.cn

[G06] 重写方法
来源：http://eu.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://as.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vq.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://qd.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://fk.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://up.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sj.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://az.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://vv.newstarts.cn

[G07] 调用父类方法
来源：http://va.yuntaijiaju.cn

Py:   super().greet()
来源：http://qq.huanxung.cn

PHP:  parent::greet();
来源：http://jo.hahajie.cn

JS:   super.greet();
来源：http://kk.yuntaijiaju.cn

TS:   super.greet();
来源：http://qi.chemitech.net.cn

Java: super.greet();
来源：http://jr.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tf.wgjwhj.cn

Ruby: super
来源：http://wk.huixiangedu.cn

C#:   base.Greet();
来源：http://wd.nszjky.cn

[G08] 静态方法与属性
来源：http://xz.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yx.wgjwhj.cn

PHP:  public static function f() {}
来源：http://bh.huixiangedu.cn

JS:   static f() {}
来源：http://vx.521024.cn

TS:   static f(): void {}
来源：http://xc.yuntaijiaju.cn

Java: static void f() {}
来源：http://su.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aw.asd995.cn

Ruby: def self.f; end
来源：http://wq.newstarts.cn

C#:   public static void F() {}
来源：http://ss.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://jd.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://gu.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kr.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pf.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://sd.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://kq.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://gh.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fc.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://pd.newstarts.cn

[G10] 访问控制
来源：http://ho.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://tx.chemitech.net.cn

PHP:  public / protected / private
来源：http://my.hahajie.cn

JS:   #private 字段；其余公开
来源：http://jt.hahajie.cn

TS:   public / protected / private
来源：http://iv.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://hj.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eu.shtwfgs.cn

Ruby: public / protected / private
来源：http://dj.szsharing.cn

C#:   public / protected / private / internal
来源：http://nk.bookmarksfly.cn

[G11] getter / setter
来源：http://lq.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://du.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iv.521024.cn

JS:   get name() { return this._name; }
来源：http://lj.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://cf.szxytkj.cn

Java: public String getName() { return name; }
来源：http://oe.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zg.lnxyls.cn

Ruby: attr_accessor :name
来源：http://it.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://le.newstarts.cn

[G12] 对象转字符串
来源：http://ya.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://hx.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fd.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://io.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://pi.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://ok.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ck.huanxung.cn

Ruby: def to_s; @name; end
来源：http://bo.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://la.shxzukj.cn

[G13] 判断对象类型
来源：http://ad.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://ze.huixiangedu.cn

PHP:  $u instanceof User
来源：http://oc.hnjuh.cn

JS:   u instanceof User
来源：http://ie.jianghongdianzi.cn

TS:   u instanceof User
来源：http://gk.shxzskj.cn

Java: u instanceof User
来源：http://kx.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ev.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://an.bookmarksfly.cn

C#:   u is User
来源：http://iq.bjjhwx.cn

[G14] 数据类 / record
来源：http://kc.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ef.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://gm.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://it.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://cx.asd995.cn

Java: record User(String name, int age) {}
来源：http://fk.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://pp.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kn.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://is.gzmigu.cn

[G15] 枚举
来源：http://kt.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ai.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ag.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uv.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gz.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://dp.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kg.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://jk.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ga.colortex.cn

[G16] 对象转数组 / 字典
来源：http://lr.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cx.yuexingan06.cn


<!-- 参考信息 -->