代发 wailian999

Py:   for ch in s: print(ch)
来源：http://gi.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vk.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rl.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yr.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sz.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mw.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://da.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qd.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://tk.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sd.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://li.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jm.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ym.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qs.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ih.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bl.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ly.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://mn.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dn.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iv.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wo.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jp.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ku.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fb.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gd.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rz.bjjhwx.cn

[E16] 数字千分位
来源：http://sd.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://mz.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://dz.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dh.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://av.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rf.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yb.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ma.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://zj.chemitech.net.cn

[E17] 首字母大写
来源：http://rg.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tp.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bb.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nt.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oy.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pw.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uc.shtwfgs.cn

Ruby: s.capitalize
来源：http://lx.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ew.szxytkj.cn

[E18] 模板占位符替换
来源：http://vo.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dn.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ko.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xo.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lq.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jh.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://au.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yx.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yy.nicolike.cn

[E19] 多行文本按行拆分
来源：http://yt.colortex.cn

Py:   s.splitlines()
来源：http://vg.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://li.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://uw.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://yz.nszjky.cn

Java: s.lines().toList()
来源：http://ux.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://vq.huanxung.cn

Ruby: s.lines
来源：http://ws.muxihuayi.cn

C#:   s.Split('\n')
来源：http://cn.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://lt.newstarts.cn

Py:   if not s:
来源：http://rf.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cm.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nt.haigaiapp.cn

TS:   if (s === "") {}
来源：http://de.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://id.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://uh.newstarts.cn

Ruby: if s.empty?
来源：http://cb.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lv.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://fj.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ij.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fq.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://un.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ef.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ij.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://yb.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mt.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tn.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://qo.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cq.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kw.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rs.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ul.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xq.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://el.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://ks.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ct.newstarts.cn

================================================================================
来源：http://lc.bjjhwx.cn

F. 文件与目录
来源：http://xp.yuexingan06.cn

================================================================================
来源：http://vv.bjjhwx.cn

[F01] 读取整个文件
来源：http://oa.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dg.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://kh.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ns.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tm.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ow.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sd.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://fg.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://oa.jctech888.com.cn

[F02] 逐行读取文件
来源：http://oy.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pt.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://le.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bp.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pd.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qd.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://go.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kw.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ht.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://ch.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://er.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wh.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ed.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mg.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ip.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zr.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ln.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qv.gzmigu.cn

[F04] 追加写入文件
来源：http://ex.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ae.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xx.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gs.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mv.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zo.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bw.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://af.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sm.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://vh.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tx.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://so.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://gu.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://bw.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zl.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ja.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://dv.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://ah.wgjwhj.cn

[F06] 删除文件
来源：http://vx.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://tx.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://ye.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gg.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ov.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vj.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://fi.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://ge.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://tb.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://yq.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zh.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ik.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gv.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bl.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://df.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pk.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dg.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://av.newstarts.cn

[F08] 遍历目录
来源：http://rc.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aw.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kk.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://jm.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://pq.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fn.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pz.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://ji.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://ox.panjiajie.cn

[F09] 获取文件大小
来源：http://vi.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://bu.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://ko.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://bp.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://hs.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://up.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jy.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://mr.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://pm.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://ek.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://om.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xz.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qn.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://ym.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vz.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iz.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bp.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ds.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://br.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bm.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gm.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fr.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wr.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fr.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nl.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ry.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wd.shxzukj.cn

[F12] CSV 读写
来源：http://ae.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hf.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ki.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ir.asd995.cn

TS:   // 同上
来源：http://vp.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://by.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nl.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aw.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hc.colortex.cn

================================================================================
来源：http://kh.panjiajie.cn

G. 面向对象
来源：http://xx.huixinmuqiang.cn

================================================================================
来源：http://nd.bjjhwx.cn

[G01] 定义类
来源：http://xz.huixiangedu.cn

Py:   class User: pass
来源：http://tt.hnjuh.cn

PHP:  class User {}
来源：http://bc.chemitech.net.cn

JS:   class User {}
来源：http://wn.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://xb.hahajie.cn

Java: class User {}
来源：http://ey.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://cq.nicolike.cn

Ruby: class User; end
来源：http://cz.hnjuh.cn

C#:   class User {}
来源：http://na.chemitech.net.cn

[G02] 构造函数
来源：http://jb.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://ed.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://ut.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://oc.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://hu.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://pg.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://re.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://ix.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://pe.szsharing.cn

[G03] 实例属性
来源：http://kp.shxzukj.cn

Py:   self.name = "x"
来源：http://ns.huanxung.cn

PHP:  public string $name = "x";
来源：http://aw.nszjky.cn

JS:   this.name = "x";
来源：http://cz.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://be.bjjhwx.cn

Java: private String name;
来源：http://wh.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uu.hahajie.cn

Ruby: @name = "x"
来源：http://ti.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://cd.lnxyls.cn

[G04] 定义方法
来源：http://yh.huanxung.cn

Py:   def greet(self): return self.name
来源：http://pu.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ub.hahajie.cn

JS:   greet() { return this.name; }
来源：http://wi.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://qc.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://kq.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dd.huanxung.cn

Ruby: def greet; @name; end
来源：http://we.hahajie.cn

C#:   public string Greet() => Name;
来源：http://dy.yuexingan06.cn

[G05] 继承
来源：http://za.hahajie.cn

Py:   class Admin(User): pass
来源：http://rq.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://dl.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://wc.9csxet.cn

TS:   class Admin extends User {}
来源：http://rm.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://fm.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pk.szxytkj.cn

Ruby: class Admin < User; end
来源：http://la.lnxyls.cn

C#:   class Admin : User {}
来源：http://cj.huixinmuqiang.cn

[G06] 重写方法
来源：http://ht.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://dy.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qm.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://iu.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://kf.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://cq.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wb.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://jg.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://yg.shxzskj.cn

[G07] 调用父类方法
来源：http://zp.shtwfgs.cn

Py:   super().greet()
来源：http://ml.hahajie.cn

PHP:  parent::greet();
来源：http://wt.newstarts.cn

JS:   super.greet();
来源：http://rw.huixiangedu.cn

TS:   super.greet();
来源：http://br.bookmarksfly.cn

Java: super.greet();
来源：http://aj.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rt.panjiajie.cn

Ruby: super
来源：http://yw.wgjwhj.cn

C#:   base.Greet();
来源：http://sa.jctech888.com.cn

[G08] 静态方法与属性
来源：http://io.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pt.newstarts.cn

PHP:  public static function f() {}
来源：http://ic.newstarts.cn

JS:   static f() {}
来源：http://ke.9csxet.cn

TS:   static f(): void {}
来源：http://fh.nszjky.cn

Java: static void f() {}
来源：http://qe.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ft.nszjky.cn

Ruby: def self.f; end
来源：http://ta.bjjhwx.cn

C#:   public static void F() {}
来源：http://wv.9csxet.cn

[G09] 接口 / 抽象类
来源：http://gl.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://hj.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ur.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dk.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://lb.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://tj.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://ap.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yh.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://na.nicolike.cn

[G10] 访问控制
来源：http://kq.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://lz.nszjky.cn

PHP:  public / protected / private
来源：http://vl.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://qb.jianghongdianzi.cn

TS:   public / protected / private
来源：http://kp.521024.cn

Java: public / protected / private / 默认包级
来源：http://dp.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rz.yuexingan06.cn

Ruby: public / protected / private
来源：http://zb.lnxyls.cn

C#:   public / protected / private / internal
来源：http://yh.colortex.cn

[G11] getter / setter
来源：http://wc.asd995.cn

Py:   @property 与 @x.setter
来源：http://af.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fv.9csxet.cn

JS:   get name() { return this._name; }
来源：http://ev.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://fa.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://cw.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fx.yuexingan06.cn


<!-- 参考信息 -->