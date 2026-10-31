代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dz.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pu.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://fz.haigaiapp.cn

[E17] 首字母大写
来源：http://ig.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tk.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nj.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dd.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ue.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://we.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ya.nicolike.cn

Ruby: s.capitalize
来源：http://iw.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://av.hnjuh.cn

[E18] 模板占位符替换
来源：http://ue.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ox.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tg.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nc.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oq.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qu.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rv.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aa.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rd.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://dg.muxihuayi.cn

Py:   s.splitlines()
来源：http://hj.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hd.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://nu.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://hz.gzmigu.cn

Java: s.lines().toList()
来源：http://et.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://or.szxytkj.cn

Ruby: s.lines
来源：http://fk.panjiajie.cn

C#:   s.Split('\n')
来源：http://cz.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://um.hnjuh.cn

Py:   if not s:
来源：http://tx.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ib.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ym.szsharing.cn

TS:   if (s === "") {}
来源：http://ta.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://fh.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://vr.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://qc.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iz.shxzskj.cn

[E21] 超长截断加省略号
来源：http://lq.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qo.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yj.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tp.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ep.521024.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dx.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://cr.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://va.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vi.nicolike.cn

[E22] 字节长度与字符长度
来源：http://ix.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://la.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://do.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lu.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yi.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fj.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qo.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://kc.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zm.hnjuh.cn

================================================================================
来源：http://qc.shxzukj.cn

F. 文件与目录
来源：http://mo.asd995.cn

================================================================================
来源：http://ib.521024.cn

[F01] 读取整个文件
来源：http://vp.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kr.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://jl.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://na.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ap.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qx.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://op.nszjky.cn

Ruby: File.read("a.txt")
来源：http://uy.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://bd.nszjky.cn

[F02] 逐行读取文件
来源：http://bw.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://um.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gh.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hh.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rq.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://um.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hw.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rf.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cc.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://gz.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pj.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pm.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ff.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mx.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fk.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ng.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://ce.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mi.panjiajie.cn

[F04] 追加写入文件
来源：http://se.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lz.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xr.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rk.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yv.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aq.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yx.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fl.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lg.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://gp.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kt.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://dn.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://di.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://nc.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://io.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qp.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://qg.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://co.nszjky.cn

[F06] 删除文件
来源：http://xe.521024.cn

Py:   os.remove("a.txt")
来源：http://cw.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://lh.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tj.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cx.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hr.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://so.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://nn.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://zs.9csxet.cn

[F07] 创建目录（含多级）
来源：http://so.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vd.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cd.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hw.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zt.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tl.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sd.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pz.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hx.jianghongdianzi.cn

[F08] 遍历目录
来源：http://la.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wc.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://da.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://kp.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://ks.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ux.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fb.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://yd.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://tw.panjiajie.cn

[F09] 获取文件大小
来源：http://uj.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://kz.huanxung.cn

PHP:  filesize("a.txt");
来源：http://hs.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://lt.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://kv.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mv.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sm.hahajie.cn

Ruby: File.size("a.txt")
来源：http://cu.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://nb.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://yv.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dk.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ia.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pu.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://ur.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ji.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qx.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ud.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wm.jctech888.com.cn

[F11] 复制与移动文件
来源：http://vj.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gs.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pm.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zi.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gk.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ey.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fy.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sp.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oc.yuexingan06.cn

[F12] CSV 读写
来源：http://xs.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ww.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cn.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cz.lnxyls.cn

TS:   // 同上
来源：http://uv.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pm.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ys.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dj.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kr.huixinmuqiang.cn

================================================================================
来源：http://wq.bjjhwx.cn

G. 面向对象
来源：http://jv.lnxyls.cn

================================================================================
来源：http://su.shxzukj.cn

[G01] 定义类
来源：http://az.lnxyls.cn

Py:   class User: pass
来源：http://dp.nszjky.cn

PHP:  class User {}
来源：http://ue.lnxyls.cn

JS:   class User {}
来源：http://aw.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://by.huixiangedu.cn

Java: class User {}
来源：http://tv.hahajie.cn

Go:   type User struct { Name string }
来源：http://ju.lnxyls.cn

Ruby: class User; end
来源：http://vn.shxzskj.cn

C#:   class User {}
来源：http://wp.asd995.cn

[G02] 构造函数
来源：http://ao.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://yy.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://le.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://zr.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://zf.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://sg.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fk.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://sh.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://xt.shxzukj.cn

[G03] 实例属性
来源：http://dz.bookmarksfly.cn

Py:   self.name = "x"
来源：http://uu.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://wl.yuexingan06.cn

JS:   this.name = "x";
来源：http://up.muxihuayi.cn

TS:   name: string = "x";
来源：http://kx.yuexingan06.cn

Java: private String name;
来源：http://qu.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tq.chemitech.net.cn

Ruby: @name = "x"
来源：http://wn.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ri.shxzukj.cn

[G04] 定义方法
来源：http://iu.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://fl.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ou.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://jp.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://ki.huanxung.cn

Java: String greet() { return name; }
来源：http://ay.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gk.shxzukj.cn

Ruby: def greet; @name; end
来源：http://cq.colortex.cn

C#:   public string Greet() => Name;
来源：http://uw.bookmarksfly.cn

[G05] 继承
来源：http://vl.hahajie.cn

Py:   class Admin(User): pass
来源：http://ph.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://rm.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://yk.gzmigu.cn

TS:   class Admin extends User {}
来源：http://qk.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://su.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jv.panjiajie.cn

Ruby: class Admin < User; end
来源：http://jf.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ov.haigaiapp.cn

[G06] 重写方法
来源：http://sl.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://mx.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vn.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://nl.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://aq.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://if.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fq.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://qq.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://jb.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://qg.asd995.cn

Py:   super().greet()
来源：http://kn.newstarts.cn

PHP:  parent::greet();
来源：http://dy.yuexingan06.cn

JS:   super.greet();
来源：http://yg.nicolike.cn

TS:   super.greet();
来源：http://wm.szxytkj.cn

Java: super.greet();
来源：http://nx.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ci.szxytkj.cn

Ruby: super
来源：http://wc.panjiajie.cn

C#:   base.Greet();
来源：http://lw.wgjwhj.cn

[G08] 静态方法与属性
来源：http://dz.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cs.haigaiapp.cn

PHP:  public static function f() {}
来源：http://pk.muxihuayi.cn

JS:   static f() {}
来源：http://bh.chemitech.net.cn

TS:   static f(): void {}
来源：http://dl.wgjwhj.cn

Java: static void f() {}
来源：http://bk.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jx.gzmigu.cn

Ruby: def self.f; end
来源：http://qx.colortex.cn

C#:   public static void F() {}
来源：http://to.521024.cn

[G09] 接口 / 抽象类
来源：http://bl.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://sm.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qc.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pw.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://zd.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://bz.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://pl.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bs.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://zj.panjiajie.cn

[G10] 访问控制
来源：http://eh.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://yc.shxzukj.cn

PHP:  public / protected / private
来源：http://vk.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://vt.asd995.cn

TS:   public / protected / private
来源：http://wk.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://pr.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ux.gzmigu.cn

Ruby: public / protected / private
来源：http://el.hnjuh.cn

C#:   public / protected / private / internal
来源：http://vv.lnxyls.cn

[G11] getter / setter
来源：http://ax.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://is.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://dh.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://lj.lnxyls.cn

Java: public String getName() { return name; }
来源：http://yz.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fa.lnxyls.cn

Ruby: attr_accessor :name
来源：http://vs.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://yq.hahajie.cn

[G12] 对象转字符串
来源：http://gz.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://iu.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nz.asd995.cn

JS:   toString() { return this.name; }
来源：http://iv.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://ct.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://dh.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mw.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://nr.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://do.nicolike.cn

[G13] 判断对象类型
来源：http://ew.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://tx.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://zm.521024.cn

JS:   u instanceof User
来源：http://sw.shtwfgs.cn

TS:   u instanceof User
来源：http://uj.bookmarksfly.cn

Java: u instanceof User
来源：http://ka.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://he.huanxung.cn

Ruby: u.is_a?(User)
来源：http://yi.nicolike.cn

C#:   u is User
来源：http://ek.yuexingan06.cn

[G14] 数据类 / record
来源：http://so.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qc.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://lv.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qh.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://hl.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://er.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://aj.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ci.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://aw.bjjhwx.cn

[G15] 枚举
来源：http://wh.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rz.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ng.muxihuayi.cn


<!-- 参考信息 -->