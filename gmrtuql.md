代发 wailian999

PHP:  number_format(1234567);
来源：http://dl.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gh.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ta.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ee.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sv.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jw.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://np.bjjhwx.cn

[E17] 首字母大写
来源：http://ni.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gh.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ww.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bo.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qj.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wo.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sd.shxzukj.cn

Ruby: s.capitalize
来源：http://un.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://li.hnjuh.cn

[E18] 模板占位符替换
来源：http://zt.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gr.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ov.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ud.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tg.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ga.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dg.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fv.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hf.hahajie.cn

[E19] 多行文本按行拆分
来源：http://pr.shtwfgs.cn

Py:   s.splitlines()
来源：http://ln.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nt.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://qy.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://bc.hnjuh.cn

Java: s.lines().toList()
来源：http://bd.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://zb.yuexingan06.cn

Ruby: s.lines
来源：http://ti.lnxyls.cn

C#:   s.Split('\n')
来源：http://vo.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://pk.wgjwhj.cn

Py:   if not s:
来源：http://hz.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lq.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gu.huixiangedu.cn

TS:   if (s === "") {}
来源：http://jc.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://uz.nszjky.cn

Go:   if s == "" {}
来源：http://tg.panjiajie.cn

Ruby: if s.empty?
来源：http://jw.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oi.huanxung.cn

[E21] 超长截断加省略号
来源：http://fd.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kg.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ub.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vm.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ua.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zz.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://uo.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nx.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cm.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://ko.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wb.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jh.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ia.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zd.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ci.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://la.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://su.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nz.panjiajie.cn

================================================================================
来源：http://is.huixinmuqiang.cn

F. 文件与目录
来源：http://uz.huanxung.cn

================================================================================
来源：http://ka.gzmigu.cn

[F01] 读取整个文件
来源：http://qv.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fg.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://kh.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xu.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ze.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pg.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fq.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://pf.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://jv.yuexingan06.cn

[F02] 逐行读取文件
来源：http://ef.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pk.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pa.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oj.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gw.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dx.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jy.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fi.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xo.521024.cn

[F03] 写入文件（覆盖）
来源：http://cq.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ev.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gu.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://st.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://po.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uo.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://np.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://st.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oz.wgjwhj.cn

[F04] 追加写入文件
来源：http://la.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zf.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fz.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rp.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uj.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ym.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rq.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iq.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dy.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://ao.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ac.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://zw.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://yz.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://pr.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ol.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sh.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://dg.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://wv.nszjky.cn

[F06] 删除文件
来源：http://wa.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://at.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://ef.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rt.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pe.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hd.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://tc.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://bx.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://lm.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://hc.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jx.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ei.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cb.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wg.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mh.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yt.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hh.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nx.wgjwhj.cn

[F08] 遍历目录
来源：http://xk.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qe.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lr.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://aw.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://te.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oe.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rc.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://ph.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://to.shxzukj.cn

[F09] 获取文件大小
来源：http://yj.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://ri.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://tz.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://ro.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://nf.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vj.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jc.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://fv.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://ec.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://ik.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eh.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yf.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gc.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://oe.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://by.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sj.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yc.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kj.nicolike.cn

[F11] 复制与移动文件
来源：http://ww.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://id.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ak.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gm.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dy.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lm.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jc.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rd.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jk.shxzukj.cn

[F12] CSV 读写
来源：http://cc.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gz.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bs.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yj.nicolike.cn

TS:   // 同上
来源：http://dq.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tg.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dz.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://et.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cn.521024.cn

================================================================================
来源：http://qc.jianghongdianzi.cn

G. 面向对象
来源：http://ro.nicolike.cn

================================================================================
来源：http://ll.jctech888.com.cn

[G01] 定义类
来源：http://zb.9csxet.cn

Py:   class User: pass
来源：http://ta.shxzskj.cn

PHP:  class User {}
来源：http://cl.shxzskj.cn

JS:   class User {}
来源：http://tw.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://nj.hahajie.cn

Java: class User {}
来源：http://in.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://fe.bjjhwx.cn

Ruby: class User; end
来源：http://hf.shtwfgs.cn

C#:   class User {}
来源：http://rg.szxytkj.cn

[G02] 构造函数
来源：http://tc.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://cj.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://hs.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://sl.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://qo.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://or.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dz.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://wt.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ov.yuntaijiaju.cn

[G03] 实例属性
来源：http://yt.muxihuayi.cn

Py:   self.name = "x"
来源：http://uy.shxzskj.cn

PHP:  public string $name = "x";
来源：http://rv.yuexingan06.cn

JS:   this.name = "x";
来源：http://xh.haigaiapp.cn

TS:   name: string = "x";
来源：http://eh.lnxyls.cn

Java: private String name;
来源：http://yn.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zw.bookmarksfly.cn

Ruby: @name = "x"
来源：http://nf.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://rw.nszjky.cn

[G04] 定义方法
来源：http://ev.hahajie.cn

Py:   def greet(self): return self.name
来源：http://ux.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kc.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://wf.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://uu.muxihuayi.cn

Java: String greet() { return name; }
来源：http://na.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jq.huanxung.cn

Ruby: def greet; @name; end
来源：http://rd.9csxet.cn

C#:   public string Greet() => Name;
来源：http://rs.gzmigu.cn

[G05] 继承
来源：http://it.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://en.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://mg.szsharing.cn

JS:   class Admin extends User {}
来源：http://hh.lnxyls.cn

TS:   class Admin extends User {}
来源：http://ea.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://fx.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zk.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://zc.szxytkj.cn

C#:   class Admin : User {}
来源：http://yp.wgjwhj.cn

[G06] 重写方法
来源：http://en.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://hs.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gu.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://tt.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://de.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://qo.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cz.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://ti.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://nf.gzmigu.cn

[G07] 调用父类方法
来源：http://gg.muxihuayi.cn

Py:   super().greet()
来源：http://ss.shxzskj.cn

PHP:  parent::greet();
来源：http://ut.wgjwhj.cn

JS:   super.greet();
来源：http://mi.huanxung.cn

TS:   super.greet();
来源：http://dv.yuntaijiaju.cn

Java: super.greet();
来源：http://qm.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pg.jianghongdianzi.cn

Ruby: super
来源：http://lr.shtwfgs.cn

C#:   base.Greet();
来源：http://ld.shtwfgs.cn

[G08] 静态方法与属性
来源：http://hv.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cv.hahajie.cn

PHP:  public static function f() {}
来源：http://rz.jianghongdianzi.cn

JS:   static f() {}
来源：http://nr.colortex.cn

TS:   static f(): void {}
来源：http://xb.nicolike.cn

Java: static void f() {}
来源：http://jk.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uw.shxzukj.cn

Ruby: def self.f; end
来源：http://ke.bjjhwx.cn

C#:   public static void F() {}
来源：http://gg.521024.cn

[G09] 接口 / 抽象类
来源：http://ps.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://zf.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pe.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sn.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://uv.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://ir.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://tq.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xz.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://sl.yuntaijiaju.cn

[G10] 访问控制
来源：http://vr.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://dp.newstarts.cn

PHP:  public / protected / private
来源：http://el.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://pr.hnjuh.cn

TS:   public / protected / private
来源：http://tf.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://et.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ix.shxzskj.cn

Ruby: public / protected / private
来源：http://kf.asd995.cn

C#:   public / protected / private / internal
来源：http://eb.gzmigu.cn

[G11] getter / setter
来源：http://pm.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://ng.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nt.9csxet.cn

JS:   get name() { return this._name; }
来源：http://pr.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://yd.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://ka.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rp.szxytkj.cn

Ruby: attr_accessor :name
来源：http://qu.521024.cn

C#:   public string Name { get; set; }
来源：http://iv.muxihuayi.cn

[G12] 对象转字符串
来源：http://tr.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://tt.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rm.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://ux.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://bq.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://mv.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wt.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://rl.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://vy.lnxyls.cn

[G13] 判断对象类型
来源：http://vr.hahajie.cn

Py:   isinstance(u, User)
来源：http://bd.jctech888.com.cn

PHP:  $u instanceof User
来源：http://bp.jianghongdianzi.cn

JS:   u instanceof User
来源：http://nf.panjiajie.cn

TS:   u instanceof User
来源：http://nd.jctech888.com.cn

Java: u instanceof User
来源：http://nk.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dq.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://tu.newstarts.cn

C#:   u is User
来源：http://ib.huixiangedu.cn

[G14] 数据类 / record
来源：http://qy.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ca.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://xo.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://io.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://pl.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://le.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://yy.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eo.haigaiapp.cn


<!-- 参考信息 -->