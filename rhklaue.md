代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zw.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rx.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://el.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://np.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wc.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yz.nicolike.cn

Ruby: s.capitalize
来源：http://yz.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://or.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ah.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ve.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tk.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ml.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sp.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gi.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dm.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hj.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kj.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://ic.colortex.cn

Py:   s.splitlines()
来源：http://so.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vz.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ti.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://od.szxytkj.cn

Java: s.lines().toList()
来源：http://eg.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://hd.panjiajie.cn

Ruby: s.lines
来源：http://lu.bjjhwx.cn

C#:   s.Split('\n')
来源：http://wq.nszjky.cn

[E20] 判断字符串是否为空
来源：http://cb.jctech888.com.cn

Py:   if not s:
来源：http://si.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ws.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eu.shxzukj.cn

TS:   if (s === "") {}
来源：http://ah.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://sp.huanxung.cn

Go:   if s == "" {}
来源：http://qc.hahajie.cn

Ruby: if s.empty?
来源：http://dz.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dq.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://zm.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zb.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gm.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pf.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ow.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dj.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://uw.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tm.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ya.asd995.cn

[E22] 字节长度与字符长度
来源：http://pd.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qp.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yx.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fn.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qo.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lu.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://by.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dy.huixiangedu.cn

================================================================================
来源：http://qv.lnxyls.cn

F. 文件与目录
来源：http://rj.haigaiapp.cn

================================================================================
来源：http://gs.asd995.cn

[F01] 读取整个文件
来源：http://ls.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://or.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://lv.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://er.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ay.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fp.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ds.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://hj.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://wz.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://pe.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://di.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ue.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ic.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://me.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bw.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eu.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zl.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://hv.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rh.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bz.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://de.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bt.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hy.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kw.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://so.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yo.bookmarksfly.cn

[F04] 追加写入文件
来源：http://md.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wu.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://th.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bd.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oq.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yc.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jz.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ya.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cu.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://sz.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gp.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://jh.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://wq.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://xu.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zl.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pz.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://tm.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://br.nicolike.cn

[F06] 删除文件
来源：http://pt.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://xx.nicolike.cn

PHP:  unlink("a.txt");
来源：http://po.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tq.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://es.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ua.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://kj.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://bj.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://hc.newstarts.cn

[F07] 创建目录（含多级）
来源：http://my.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wz.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wz.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mi.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://db.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mt.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rc.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qf.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uz.hahajie.cn

[F08] 遍历目录
来源：http://it.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pc.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hr.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://ms.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://on.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ud.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qq.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://jd.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://qt.szxytkj.cn

[F09] 获取文件大小
来源：http://rj.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://ue.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://en.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://nz.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://jw.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fh.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cc.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://mj.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://rb.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://ce.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://md.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mc.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sa.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://ft.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ts.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ng.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ie.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lz.lnxyls.cn

[F11] 复制与移动文件
来源：http://vd.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tl.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hi.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rw.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qk.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oy.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://te.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rw.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qm.nszjky.cn

[F12] CSV 读写
来源：http://ft.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ny.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rj.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://au.hnjuh.cn

TS:   // 同上
来源：http://ih.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ov.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zt.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eb.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hq.yuexingan06.cn

================================================================================
来源：http://we.hahajie.cn

G. 面向对象
来源：http://ya.9csxet.cn

================================================================================
来源：http://hw.haigaiapp.cn

[G01] 定义类
来源：http://sq.panjiajie.cn

Py:   class User: pass
来源：http://se.newstarts.cn

PHP:  class User {}
来源：http://ex.colortex.cn

JS:   class User {}
来源：http://np.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://if.chemitech.net.cn

Java: class User {}
来源：http://rl.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://go.szsharing.cn

Ruby: class User; end
来源：http://lx.haigaiapp.cn

C#:   class User {}
来源：http://ts.panjiajie.cn

[G02] 构造函数
来源：http://yg.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://on.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://nk.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://xq.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://mq.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://wz.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ia.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://th.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://bt.bjjhwx.cn

[G03] 实例属性
来源：http://an.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://wp.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://vw.nicolike.cn

JS:   this.name = "x";
来源：http://ou.asd995.cn

TS:   name: string = "x";
来源：http://xd.asd995.cn

Java: private String name;
来源：http://pl.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://co.szxytkj.cn

Ruby: @name = "x"
来源：http://bp.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://yx.asd995.cn

[G04] 定义方法
来源：http://yb.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://td.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gg.newstarts.cn

JS:   greet() { return this.name; }
来源：http://xi.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://cr.521024.cn

Java: String greet() { return name; }
来源：http://nk.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mr.shxzukj.cn

Ruby: def greet; @name; end
来源：http://ar.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://ff.gzmigu.cn

[G05] 继承
来源：http://eq.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://ds.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://wj.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://tz.hnjuh.cn

TS:   class Admin extends User {}
来源：http://nw.hnjuh.cn

Java: class Admin extends User {}
来源：http://js.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ai.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://fk.szxytkj.cn

C#:   class Admin : User {}
来源：http://ug.muxihuayi.cn

[G06] 重写方法
来源：http://gx.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://xw.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vw.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://hk.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://de.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://wg.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://io.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://tu.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://ad.szxytkj.cn

[G07] 调用父类方法
来源：http://xy.haigaiapp.cn

Py:   super().greet()
来源：http://qd.hnjuh.cn

PHP:  parent::greet();
来源：http://xb.nicolike.cn

JS:   super.greet();
来源：http://ap.muxihuayi.cn

TS:   super.greet();
来源：http://xb.nszjky.cn

Java: super.greet();
来源：http://py.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lv.wgjwhj.cn

Ruby: super
来源：http://lo.haigaiapp.cn

C#:   base.Greet();
来源：http://lh.jctech888.com.cn

[G08] 静态方法与属性
来源：http://mt.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ys.chemitech.net.cn

PHP:  public static function f() {}
来源：http://rz.wgjwhj.cn

JS:   static f() {}
来源：http://fz.nicolike.cn

TS:   static f(): void {}
来源：http://pj.szsharing.cn

Java: static void f() {}
来源：http://jx.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oc.shxzskj.cn

Ruby: def self.f; end
来源：http://do.nszjky.cn

C#:   public static void F() {}
来源：http://kf.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://ay.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://cq.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mi.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eh.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://df.hahajie.cn

Java: interface Shape { double area(); }
来源：http://uq.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://rx.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://el.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://fd.muxihuayi.cn

[G10] 访问控制
来源：http://ml.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://hc.panjiajie.cn

PHP:  public / protected / private
来源：http://nb.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://bz.huixinmuqiang.cn

TS:   public / protected / private
来源：http://xz.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://gy.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hw.gzmigu.cn

Ruby: public / protected / private
来源：http://oi.szxytkj.cn

C#:   public / protected / private / internal
来源：http://tn.huixinmuqiang.cn

[G11] getter / setter
来源：http://da.asd995.cn

Py:   @property 与 @x.setter
来源：http://ba.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pu.huanxung.cn

JS:   get name() { return this._name; }
来源：http://el.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://gf.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://qg.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ki.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://lg.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://ii.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://sg.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://dk.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ih.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://yw.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://ke.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://il.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fw.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://dc.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://wq.szxytkj.cn

[G13] 判断对象类型
来源：http://ot.521024.cn

Py:   isinstance(u, User)
来源：http://fc.colortex.cn

PHP:  $u instanceof User
来源：http://wk.shxzukj.cn

JS:   u instanceof User
来源：http://lz.huanxung.cn

TS:   u instanceof User
来源：http://yk.huixiangedu.cn

Java: u instanceof User
来源：http://qa.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ba.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://sd.nszjky.cn

C#:   u is User
来源：http://aw.chemitech.net.cn

[G14] 数据类 / record
来源：http://lf.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jc.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://mr.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qu.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://nl.huanxung.cn

Java: record User(String name, int age) {}
来源：http://wj.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://cp.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tn.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://bm.bjjhwx.cn

[G15] 枚举
来源：http://ok.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ue.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kn.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hw.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dn.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://mz.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oh.jctech888.com.cn


<!-- 参考信息 -->