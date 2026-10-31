代发 wailian999

PHP:  number_format(1234567);
来源：http://so.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://or.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wh.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wh.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ez.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ec.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://tk.521024.cn

[E17] 首字母大写
来源：http://yb.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qy.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ly.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bm.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zy.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xu.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lz.9csxet.cn

Ruby: s.capitalize
来源：http://rm.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ve.szsharing.cn

[E18] 模板占位符替换
来源：http://dp.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jy.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lr.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tj.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uf.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hl.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oi.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hv.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vv.newstarts.cn

[E19] 多行文本按行拆分
来源：http://ge.shxzskj.cn

Py:   s.splitlines()
来源：http://dp.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qd.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://yy.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://jq.jctech888.com.cn

Java: s.lines().toList()
来源：http://jt.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://rn.jianghongdianzi.cn

Ruby: s.lines
来源：http://nx.bjjhwx.cn

C#:   s.Split('\n')
来源：http://ph.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://pn.shtwfgs.cn

Py:   if not s:
来源：http://ba.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rd.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rm.9csxet.cn

TS:   if (s === "") {}
来源：http://fi.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://kn.hahajie.cn

Go:   if s == "" {}
来源：http://ho.chemitech.net.cn

Ruby: if s.empty?
来源：http://pr.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ye.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://pz.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xo.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dl.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ms.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ym.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qt.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://xr.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yo.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wy.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://py.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xq.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ay.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bi.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aa.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rz.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fg.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://fo.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bn.newstarts.cn

================================================================================
来源：http://zc.haigaiapp.cn

F. 文件与目录
来源：http://ef.yuntaijiaju.cn

================================================================================
来源：http://si.bjjhwx.cn

[F01] 读取整个文件
来源：http://kf.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qj.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://se.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xs.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mb.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gq.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://in.9csxet.cn

Ruby: File.read("a.txt")
来源：http://zz.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://jb.jctech888.com.cn

[F02] 逐行读取文件
来源：http://ba.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mg.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kq.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mn.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uk.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dd.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pe.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ni.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xf.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://xy.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jl.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kf.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cb.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gr.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wn.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pp.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://xr.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fe.gzmigu.cn

[F04] 追加写入文件
来源：http://ug.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ty.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vd.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kj.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tw.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ku.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xy.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gp.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wh.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://tv.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gf.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://in.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://dd.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://vf.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fn.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ad.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://ys.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://ib.huixinmuqiang.cn

[F06] 删除文件
来源：http://xw.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://xq.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://ui.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dz.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zs.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xm.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://gr.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://rf.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://sx.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://fi.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cm.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ym.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ma.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://db.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rc.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lw.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ag.szsharing.cn

[F08] 遍历目录
来源：http://zh.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yd.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nv.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://ys.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://mu.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://au.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xe.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://uq.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://eu.haigaiapp.cn

[F09] 获取文件大小
来源：http://qb.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://it.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://pd.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://pn.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://cn.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hb.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ih.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://pr.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://yu.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://gw.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eo.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jl.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sa.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ix.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ty.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ji.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qk.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kv.huixiangedu.cn

[F11] 复制与移动文件
来源：http://rk.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vl.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tt.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uo.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ru.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hy.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pi.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hc.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ne.bookmarksfly.cn

[F12] CSV 读写
来源：http://hl.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ob.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fp.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bt.521024.cn

TS:   // 同上
来源：http://hs.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ms.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eb.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tl.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lq.hnjuh.cn

================================================================================
来源：http://tm.colortex.cn

G. 面向对象
来源：http://zu.szsharing.cn

================================================================================
来源：http://tv.nszjky.cn

[G01] 定义类
来源：http://gq.bookmarksfly.cn

Py:   class User: pass
来源：http://tk.huixinmuqiang.cn

PHP:  class User {}
来源：http://pi.newstarts.cn

JS:   class User {}
来源：http://cm.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://be.yuntaijiaju.cn

Java: class User {}
来源：http://xd.hnjuh.cn

Go:   type User struct { Name string }
来源：http://wb.nicolike.cn

Ruby: class User; end
来源：http://lc.huixinmuqiang.cn

C#:   class User {}
来源：http://wv.huanxung.cn

[G02] 构造函数
来源：http://hr.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://av.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ie.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://uy.521024.cn

TS:   constructor(public name: string) {}
来源：http://bn.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://ac.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fg.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://at.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://lg.lnxyls.cn

[G03] 实例属性
来源：http://yy.hahajie.cn

Py:   self.name = "x"
来源：http://um.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://js.gzmigu.cn

JS:   this.name = "x";
来源：http://ox.bookmarksfly.cn

TS:   name: string = "x";
来源：http://bf.wgjwhj.cn

Java: private String name;
来源：http://il.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ov.wgjwhj.cn

Ruby: @name = "x"
来源：http://cw.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://vc.wgjwhj.cn

[G04] 定义方法
来源：http://nd.asd995.cn

Py:   def greet(self): return self.name
来源：http://fa.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fk.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://cp.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://gk.panjiajie.cn

Java: String greet() { return name; }
来源：http://kq.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ne.521024.cn

Ruby: def greet; @name; end
来源：http://ce.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://nv.nicolike.cn

[G05] 继承
来源：http://sp.szsharing.cn

Py:   class Admin(User): pass
来源：http://op.hahajie.cn

PHP:  class Admin extends User {}
来源：http://ns.9csxet.cn

JS:   class Admin extends User {}
来源：http://wt.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://tl.huanxung.cn

Java: class Admin extends User {}
来源：http://rs.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ef.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://mg.nicolike.cn

C#:   class Admin : User {}
来源：http://uf.yuntaijiaju.cn

[G06] 重写方法
来源：http://ae.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://jm.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ef.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ae.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://dq.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://qu.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gn.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://vr.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://ls.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://zz.muxihuayi.cn

Py:   super().greet()
来源：http://yb.gzmigu.cn

PHP:  parent::greet();
来源：http://fq.shxzukj.cn

JS:   super.greet();
来源：http://xg.nicolike.cn

TS:   super.greet();
来源：http://md.colortex.cn

Java: super.greet();
来源：http://pz.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cc.bookmarksfly.cn

Ruby: super
来源：http://wz.nszjky.cn

C#:   base.Greet();
来源：http://ys.lnxyls.cn

[G08] 静态方法与属性
来源：http://mt.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bg.chemitech.net.cn

PHP:  public static function f() {}
来源：http://wf.jctech888.com.cn

JS:   static f() {}
来源：http://bf.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://xc.szxytkj.cn

Java: static void f() {}
来源：http://zz.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vm.521024.cn

Ruby: def self.f; end
来源：http://in.nszjky.cn

C#:   public static void F() {}
来源：http://pl.colortex.cn

[G09] 接口 / 抽象类
来源：http://pu.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://hq.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jd.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vf.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://nx.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://ov.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://dx.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mn.521024.cn

C#:   interface IShape { double Area(); }
来源：http://yk.huanxung.cn

[G10] 访问控制
来源：http://rg.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hq.huanxung.cn

PHP:  public / protected / private
来源：http://yz.9csxet.cn

JS:   #private 字段；其余公开
来源：http://bn.nicolike.cn

TS:   public / protected / private
来源：http://vl.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://yz.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pt.wgjwhj.cn

Ruby: public / protected / private
来源：http://iq.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://ue.shxzskj.cn

[G11] getter / setter
来源：http://jr.hahajie.cn

Py:   @property 与 @x.setter
来源：http://vg.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bk.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://gz.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://zt.nicolike.cn

Java: public String getName() { return name; }
来源：http://hx.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wb.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://ye.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://cz.yuexingan06.cn

[G12] 对象转字符串
来源：http://ou.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://fm.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sl.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://ww.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://qv.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://zb.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jk.colortex.cn

Ruby: def to_s; @name; end
来源：http://rx.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://hp.shtwfgs.cn

[G13] 判断对象类型
来源：http://pu.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://os.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://un.nszjky.cn

JS:   u instanceof User
来源：http://os.bjjhwx.cn

TS:   u instanceof User
来源：http://tw.colortex.cn

Java: u instanceof User
来源：http://an.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nm.nicolike.cn

Ruby: u.is_a?(User)
来源：http://hn.gzmigu.cn

C#:   u is User
来源：http://in.szxytkj.cn

[G14] 数据类 / record
来源：http://ld.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lj.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://sa.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hy.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://uv.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://au.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://gv.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rc.shxzskj.cn


<!-- 参考信息 -->