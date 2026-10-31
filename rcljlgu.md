代发 wailian999

PHP:  number_format(1234567);
来源：http://xc.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sh.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ei.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jn.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ev.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vb.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://qh.shxzskj.cn

[E17] 首字母大写
来源：http://ku.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rt.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jp.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ca.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ym.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vy.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cu.newstarts.cn

Ruby: s.capitalize
来源：http://gv.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yg.szsharing.cn

[E18] 模板占位符替换
来源：http://xd.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hm.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://om.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zz.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gv.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lt.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tw.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tc.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sm.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://ul.newstarts.cn

Py:   s.splitlines()
来源：http://zi.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rq.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://an.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://nj.nszjky.cn

Java: s.lines().toList()
来源：http://tm.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://nx.wgjwhj.cn

Ruby: s.lines
来源：http://qr.jctech888.com.cn

C#:   s.Split('\n')
来源：http://rt.nszjky.cn

[E20] 判断字符串是否为空
来源：http://pc.szxytkj.cn

Py:   if not s:
来源：http://gm.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zq.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tz.asd995.cn

TS:   if (s === "") {}
来源：http://eo.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://nq.szsharing.cn

Go:   if s == "" {}
来源：http://bc.521024.cn

Ruby: if s.empty?
来源：http://bq.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bl.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://qi.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kf.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pc.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ua.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://at.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bo.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://ub.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mi.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hj.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://xt.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qi.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kj.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uc.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zm.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eq.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ze.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://jl.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oi.bookmarksfly.cn

================================================================================
来源：http://jm.nszjky.cn

F. 文件与目录
来源：http://xk.haigaiapp.cn

================================================================================
来源：http://oc.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://dr.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gd.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://xw.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ft.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xg.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ig.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qy.szsharing.cn

Ruby: File.read("a.txt")
来源：http://eo.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://be.muxihuayi.cn

[F02] 逐行读取文件
来源：http://re.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kn.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fz.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qj.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aj.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wu.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yz.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ia.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mn.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://yr.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gp.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yg.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gk.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jq.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wn.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://au.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://nt.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lu.szxytkj.cn

[F04] 追加写入文件
来源：http://pz.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ek.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://np.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zw.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fv.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ju.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qz.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dr.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jv.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://mj.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nm.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://jw.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://nt.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://ak.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://og.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aq.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://ot.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://uk.szxytkj.cn

[F06] 删除文件
来源：http://da.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://xa.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://aj.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sw.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fo.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xv.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://yv.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://da.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://qi.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://hw.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tp.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bn.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://si.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rb.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yg.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://op.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eg.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ea.gzmigu.cn

[F08] 遍历目录
来源：http://rl.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bq.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://he.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://gs.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://xt.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qn.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jq.szsharing.cn

Ruby: Dir.children("dir")
来源：http://zb.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://by.panjiajie.cn

[F09] 获取文件大小
来源：http://aq.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://fq.hahajie.cn

PHP:  filesize("a.txt");
来源：http://oh.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://kz.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://og.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://im.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xm.nszjky.cn

Ruby: File.size("a.txt")
来源：http://ox.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://up.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://gr.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zr.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sj.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xn.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ze.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tb.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://be.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qw.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ux.muxihuayi.cn

[F11] 复制与移动文件
来源：http://wq.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://um.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ux.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vj.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hd.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qw.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dj.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qk.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cl.jianghongdianzi.cn

[F12] CSV 读写
来源：http://kz.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ut.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ek.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pd.asd995.cn

TS:   // 同上
来源：http://fr.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://er.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://by.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ci.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zh.hahajie.cn

================================================================================
来源：http://bz.nszjky.cn

G. 面向对象
来源：http://ro.wgjwhj.cn

================================================================================
来源：http://tm.panjiajie.cn

[G01] 定义类
来源：http://go.bookmarksfly.cn

Py:   class User: pass
来源：http://jm.bookmarksfly.cn

PHP:  class User {}
来源：http://gp.hnjuh.cn

JS:   class User {}
来源：http://ez.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://uo.colortex.cn

Java: class User {}
来源：http://ly.newstarts.cn

Go:   type User struct { Name string }
来源：http://jj.huixinmuqiang.cn

Ruby: class User; end
来源：http://we.9csxet.cn

C#:   class User {}
来源：http://pr.hahajie.cn

[G02] 构造函数
来源：http://nq.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://yf.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://qn.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://uf.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://kf.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://pl.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tk.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gy.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://wd.nicolike.cn

[G03] 实例属性
来源：http://ze.jctech888.com.cn

Py:   self.name = "x"
来源：http://sp.panjiajie.cn

PHP:  public string $name = "x";
来源：http://pr.shtwfgs.cn

JS:   this.name = "x";
来源：http://wv.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://gs.9csxet.cn

Java: private String name;
来源：http://po.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gw.lnxyls.cn

Ruby: @name = "x"
来源：http://pt.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://rm.9csxet.cn

[G04] 定义方法
来源：http://bw.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://wf.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mk.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://zz.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://mp.nszjky.cn

Java: String greet() { return name; }
来源：http://rx.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qo.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://we.huanxung.cn

C#:   public string Greet() => Name;
来源：http://yf.nicolike.cn

[G05] 继承
来源：http://no.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://qf.colortex.cn

PHP:  class Admin extends User {}
来源：http://av.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://jn.gzmigu.cn

TS:   class Admin extends User {}
来源：http://bq.lnxyls.cn

Java: class Admin extends User {}
来源：http://pa.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bh.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://jm.panjiajie.cn

C#:   class Admin : User {}
来源：http://wx.panjiajie.cn

[G06] 重写方法
来源：http://vx.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://no.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fg.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://gw.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://yk.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://qb.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xi.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://kt.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://ta.newstarts.cn

[G07] 调用父类方法
来源：http://xp.panjiajie.cn

Py:   super().greet()
来源：http://vl.nicolike.cn

PHP:  parent::greet();
来源：http://hw.bjjhwx.cn

JS:   super.greet();
来源：http://pq.nicolike.cn

TS:   super.greet();
来源：http://nv.yuexingan06.cn

Java: super.greet();
来源：http://vt.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wa.huanxung.cn

Ruby: super
来源：http://ur.yuntaijiaju.cn

C#:   base.Greet();
来源：http://mz.wgjwhj.cn

[G08] 静态方法与属性
来源：http://og.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bh.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://wf.nicolike.cn

JS:   static f() {}
来源：http://fg.shxzskj.cn

TS:   static f(): void {}
来源：http://gl.szxytkj.cn

Java: static void f() {}
来源：http://bt.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://we.bookmarksfly.cn

Ruby: def self.f; end
来源：http://rb.szsharing.cn

C#:   public static void F() {}
来源：http://dj.nszjky.cn

[G09] 接口 / 抽象类
来源：http://lw.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://eg.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vr.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hk.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://hp.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://tt.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://ak.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hd.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://jm.asd995.cn

[G10] 访问控制
来源：http://mk.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://wq.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://oe.szsharing.cn

JS:   #private 字段；其余公开
来源：http://ax.nszjky.cn

TS:   public / protected / private
来源：http://ze.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://uy.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qb.gzmigu.cn

Ruby: public / protected / private
来源：http://kb.shxzukj.cn

C#:   public / protected / private / internal
来源：http://ga.huixinmuqiang.cn

[G11] getter / setter
来源：http://vn.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://za.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pl.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://au.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://la.9csxet.cn

Java: public String getName() { return name; }
来源：http://ss.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://io.nszjky.cn

Ruby: attr_accessor :name
来源：http://me.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://vc.szsharing.cn

[G12] 对象转字符串
来源：http://ks.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://hx.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dt.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://on.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://oz.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://bg.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oz.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://bm.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://vi.colortex.cn

[G13] 判断对象类型
来源：http://hq.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://ko.521024.cn

PHP:  $u instanceof User
来源：http://dw.521024.cn

JS:   u instanceof User
来源：http://dt.hahajie.cn

TS:   u instanceof User
来源：http://su.9csxet.cn

Java: u instanceof User
来源：http://qk.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zv.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://xz.gzmigu.cn

C#:   u is User
来源：http://ho.9csxet.cn

[G14] 数据类 / record
来源：http://yb.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ni.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://hl.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zb.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://py.hahajie.cn

Java: record User(String name, int age) {}
来源：http://jg.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://hp.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lb.asd995.cn


<!-- 参考信息 -->