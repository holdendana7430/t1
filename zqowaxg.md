代发 wailian999

[E18] 模板占位符替换
来源：http://uq.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rl.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qz.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://em.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cm.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zm.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fy.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://be.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zh.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://fb.lnxyls.cn

Py:   s.splitlines()
来源：http://ku.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ol.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://ua.521024.cn

TS:   s.split(/\r?\n/)
来源：http://oq.muxihuayi.cn

Java: s.lines().toList()
来源：http://im.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://ed.szxytkj.cn

Ruby: s.lines
来源：http://rq.shxzukj.cn

C#:   s.Split('\n')
来源：http://ww.9csxet.cn

[E20] 判断字符串是否为空
来源：http://xp.panjiajie.cn

Py:   if not s:
来源：http://xo.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yo.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yy.colortex.cn

TS:   if (s === "") {}
来源：http://dq.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://gg.muxihuayi.cn

Go:   if s == "" {}
来源：http://zt.bookmarksfly.cn

Ruby: if s.empty?
来源：http://bh.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aw.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://pu.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mz.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zh.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ad.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://af.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mk.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://jr.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jp.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cx.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://tm.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ru.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fo.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nn.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yp.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fv.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sl.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://ju.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nn.haigaiapp.cn

================================================================================
来源：http://ya.asd995.cn

F. 文件与目录
来源：http://kz.yuntaijiaju.cn

================================================================================
来源：http://af.colortex.cn

[F01] 读取整个文件
来源：http://ns.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hh.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://ze.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dm.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tq.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://el.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qm.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://hp.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://tq.muxihuayi.cn

[F02] 逐行读取文件
来源：http://fz.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cj.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vd.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tn.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ds.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ke.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nl.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ub.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lf.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://ov.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zv.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qo.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hi.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yy.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fw.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hm.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://zz.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ub.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://ru.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ov.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rv.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://en.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gd.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bh.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qq.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qv.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vk.521024.cn

[F05] 判断文件或目录是否存在
来源：http://lu.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kb.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://gg.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ss.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://fy.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qj.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rv.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://ez.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://gd.muxihuayi.cn

[F06] 删除文件
来源：http://wk.colortex.cn

Py:   os.remove("a.txt")
来源：http://hu.9csxet.cn

PHP:  unlink("a.txt");
来源：http://os.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yb.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ui.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vh.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://ec.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://ex.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://qb.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://bt.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ds.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gd.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uq.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://co.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sb.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gp.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jo.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cc.szxytkj.cn

[F08] 遍历目录
来源：http://hs.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ix.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qs.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://jl.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://rk.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ho.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jd.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://bt.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://dg.szxytkj.cn

[F09] 获取文件大小
来源：http://kk.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://nx.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://ku.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://so.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://us.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://le.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rn.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://el.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://rt.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://ol.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ph.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zc.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://td.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://zr.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://te.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://is.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sf.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pa.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://rm.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tt.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xf.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ol.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nb.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://en.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eu.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://og.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cs.yuntaijiaju.cn

[F12] CSV 读写
来源：http://bf.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uq.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gp.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sq.wgjwhj.cn

TS:   // 同上
来源：http://ab.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rw.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ty.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tb.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fp.lnxyls.cn

================================================================================
来源：http://ws.lnxyls.cn

G. 面向对象
来源：http://kk.muxihuayi.cn

================================================================================
来源：http://mx.jianghongdianzi.cn

[G01] 定义类
来源：http://rw.hnjuh.cn

Py:   class User: pass
来源：http://vj.szsharing.cn

PHP:  class User {}
来源：http://ch.lnxyls.cn

JS:   class User {}
来源：http://qf.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://he.huanxung.cn

Java: class User {}
来源：http://ur.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://aa.shxzskj.cn

Ruby: class User; end
来源：http://ib.hahajie.cn

C#:   class User {}
来源：http://jo.szxytkj.cn

[G02] 构造函数
来源：http://fg.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://zf.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://hm.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://fs.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://ih.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://iq.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://np.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://vj.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://tc.szxytkj.cn

[G03] 实例属性
来源：http://kz.szxytkj.cn

Py:   self.name = "x"
来源：http://lq.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://ay.hnjuh.cn

JS:   this.name = "x";
来源：http://hl.newstarts.cn

TS:   name: string = "x";
来源：http://qy.muxihuayi.cn

Java: private String name;
来源：http://ve.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mf.gzmigu.cn

Ruby: @name = "x"
来源：http://ec.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://ul.huixiangedu.cn

[G04] 定义方法
来源：http://lf.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://hr.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://us.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://hs.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://na.shxzukj.cn

Java: String greet() { return name; }
来源：http://pk.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mv.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://wq.9csxet.cn

C#:   public string Greet() => Name;
来源：http://xy.colortex.cn

[G05] 继承
来源：http://hc.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://vd.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://ja.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://nj.lnxyls.cn

TS:   class Admin extends User {}
来源：http://ez.9csxet.cn

Java: class Admin extends User {}
来源：http://mm.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cd.asd995.cn

Ruby: class Admin < User; end
来源：http://ci.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://wi.yuexingan06.cn

[G06] 重写方法
来源：http://sf.521024.cn

Py:   def greet(self): return "admin"
来源：http://it.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mp.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://gm.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://io.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://bq.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cv.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://ju.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://lo.shtwfgs.cn

[G07] 调用父类方法
来源：http://vd.gzmigu.cn

Py:   super().greet()
来源：http://bc.haigaiapp.cn

PHP:  parent::greet();
来源：http://jz.huanxung.cn

JS:   super.greet();
来源：http://ry.gzmigu.cn

TS:   super.greet();
来源：http://ok.colortex.cn

Java: super.greet();
来源：http://vv.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rn.panjiajie.cn

Ruby: super
来源：http://od.huanxung.cn

C#:   base.Greet();
来源：http://ph.shtwfgs.cn

[G08] 静态方法与属性
来源：http://yd.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aj.szxytkj.cn

PHP:  public static function f() {}
来源：http://if.huixinmuqiang.cn

JS:   static f() {}
来源：http://ex.huanxung.cn

TS:   static f(): void {}
来源：http://gf.yuntaijiaju.cn

Java: static void f() {}
来源：http://ct.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hs.chemitech.net.cn

Ruby: def self.f; end
来源：http://jt.huanxung.cn

C#:   public static void F() {}
来源：http://pn.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://we.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://dq.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ss.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fo.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://uc.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://tt.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ko.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ar.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://ms.gzmigu.cn

[G10] 访问控制
来源：http://hu.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://jy.wgjwhj.cn

PHP:  public / protected / private
来源：http://hr.hahajie.cn

JS:   #private 字段；其余公开
来源：http://vb.gzmigu.cn

TS:   public / protected / private
来源：http://th.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ej.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zn.szsharing.cn

Ruby: public / protected / private
来源：http://dh.panjiajie.cn

C#:   public / protected / private / internal
来源：http://hk.huixinmuqiang.cn

[G11] getter / setter
来源：http://jm.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://cm.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vn.9csxet.cn

JS:   get name() { return this._name; }
来源：http://nf.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://em.shxzukj.cn

Java: public String getName() { return name; }
来源：http://fg.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ee.9csxet.cn

Ruby: attr_accessor :name
来源：http://hq.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://wc.nicolike.cn

[G12] 对象转字符串
来源：http://rk.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://jn.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://md.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://mf.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://fl.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://zl.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kk.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://xt.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://rc.haigaiapp.cn

[G13] 判断对象类型
来源：http://jg.hnjuh.cn

Py:   isinstance(u, User)
来源：http://cc.chemitech.net.cn

PHP:  $u instanceof User
来源：http://gi.panjiajie.cn

JS:   u instanceof User
来源：http://bg.521024.cn

TS:   u instanceof User
来源：http://pv.muxihuayi.cn

Java: u instanceof User
来源：http://ut.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dm.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://ln.bjjhwx.cn

C#:   u is User
来源：http://hx.lnxyls.cn

[G14] 数据类 / record
来源：http://yb.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cu.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://mn.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mi.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://dh.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://lz.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://hl.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ya.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://zz.yuexingan06.cn

[G15] 枚举
来源：http://qy.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sk.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ig.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lo.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gw.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://di.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://et.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://im.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jb.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://dq.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gt.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://px.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://ci.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://rk.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zo.521024.cn


<!-- 参考信息 -->