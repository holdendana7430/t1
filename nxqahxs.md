代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lw.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://av.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://lg.shxzskj.cn

[E17] 首字母大写
来源：http://bz.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lw.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jw.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fm.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://on.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mz.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mk.shxzskj.cn

Ruby: s.capitalize
来源：http://pv.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hu.huixiangedu.cn

[E18] 模板占位符替换
来源：http://ph.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ff.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wp.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eu.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xp.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rb.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zb.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pl.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://km.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://dd.gzmigu.cn

Py:   s.splitlines()
来源：http://ga.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vk.521024.cn

JS:   s.split(/\r?\n/)
来源：http://je.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://oz.bjjhwx.cn

Java: s.lines().toList()
来源：http://pz.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://as.hahajie.cn

Ruby: s.lines
来源：http://wv.gzmigu.cn

C#:   s.Split('\n')
来源：http://fs.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://nn.muxihuayi.cn

Py:   if not s:
来源：http://pg.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ye.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fr.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://zt.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://nf.bookmarksfly.cn

Go:   if s == "" {}
来源：http://xh.chemitech.net.cn

Ruby: if s.empty?
来源：http://pq.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gu.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://hb.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lc.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xh.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gp.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jj.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dx.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://ih.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qo.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://td.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://dt.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xd.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nx.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fe.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ug.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oo.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sr.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://jw.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xh.chemitech.net.cn

================================================================================
来源：http://jg.521024.cn

F. 文件与目录
来源：http://aj.gzmigu.cn

================================================================================
来源：http://rr.yuexingan06.cn

[F01] 读取整个文件
来源：http://it.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gf.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://yd.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gw.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bm.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ry.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rb.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://gi.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://ch.wgjwhj.cn

[F02] 逐行读取文件
来源：http://yy.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ee.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yf.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kg.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ok.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vf.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ua.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lg.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ml.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://dp.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xi.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mu.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uq.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ni.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kl.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ef.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://qc.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ky.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://jd.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ah.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://af.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://li.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pr.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gg.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zs.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://er.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ut.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://sp.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mj.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://jf.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ev.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://yj.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sx.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hb.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://dy.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://xt.521024.cn

[F06] 删除文件
来源：http://kj.huanxung.cn

Py:   os.remove("a.txt")
来源：http://kg.521024.cn

PHP:  unlink("a.txt");
来源：http://qm.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://np.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eb.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://na.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://ho.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://km.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://lx.nicolike.cn

[F07] 创建目录（含多级）
来源：http://yv.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ri.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ah.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hd.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rs.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dl.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kk.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yt.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ke.9csxet.cn

[F08] 遍历目录
来源：http://hy.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wb.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cd.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ev.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ed.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jx.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ip.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://hn.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://el.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://jb.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://dc.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://fi.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://zb.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://zh.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://no.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bz.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://fh.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://yo.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://pv.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qw.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zd.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jw.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://fo.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://or.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gz.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ub.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lq.nszjky.cn

[F11] 复制与移动文件
来源：http://fp.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nu.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uo.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gh.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fl.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bn.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sg.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xk.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lr.hnjuh.cn

[F12] CSV 读写
来源：http://gx.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cw.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ss.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bk.szsharing.cn

TS:   // 同上
来源：http://ao.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ne.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rd.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ru.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ba.huixiangedu.cn

================================================================================
来源：http://ev.nicolike.cn

G. 面向对象
来源：http://ro.gzmigu.cn

================================================================================
来源：http://rv.bjjhwx.cn

[G01] 定义类
来源：http://ja.chemitech.net.cn

Py:   class User: pass
来源：http://xm.lnxyls.cn

PHP:  class User {}
来源：http://xp.nicolike.cn

JS:   class User {}
来源：http://uh.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://rn.shxzskj.cn

Java: class User {}
来源：http://zk.colortex.cn

Go:   type User struct { Name string }
来源：http://vr.hnjuh.cn

Ruby: class User; end
来源：http://ga.shxzukj.cn

C#:   class User {}
来源：http://cv.shxzukj.cn

[G02] 构造函数
来源：http://yp.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://br.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://op.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://gv.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://xu.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://uw.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iu.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://nk.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://bo.hnjuh.cn

[G03] 实例属性
来源：http://yg.gzmigu.cn

Py:   self.name = "x"
来源：http://gg.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://qc.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://zi.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://hg.nicolike.cn

Java: private String name;
来源：http://ym.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ly.bjjhwx.cn

Ruby: @name = "x"
来源：http://mu.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ym.wgjwhj.cn

[G04] 定义方法
来源：http://so.huanxung.cn

Py:   def greet(self): return self.name
来源：http://kk.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rh.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://ou.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://ew.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://ek.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ur.hnjuh.cn

Ruby: def greet; @name; end
来源：http://ll.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://tu.shxzukj.cn

[G05] 继承
来源：http://rd.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://wl.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ef.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://yc.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://hk.haigaiapp.cn

Java: class Admin extends User {}
来源：http://vm.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ys.colortex.cn

Ruby: class Admin < User; end
来源：http://hu.yuexingan06.cn

C#:   class Admin : User {}
来源：http://iu.nicolike.cn

[G06] 重写方法
来源：http://ry.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ez.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xc.asd995.cn

JS:   greet() { return "admin"; }
来源：http://hi.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://cp.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://lu.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jf.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://kg.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://am.nicolike.cn

[G07] 调用父类方法
来源：http://eo.jctech888.com.cn

Py:   super().greet()
来源：http://bs.lnxyls.cn

PHP:  parent::greet();
来源：http://og.bjjhwx.cn

JS:   super.greet();
来源：http://it.nszjky.cn

TS:   super.greet();
来源：http://qe.szxytkj.cn

Java: super.greet();
来源：http://jq.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iq.gzmigu.cn

Ruby: super
来源：http://vs.newstarts.cn

C#:   base.Greet();
来源：http://kv.nszjky.cn

[G08] 静态方法与属性
来源：http://wq.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dv.9csxet.cn

PHP:  public static function f() {}
来源：http://rm.huixinmuqiang.cn

JS:   static f() {}
来源：http://yc.haigaiapp.cn

TS:   static f(): void {}
来源：http://sb.chemitech.net.cn

Java: static void f() {}
来源：http://cp.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aw.muxihuayi.cn

Ruby: def self.f; end
来源：http://fv.muxihuayi.cn

C#:   public static void F() {}
来源：http://cs.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://bh.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://dn.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yl.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://io.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://bc.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://br.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ue.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://yh.lnxyls.cn

[G10] 访问控制
来源：http://lz.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://lk.haigaiapp.cn

PHP:  public / protected / private
来源：http://vd.nicolike.cn

JS:   #private 字段；其余公开
来源：http://ai.nszjky.cn

TS:   public / protected / private
来源：http://zu.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://av.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tm.huanxung.cn

Ruby: public / protected / private
来源：http://zx.shxzukj.cn

C#:   public / protected / private / internal
来源：http://xh.shxzukj.cn

[G11] getter / setter
来源：http://td.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://wi.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bz.szsharing.cn

JS:   get name() { return this._name; }
来源：http://yx.521024.cn

TS:   get name(): string { return this._name; }
来源：http://op.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://es.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jh.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://gw.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://io.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://ox.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://qj.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yp.colortex.cn

JS:   toString() { return this.name; }
来源：http://fo.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://dn.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://nn.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ds.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://rm.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://ia.hahajie.cn

[G13] 判断对象类型
来源：http://ut.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://tl.yuexingan06.cn

PHP:  $u instanceof User
来源：http://hz.wgjwhj.cn

JS:   u instanceof User
来源：http://hf.huixiangedu.cn

TS:   u instanceof User
来源：http://qb.asd995.cn

Java: u instanceof User
来源：http://rf.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://id.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://xc.haigaiapp.cn

C#:   u is User
来源：http://vn.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://cd.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qz.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://mn.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lr.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://pu.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://lm.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://kn.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tr.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://sg.panjiajie.cn

[G15] 枚举
来源：http://be.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gr.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pq.muxihuayi.cn


<!-- 参考信息 -->