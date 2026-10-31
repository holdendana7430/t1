代发 wailian999

Py:   for ch in s: print(ch)
来源：http://by.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://of.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://se.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ub.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pe.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jt.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iv.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iy.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://iy.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://us.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://az.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yf.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://og.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://am.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ob.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fc.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ek.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://nw.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jo.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ln.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zy.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ro.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zg.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://td.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hu.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ix.lnxyls.cn

[E16] 数字千分位
来源：http://mc.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://cg.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://fo.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ut.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rn.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ci.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zx.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sd.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://vn.nicolike.cn

[E17] 首字母大写
来源：http://rn.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mi.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qv.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ke.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://np.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ww.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ob.shxzskj.cn

Ruby: s.capitalize
来源：http://vs.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://od.szxytkj.cn

[E18] 模板占位符替换
来源：http://kr.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fw.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xm.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yc.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ue.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yt.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lt.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://il.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wk.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://ax.hahajie.cn

Py:   s.splitlines()
来源：http://dy.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ou.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://gs.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://jq.chemitech.net.cn

Java: s.lines().toList()
来源：http://fh.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://aw.huanxung.cn

Ruby: s.lines
来源：http://il.521024.cn

C#:   s.Split('\n')
来源：http://ar.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://sb.bookmarksfly.cn

Py:   if not s:
来源：http://aw.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ph.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kc.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://wl.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://pc.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://vs.shxzukj.cn

Ruby: if s.empty?
来源：http://ak.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bw.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://px.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://df.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xz.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gq.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aj.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ef.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://kb.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sr.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qk.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://uq.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zx.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lr.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ew.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yf.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sy.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cc.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://os.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yj.hnjuh.cn

================================================================================
来源：http://qj.jianghongdianzi.cn

F. 文件与目录
来源：http://ec.lnxyls.cn

================================================================================
来源：http://wi.bookmarksfly.cn

[F01] 读取整个文件
来源：http://wq.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ol.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://nd.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nc.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ma.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qx.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://la.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://qn.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://zy.shxzukj.cn

[F02] 逐行读取文件
来源：http://vs.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bj.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xj.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lk.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ka.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qc.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hg.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yz.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xh.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://ck.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rz.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://on.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dd.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uz.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vq.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wk.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://ve.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zc.huanxung.cn

[F04] 追加写入文件
来源：http://mt.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rs.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ie.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uk.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wt.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gx.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hi.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://di.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://js.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://za.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xp.colortex.cn

PHP:  file_exists("a.txt");
来源：http://vo.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ny.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://ff.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cx.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xj.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://od.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://mn.huanxung.cn

[F06] 删除文件
来源：http://ch.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://is.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://nu.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zk.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ky.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qe.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://vt.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://wr.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://pb.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://dq.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wy.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aa.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ry.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pc.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ty.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ix.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ks.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yr.colortex.cn

[F08] 遍历目录
来源：http://oe.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rm.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://po.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://la.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://ad.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rk.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ve.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://fw.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://fv.chemitech.net.cn

[F09] 获取文件大小
来源：http://fo.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://xq.hahajie.cn

PHP:  filesize("a.txt");
来源：http://vr.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://tp.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ix.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pa.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sa.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://gh.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://xo.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://mr.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rf.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://km.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yd.szsharing.cn

TS:   path.extname("a.txt")
来源：http://yf.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uf.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pg.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ya.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mb.521024.cn

[F11] 复制与移动文件
来源：http://bu.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bn.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qb.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nw.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bu.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eg.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://st.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yl.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ob.jctech888.com.cn

[F12] CSV 读写
来源：http://or.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mb.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cx.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oz.yuntaijiaju.cn

TS:   // 同上
来源：http://vz.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dy.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gj.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zn.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hu.jctech888.com.cn

================================================================================
来源：http://at.szsharing.cn

G. 面向对象
来源：http://ok.panjiajie.cn

================================================================================
来源：http://tx.szsharing.cn

[G01] 定义类
来源：http://rn.huixiangedu.cn

Py:   class User: pass
来源：http://qk.colortex.cn

PHP:  class User {}
来源：http://ni.colortex.cn

JS:   class User {}
来源：http://kk.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://it.yuexingan06.cn

Java: class User {}
来源：http://ne.newstarts.cn

Go:   type User struct { Name string }
来源：http://zv.huanxung.cn

Ruby: class User; end
来源：http://hw.wgjwhj.cn

C#:   class User {}
来源：http://wq.nicolike.cn

[G02] 构造函数
来源：http://lv.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://ws.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://kb.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://ym.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://yx.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://xo.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jt.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://vy.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ud.szxytkj.cn

[G03] 实例属性
来源：http://ps.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://fs.huanxung.cn

PHP:  public string $name = "x";
来源：http://qm.nszjky.cn

JS:   this.name = "x";
来源：http://pt.newstarts.cn

TS:   name: string = "x";
来源：http://wc.shxzskj.cn

Java: private String name;
来源：http://fu.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sg.jctech888.com.cn

Ruby: @name = "x"
来源：http://lp.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://rt.newstarts.cn

[G04] 定义方法
来源：http://ed.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://vp.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fp.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://ao.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://eu.haigaiapp.cn

Java: String greet() { return name; }
来源：http://bx.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gj.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://yv.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://em.panjiajie.cn

[G05] 继承
来源：http://hu.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://oj.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://lg.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://bp.szxytkj.cn

TS:   class Admin extends User {}
来源：http://bt.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://sq.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tv.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://cp.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://ln.yuntaijiaju.cn

[G06] 重写方法
来源：http://pz.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://rz.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pn.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://bs.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://tn.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://lp.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wa.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://ns.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://ix.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://fb.huixinmuqiang.cn

Py:   super().greet()
来源：http://zl.szsharing.cn

PHP:  parent::greet();
来源：http://we.shxzukj.cn

JS:   super.greet();
来源：http://qy.shxzukj.cn

TS:   super.greet();
来源：http://hz.panjiajie.cn

Java: super.greet();
来源：http://vm.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ed.bjjhwx.cn

Ruby: super
来源：http://pw.521024.cn

C#:   base.Greet();
来源：http://dy.nicolike.cn

[G08] 静态方法与属性
来源：http://ye.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vh.9csxet.cn

PHP:  public static function f() {}
来源：http://hv.nszjky.cn

JS:   static f() {}
来源：http://en.shtwfgs.cn

TS:   static f(): void {}
来源：http://ng.newstarts.cn

Java: static void f() {}
来源：http://du.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tr.yuexingan06.cn

Ruby: def self.f; end
来源：http://qk.shtwfgs.cn

C#:   public static void F() {}
来源：http://yq.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://td.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://lx.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qk.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pp.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://ha.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://yy.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://no.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hk.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://xe.huixinmuqiang.cn

[G10] 访问控制
来源：http://jr.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://kk.haigaiapp.cn

PHP:  public / protected / private
来源：http://ci.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://pz.hnjuh.cn

TS:   public / protected / private
来源：http://fl.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://az.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://un.9csxet.cn

Ruby: public / protected / private
来源：http://nz.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://wn.9csxet.cn

[G11] getter / setter
来源：http://bs.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://tc.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ta.nszjky.cn

JS:   get name() { return this._name; }
来源：http://fo.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://vn.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://fn.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wg.shtwfgs.cn


<!-- 参考信息 -->