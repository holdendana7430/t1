代发 wailian999

[E18] 模板占位符替换
来源：http://ju.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nj.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vv.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zj.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yg.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jd.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zn.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fg.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wr.521024.cn

[E19] 多行文本按行拆分
来源：http://ez.newstarts.cn

Py:   s.splitlines()
来源：http://np.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://va.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://go.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://cp.shtwfgs.cn

Java: s.lines().toList()
来源：http://hu.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://rs.chemitech.net.cn

Ruby: s.lines
来源：http://ig.panjiajie.cn

C#:   s.Split('\n')
来源：http://ok.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://ai.bookmarksfly.cn

Py:   if not s:
来源：http://am.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cv.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vw.newstarts.cn

TS:   if (s === "") {}
来源：http://tc.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://ek.newstarts.cn

Go:   if s == "" {}
来源：http://id.newstarts.cn

Ruby: if s.empty?
来源：http://lc.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hu.hahajie.cn

[E21] 超长截断加省略号
来源：http://js.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wp.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://os.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kh.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sg.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vi.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://on.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ga.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qm.szsharing.cn

[E22] 字节长度与字符长度
来源：http://gg.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sv.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://de.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dr.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oa.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lo.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qs.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://bi.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bh.lnxyls.cn

================================================================================
来源：http://vc.szxytkj.cn

F. 文件与目录
来源：http://aw.huanxung.cn

================================================================================
来源：http://sc.newstarts.cn

[F01] 读取整个文件
来源：http://db.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fm.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://kh.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cm.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vq.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mk.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ap.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://wh.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://gh.521024.cn

[F02] 逐行读取文件
来源：http://ye.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tf.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dy.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gz.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ys.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ul.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oq.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zj.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dz.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://cs.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wi.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zg.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wu.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dy.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zz.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bw.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://io.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ic.bjjhwx.cn

[F04] 追加写入文件
来源：http://ay.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wy.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lg.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cm.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mk.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xn.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pb.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ne.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wm.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://dg.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bu.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://pd.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://nm.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://fo.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://al.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ru.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://an.colortex.cn

C#:   File.Exists("a.txt")
来源：http://gz.shtwfgs.cn

[F06] 删除文件
来源：http://ji.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://lu.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://zk.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xl.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://du.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nj.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://fc.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://qw.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://lc.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://tz.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dm.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xq.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gs.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qr.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://st.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vl.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vb.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vi.nszjky.cn

[F08] 遍历目录
来源：http://lg.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cn.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sx.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://wm.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://vv.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://me.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mb.nszjky.cn

Ruby: Dir.children("dir")
来源：http://fm.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://yx.chemitech.net.cn

[F09] 获取文件大小
来源：http://or.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://qd.colortex.cn

PHP:  filesize("a.txt");
来源：http://le.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ta.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://dv.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bh.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ju.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://we.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://iq.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://md.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rn.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://td.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hn.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ac.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tc.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uo.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kt.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hi.panjiajie.cn

[F11] 复制与移动文件
来源：http://bp.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pu.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vy.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fd.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ef.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eg.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ns.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uk.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://da.szsharing.cn

[F12] CSV 读写
来源：http://ke.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xk.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uy.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://op.huanxung.cn

TS:   // 同上
来源：http://wr.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lq.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lk.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rs.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kf.yuexingan06.cn

================================================================================
来源：http://cw.newstarts.cn

G. 面向对象
来源：http://vm.huixinmuqiang.cn

================================================================================
来源：http://vs.shxzukj.cn

[G01] 定义类
来源：http://iw.shxzskj.cn

Py:   class User: pass
来源：http://pw.huixiangedu.cn

PHP:  class User {}
来源：http://ze.panjiajie.cn

JS:   class User {}
来源：http://or.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://nc.jctech888.com.cn

Java: class User {}
来源：http://sq.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://lm.chemitech.net.cn

Ruby: class User; end
来源：http://ma.chemitech.net.cn

C#:   class User {}
来源：http://kw.hnjuh.cn

[G02] 构造函数
来源：http://km.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://pi.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://sd.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://rq.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://jl.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://jg.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nw.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://qk.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://rz.hahajie.cn

[G03] 实例属性
来源：http://dt.nszjky.cn

Py:   self.name = "x"
来源：http://cv.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://fe.newstarts.cn

JS:   this.name = "x";
来源：http://vq.muxihuayi.cn

TS:   name: string = "x";
来源：http://ab.haigaiapp.cn

Java: private String name;
来源：http://tb.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cn.szxytkj.cn

Ruby: @name = "x"
来源：http://ns.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://js.haigaiapp.cn

[G04] 定义方法
来源：http://kn.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://vw.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xy.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://mc.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://dx.huanxung.cn

Java: String greet() { return name; }
来源：http://jn.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pg.szxytkj.cn

Ruby: def greet; @name; end
来源：http://nc.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://qp.asd995.cn

[G05] 继承
来源：http://fi.shxzskj.cn

Py:   class Admin(User): pass
来源：http://se.hahajie.cn

PHP:  class Admin extends User {}
来源：http://kk.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://sm.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://xj.521024.cn

Java: class Admin extends User {}
来源：http://zq.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ix.nszjky.cn

Ruby: class Admin < User; end
来源：http://ke.yuexingan06.cn

C#:   class Admin : User {}
来源：http://nc.newstarts.cn

[G06] 重写方法
来源：http://je.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://ak.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lm.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ko.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://zm.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://rn.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jr.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://sm.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://df.asd995.cn

[G07] 调用父类方法
来源：http://xs.yuntaijiaju.cn

Py:   super().greet()
来源：http://ik.szxytkj.cn

PHP:  parent::greet();
来源：http://xe.szsharing.cn

JS:   super.greet();
来源：http://yu.shtwfgs.cn

TS:   super.greet();
来源：http://vo.hnjuh.cn

Java: super.greet();
来源：http://ev.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xf.wgjwhj.cn

Ruby: super
来源：http://et.nicolike.cn

C#:   base.Greet();
来源：http://fo.gzmigu.cn

[G08] 静态方法与属性
来源：http://wk.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cb.hahajie.cn

PHP:  public static function f() {}
来源：http://me.panjiajie.cn

JS:   static f() {}
来源：http://cn.colortex.cn

TS:   static f(): void {}
来源：http://xr.newstarts.cn

Java: static void f() {}
来源：http://pc.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://si.chemitech.net.cn

Ruby: def self.f; end
来源：http://bw.huanxung.cn

C#:   public static void F() {}
来源：http://ra.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://kz.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://ow.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tb.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ys.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://dc.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://sc.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://ll.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hi.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://jd.bookmarksfly.cn

[G10] 访问控制
来源：http://hw.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://pd.chemitech.net.cn

PHP:  public / protected / private
来源：http://az.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://lt.jctech888.com.cn

TS:   public / protected / private
来源：http://ix.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://kx.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jq.muxihuayi.cn

Ruby: public / protected / private
来源：http://ez.colortex.cn

C#:   public / protected / private / internal
来源：http://qq.huanxung.cn

[G11] getter / setter
来源：http://ya.huanxung.cn

Py:   @property 与 @x.setter
来源：http://kr.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fb.huanxung.cn

JS:   get name() { return this._name; }
来源：http://xt.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://by.colortex.cn

Java: public String getName() { return name; }
来源：http://pp.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zq.hnjuh.cn

Ruby: attr_accessor :name
来源：http://re.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://ig.huixiangedu.cn

[G12] 对象转字符串
来源：http://qp.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ne.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mc.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://mh.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://pj.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://mz.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ad.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://ui.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://nd.nszjky.cn

[G13] 判断对象类型
来源：http://pg.hnjuh.cn

Py:   isinstance(u, User)
来源：http://lc.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://ib.szsharing.cn

JS:   u instanceof User
来源：http://jw.jctech888.com.cn

TS:   u instanceof User
来源：http://xh.bjjhwx.cn

Java: u instanceof User
来源：http://aj.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sg.nicolike.cn

Ruby: u.is_a?(User)
来源：http://nw.newstarts.cn

C#:   u is User
来源：http://ew.huanxung.cn

[G14] 数据类 / record
来源：http://kl.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zz.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ee.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pq.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://es.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://hm.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://fc.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ch.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://yc.lnxyls.cn

[G15] 枚举
来源：http://ba.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pg.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ra.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ec.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ad.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://fu.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ai.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://rd.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hv.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://lx.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ns.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://nv.hahajie.cn

JS:   Object.entries(obj)
来源：http://fm.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://xx.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eu.chemitech.net.cn


<!-- 参考信息 -->