代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://zx.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vr.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bb.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pl.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rb.newstarts.cn

[E19] 多行文本按行拆分
来源：http://qo.nicolike.cn

Py:   s.splitlines()
来源：http://nq.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://do.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://pl.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://xc.chemitech.net.cn

Java: s.lines().toList()
来源：http://ri.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://gs.huanxung.cn

Ruby: s.lines
来源：http://mi.muxihuayi.cn

C#:   s.Split('\n')
来源：http://ib.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://af.huixiangedu.cn

Py:   if not s:
来源：http://fh.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dv.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yc.shxzskj.cn

TS:   if (s === "") {}
来源：http://fb.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://up.panjiajie.cn

Go:   if s == "" {}
来源：http://ye.shxzskj.cn

Ruby: if s.empty?
来源：http://hk.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uw.panjiajie.cn

[E21] 超长截断加省略号
来源：http://rf.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fc.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sw.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://no.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://as.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yk.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://ll.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gk.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wm.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://ju.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oz.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sw.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dh.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yu.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sa.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lo.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://rd.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kw.muxihuayi.cn

================================================================================
来源：http://sz.szsharing.cn

F. 文件与目录
来源：http://wr.hahajie.cn

================================================================================
来源：http://af.szsharing.cn

[F01] 读取整个文件
来源：http://ip.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yu.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://bd.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ba.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mb.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eo.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hd.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://qj.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://sa.muxihuayi.cn

[F02] 逐行读取文件
来源：http://jt.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kb.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aa.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lu.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oa.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ll.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mf.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ko.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gk.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://gq.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iw.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yq.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://li.hnjuh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://di.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zu.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iw.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://ks.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mr.521024.cn

[F04] 追加写入文件
来源：http://ei.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://il.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hs.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pq.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yi.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ls.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xk.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rw.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ix.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://ht.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://km.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://jc.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://oi.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://dd.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://my.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mn.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://vu.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://mj.bjjhwx.cn

[F06] 删除文件
来源：http://wc.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://vr.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://ao.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vi.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yk.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dm.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://ij.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://iv.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://sp.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://al.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qg.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ai.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tr.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tl.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cm.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://po.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ml.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ul.shtwfgs.cn

[F08] 遍历目录
来源：http://bx.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bb.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vj.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://sj.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://st.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sw.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ya.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://qq.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://nf.gzmigu.cn

[F09] 获取文件大小
来源：http://aj.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://uk.nicolike.cn

PHP:  filesize("a.txt");
来源：http://xm.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://rx.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://xb.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xp.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rd.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://qe.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://im.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://se.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nv.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mh.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hv.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://op.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kv.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sh.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kv.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ru.9csxet.cn

[F11] 复制与移动文件
来源：http://dd.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wu.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qk.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ki.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fw.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bx.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ql.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://do.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ah.haigaiapp.cn

[F12] CSV 读写
来源：http://xh.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bs.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yf.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.jianghongdianzi.cn

TS:   // 同上
来源：http://st.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://si.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vo.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pa.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iq.bjjhwx.cn

================================================================================
来源：http://aq.521024.cn

G. 面向对象
来源：http://qj.asd995.cn

================================================================================
来源：http://cy.gzmigu.cn

[G01] 定义类
来源：http://ue.yuexingan06.cn

Py:   class User: pass
来源：http://gz.muxihuayi.cn

PHP:  class User {}
来源：http://tc.haigaiapp.cn

JS:   class User {}
来源：http://xl.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://dr.jctech888.com.cn

Java: class User {}
来源：http://no.huanxung.cn

Go:   type User struct { Name string }
来源：http://vc.yuexingan06.cn

Ruby: class User; end
来源：http://lh.gzmigu.cn

C#:   class User {}
来源：http://mr.nszjky.cn

[G02] 构造函数
来源：http://zx.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://rd.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://al.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://gc.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://gk.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://cp.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yu.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://ap.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://xy.szsharing.cn

[G03] 实例属性
来源：http://vx.huanxung.cn

Py:   self.name = "x"
来源：http://ej.9csxet.cn

PHP:  public string $name = "x";
来源：http://sa.wgjwhj.cn

JS:   this.name = "x";
来源：http://mi.szsharing.cn

TS:   name: string = "x";
来源：http://us.shtwfgs.cn

Java: private String name;
来源：http://zd.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ke.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://yt.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://td.haigaiapp.cn

[G04] 定义方法
来源：http://iv.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://sm.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qz.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://vf.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://cz.haigaiapp.cn

Java: String greet() { return name; }
来源：http://mm.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lj.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://ns.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://ri.colortex.cn

[G05] 继承
来源：http://zu.panjiajie.cn

Py:   class Admin(User): pass
来源：http://fn.asd995.cn

PHP:  class Admin extends User {}
来源：http://wo.gzmigu.cn

JS:   class Admin extends User {}
来源：http://kg.shxzukj.cn

TS:   class Admin extends User {}
来源：http://ah.huixiangedu.cn

Java: class Admin extends User {}
来源：http://yp.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xq.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://ji.lnxyls.cn

C#:   class Admin : User {}
来源：http://pi.521024.cn

[G06] 重写方法
来源：http://kd.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://pe.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zk.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://lp.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://al.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://ju.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vx.asd995.cn

Ruby: def greet; "admin"; end
来源：http://af.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://pw.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://tf.chemitech.net.cn

Py:   super().greet()
来源：http://gu.hnjuh.cn

PHP:  parent::greet();
来源：http://al.szsharing.cn

JS:   super.greet();
来源：http://xt.lnxyls.cn

TS:   super.greet();
来源：http://uo.haigaiapp.cn

Java: super.greet();
来源：http://fy.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hm.lnxyls.cn

Ruby: super
来源：http://be.nszjky.cn

C#:   base.Greet();
来源：http://qn.shxzskj.cn

[G08] 静态方法与属性
来源：http://yf.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ew.huixiangedu.cn

PHP:  public static function f() {}
来源：http://vr.huixiangedu.cn

JS:   static f() {}
来源：http://al.panjiajie.cn

TS:   static f(): void {}
来源：http://hu.shtwfgs.cn

Java: static void f() {}
来源：http://nz.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ju.hnjuh.cn

Ruby: def self.f; end
来源：http://ak.haigaiapp.cn

C#:   public static void F() {}
来源：http://zn.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://yy.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://mh.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pc.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dz.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://jj.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://sq.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://gd.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kc.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://fd.szxytkj.cn

[G10] 访问控制
来源：http://fz.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://hx.nicolike.cn

PHP:  public / protected / private
来源：http://un.newstarts.cn

JS:   #private 字段；其余公开
来源：http://gz.muxihuayi.cn

TS:   public / protected / private
来源：http://rm.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://tg.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sr.hnjuh.cn

Ruby: public / protected / private
来源：http://ls.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://iu.shtwfgs.cn

[G11] getter / setter
来源：http://wo.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://va.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ic.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://ip.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://nw.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://hy.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://by.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://ru.asd995.cn

C#:   public string Name { get; set; }
来源：http://hm.bjjhwx.cn

[G12] 对象转字符串
来源：http://gp.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://ee.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tf.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://kz.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://oq.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://bj.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aa.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://ma.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://bi.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://qv.hnjuh.cn

Py:   isinstance(u, User)
来源：http://wd.panjiajie.cn

PHP:  $u instanceof User
来源：http://mv.chemitech.net.cn

JS:   u instanceof User
来源：http://bs.wgjwhj.cn

TS:   u instanceof User
来源：http://ro.chemitech.net.cn

Java: u instanceof User
来源：http://ya.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yr.521024.cn

Ruby: u.is_a?(User)
来源：http://fe.colortex.cn

C#:   u is User
来源：http://th.nszjky.cn

[G14] 数据类 / record
来源：http://td.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wh.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://kd.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://al.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://dz.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://ss.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://nq.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fk.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://dl.huixiangedu.cn

[G15] 枚举
来源：http://bv.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hv.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ov.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://le.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rv.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://wj.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cg.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://ev.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ny.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://qn.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lv.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://ih.gzmigu.cn

JS:   Object.entries(obj)
来源：http://vq.hnjuh.cn

TS:   Object.entries(obj)
来源：http://bb.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xn.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fs.hnjuh.cn

Ruby: obj.instance_variables
来源：http://nh.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://pm.nszjky.cn

================================================================================
来源：http://na.colortex.cn


<!-- 参考信息 -->