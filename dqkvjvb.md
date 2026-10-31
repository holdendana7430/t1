代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lf.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pz.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://vi.wgjwhj.cn

[E17] 首字母大写
来源：http://bm.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pf.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zt.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pn.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sy.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vq.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zi.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://ab.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zg.panjiajie.cn

[E18] 模板占位符替换
来源：http://zu.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ua.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bd.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fh.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wp.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xa.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fq.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ap.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ym.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://iu.jctech888.com.cn

Py:   s.splitlines()
来源：http://fj.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rc.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://ps.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ya.hnjuh.cn

Java: s.lines().toList()
来源：http://dq.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://cm.shxzukj.cn

Ruby: s.lines
来源：http://iz.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://mm.hahajie.cn

[E20] 判断字符串是否为空
来源：http://qr.colortex.cn

Py:   if not s:
来源：http://nd.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yt.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bn.shxzukj.cn

TS:   if (s === "") {}
来源：http://xf.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://ak.shxzukj.cn

Go:   if s == "" {}
来源：http://qx.szxytkj.cn

Ruby: if s.empty?
来源：http://vj.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wo.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://tw.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gt.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mp.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yo.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pb.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://se.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://hj.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://de.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xb.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://st.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ea.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ch.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ly.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pa.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kv.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kx.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://nd.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qn.shxzukj.cn

================================================================================
来源：http://kt.szxytkj.cn

F. 文件与目录
来源：http://lg.9csxet.cn

================================================================================
来源：http://ec.shxzskj.cn

[F01] 读取整个文件
来源：http://oy.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gd.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://yn.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vz.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bc.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://it.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://op.hahajie.cn

Ruby: File.read("a.txt")
来源：http://dq.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://ur.shtwfgs.cn

[F02] 逐行读取文件
来源：http://tq.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://za.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nf.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cc.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pi.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ux.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ne.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kq.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://el.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://af.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gx.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tr.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://er.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ha.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://al.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jg.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://th.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ro.panjiajie.cn

[F04] 追加写入文件
来源：http://ui.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zb.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ku.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://um.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wf.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oi.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mw.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://it.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vf.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://vu.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://va.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://el.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://pf.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://mw.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yk.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rw.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://ud.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://be.newstarts.cn

[F06] 删除文件
来源：http://mc.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://il.nicolike.cn

PHP:  unlink("a.txt");
来源：http://bd.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://da.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ff.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rk.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://im.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://ik.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://qw.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://aw.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rr.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ea.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://en.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ie.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://da.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://us.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gt.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://op.lnxyls.cn

[F08] 遍历目录
来源：http://wa.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ss.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kw.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://bm.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://kc.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ub.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ny.newstarts.cn

Ruby: Dir.children("dir")
来源：http://kw.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://df.muxihuayi.cn

[F09] 获取文件大小
来源：http://go.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://as.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://hz.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://zy.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://gd.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xw.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ag.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://nd.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://gd.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ef.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gt.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ki.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bx.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://pf.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ix.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wh.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ww.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ht.haigaiapp.cn

[F11] 复制与移动文件
来源：http://oh.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nv.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ze.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pg.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ed.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ay.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zu.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wz.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xg.huixinmuqiang.cn

[F12] CSV 读写
来源：http://cj.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fe.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sc.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yh.521024.cn

TS:   // 同上
来源：http://rl.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ib.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oi.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://to.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qh.huixinmuqiang.cn

================================================================================
来源：http://va.gzmigu.cn

G. 面向对象
来源：http://bk.shxzskj.cn

================================================================================
来源：http://tg.shxzukj.cn

[G01] 定义类
来源：http://ux.wgjwhj.cn

Py:   class User: pass
来源：http://nn.yuexingan06.cn

PHP:  class User {}
来源：http://oz.colortex.cn

JS:   class User {}
来源：http://pg.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://qz.shxzukj.cn

Java: class User {}
来源：http://rk.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://ie.haigaiapp.cn

Ruby: class User; end
来源：http://gx.shtwfgs.cn

C#:   class User {}
来源：http://he.bookmarksfly.cn

[G02] 构造函数
来源：http://wb.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://lm.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://cx.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://qo.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://wv.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://ym.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aq.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ts.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://pn.shtwfgs.cn

[G03] 实例属性
来源：http://nv.hahajie.cn

Py:   self.name = "x"
来源：http://ev.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://jj.gzmigu.cn

JS:   this.name = "x";
来源：http://hv.bookmarksfly.cn

TS:   name: string = "x";
来源：http://dy.shxzukj.cn

Java: private String name;
来源：http://tv.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mh.panjiajie.cn

Ruby: @name = "x"
来源：http://pv.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://jm.muxihuayi.cn

[G04] 定义方法
来源：http://oi.szsharing.cn

Py:   def greet(self): return self.name
来源：http://kp.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hx.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://kn.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://fi.muxihuayi.cn

Java: String greet() { return name; }
来源：http://iq.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sr.hahajie.cn

Ruby: def greet; @name; end
来源：http://wn.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://jm.bookmarksfly.cn

[G05] 继承
来源：http://iq.9csxet.cn

Py:   class Admin(User): pass
来源：http://ul.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://sp.newstarts.cn

JS:   class Admin extends User {}
来源：http://lw.shxzukj.cn

TS:   class Admin extends User {}
来源：http://oc.haigaiapp.cn

Java: class Admin extends User {}
来源：http://wo.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://up.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://no.muxihuayi.cn

C#:   class Admin : User {}
来源：http://rx.panjiajie.cn

[G06] 重写方法
来源：http://zc.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://zd.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ao.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://gr.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://aj.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://zi.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ni.521024.cn

Ruby: def greet; "admin"; end
来源：http://ml.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://ec.jctech888.com.cn

[G07] 调用父类方法
来源：http://tz.szxytkj.cn

Py:   super().greet()
来源：http://zm.chemitech.net.cn

PHP:  parent::greet();
来源：http://kn.chemitech.net.cn

JS:   super.greet();
来源：http://ct.huixinmuqiang.cn

TS:   super.greet();
来源：http://wt.jianghongdianzi.cn

Java: super.greet();
来源：http://hs.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://np.shtwfgs.cn

Ruby: super
来源：http://az.huanxung.cn

C#:   base.Greet();
来源：http://tv.muxihuayi.cn

[G08] 静态方法与属性
来源：http://of.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nk.szxytkj.cn

PHP:  public static function f() {}
来源：http://se.shtwfgs.cn

JS:   static f() {}
来源：http://ec.huixiangedu.cn

TS:   static f(): void {}
来源：http://wv.huanxung.cn

Java: static void f() {}
来源：http://ng.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nz.shxzskj.cn

Ruby: def self.f; end
来源：http://mk.lnxyls.cn

C#:   public static void F() {}
来源：http://sr.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://cq.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://ef.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://be.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vs.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://lv.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://sd.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://kb.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://do.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://me.muxihuayi.cn

[G10] 访问控制
来源：http://kp.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://ky.huanxung.cn

PHP:  public / protected / private
来源：http://wk.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://vi.9csxet.cn

TS:   public / protected / private
来源：http://ry.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://mt.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zk.chemitech.net.cn

Ruby: public / protected / private
来源：http://lv.lnxyls.cn

C#:   public / protected / private / internal
来源：http://kp.shxzukj.cn

[G11] getter / setter
来源：http://jc.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://rj.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://do.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://aw.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://yz.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://dd.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://th.lnxyls.cn

Ruby: attr_accessor :name
来源：http://xg.newstarts.cn

C#:   public string Name { get; set; }
来源：http://gj.jctech888.com.cn

[G12] 对象转字符串
来源：http://iv.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://em.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ru.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://us.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://zl.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://pu.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hx.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://hu.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://au.gzmigu.cn

[G13] 判断对象类型
来源：http://eb.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://rv.hnjuh.cn

PHP:  $u instanceof User
来源：http://cq.521024.cn

JS:   u instanceof User
来源：http://ro.nszjky.cn

TS:   u instanceof User
来源：http://kj.shtwfgs.cn

Java: u instanceof User
来源：http://bl.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vq.9csxet.cn

Ruby: u.is_a?(User)
来源：http://ii.shxzskj.cn

C#:   u is User
来源：http://lb.hnjuh.cn

[G14] 数据类 / record
来源：http://ir.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sc.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://iw.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eh.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://sv.asd995.cn

Java: record User(String name, int age) {}
来源：http://wq.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://ox.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wb.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://dx.huixinmuqiang.cn

[G15] 枚举
来源：http://cb.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yj.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ac.chemitech.net.cn


<!-- 参考信息 -->