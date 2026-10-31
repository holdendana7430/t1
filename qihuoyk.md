代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xn.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wi.gzmigu.cn

Ruby: s.capitalize
来源：http://es.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jq.nicolike.cn

[E18] 模板占位符替换
来源：http://mb.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dq.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ts.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uh.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qo.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hk.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nt.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cg.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jz.hahajie.cn

[E19] 多行文本按行拆分
来源：http://fo.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://sq.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jy.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://pg.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://tc.yuexingan06.cn

Java: s.lines().toList()
来源：http://cz.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://wl.panjiajie.cn

Ruby: s.lines
来源：http://cj.yuexingan06.cn

C#:   s.Split('\n')
来源：http://ue.newstarts.cn

[E20] 判断字符串是否为空
来源：http://qx.szxytkj.cn

Py:   if not s:
来源：http://sh.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tx.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dl.shxzukj.cn

TS:   if (s === "") {}
来源：http://nd.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ck.wgjwhj.cn

Go:   if s == "" {}
来源：http://et.521024.cn

Ruby: if s.empty?
来源：http://xc.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fm.panjiajie.cn

[E21] 超长截断加省略号
来源：http://bq.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sm.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pq.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qd.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dn.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jq.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://ik.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://if.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ze.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://zq.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zk.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lp.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://su.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qf.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fm.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kb.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://bx.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gs.asd995.cn

================================================================================
来源：http://mt.szsharing.cn

F. 文件与目录
来源：http://pw.yuntaijiaju.cn

================================================================================
来源：http://io.newstarts.cn

[F01] 读取整个文件
来源：http://hm.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ce.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://bt.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ta.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rn.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jc.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rp.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://ms.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://qq.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://fk.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sx.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://si.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lq.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kg.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nm.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tw.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fc.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://lo.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ax.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xs.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ab.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eu.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://me.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ph.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://ey.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mq.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://it.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eg.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qx.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gr.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mn.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fo.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://id.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zl.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jz.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://po.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oe.asd995.cn

PHP:  file_exists("a.txt");
来源：http://mv.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://hw.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://zj.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hs.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nv.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://ld.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://nw.newstarts.cn

[F06] 删除文件
来源：http://sz.colortex.cn

Py:   os.remove("a.txt")
来源：http://bj.asd995.cn

PHP:  unlink("a.txt");
来源：http://ao.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://br.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yb.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ks.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://uq.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://yt.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://vp.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://ok.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uy.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ur.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bg.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bn.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eb.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xh.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ru.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iv.yuntaijiaju.cn

[F08] 遍历目录
来源：http://dy.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cu.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ij.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://vo.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://ss.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yc.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rm.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://qd.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://jt.gzmigu.cn

[F09] 获取文件大小
来源：http://zz.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://dw.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://ij.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://rp.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://nr.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ez.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vo.nicolike.cn

Ruby: File.size("a.txt")
来源：http://bk.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://hm.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://wm.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kw.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xj.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://km.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://cc.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://td.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hd.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jl.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xd.nszjky.cn

[F11] 复制与移动文件
来源：http://xf.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rd.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ew.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uu.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bh.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zb.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sh.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dz.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hl.521024.cn

[F12] CSV 读写
来源：http://ve.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sy.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://km.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oc.newstarts.cn

TS:   // 同上
来源：http://lj.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iw.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jx.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gm.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iv.wgjwhj.cn

================================================================================
来源：http://xk.newstarts.cn

G. 面向对象
来源：http://ra.colortex.cn

================================================================================
来源：http://bz.huanxung.cn

[G01] 定义类
来源：http://yp.hahajie.cn

Py:   class User: pass
来源：http://ie.bjjhwx.cn

PHP:  class User {}
来源：http://sc.9csxet.cn

JS:   class User {}
来源：http://br.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://ov.huixiangedu.cn

Java: class User {}
来源：http://fa.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://yi.shtwfgs.cn

Ruby: class User; end
来源：http://vu.colortex.cn

C#:   class User {}
来源：http://ag.chemitech.net.cn

[G02] 构造函数
来源：http://kg.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://xc.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://ov.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://qc.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://bu.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://pq.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ga.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://ob.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://uo.colortex.cn

[G03] 实例属性
来源：http://ms.wgjwhj.cn

Py:   self.name = "x"
来源：http://ts.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://qh.hnjuh.cn

JS:   this.name = "x";
来源：http://td.muxihuayi.cn

TS:   name: string = "x";
来源：http://sp.bookmarksfly.cn

Java: private String name;
来源：http://as.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wf.shxzskj.cn

Ruby: @name = "x"
来源：http://mp.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://qp.jianghongdianzi.cn

[G04] 定义方法
来源：http://dg.521024.cn

Py:   def greet(self): return self.name
来源：http://tq.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ee.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://rf.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://yi.haigaiapp.cn

Java: String greet() { return name; }
来源：http://ae.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://go.521024.cn

Ruby: def greet; @name; end
来源：http://ck.szsharing.cn

C#:   public string Greet() => Name;
来源：http://bo.521024.cn

[G05] 继承
来源：http://bd.szxytkj.cn

Py:   class Admin(User): pass
来源：http://ez.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://rs.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://dx.521024.cn

TS:   class Admin extends User {}
来源：http://su.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://vl.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tg.panjiajie.cn

Ruby: class Admin < User; end
来源：http://by.lnxyls.cn

C#:   class Admin : User {}
来源：http://as.bookmarksfly.cn

[G06] 重写方法
来源：http://zj.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://xc.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oc.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://rs.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://ka.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://sw.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fy.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://rw.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://yc.nszjky.cn

[G07] 调用父类方法
来源：http://ra.9csxet.cn

Py:   super().greet()
来源：http://da.shxzskj.cn

PHP:  parent::greet();
来源：http://ai.jianghongdianzi.cn

JS:   super.greet();
来源：http://bp.panjiajie.cn

TS:   super.greet();
来源：http://nn.yuexingan06.cn

Java: super.greet();
来源：http://sx.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ec.jctech888.com.cn

Ruby: super
来源：http://kb.bookmarksfly.cn

C#:   base.Greet();
来源：http://ux.shxzukj.cn

[G08] 静态方法与属性
来源：http://wc.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tk.nicolike.cn

PHP:  public static function f() {}
来源：http://ew.colortex.cn

JS:   static f() {}
来源：http://pw.chemitech.net.cn

TS:   static f(): void {}
来源：http://op.yuexingan06.cn

Java: static void f() {}
来源：http://we.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ed.szsharing.cn

Ruby: def self.f; end
来源：http://ez.hnjuh.cn

C#:   public static void F() {}
来源：http://dy.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://bj.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://nz.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pl.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tw.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://xd.nszjky.cn

Java: interface Shape { double area(); }
来源：http://qa.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://dp.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xv.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://wm.yuntaijiaju.cn

[G10] 访问控制
来源：http://mr.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://of.521024.cn

PHP:  public / protected / private
来源：http://po.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://ff.jctech888.com.cn

TS:   public / protected / private
来源：http://ef.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://ie.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vv.haigaiapp.cn

Ruby: public / protected / private
来源：http://ut.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://jb.lnxyls.cn

[G11] getter / setter
来源：http://bw.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://uo.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ae.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://ad.521024.cn

TS:   get name(): string { return this._name; }
来源：http://xb.colortex.cn

Java: public String getName() { return name; }
来源：http://rk.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://si.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://tu.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://pw.hahajie.cn

[G12] 对象转字符串
来源：http://oe.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://nm.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://it.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://vi.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://yp.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://uy.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ol.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://ug.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://na.colortex.cn

[G13] 判断对象类型
来源：http://be.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://ty.colortex.cn

PHP:  $u instanceof User
来源：http://mg.huixinmuqiang.cn

JS:   u instanceof User
来源：http://ur.colortex.cn

TS:   u instanceof User
来源：http://sl.huanxung.cn

Java: u instanceof User
来源：http://gq.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ms.hahajie.cn

Ruby: u.is_a?(User)
来源：http://oq.gzmigu.cn

C#:   u is User
来源：http://ur.szsharing.cn

[G14] 数据类 / record
来源：http://di.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wo.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://yh.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://td.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://ky.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://ll.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://xp.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dc.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://nk.yuntaijiaju.cn

[G15] 枚举
来源：http://we.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ab.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vy.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://da.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xj.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://cz.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://za.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://pz.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rb.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://um.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oj.muxihuayi.cn


<!-- 参考信息 -->