代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nb.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eq.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zf.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ag.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xu.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dn.nszjky.cn

Ruby: s.capitalize
来源：http://tk.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pj.panjiajie.cn

[E18] 模板占位符替换
来源：http://fa.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pm.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tu.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vc.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://of.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://re.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hq.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nn.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ws.huanxung.cn

[E19] 多行文本按行拆分
来源：http://vx.shtwfgs.cn

Py:   s.splitlines()
来源：http://ip.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aa.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://lk.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://tu.521024.cn

Java: s.lines().toList()
来源：http://ej.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://cn.nszjky.cn

Ruby: s.lines
来源：http://ub.hnjuh.cn

C#:   s.Split('\n')
来源：http://vm.szsharing.cn

[E20] 判断字符串是否为空
来源：http://cx.huanxung.cn

Py:   if not s:
来源：http://qc.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wt.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oo.panjiajie.cn

TS:   if (s === "") {}
来源：http://bc.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://hw.szsharing.cn

Go:   if s == "" {}
来源：http://li.muxihuayi.cn

Ruby: if s.empty?
来源：http://wv.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wl.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://kt.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yi.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lw.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vi.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nq.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://px.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://gk.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eg.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ex.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://ug.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qh.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zx.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vt.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ep.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nq.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ud.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://qj.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zz.newstarts.cn

================================================================================
来源：http://rm.wgjwhj.cn

F. 文件与目录
来源：http://no.shtwfgs.cn

================================================================================
来源：http://cc.chemitech.net.cn

[F01] 读取整个文件
来源：http://ji.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sx.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://um.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ui.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ba.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dk.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ts.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://bn.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://gu.bjjhwx.cn

[F02] 逐行读取文件
来源：http://zr.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fh.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://in.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ud.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kd.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ha.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lm.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sy.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cx.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://xi.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ht.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wl.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rl.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dc.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bd.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cv.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://fz.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tm.huixiangedu.cn

[F04] 追加写入文件
来源：http://qb.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pj.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lf.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yx.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://py.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cr.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sn.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hv.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lq.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://ix.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zb.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://fs.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://gw.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://qp.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fv.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mq.521024.cn

Ruby: File.exist?("a.txt")
来源：http://wa.colortex.cn

C#:   File.Exists("a.txt")
来源：http://ku.muxihuayi.cn

[F06] 删除文件
来源：http://kd.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://la.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://zw.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ss.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://si.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xe.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://wf.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://zc.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://qy.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://qa.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vz.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xo.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wk.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fl.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mw.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ya.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cn.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xc.lnxyls.cn

[F08] 遍历目录
来源：http://ka.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ih.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lk.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://lu.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://oi.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cd.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ff.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://fk.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://xf.shxzukj.cn

[F09] 获取文件大小
来源：http://zb.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://ey.nicolike.cn

PHP:  filesize("a.txt");
来源：http://bw.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://mw.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://kg.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oj.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oq.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://fi.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://wt.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://ex.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hl.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rx.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vr.nicolike.cn

TS:   path.extname("a.txt")
来源：http://nj.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ay.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ah.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pi.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jw.nszjky.cn

[F11] 复制与移动文件
来源：http://mw.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jz.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zt.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ap.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mo.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://go.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ve.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hj.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xb.jianghongdianzi.cn

[F12] CSV 读写
来源：http://wz.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kc.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://co.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nk.shtwfgs.cn

TS:   // 同上
来源：http://lg.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nh.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lu.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mj.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gh.panjiajie.cn

================================================================================
来源：http://er.muxihuayi.cn

G. 面向对象
来源：http://vm.wgjwhj.cn

================================================================================
来源：http://aj.szxytkj.cn

[G01] 定义类
来源：http://bu.yuntaijiaju.cn

Py:   class User: pass
来源：http://pw.chemitech.net.cn

PHP:  class User {}
来源：http://sd.asd995.cn

JS:   class User {}
来源：http://pj.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://pi.shxzskj.cn

Java: class User {}
来源：http://sw.hnjuh.cn

Go:   type User struct { Name string }
来源：http://md.nicolike.cn

Ruby: class User; end
来源：http://ib.haigaiapp.cn

C#:   class User {}
来源：http://lp.huanxung.cn

[G02] 构造函数
来源：http://xi.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://uw.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://mk.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://uq.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://ip.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://rd.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://py.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://md.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://ba.chemitech.net.cn

[G03] 实例属性
来源：http://wz.wgjwhj.cn

Py:   self.name = "x"
来源：http://hk.shxzskj.cn

PHP:  public string $name = "x";
来源：http://en.szxytkj.cn

JS:   this.name = "x";
来源：http://ah.szsharing.cn

TS:   name: string = "x";
来源：http://tb.nszjky.cn

Java: private String name;
来源：http://va.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://in.521024.cn

Ruby: @name = "x"
来源：http://af.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://ne.jctech888.com.cn

[G04] 定义方法
来源：http://lo.9csxet.cn

Py:   def greet(self): return self.name
来源：http://ss.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://za.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://ik.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://wh.lnxyls.cn

Java: String greet() { return name; }
来源：http://iv.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mg.asd995.cn

Ruby: def greet; @name; end
来源：http://ln.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://hk.huanxung.cn

[G05] 继承
来源：http://nm.shxzukj.cn

Py:   class Admin(User): pass
来源：http://xr.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://ll.colortex.cn

JS:   class Admin extends User {}
来源：http://rl.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://lw.lnxyls.cn

Java: class Admin extends User {}
来源：http://bb.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://as.szxytkj.cn

Ruby: class Admin < User; end
来源：http://zw.huanxung.cn

C#:   class Admin : User {}
来源：http://jw.colortex.cn

[G06] 重写方法
来源：http://cc.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://xj.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pr.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://gc.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://fm.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://cw.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lq.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://pz.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://xw.bjjhwx.cn

[G07] 调用父类方法
来源：http://hv.shxzukj.cn

Py:   super().greet()
来源：http://kt.muxihuayi.cn

PHP:  parent::greet();
来源：http://mv.jianghongdianzi.cn

JS:   super.greet();
来源：http://zk.haigaiapp.cn

TS:   super.greet();
来源：http://qy.shtwfgs.cn

Java: super.greet();
来源：http://hg.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qf.chemitech.net.cn

Ruby: super
来源：http://ke.huixiangedu.cn

C#:   base.Greet();
来源：http://ub.shxzskj.cn

[G08] 静态方法与属性
来源：http://mg.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qp.shxzukj.cn

PHP:  public static function f() {}
来源：http://al.nicolike.cn

JS:   static f() {}
来源：http://dl.shtwfgs.cn

TS:   static f(): void {}
来源：http://la.panjiajie.cn

Java: static void f() {}
来源：http://ix.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://md.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://yj.nicolike.cn

C#:   public static void F() {}
来源：http://ol.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://bs.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://lt.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qs.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ql.521024.cn

TS:   interface Shape { area(): number; }
来源：http://if.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://tb.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://bp.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zf.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://rp.shxzukj.cn

[G10] 访问控制
来源：http://te.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://ox.521024.cn

PHP:  public / protected / private
来源：http://jb.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://qg.haigaiapp.cn

TS:   public / protected / private
来源：http://xs.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://db.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kf.shtwfgs.cn

Ruby: public / protected / private
来源：http://vp.9csxet.cn

C#:   public / protected / private / internal
来源：http://sy.huanxung.cn

[G11] getter / setter
来源：http://di.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://by.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fq.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ps.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ks.panjiajie.cn

Java: public String getName() { return name; }
来源：http://hz.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xw.nicolike.cn

Ruby: attr_accessor :name
来源：http://fa.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://vm.hnjuh.cn

[G12] 对象转字符串
来源：http://zz.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://qs.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yl.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://uz.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://el.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://oh.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eo.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://mn.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://ba.jctech888.com.cn

[G13] 判断对象类型
来源：http://jz.newstarts.cn

Py:   isinstance(u, User)
来源：http://jw.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://xx.jctech888.com.cn

JS:   u instanceof User
来源：http://uo.jctech888.com.cn

TS:   u instanceof User
来源：http://oa.nicolike.cn

Java: u instanceof User
来源：http://wc.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rb.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://ua.shtwfgs.cn

C#:   u is User
来源：http://ko.521024.cn

[G14] 数据类 / record
来源：http://vs.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yv.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://az.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uz.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ts.521024.cn

Java: record User(String name, int age) {}
来源：http://iq.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://dk.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lp.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://yz.colortex.cn

[G15] 枚举
来源：http://mq.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zg.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zd.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jr.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uz.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://cv.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ad.gzmigu.cn


<!-- 参考信息 -->