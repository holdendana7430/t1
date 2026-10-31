代发 wailian999

Py:   for ch in s: print(ch)
来源：http://eg.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ob.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sb.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vq.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nc.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jn.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jc.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fo.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://sq.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xi.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xf.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bw.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dm.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tc.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mv.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ln.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://zk.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yy.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fw.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://it.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ob.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://is.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fz.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qg.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cm.hnjuh.cn

[E16] 数字千分位
来源：http://sc.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://rr.nicolike.cn

PHP:  number_format(1234567);
来源：http://tc.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lf.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fz.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zo.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uf.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wj.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://xp.szxytkj.cn

[E17] 首字母大写
来源：http://ye.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hk.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fz.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rc.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yn.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xm.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hr.jctech888.com.cn

Ruby: s.capitalize
来源：http://av.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ls.shtwfgs.cn

[E18] 模板占位符替换
来源：http://ds.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ms.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uf.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mr.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://te.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vk.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wu.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gs.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ax.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://xf.hahajie.cn

Py:   s.splitlines()
来源：http://gj.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ec.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://mf.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://ua.yuexingan06.cn

Java: s.lines().toList()
来源：http://if.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ek.yuntaijiaju.cn

Ruby: s.lines
来源：http://fm.panjiajie.cn

C#:   s.Split('\n')
来源：http://gj.colortex.cn

[E20] 判断字符串是否为空
来源：http://mj.yuntaijiaju.cn

Py:   if not s:
来源：http://jc.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yh.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lg.nszjky.cn

TS:   if (s === "") {}
来源：http://zw.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://bi.haigaiapp.cn

Go:   if s == "" {}
来源：http://wj.lnxyls.cn

Ruby: if s.empty?
来源：http://sh.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dc.gzmigu.cn

[E21] 超长截断加省略号
来源：http://ig.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qo.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ld.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oe.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bh.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uq.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://ds.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ye.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kk.newstarts.cn

[E22] 字节长度与字符长度
来源：http://mx.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tt.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dy.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ix.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eg.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://da.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://gq.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ox.huixiangedu.cn

================================================================================
来源：http://ak.hahajie.cn

F. 文件与目录
来源：http://lw.muxihuayi.cn

================================================================================
来源：http://xy.muxihuayi.cn

[F01] 读取整个文件
来源：http://tt.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lw.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://jj.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bk.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ij.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://di.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lx.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://hi.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://jv.shtwfgs.cn

[F02] 逐行读取文件
来源：http://at.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://il.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cn.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gu.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xx.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://et.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jq.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nc.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jc.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://mq.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gg.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://on.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fr.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jp.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ez.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lw.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://yw.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nk.9csxet.cn

[F04] 追加写入文件
来源：http://jw.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wc.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://er.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mq.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uj.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mc.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://we.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dz.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nz.521024.cn

[F05] 判断文件或目录是否存在
来源：http://oj.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ef.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://fe.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://gb.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://nl.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eo.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zc.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://qb.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://zs.newstarts.cn

[F06] 删除文件
来源：http://nj.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://uk.nszjky.cn

PHP:  unlink("a.txt");
来源：http://nu.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xp.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ax.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xe.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://kt.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://ho.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://my.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://um.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dy.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qq.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://re.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fy.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gm.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bg.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yz.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ti.shxzukj.cn

[F08] 遍历目录
来源：http://hd.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zr.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wv.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://qn.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://gp.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kk.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ch.9csxet.cn

Ruby: Dir.children("dir")
来源：http://mq.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://tl.newstarts.cn

[F09] 获取文件大小
来源：http://wd.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://rw.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://sx.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://hk.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://lj.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eo.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zx.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://po.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://aj.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://pd.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://se.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kp.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iq.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://ig.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cr.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gm.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ml.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xn.newstarts.cn

[F11] 复制与移动文件
来源：http://ay.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://af.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cq.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tm.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tj.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xp.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ri.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ug.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xz.colortex.cn

[F12] CSV 读写
来源：http://aw.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fb.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wb.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pn.nszjky.cn

TS:   // 同上
来源：http://wf.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yw.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cm.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ws.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vl.shxzskj.cn

================================================================================
来源：http://sx.hnjuh.cn

G. 面向对象
来源：http://ra.asd995.cn

================================================================================
来源：http://sh.hnjuh.cn

[G01] 定义类
来源：http://ld.asd995.cn

Py:   class User: pass
来源：http://fm.yuexingan06.cn

PHP:  class User {}
来源：http://ew.hahajie.cn

JS:   class User {}
来源：http://jh.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://am.hnjuh.cn

Java: class User {}
来源：http://sm.asd995.cn

Go:   type User struct { Name string }
来源：http://fo.gzmigu.cn

Ruby: class User; end
来源：http://ok.muxihuayi.cn

C#:   class User {}
来源：http://ch.szsharing.cn

[G02] 构造函数
来源：http://fr.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://xg.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://rx.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ee.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://hb.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://dp.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bv.hnjuh.cn

Ruby: def initialize(name); @name = name; end
来源：http://zl.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://mj.wgjwhj.cn

[G03] 实例属性
来源：http://di.muxihuayi.cn

Py:   self.name = "x"
来源：http://st.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://yw.shxzskj.cn

JS:   this.name = "x";
来源：http://po.hnjuh.cn

TS:   name: string = "x";
来源：http://ks.huixiangedu.cn

Java: private String name;
来源：http://qb.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pz.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://ul.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://bn.shtwfgs.cn

[G04] 定义方法
来源：http://it.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://zh.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qb.nszjky.cn

JS:   greet() { return this.name; }
来源：http://nu.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://mm.521024.cn

Java: String greet() { return name; }
来源：http://pe.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yd.521024.cn

Ruby: def greet; @name; end
来源：http://ki.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://tf.bjjhwx.cn

[G05] 继承
来源：http://qy.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://ur.hahajie.cn

PHP:  class Admin extends User {}
来源：http://nj.newstarts.cn

JS:   class Admin extends User {}
来源：http://ko.hnjuh.cn

TS:   class Admin extends User {}
来源：http://kp.huanxung.cn

Java: class Admin extends User {}
来源：http://vd.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ey.gzmigu.cn

Ruby: class Admin < User; end
来源：http://kr.jctech888.com.cn

C#:   class Admin : User {}
来源：http://fl.nicolike.cn

[G06] 重写方法
来源：http://dk.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://qe.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://et.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://tr.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://qs.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ub.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ji.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://rc.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://sy.521024.cn

[G07] 调用父类方法
来源：http://db.chemitech.net.cn

Py:   super().greet()
来源：http://yk.lnxyls.cn

PHP:  parent::greet();
来源：http://jn.chemitech.net.cn

JS:   super.greet();
来源：http://vi.newstarts.cn

TS:   super.greet();
来源：http://ac.jianghongdianzi.cn

Java: super.greet();
来源：http://js.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qe.szxytkj.cn

Ruby: super
来源：http://tz.jianghongdianzi.cn

C#:   base.Greet();
来源：http://dt.bjjhwx.cn

[G08] 静态方法与属性
来源：http://cs.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ag.haigaiapp.cn

PHP:  public static function f() {}
来源：http://je.hahajie.cn

JS:   static f() {}
来源：http://yb.newstarts.cn

TS:   static f(): void {}
来源：http://lv.shtwfgs.cn

Java: static void f() {}
来源：http://kc.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zf.muxihuayi.cn

Ruby: def self.f; end
来源：http://vo.asd995.cn

C#:   public static void F() {}
来源：http://ko.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://lf.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://ek.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qz.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fo.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://hd.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://wf.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ss.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bn.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://zy.haigaiapp.cn

[G10] 访问控制
来源：http://xc.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://im.huixiangedu.cn

PHP:  public / protected / private
来源：http://xn.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://dp.jctech888.com.cn

TS:   public / protected / private
来源：http://dv.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://zg.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kv.huixiangedu.cn

Ruby: public / protected / private
来源：http://tg.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://ov.nicolike.cn

[G11] getter / setter
来源：http://qc.nicolike.cn

Py:   @property 与 @x.setter
来源：http://fx.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fe.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://in.521024.cn

TS:   get name(): string { return this._name; }
来源：http://qv.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://ka.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ey.hahajie.cn


<!-- 参考信息 -->