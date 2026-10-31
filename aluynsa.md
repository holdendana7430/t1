代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fx.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ft.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cc.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sz.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hs.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://db.panjiajie.cn

Ruby: s.capitalize
来源：http://mk.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ta.asd995.cn

[E18] 模板占位符替换
来源：http://lp.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tk.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sv.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dv.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ok.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fm.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ly.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pf.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nh.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://hq.chemitech.net.cn

Py:   s.splitlines()
来源：http://zz.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gr.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://ve.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://br.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://se.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://qx.huixiangedu.cn

Ruby: s.lines
来源：http://qf.szsharing.cn

C#:   s.Split('\n')
来源：http://ym.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://ug.wgjwhj.cn

Py:   if not s:
来源：http://oi.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oe.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ia.huixiangedu.cn

TS:   if (s === "") {}
来源：http://jf.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://mb.muxihuayi.cn

Go:   if s == "" {}
来源：http://wv.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://aj.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yj.huanxung.cn

[E21] 超长截断加省略号
来源：http://yd.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uu.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xi.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jd.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iw.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rd.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://xb.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xi.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lz.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://ov.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yo.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ts.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sz.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sd.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ln.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pf.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://ja.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iz.yuntaijiaju.cn

================================================================================
来源：http://ri.jianghongdianzi.cn

F. 文件与目录
来源：http://ul.chemitech.net.cn

================================================================================
来源：http://aw.shtwfgs.cn

[F01] 读取整个文件
来源：http://wk.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zf.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://gn.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wi.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sn.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dz.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sx.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://ap.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://oz.yuexingan06.cn

[F02] 逐行读取文件
来源：http://au.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hf.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wm.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hd.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uq.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bk.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rd.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xr.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pq.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://ta.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ts.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bn.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ow.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ml.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sl.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ju.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://sq.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://di.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://vt.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dz.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xn.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dq.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://re.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jz.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ne.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hh.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uq.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://ei.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ke.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://vb.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://uc.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://re.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dg.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ru.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://lc.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://rb.shxzskj.cn

[F06] 删除文件
来源：http://pa.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://gy.asd995.cn

PHP:  unlink("a.txt");
来源：http://ip.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cj.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yc.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kk.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://kz.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://hj.521024.cn

C#:   File.Delete("a.txt");
来源：http://cc.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://jl.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://np.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qo.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fj.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://or.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wo.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dt.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tu.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ba.asd995.cn

[F08] 遍历目录
来源：http://ul.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nq.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jl.521024.cn

JS:   fs.readdirSync("dir")
来源：http://rf.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://ps.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xa.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pa.hahajie.cn

Ruby: Dir.children("dir")
来源：http://rf.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://zv.521024.cn

[F09] 获取文件大小
来源：http://ox.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://xs.colortex.cn

PHP:  filesize("a.txt");
来源：http://ki.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://cq.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://om.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ag.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jw.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://el.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://yi.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://fx.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wn.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qb.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fm.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://hf.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zp.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sv.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qg.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ma.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://zr.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bq.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ww.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xy.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bo.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qp.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jj.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ta.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jg.muxihuayi.cn

[F12] CSV 读写
来源：http://bs.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ej.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rx.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ir.lnxyls.cn

TS:   // 同上
来源：http://zj.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ny.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ab.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eh.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dk.521024.cn

================================================================================
来源：http://ly.huixiangedu.cn

G. 面向对象
来源：http://se.newstarts.cn

================================================================================
来源：http://op.huixinmuqiang.cn

[G01] 定义类
来源：http://ip.szxytkj.cn

Py:   class User: pass
来源：http://cw.9csxet.cn

PHP:  class User {}
来源：http://rs.gzmigu.cn

JS:   class User {}
来源：http://wh.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://pb.huixinmuqiang.cn

Java: class User {}
来源：http://kf.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://fp.nicolike.cn

Ruby: class User; end
来源：http://cy.shxzukj.cn

C#:   class User {}
来源：http://ex.jianghongdianzi.cn

[G02] 构造函数
来源：http://sx.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://cv.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://yj.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://du.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://ll.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://nn.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lt.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://bi.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://jb.shxzukj.cn

[G03] 实例属性
来源：http://fq.newstarts.cn

Py:   self.name = "x"
来源：http://er.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://cq.shxzskj.cn

JS:   this.name = "x";
来源：http://sb.9csxet.cn

TS:   name: string = "x";
来源：http://ac.jianghongdianzi.cn

Java: private String name;
来源：http://ig.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jd.wgjwhj.cn

Ruby: @name = "x"
来源：http://su.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://bz.huanxung.cn

[G04] 定义方法
来源：http://qv.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://qu.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://td.newstarts.cn

JS:   greet() { return this.name; }
来源：http://sq.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://cf.haigaiapp.cn

Java: String greet() { return name; }
来源：http://zf.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ft.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://ff.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://nb.newstarts.cn

[G05] 继承
来源：http://wq.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://ou.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://cm.panjiajie.cn

JS:   class Admin extends User {}
来源：http://as.hahajie.cn

TS:   class Admin extends User {}
来源：http://nl.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://he.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xy.colortex.cn

Ruby: class Admin < User; end
来源：http://hl.haigaiapp.cn

C#:   class Admin : User {}
来源：http://zq.szxytkj.cn

[G06] 重写方法
来源：http://rl.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://mp.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vy.colortex.cn

JS:   greet() { return "admin"; }
来源：http://yt.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://mk.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://su.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yu.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://ib.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://jc.asd995.cn

[G07] 调用父类方法
来源：http://tz.lnxyls.cn

Py:   super().greet()
来源：http://gs.muxihuayi.cn

PHP:  parent::greet();
来源：http://wc.nicolike.cn

JS:   super.greet();
来源：http://rm.bjjhwx.cn

TS:   super.greet();
来源：http://wz.chemitech.net.cn

Java: super.greet();
来源：http://ai.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hr.jianghongdianzi.cn

Ruby: super
来源：http://rq.hahajie.cn

C#:   base.Greet();
来源：http://yr.asd995.cn

[G08] 静态方法与属性
来源：http://tw.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xd.shxzukj.cn

PHP:  public static function f() {}
来源：http://zz.jianghongdianzi.cn

JS:   static f() {}
来源：http://fk.panjiajie.cn

TS:   static f(): void {}
来源：http://lt.szxytkj.cn

Java: static void f() {}
来源：http://le.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xj.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://xs.huixiangedu.cn

C#:   public static void F() {}
来源：http://io.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://zf.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://gx.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ac.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kt.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://xq.asd995.cn

Java: interface Shape { double area(); }
来源：http://yg.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://qb.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ub.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://hp.muxihuayi.cn

[G10] 访问控制
来源：http://aa.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://cd.muxihuayi.cn

PHP:  public / protected / private
来源：http://ly.9csxet.cn

JS:   #private 字段；其余公开
来源：http://qm.muxihuayi.cn

TS:   public / protected / private
来源：http://ra.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://gl.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iz.asd995.cn

Ruby: public / protected / private
来源：http://sa.nicolike.cn

C#:   public / protected / private / internal
来源：http://qi.bjjhwx.cn

[G11] getter / setter
来源：http://sj.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://bi.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xb.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://kn.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://io.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://ht.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tj.szxytkj.cn

Ruby: attr_accessor :name
来源：http://zy.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://nm.szxytkj.cn

[G12] 对象转字符串
来源：http://rb.asd995.cn

Py:   def __str__(self): return self.name
来源：http://uv.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jk.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://fl.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://mo.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://uz.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dc.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ic.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://zk.huanxung.cn

[G13] 判断对象类型
来源：http://ps.huanxung.cn

Py:   isinstance(u, User)
来源：http://pl.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ij.shtwfgs.cn

JS:   u instanceof User
来源：http://it.nicolike.cn

TS:   u instanceof User
来源：http://oe.muxihuayi.cn

Java: u instanceof User
来源：http://vi.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nb.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://ck.asd995.cn

C#:   u is User
来源：http://wk.szxytkj.cn

[G14] 数据类 / record
来源：http://sh.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zl.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://em.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rp.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://dt.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://qw.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://xl.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zm.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://dc.nicolike.cn

[G15] 枚举
来源：http://fl.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mr.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://te.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oe.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://al.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://rn.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oq.nszjky.cn


<!-- 参考信息 -->