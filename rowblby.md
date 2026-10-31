代发 wailian999

JS:   [...s].reverse().join("")
来源：http://yg.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://nk.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fw.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cc.yuexingan06.cn

Ruby: s.reverse
来源：http://ta.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ml.colortex.cn

[E12] 统计某字符出现次数
来源：http://jp.yuexingan06.cn

Py:   s.count("a")
来源：http://gv.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://pq.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://ii.hahajie.cn

TS:   s.split("a").length - 1
来源：http://ph.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ft.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://el.nszjky.cn

Ruby: s.count("a")
来源：http://ry.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://sg.hahajie.cn

[E13] 逐字符遍历
来源：http://tc.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://zk.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mx.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ho.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lp.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://py.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eo.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dn.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://np.521024.cn

[E14] URL 编码与 Base64
来源：http://ne.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nn.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rw.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bg.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cx.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fz.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fv.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iw.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ne.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://bi.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hs.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://da.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yb.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xe.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gh.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://po.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vd.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wx.huixiangedu.cn

[E16] 数字千分位
来源：http://gs.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://jw.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ad.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://af.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ay.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ax.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ei.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nn.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://rf.szxytkj.cn

[E17] 首字母大写
来源：http://uy.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kn.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fj.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rk.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://to.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jh.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gs.shtwfgs.cn

Ruby: s.capitalize
来源：http://zr.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aw.bjjhwx.cn

[E18] 模板占位符替换
来源：http://xh.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://db.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ya.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ib.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ip.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cy.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bv.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wh.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wj.szsharing.cn

[E19] 多行文本按行拆分
来源：http://wl.wgjwhj.cn

Py:   s.splitlines()
来源：http://bl.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wh.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://xw.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://bp.yuexingan06.cn

Java: s.lines().toList()
来源：http://dp.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://ld.huixiangedu.cn

Ruby: s.lines
来源：http://kb.panjiajie.cn

C#:   s.Split('\n')
来源：http://ho.asd995.cn

[E20] 判断字符串是否为空
来源：http://ir.nicolike.cn

Py:   if not s:
来源：http://jy.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pc.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rz.bjjhwx.cn

TS:   if (s === "") {}
来源：http://on.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://dp.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://ub.huanxung.cn

Ruby: if s.empty?
来源：http://jw.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://de.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://dc.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kt.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fc.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ek.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lx.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://op.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://sc.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yb.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kd.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://rv.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xp.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vu.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jp.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hb.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uz.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nc.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://hv.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zs.shtwfgs.cn

================================================================================
来源：http://dw.jianghongdianzi.cn

F. 文件与目录
来源：http://by.huanxung.cn

================================================================================
来源：http://if.lnxyls.cn

[F01] 读取整个文件
来源：http://qa.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ls.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://wa.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://es.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://be.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cp.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://um.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://ef.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://pv.shxzskj.cn

[F02] 逐行读取文件
来源：http://qi.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fm.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xv.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hy.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iw.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ir.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xp.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wz.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ac.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ii.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eb.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sq.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ya.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qx.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xs.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qp.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://nt.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mk.colortex.cn

[F04] 追加写入文件
来源：http://hu.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qz.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zq.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vn.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jy.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rm.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bb.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zm.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://il.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://iz.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rc.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://jh.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://mn.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://jo.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jr.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jv.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://kn.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://dg.shxzukj.cn

[F06] 删除文件
来源：http://mh.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://dd.521024.cn

PHP:  unlink("a.txt");
来源：http://dh.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://or.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nb.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://od.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://np.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://ez.asd995.cn

C#:   File.Delete("a.txt");
来源：http://zm.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://nr.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rh.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xg.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ux.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xc.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vm.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rj.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lq.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dt.muxihuayi.cn

[F08] 遍历目录
来源：http://nd.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gz.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sl.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://wx.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://az.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://og.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uu.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://sj.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ma.newstarts.cn

[F09] 获取文件大小
来源：http://sh.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://tu.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://yj.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://eb.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://zi.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://md.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vt.9csxet.cn

Ruby: File.size("a.txt")
来源：http://bu.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://fg.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://yc.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rj.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ld.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://na.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://da.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fw.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://te.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nx.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xg.huanxung.cn

[F11] 复制与移动文件
来源：http://rh.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rt.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ed.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ik.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wf.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fn.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ts.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tx.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jy.huixinmuqiang.cn

[F12] CSV 读写
来源：http://fc.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lq.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bo.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oo.hahajie.cn

TS:   // 同上
来源：http://df.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zr.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nf.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vj.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ij.newstarts.cn

================================================================================
来源：http://me.huanxung.cn

G. 面向对象
来源：http://sq.chemitech.net.cn

================================================================================
来源：http://hv.yuexingan06.cn

[G01] 定义类
来源：http://io.szxytkj.cn

Py:   class User: pass
来源：http://kg.shxzukj.cn

PHP:  class User {}
来源：http://iz.lnxyls.cn

JS:   class User {}
来源：http://ja.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://ik.shxzukj.cn

Java: class User {}
来源：http://wt.lnxyls.cn

Go:   type User struct { Name string }
来源：http://az.521024.cn

Ruby: class User; end
来源：http://gc.wgjwhj.cn

C#:   class User {}
来源：http://ii.hnjuh.cn

[G02] 构造函数
来源：http://lq.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://fz.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ki.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://pe.colortex.cn

TS:   constructor(public name: string) {}
来源：http://lr.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://wi.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ag.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://xs.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://dz.bjjhwx.cn

[G03] 实例属性
来源：http://qv.jctech888.com.cn

Py:   self.name = "x"
来源：http://ce.9csxet.cn

PHP:  public string $name = "x";
来源：http://tg.shxzukj.cn

JS:   this.name = "x";
来源：http://mc.521024.cn

TS:   name: string = "x";
来源：http://we.huixinmuqiang.cn

Java: private String name;
来源：http://ul.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://em.panjiajie.cn

Ruby: @name = "x"
来源：http://xd.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://pp.hnjuh.cn

[G04] 定义方法
来源：http://av.szsharing.cn

Py:   def greet(self): return self.name
来源：http://gt.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ps.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://rw.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://zl.hnjuh.cn

Java: String greet() { return name; }
来源：http://kt.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cg.hahajie.cn

Ruby: def greet; @name; end
来源：http://sb.9csxet.cn

C#:   public string Greet() => Name;
来源：http://go.panjiajie.cn

[G05] 继承
来源：http://kl.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://qo.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://dj.huanxung.cn

JS:   class Admin extends User {}
来源：http://pt.szsharing.cn

TS:   class Admin extends User {}
来源：http://hs.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://mr.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://px.panjiajie.cn

Ruby: class Admin < User; end
来源：http://py.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://er.jctech888.com.cn

[G06] 重写方法
来源：http://xz.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://mi.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dz.asd995.cn

JS:   greet() { return "admin"; }
来源：http://kk.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://vi.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://qe.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fg.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://qj.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://hj.colortex.cn

[G07] 调用父类方法
来源：http://mg.huanxung.cn

Py:   super().greet()
来源：http://os.chemitech.net.cn

PHP:  parent::greet();
来源：http://kn.asd995.cn

JS:   super.greet();
来源：http://bc.colortex.cn

TS:   super.greet();
来源：http://ws.wgjwhj.cn

Java: super.greet();
来源：http://op.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yu.hahajie.cn

Ruby: super
来源：http://pn.yuntaijiaju.cn

C#:   base.Greet();
来源：http://tk.jctech888.com.cn

[G08] 静态方法与属性
来源：http://zd.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vz.szsharing.cn

PHP:  public static function f() {}
来源：http://as.hahajie.cn

JS:   static f() {}
来源：http://ld.nicolike.cn

TS:   static f(): void {}
来源：http://ha.wgjwhj.cn

Java: static void f() {}
来源：http://qx.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ex.yuexingan06.cn

Ruby: def self.f; end
来源：http://fk.huanxung.cn

C#:   public static void F() {}
来源：http://da.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://we.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://bz.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bj.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://em.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://ju.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://kv.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://wt.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oa.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://fk.yuexingan06.cn


<!-- 参考信息 -->