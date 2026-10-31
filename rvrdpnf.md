代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ib.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mh.gzmigu.cn

Ruby: s.capitalize
来源：http://qt.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rf.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://oz.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sl.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fi.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ko.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cl.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qd.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jg.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://po.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pq.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://in.asd995.cn

Py:   s.splitlines()
来源：http://se.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zt.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ya.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://vf.shxzskj.cn

Java: s.lines().toList()
来源：http://zn.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://oc.bookmarksfly.cn

Ruby: s.lines
来源：http://ny.shxzskj.cn

C#:   s.Split('\n')
来源：http://vn.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://hm.521024.cn

Py:   if not s:
来源：http://md.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ay.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uv.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://mq.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://hi.yuexingan06.cn

Go:   if s == "" {}
来源：http://fw.jctech888.com.cn

Ruby: if s.empty?
来源：http://am.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sv.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://xi.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fu.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cz.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uu.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wl.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zj.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://ja.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ab.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xj.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://fp.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uz.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yo.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yl.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mw.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dn.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zh.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://dk.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://by.gzmigu.cn

================================================================================
来源：http://qi.haigaiapp.cn

F. 文件与目录
来源：http://hq.huixinmuqiang.cn

================================================================================
来源：http://wn.nicolike.cn

[F01] 读取整个文件
来源：http://po.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cf.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://vj.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mb.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://of.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mf.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mh.szsharing.cn

Ruby: File.read("a.txt")
来源：http://wp.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://fe.nszjky.cn

[F02] 逐行读取文件
来源：http://uk.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dg.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wr.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mr.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ee.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cx.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jb.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ys.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hf.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://dl.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rf.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ud.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xr.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pi.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ud.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xh.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://hk.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fv.yuexingan06.cn

[F04] 追加写入文件
来源：http://vd.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vz.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hc.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://us.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hl.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eu.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kr.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mg.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qc.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://je.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://op.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://xn.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://fy.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://vt.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xw.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nj.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://ot.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://su.huixiangedu.cn

[F06] 删除文件
来源：http://uh.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://ez.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://js.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fa.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vl.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tg.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://vg.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://af.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://pz.nicolike.cn

[F07] 创建目录（含多级）
来源：http://ux.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yj.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ol.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gq.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://si.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oz.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zu.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xp.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rv.shtwfgs.cn

[F08] 遍历目录
来源：http://aw.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lc.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vz.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://fw.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://nx.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mw.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ec.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://hc.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://co.shxzukj.cn

[F09] 获取文件大小
来源：http://sa.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://ie.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://bb.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://lg.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://yy.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bj.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jx.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://dy.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://re.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://vg.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ox.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bk.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bu.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://sc.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uy.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gm.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wo.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rd.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://ui.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yd.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qx.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vm.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://io.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gx.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gr.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jp.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://of.lnxyls.cn

[F12] CSV 读写
来源：http://be.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ni.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ku.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ds.colortex.cn

TS:   // 同上
来源：http://lm.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ir.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pr.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tn.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jj.9csxet.cn

================================================================================
来源：http://sk.wgjwhj.cn

G. 面向对象
来源：http://ge.shxzskj.cn

================================================================================
来源：http://zw.jctech888.com.cn

[G01] 定义类
来源：http://ho.newstarts.cn

Py:   class User: pass
来源：http://rp.haigaiapp.cn

PHP:  class User {}
来源：http://ki.shxzukj.cn

JS:   class User {}
来源：http://iq.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ww.gzmigu.cn

Java: class User {}
来源：http://ch.9csxet.cn

Go:   type User struct { Name string }
来源：http://zk.yuntaijiaju.cn

Ruby: class User; end
来源：http://gl.521024.cn

C#:   class User {}
来源：http://ge.shxzukj.cn

[G02] 构造函数
来源：http://xm.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://bu.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://qq.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://mb.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://lg.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://vd.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gw.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://zh.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://ht.newstarts.cn

[G03] 实例属性
来源：http://zs.newstarts.cn

Py:   self.name = "x"
来源：http://sr.lnxyls.cn

PHP:  public string $name = "x";
来源：http://ar.newstarts.cn

JS:   this.name = "x";
来源：http://ku.shxzukj.cn

TS:   name: string = "x";
来源：http://gq.gzmigu.cn

Java: private String name;
来源：http://df.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yx.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://ju.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://wc.bjjhwx.cn

[G04] 定义方法
来源：http://ea.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://sx.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wq.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://gp.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://ru.gzmigu.cn

Java: String greet() { return name; }
来源：http://qu.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qg.shxzukj.cn

Ruby: def greet; @name; end
来源：http://cu.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://gt.chemitech.net.cn

[G05] 继承
来源：http://dh.nszjky.cn

Py:   class Admin(User): pass
来源：http://sp.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://yr.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://kd.panjiajie.cn

TS:   class Admin extends User {}
来源：http://fu.nszjky.cn

Java: class Admin extends User {}
来源：http://fq.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yq.nicolike.cn

Ruby: class Admin < User; end
来源：http://df.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://jx.nicolike.cn

[G06] 重写方法
来源：http://qe.asd995.cn

Py:   def greet(self): return "admin"
来源：http://ba.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ks.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://zc.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://eu.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://od.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zz.asd995.cn

Ruby: def greet; "admin"; end
来源：http://xz.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://za.szxytkj.cn

[G07] 调用父类方法
来源：http://xg.yuexingan06.cn

Py:   super().greet()
来源：http://js.huixiangedu.cn

PHP:  parent::greet();
来源：http://nn.shtwfgs.cn

JS:   super.greet();
来源：http://la.szxytkj.cn

TS:   super.greet();
来源：http://ng.wgjwhj.cn

Java: super.greet();
来源：http://ut.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ih.huanxung.cn

Ruby: super
来源：http://ci.haigaiapp.cn

C#:   base.Greet();
来源：http://go.lnxyls.cn

[G08] 静态方法与属性
来源：http://ac.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sf.hnjuh.cn

PHP:  public static function f() {}
来源：http://ej.chemitech.net.cn

JS:   static f() {}
来源：http://jn.shxzskj.cn

TS:   static f(): void {}
来源：http://dw.bjjhwx.cn

Java: static void f() {}
来源：http://tp.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mh.haigaiapp.cn

Ruby: def self.f; end
来源：http://wm.colortex.cn

C#:   public static void F() {}
来源：http://ls.521024.cn

[G09] 接口 / 抽象类
来源：http://lw.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://kg.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dj.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cy.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://ga.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://tz.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://wl.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zy.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://jz.huixinmuqiang.cn

[G10] 访问控制
来源：http://hr.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://zv.lnxyls.cn

PHP:  public / protected / private
来源：http://ro.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://hn.nszjky.cn

TS:   public / protected / private
来源：http://ql.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://wm.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yz.lnxyls.cn

Ruby: public / protected / private
来源：http://ca.panjiajie.cn

C#:   public / protected / private / internal
来源：http://sf.bookmarksfly.cn

[G11] getter / setter
来源：http://ck.521024.cn

Py:   @property 与 @x.setter
来源：http://as.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bg.szsharing.cn

JS:   get name() { return this._name; }
来源：http://zu.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://mw.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://du.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://el.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://uf.521024.cn

C#:   public string Name { get; set; }
来源：http://oq.colortex.cn

[G12] 对象转字符串
来源：http://ze.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://tf.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nz.hahajie.cn

JS:   toString() { return this.name; }
来源：http://cl.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://nh.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://us.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gs.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://tc.521024.cn

C#:   public override string ToString() => Name;
来源：http://oj.szsharing.cn

[G13] 判断对象类型
来源：http://es.9csxet.cn

Py:   isinstance(u, User)
来源：http://im.chemitech.net.cn

PHP:  $u instanceof User
来源：http://jj.521024.cn

JS:   u instanceof User
来源：http://bw.haigaiapp.cn

TS:   u instanceof User
来源：http://da.hnjuh.cn

Java: u instanceof User
来源：http://km.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cj.huanxung.cn

Ruby: u.is_a?(User)
来源：http://tb.jctech888.com.cn

C#:   u is User
来源：http://ul.newstarts.cn

[G14] 数据类 / record
来源：http://he.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wg.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://rw.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bt.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://nl.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://qd.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://uv.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rw.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://dj.shxzskj.cn

[G15] 枚举
来源：http://fr.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kj.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vq.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://un.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://re.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://nl.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ht.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://hx.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yi.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://ez.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fb.szxytkj.cn


<!-- 参考信息 -->