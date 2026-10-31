代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yo.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vs.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://ul.yuexingan06.cn

[E17] 首字母大写
来源：http://ig.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ig.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ed.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vb.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nu.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xn.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ri.colortex.cn

Ruby: s.capitalize
来源：http://fb.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://da.muxihuayi.cn

[E18] 模板占位符替换
来源：http://ou.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pk.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fn.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gr.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pi.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uf.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cu.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ij.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dm.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://da.asd995.cn

Py:   s.splitlines()
来源：http://ny.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hk.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://jc.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://zk.jctech888.com.cn

Java: s.lines().toList()
来源：http://zw.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://mo.shxzukj.cn

Ruby: s.lines
来源：http://tc.huanxung.cn

C#:   s.Split('\n')
来源：http://yx.asd995.cn

[E20] 判断字符串是否为空
来源：http://yy.shxzukj.cn

Py:   if not s:
来源：http://pn.shtwfgs.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yy.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qp.gzmigu.cn

TS:   if (s === "") {}
来源：http://he.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://pd.nicolike.cn

Go:   if s == "" {}
来源：http://xy.wgjwhj.cn

Ruby: if s.empty?
来源：http://rz.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xb.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://cl.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cz.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sa.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cx.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fx.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xh.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://zy.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://if.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fx.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://iz.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://as.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cy.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vb.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xa.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rd.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://di.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://ef.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hc.jianghongdianzi.cn

================================================================================
来源：http://vq.huixiangedu.cn

F. 文件与目录
来源：http://hk.hahajie.cn

================================================================================
来源：http://al.shxzskj.cn

[F01] 读取整个文件
来源：http://ge.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pa.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://ds.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iu.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qu.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://et.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iv.9csxet.cn

Ruby: File.read("a.txt")
来源：http://lt.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://jn.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ms.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qc.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sr.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ub.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ux.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vb.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ib.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://st.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ub.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://ot.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vj.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mt.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mf.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bv.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ui.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qo.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://bb.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://li.shtwfgs.cn

[F04] 追加写入文件
来源：http://gt.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cr.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vk.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xc.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ch.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cl.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ai.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vr.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kz.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://qe.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ji.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://em.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://ec.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://wx.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tx.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tv.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://jv.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://sf.hnjuh.cn

[F06] 删除文件
来源：http://sf.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://se.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://xy.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kh.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hl.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://el.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://un.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://wv.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://nh.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://jb.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nl.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://az.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jt.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nt.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dd.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://di.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sx.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dj.colortex.cn

[F08] 遍历目录
来源：http://mj.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://we.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://br.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://ae.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://zh.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vi.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ay.9csxet.cn

Ruby: Dir.children("dir")
来源：http://vw.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://ru.muxihuayi.cn

[F09] 获取文件大小
来源：http://vo.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://co.9csxet.cn

PHP:  filesize("a.txt");
来源：http://oq.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://xs.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://ct.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hg.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vq.9csxet.cn

Ruby: File.size("a.txt")
来源：http://nb.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://ht.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://wd.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lp.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lr.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zj.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://vl.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tz.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ew.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nd.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zm.haigaiapp.cn

[F11] 复制与移动文件
来源：http://gh.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://be.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hf.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pf.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nc.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gp.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://es.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oj.newstarts.cn

[F12] CSV 读写
来源：http://ef.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fg.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sf.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wq.shxzukj.cn

TS:   // 同上
来源：http://no.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vr.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://py.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://en.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bp.gzmigu.cn

================================================================================
来源：http://wx.asd995.cn

G. 面向对象
来源：http://qw.haigaiapp.cn

================================================================================
来源：http://hp.huixinmuqiang.cn

[G01] 定义类
来源：http://nk.huanxung.cn

Py:   class User: pass
来源：http://nr.nszjky.cn

PHP:  class User {}
来源：http://gx.shxzskj.cn

JS:   class User {}
来源：http://yp.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://hm.bjjhwx.cn

Java: class User {}
来源：http://gi.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://mn.lnxyls.cn

Ruby: class User; end
来源：http://hl.colortex.cn

C#:   class User {}
来源：http://on.nicolike.cn

[G02] 构造函数
来源：http://yu.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://js.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://wk.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://qf.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://ia.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://if.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bl.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://xq.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://xo.huanxung.cn

[G03] 实例属性
来源：http://ve.shtwfgs.cn

Py:   self.name = "x"
来源：http://qj.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://ox.bookmarksfly.cn

JS:   this.name = "x";
来源：http://ev.lnxyls.cn

TS:   name: string = "x";
来源：http://ud.yuntaijiaju.cn

Java: private String name;
来源：http://kv.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eb.szxytkj.cn

Ruby: @name = "x"
来源：http://ye.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://he.bookmarksfly.cn

[G04] 定义方法
来源：http://hf.521024.cn

Py:   def greet(self): return self.name
来源：http://th.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gz.colortex.cn

JS:   greet() { return this.name; }
来源：http://jv.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://qb.wgjwhj.cn

Java: String greet() { return name; }
来源：http://tk.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nv.hahajie.cn

Ruby: def greet; @name; end
来源：http://rw.szsharing.cn

C#:   public string Greet() => Name;
来源：http://cj.521024.cn

[G05] 继承
来源：http://ls.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://zs.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://ub.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://kg.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://fp.9csxet.cn

Java: class Admin extends User {}
来源：http://kk.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sf.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://rt.bjjhwx.cn

C#:   class Admin : User {}
来源：http://zo.wgjwhj.cn

[G06] 重写方法
来源：http://ld.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://qe.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://my.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://dx.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://zx.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://ih.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qf.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://jc.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://dd.9csxet.cn

[G07] 调用父类方法
来源：http://ri.hahajie.cn

Py:   super().greet()
来源：http://gj.chemitech.net.cn

PHP:  parent::greet();
来源：http://rg.asd995.cn

JS:   super.greet();
来源：http://fh.huixinmuqiang.cn

TS:   super.greet();
来源：http://tw.shxzukj.cn

Java: super.greet();
来源：http://qq.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://am.nicolike.cn

Ruby: super
来源：http://fg.jctech888.com.cn

C#:   base.Greet();
来源：http://gw.huanxung.cn

[G08] 静态方法与属性
来源：http://vw.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nh.hnjuh.cn

PHP:  public static function f() {}
来源：http://zs.muxihuayi.cn

JS:   static f() {}
来源：http://tk.yuexingan06.cn

TS:   static f(): void {}
来源：http://wu.hnjuh.cn

Java: static void f() {}
来源：http://gt.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vw.nszjky.cn

Ruby: def self.f; end
来源：http://qz.colortex.cn

C#:   public static void F() {}
来源：http://np.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://wf.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://kr.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wt.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cq.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://cf.newstarts.cn

Java: interface Shape { double area(); }
来源：http://hy.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://mi.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pl.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ct.hnjuh.cn

[G10] 访问控制
来源：http://mj.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://mc.shxzskj.cn

PHP:  public / protected / private
来源：http://wc.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://bz.shtwfgs.cn

TS:   public / protected / private
来源：http://kf.521024.cn

Java: public / protected / private / 默认包级
来源：http://sb.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zs.gzmigu.cn

Ruby: public / protected / private
来源：http://hv.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://kd.521024.cn

[G11] getter / setter
来源：http://mx.hahajie.cn

Py:   @property 与 @x.setter
来源：http://ie.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dy.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://zu.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://tt.gzmigu.cn

Java: public String getName() { return name; }
来源：http://os.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://op.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://wm.nszjky.cn

C#:   public string Name { get; set; }
来源：http://xa.hnjuh.cn

[G12] 对象转字符串
来源：http://cp.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://dh.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wf.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://ym.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://fh.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://oo.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gb.521024.cn

Ruby: def to_s; @name; end
来源：http://eh.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://ne.lnxyls.cn

[G13] 判断对象类型
来源：http://pa.newstarts.cn

Py:   isinstance(u, User)
来源：http://uj.chemitech.net.cn

PHP:  $u instanceof User
来源：http://qk.muxihuayi.cn

JS:   u instanceof User
来源：http://dt.shxzukj.cn

TS:   u instanceof User
来源：http://qs.jianghongdianzi.cn

Java: u instanceof User
来源：http://ud.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ix.nszjky.cn

Ruby: u.is_a?(User)
来源：http://wf.wgjwhj.cn

C#:   u is User
来源：http://xx.muxihuayi.cn

[G14] 数据类 / record
来源：http://sx.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vo.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://gp.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://az.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://be.colortex.cn

Java: record User(String name, int age) {}
来源：http://ge.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://yj.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qk.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://pr.nszjky.cn

[G15] 枚举
来源：http://tu.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gg.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ie.newstarts.cn


<!-- 参考信息 -->