代发 wailian999

Py:   for ch in s: print(ch)
来源：http://yo.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://si.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ez.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sq.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xz.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://of.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tq.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://df.521024.cn

[E14] URL 编码与 Base64
来源：http://qr.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jp.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://am.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yf.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vl.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ci.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oj.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fq.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nb.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://op.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rf.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vz.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ng.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hs.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xj.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vm.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hi.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ss.yuntaijiaju.cn

[E16] 数字千分位
来源：http://yk.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://pp.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://xo.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wc.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wg.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dv.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qk.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cb.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://mb.bookmarksfly.cn

[E17] 首字母大写
来源：http://lz.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yg.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sx.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mc.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://be.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fv.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mb.lnxyls.cn

Ruby: s.capitalize
来源：http://yy.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ej.szsharing.cn

[E18] 模板占位符替换
来源：http://wh.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aw.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yp.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://le.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dv.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qb.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tn.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bs.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vs.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://xh.colortex.cn

Py:   s.splitlines()
来源：http://bh.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bf.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://xf.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://qw.wgjwhj.cn

Java: s.lines().toList()
来源：http://gp.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://ty.hahajie.cn

Ruby: s.lines
来源：http://du.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://li.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://us.huanxung.cn

Py:   if not s:
来源：http://mn.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://su.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cj.nicolike.cn

TS:   if (s === "") {}
来源：http://om.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://an.haigaiapp.cn

Go:   if s == "" {}
来源：http://cc.nszjky.cn

Ruby: if s.empty?
来源：http://fm.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fd.colortex.cn

[E21] 超长截断加省略号
来源：http://lo.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sd.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vo.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tb.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ys.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sn.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ud.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kq.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oz.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://kx.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gc.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uw.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://db.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sg.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://im.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ey.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://la.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://us.wgjwhj.cn

================================================================================
来源：http://wv.huixinmuqiang.cn

F. 文件与目录
来源：http://xz.hahajie.cn

================================================================================
来源：http://iz.lnxyls.cn

[F01] 读取整个文件
来源：http://do.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ho.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://cn.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wo.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zd.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ju.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mq.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://lb.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://vt.nszjky.cn

[F02] 逐行读取文件
来源：http://eh.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zh.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tq.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ch.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lh.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qi.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eg.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://go.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wt.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://da.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qd.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://db.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wu.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ax.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kp.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jn.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://rd.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qv.hnjuh.cn

[F04] 追加写入文件
来源：http://za.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://by.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ju.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://em.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bt.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://en.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mj.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ku.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://md.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://ac.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bf.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://hv.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://du.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://or.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://am.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eb.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://kv.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://lt.asd995.cn

[F06] 删除文件
来源：http://sc.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://gm.hahajie.cn

PHP:  unlink("a.txt");
来源：http://yq.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sz.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://th.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bo.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://da.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://nx.colortex.cn

C#:   File.Delete("a.txt");
来源：http://rs.521024.cn

[F07] 创建目录（含多级）
来源：http://dw.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pd.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://in.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iz.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ig.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zv.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xh.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hr.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zf.chemitech.net.cn

[F08] 遍历目录
来源：http://ny.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://di.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pl.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://jt.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://og.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cw.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ql.hahajie.cn

Ruby: Dir.children("dir")
来源：http://gx.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://gy.hahajie.cn

[F09] 获取文件大小
来源：http://il.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://st.colortex.cn

PHP:  filesize("a.txt");
来源：http://uo.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://kn.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://nz.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rc.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://es.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://cz.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://iu.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://go.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://or.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fp.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xo.9csxet.cn

TS:   path.extname("a.txt")
来源：http://nr.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jg.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fs.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lp.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xp.panjiajie.cn

[F11] 复制与移动文件
来源：http://tu.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dl.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bh.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gi.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jv.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ec.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gc.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oj.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aj.chemitech.net.cn

[F12] CSV 读写
来源：http://wf.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sf.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qs.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nx.nicolike.cn

TS:   // 同上
来源：http://xp.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rp.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://so.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://co.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gp.haigaiapp.cn

================================================================================
来源：http://cn.huixiangedu.cn

G. 面向对象
来源：http://fv.nicolike.cn

================================================================================
来源：http://jm.jianghongdianzi.cn

[G01] 定义类
来源：http://ef.nszjky.cn

Py:   class User: pass
来源：http://wq.newstarts.cn

PHP:  class User {}
来源：http://ry.shtwfgs.cn

JS:   class User {}
来源：http://rt.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://ob.huixinmuqiang.cn

Java: class User {}
来源：http://za.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://zg.shxzskj.cn

Ruby: class User; end
来源：http://uv.jctech888.com.cn

C#:   class User {}
来源：http://xh.shtwfgs.cn

[G02] 构造函数
来源：http://nu.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://it.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://vj.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://yb.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://ag.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://vq.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yw.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://bs.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://rm.huixiangedu.cn

[G03] 实例属性
来源：http://cp.chemitech.net.cn

Py:   self.name = "x"
来源：http://up.shxzukj.cn

PHP:  public string $name = "x";
来源：http://ih.asd995.cn

JS:   this.name = "x";
来源：http://zz.haigaiapp.cn

TS:   name: string = "x";
来源：http://lm.521024.cn

Java: private String name;
来源：http://cq.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sz.gzmigu.cn

Ruby: @name = "x"
来源：http://ji.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://bo.bjjhwx.cn

[G04] 定义方法
来源：http://fk.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://ye.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zu.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://fy.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://tq.huanxung.cn

Java: String greet() { return name; }
来源：http://ra.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tf.shxzukj.cn

Ruby: def greet; @name; end
来源：http://wl.szsharing.cn

C#:   public string Greet() => Name;
来源：http://pa.asd995.cn

[G05] 继承
来源：http://nt.shxzskj.cn

Py:   class Admin(User): pass
来源：http://cc.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://em.lnxyls.cn

JS:   class Admin extends User {}
来源：http://yo.shxzukj.cn

TS:   class Admin extends User {}
来源：http://rb.9csxet.cn

Java: class Admin extends User {}
来源：http://ob.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pl.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://ni.nicolike.cn

C#:   class Admin : User {}
来源：http://pp.jianghongdianzi.cn

[G06] 重写方法
来源：http://ct.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://il.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rt.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://ah.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://mg.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://xs.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nk.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://su.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://ds.haigaiapp.cn

[G07] 调用父类方法
来源：http://qs.yuexingan06.cn

Py:   super().greet()
来源：http://nj.newstarts.cn

PHP:  parent::greet();
来源：http://fs.colortex.cn

JS:   super.greet();
来源：http://oq.yuntaijiaju.cn

TS:   super.greet();
来源：http://qp.szxytkj.cn

Java: super.greet();
来源：http://ft.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ki.colortex.cn

Ruby: super
来源：http://lp.jctech888.com.cn

C#:   base.Greet();
来源：http://df.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://tn.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xp.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://bp.szsharing.cn

JS:   static f() {}
来源：http://qp.szxytkj.cn

TS:   static f(): void {}
来源：http://si.hnjuh.cn

Java: static void f() {}
来源：http://rn.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ue.yuexingan06.cn

Ruby: def self.f; end
来源：http://ye.szsharing.cn

C#:   public static void F() {}
来源：http://hw.huanxung.cn

[G09] 接口 / 抽象类
来源：http://mg.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://gk.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jx.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ej.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://zv.hahajie.cn

Java: interface Shape { double area(); }
来源：http://hb.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://gt.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ar.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://qs.huixiangedu.cn

[G10] 访问控制
来源：http://pf.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://st.panjiajie.cn

PHP:  public / protected / private
来源：http://sh.colortex.cn

JS:   #private 字段；其余公开
来源：http://oh.wgjwhj.cn

TS:   public / protected / private
来源：http://qp.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://we.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pc.bjjhwx.cn

Ruby: public / protected / private
来源：http://bb.lnxyls.cn

C#:   public / protected / private / internal
来源：http://zl.wgjwhj.cn

[G11] getter / setter
来源：http://oa.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://yv.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hl.521024.cn

JS:   get name() { return this._name; }
来源：http://np.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://xe.lnxyls.cn

Java: public String getName() { return name; }
来源：http://jo.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pb.yuexingan06.cn


<!-- 参考信息 -->