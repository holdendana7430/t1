代发 wailian999

[E18] 模板占位符替换
来源：http://xm.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://li.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ww.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pa.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hr.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fw.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xj.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jx.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pg.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://qv.shxzskj.cn

Py:   s.splitlines()
来源：http://lx.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qx.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://om.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://bs.muxihuayi.cn

Java: s.lines().toList()
来源：http://va.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://le.gzmigu.cn

Ruby: s.lines
来源：http://ma.colortex.cn

C#:   s.Split('\n')
来源：http://jj.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://nd.jctech888.com.cn

Py:   if not s:
来源：http://vx.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ux.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lq.panjiajie.cn

TS:   if (s === "") {}
来源：http://zj.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://et.nicolike.cn

Go:   if s == "" {}
来源：http://jv.gzmigu.cn

Ruby: if s.empty?
来源：http://lc.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aq.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://fg.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eu.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yb.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lt.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hf.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mf.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://ni.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fu.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jj.szsharing.cn

[E22] 字节长度与字符长度
来源：http://xu.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gy.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wa.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aw.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://os.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ea.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zj.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://tx.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rl.gzmigu.cn

================================================================================
来源：http://qx.szsharing.cn

F. 文件与目录
来源：http://am.asd995.cn

================================================================================
来源：http://ao.nicolike.cn

[F01] 读取整个文件
来源：http://oq.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uo.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://pr.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yb.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cc.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ev.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ew.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://qo.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://sa.huixiangedu.cn

[F02] 逐行读取文件
来源：http://aa.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mt.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gk.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dk.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jx.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://of.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iv.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sq.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qi.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://eh.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sr.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fd.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xe.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vk.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ne.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bf.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://rg.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dt.szxytkj.cn

[F04] 追加写入文件
来源：http://iu.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://um.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pd.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vh.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wk.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ln.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://su.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fc.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hu.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://un.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lc.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://zk.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://cg.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://zy.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kk.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://va.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://qo.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://rl.yuntaijiaju.cn

[F06] 删除文件
来源：http://jh.521024.cn

Py:   os.remove("a.txt")
来源：http://wq.9csxet.cn

PHP:  unlink("a.txt");
来源：http://yv.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jf.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fv.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zi.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://ds.colortex.cn

Ruby: File.delete("a.txt")
来源：http://ba.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://bc.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://ef.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iz.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ln.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nk.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gm.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yp.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bf.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fz.asd995.cn

[F08] 遍历目录
来源：http://ld.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wt.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rq.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://nr.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://ps.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://al.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tm.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://ay.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://pp.shxzukj.cn

[F09] 获取文件大小
来源：http://sy.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://hz.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://hg.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://je.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://hh.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iy.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bm.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://yf.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ty.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://ii.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bc.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mq.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ui.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://ma.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ss.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fk.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fv.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ch.hnjuh.cn

[F11] 复制与移动文件
来源：http://oq.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rs.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://up.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ue.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yu.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://et.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vv.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ct.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vh.muxihuayi.cn

[F12] CSV 读写
来源：http://iz.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lk.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zg.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mi.shxzukj.cn

TS:   // 同上
来源：http://aw.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dw.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sn.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tf.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vl.newstarts.cn

================================================================================
来源：http://qj.shxzskj.cn

G. 面向对象
来源：http://rc.gzmigu.cn

================================================================================
来源：http://vh.szsharing.cn

[G01] 定义类
来源：http://cs.shxzskj.cn

Py:   class User: pass
来源：http://zf.521024.cn

PHP:  class User {}
来源：http://ze.huixiangedu.cn

JS:   class User {}
来源：http://hf.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://ww.chemitech.net.cn

Java: class User {}
来源：http://an.gzmigu.cn

Go:   type User struct { Name string }
来源：http://df.shxzskj.cn

Ruby: class User; end
来源：http://ml.colortex.cn

C#:   class User {}
来源：http://fq.lnxyls.cn

[G02] 构造函数
来源：http://zm.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://nz.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://xl.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://rl.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://ud.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://iz.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bo.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://sz.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://lx.haigaiapp.cn

[G03] 实例属性
来源：http://se.nicolike.cn

Py:   self.name = "x"
来源：http://sg.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://rx.nszjky.cn

JS:   this.name = "x";
来源：http://cr.nicolike.cn

TS:   name: string = "x";
来源：http://wl.huanxung.cn

Java: private String name;
来源：http://xs.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ub.chemitech.net.cn

Ruby: @name = "x"
来源：http://di.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://ai.haigaiapp.cn

[G04] 定义方法
来源：http://rz.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://fa.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bq.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://ws.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://ze.nicolike.cn

Java: String greet() { return name; }
来源：http://ej.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nv.gzmigu.cn

Ruby: def greet; @name; end
来源：http://yw.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://hs.hnjuh.cn

[G05] 继承
来源：http://vc.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://iu.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://cn.szxytkj.cn

JS:   class Admin extends User {}
来源：http://cs.gzmigu.cn

TS:   class Admin extends User {}
来源：http://sb.jctech888.com.cn

Java: class Admin extends User {}
来源：http://qg.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xt.nicolike.cn

Ruby: class Admin < User; end
来源：http://lz.nicolike.cn

C#:   class Admin : User {}
来源：http://hr.muxihuayi.cn

[G06] 重写方法
来源：http://rz.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://bg.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qw.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://gp.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ce.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://na.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wo.asd995.cn

Ruby: def greet; "admin"; end
来源：http://uo.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://yi.asd995.cn

[G07] 调用父类方法
来源：http://no.muxihuayi.cn

Py:   super().greet()
来源：http://kv.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://jt.521024.cn

JS:   super.greet();
来源：http://wq.jctech888.com.cn

TS:   super.greet();
来源：http://gz.hnjuh.cn

Java: super.greet();
来源：http://yz.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fm.hahajie.cn

Ruby: super
来源：http://sb.jctech888.com.cn

C#:   base.Greet();
来源：http://bn.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://se.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cm.yuexingan06.cn

PHP:  public static function f() {}
来源：http://ch.newstarts.cn

JS:   static f() {}
来源：http://qf.bookmarksfly.cn

TS:   static f(): void {}
来源：http://tk.panjiajie.cn

Java: static void f() {}
来源：http://fs.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gq.wgjwhj.cn

Ruby: def self.f; end
来源：http://tq.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://bm.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://fp.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://nu.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gt.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vz.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://nw.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://rq.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://uc.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fs.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://al.9csxet.cn

[G10] 访问控制
来源：http://gx.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://il.newstarts.cn

PHP:  public / protected / private
来源：http://my.huanxung.cn

JS:   #private 字段；其余公开
来源：http://ak.szsharing.cn

TS:   public / protected / private
来源：http://qd.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://nt.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ra.shxzskj.cn

Ruby: public / protected / private
来源：http://ka.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://qp.szxytkj.cn

[G11] getter / setter
来源：http://lz.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://zx.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ok.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://od.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://iz.lnxyls.cn

Java: public String getName() { return name; }
来源：http://mt.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://os.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://hj.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://gk.bookmarksfly.cn

[G12] 对象转字符串
来源：http://dx.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://ft.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://md.colortex.cn

JS:   toString() { return this.name; }
来源：http://mm.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://hj.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://yc.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wz.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://sc.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://az.shxzukj.cn

[G13] 判断对象类型
来源：http://qx.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://jd.muxihuayi.cn

PHP:  $u instanceof User
来源：http://be.szsharing.cn

JS:   u instanceof User
来源：http://cp.bookmarksfly.cn

TS:   u instanceof User
来源：http://oa.yuexingan06.cn

Java: u instanceof User
来源：http://vy.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ts.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://xz.521024.cn

C#:   u is User
来源：http://ko.panjiajie.cn

[G14] 数据类 / record
来源：http://ub.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gw.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://ur.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ub.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://qh.521024.cn

Java: record User(String name, int age) {}
来源：http://tw.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://tm.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ah.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://bz.asd995.cn

[G15] 枚举
来源：http://vu.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ze.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bm.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vf.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pj.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://om.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vd.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://xc.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dt.colortex.cn

[G16] 对象转数组 / 字典
来源：http://jh.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kt.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://by.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://aj.521024.cn

TS:   Object.entries(obj)
来源：http://kc.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mm.jianghongdianzi.cn


<!-- 参考信息 -->