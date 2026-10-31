代发 wailian999

[E18] 模板占位符替换
来源：http://mj.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rq.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gq.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fm.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bv.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pb.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cg.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ln.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iy.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://yt.shtwfgs.cn

Py:   s.splitlines()
来源：http://me.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ku.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://rw.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://nk.wgjwhj.cn

Java: s.lines().toList()
来源：http://ue.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://pi.yuntaijiaju.cn

Ruby: s.lines
来源：http://zp.gzmigu.cn

C#:   s.Split('\n')
来源：http://kf.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://tr.hahajie.cn

Py:   if not s:
来源：http://ih.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mh.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://go.haigaiapp.cn

TS:   if (s === "") {}
来源：http://ls.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://tb.szsharing.cn

Go:   if s == "" {}
来源：http://jg.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://hd.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zd.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://td.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ji.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wh.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gn.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bb.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xw.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://nc.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ur.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jc.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://cv.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sm.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ju.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yi.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wg.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mn.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bz.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://xw.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ed.szsharing.cn

================================================================================
来源：http://pw.newstarts.cn

F. 文件与目录
来源：http://ts.shxzukj.cn

================================================================================
来源：http://zg.gzmigu.cn

[F01] 读取整个文件
来源：http://zo.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lr.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://zt.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vw.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://in.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://su.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wv.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://ab.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://gg.panjiajie.cn

[F02] 逐行读取文件
来源：http://gi.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oo.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rc.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wm.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cg.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ca.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iv.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lr.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://of.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://yx.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nx.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xx.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rx.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rb.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eo.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nq.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://hs.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ju.huanxung.cn

[F04] 追加写入文件
来源：http://wq.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fe.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://le.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jr.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ak.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bl.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vr.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bc.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cu.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://lu.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://do.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://lb.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://kd.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://sb.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yv.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xs.521024.cn

Ruby: File.exist?("a.txt")
来源：http://gn.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://rp.colortex.cn

[F06] 删除文件
来源：http://se.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://hm.nicolike.cn

PHP:  unlink("a.txt");
来源：http://tb.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zi.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vn.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jm.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://ty.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://us.521024.cn

C#:   File.Delete("a.txt");
来源：http://zp.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://ei.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fs.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uf.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xe.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kr.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nc.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hr.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ej.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xe.colortex.cn

[F08] 遍历目录
来源：http://gs.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bj.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qt.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://xh.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://jm.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ou.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dd.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ei.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://vh.wgjwhj.cn

[F09] 获取文件大小
来源：http://ln.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://vo.colortex.cn

PHP:  filesize("a.txt");
来源：http://ze.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://av.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://vx.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jg.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lp.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://jv.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://lh.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://uj.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rj.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mf.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ea.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://sp.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://va.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ew.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yw.521024.cn

[F11] 复制与移动文件
来源：http://wi.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://su.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://da.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pd.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ew.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://of.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ng.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wr.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mm.szsharing.cn

[F12] CSV 读写
来源：http://ad.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wh.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ow.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://of.jianghongdianzi.cn

TS:   // 同上
来源：http://bn.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xp.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mq.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tw.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dg.521024.cn

================================================================================
来源：http://tz.shxzukj.cn

G. 面向对象
来源：http://ar.huixinmuqiang.cn

================================================================================
来源：http://iv.haigaiapp.cn

[G01] 定义类
来源：http://kq.gzmigu.cn

Py:   class User: pass
来源：http://uh.huixinmuqiang.cn

PHP:  class User {}
来源：http://pu.muxihuayi.cn

JS:   class User {}
来源：http://rn.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://kb.asd995.cn

Java: class User {}
来源：http://zt.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://hx.nicolike.cn

Ruby: class User; end
来源：http://ht.shxzukj.cn

C#:   class User {}
来源：http://zs.chemitech.net.cn

[G02] 构造函数
来源：http://tj.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://ms.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://yq.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://ma.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://ax.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://kn.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ne.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ns.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://xi.gzmigu.cn

[G03] 实例属性
来源：http://af.gzmigu.cn

Py:   self.name = "x"
来源：http://dt.shxzukj.cn

PHP:  public string $name = "x";
来源：http://re.colortex.cn

JS:   this.name = "x";
来源：http://st.shxzukj.cn

TS:   name: string = "x";
来源：http://ns.hnjuh.cn

Java: private String name;
来源：http://gi.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://as.gzmigu.cn

Ruby: @name = "x"
来源：http://pc.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://mr.jctech888.com.cn

[G04] 定义方法
来源：http://xm.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://ag.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://la.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://rl.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://pe.shxzskj.cn

Java: String greet() { return name; }
来源：http://ob.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xj.panjiajie.cn

Ruby: def greet; @name; end
来源：http://uy.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://ni.nicolike.cn

[G05] 继承
来源：http://qd.521024.cn

Py:   class Admin(User): pass
来源：http://fq.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://fd.hahajie.cn

JS:   class Admin extends User {}
来源：http://rl.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://vs.shxzukj.cn

Java: class Admin extends User {}
来源：http://wo.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ei.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://bd.muxihuayi.cn

C#:   class Admin : User {}
来源：http://sh.chemitech.net.cn

[G06] 重写方法
来源：http://kh.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://us.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mn.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://fv.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://zs.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://dl.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ai.colortex.cn

Ruby: def greet; "admin"; end
来源：http://is.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://xp.9csxet.cn

[G07] 调用父类方法
来源：http://ii.hnjuh.cn

Py:   super().greet()
来源：http://gp.newstarts.cn

PHP:  parent::greet();
来源：http://fu.bookmarksfly.cn

JS:   super.greet();
来源：http://vv.shxzskj.cn

TS:   super.greet();
来源：http://wh.asd995.cn

Java: super.greet();
来源：http://lf.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ow.521024.cn

Ruby: super
来源：http://rs.521024.cn

C#:   base.Greet();
来源：http://us.asd995.cn

[G08] 静态方法与属性
来源：http://cm.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sq.huanxung.cn

PHP:  public static function f() {}
来源：http://mq.jctech888.com.cn

JS:   static f() {}
来源：http://sh.bookmarksfly.cn

TS:   static f(): void {}
来源：http://xd.szxytkj.cn

Java: static void f() {}
来源：http://ni.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bo.panjiajie.cn

Ruby: def self.f; end
来源：http://ux.hnjuh.cn

C#:   public static void F() {}
来源：http://qk.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://fp.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://df.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oa.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dp.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://ex.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://js.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://xy.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ck.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://nn.gzmigu.cn

[G10] 访问控制
来源：http://yu.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://rj.bjjhwx.cn

PHP:  public / protected / private
来源：http://sw.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://za.muxihuayi.cn

TS:   public / protected / private
来源：http://ny.colortex.cn

Java: public / protected / private / 默认包级
来源：http://su.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xo.huanxung.cn

Ruby: public / protected / private
来源：http://mn.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://ua.panjiajie.cn

[G11] getter / setter
来源：http://dx.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://go.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://or.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://hy.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://qg.szxytkj.cn

Java: public String getName() { return name; }
来源：http://nn.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fg.521024.cn

Ruby: attr_accessor :name
来源：http://vk.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://vc.jctech888.com.cn

[G12] 对象转字符串
来源：http://pg.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://kx.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cn.szsharing.cn

JS:   toString() { return this.name; }
来源：http://fc.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://dl.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://vd.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ag.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://fo.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://em.bookmarksfly.cn

[G13] 判断对象类型
来源：http://rj.hnjuh.cn

Py:   isinstance(u, User)
来源：http://ca.chemitech.net.cn

PHP:  $u instanceof User
来源：http://ls.jianghongdianzi.cn

JS:   u instanceof User
来源：http://mi.9csxet.cn

TS:   u instanceof User
来源：http://ys.9csxet.cn

Java: u instanceof User
来源：http://eq.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ae.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://mh.asd995.cn

C#:   u is User
来源：http://nb.bjjhwx.cn

[G14] 数据类 / record
来源：http://jz.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://js.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://og.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://na.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://ns.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://yr.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://ps.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rl.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://nb.nicolike.cn

[G15] 枚举
来源：http://ce.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yv.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gq.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ie.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ha.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://so.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bj.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ku.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jk.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://vb.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vw.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://bo.shxzskj.cn

JS:   Object.entries(obj)
来源：http://ar.colortex.cn

TS:   Object.entries(obj)
来源：http://lu.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fb.bjjhwx.cn


<!-- 参考信息 -->