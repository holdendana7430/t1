代发 wailian999

Go:   strings.Count(s, "a")
来源：http://jx.9csxet.cn

Ruby: s.count("a")
来源：http://tm.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://px.nicolike.cn

[E13] 逐字符遍历
来源：http://tv.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://zr.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ci.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wf.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gf.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ym.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jq.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cc.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jd.521024.cn

[E14] URL 编码与 Base64
来源：http://gk.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ks.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xi.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fl.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jg.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ze.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wv.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gq.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rv.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://mb.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://br.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ha.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fz.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wg.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ak.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ny.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bz.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ui.bjjhwx.cn

[E16] 数字千分位
来源：http://dd.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://rp.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://qv.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rz.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ib.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zg.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pv.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ib.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://nf.szxytkj.cn

[E17] 首字母大写
来源：http://eq.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ju.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rd.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kv.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://np.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mv.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kr.jctech888.com.cn

Ruby: s.capitalize
来源：http://rn.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://px.521024.cn

[E18] 模板占位符替换
来源：http://ot.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ll.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gy.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zr.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ga.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ta.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ge.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xf.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://li.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://zf.9csxet.cn

Py:   s.splitlines()
来源：http://ie.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wr.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://rw.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://vc.521024.cn

Java: s.lines().toList()
来源：http://zi.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://xs.hnjuh.cn

Ruby: s.lines
来源：http://fm.haigaiapp.cn

C#:   s.Split('\n')
来源：http://xo.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://zt.chemitech.net.cn

Py:   if not s:
来源：http://kd.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pe.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jz.colortex.cn

TS:   if (s === "") {}
来源：http://jd.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://ca.panjiajie.cn

Go:   if s == "" {}
来源：http://sa.lnxyls.cn

Ruby: if s.empty?
来源：http://os.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mf.9csxet.cn

[E21] 超长截断加省略号
来源：http://yi.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dz.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hh.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ge.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gt.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://un.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://da.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xd.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eh.huanxung.cn

[E22] 字节长度与字符长度
来源：http://qi.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lq.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cm.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ei.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zl.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pw.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dn.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://tm.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vf.muxihuayi.cn

================================================================================
来源：http://ef.bookmarksfly.cn

F. 文件与目录
来源：http://gn.9csxet.cn

================================================================================
来源：http://kr.shtwfgs.cn

[F01] 读取整个文件
来源：http://sf.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kb.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://vx.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fj.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hi.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wy.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ae.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://dr.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://bu.shtwfgs.cn

[F02] 逐行读取文件
来源：http://lv.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cu.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dh.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xc.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ur.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ze.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bn.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bn.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://et.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://ei.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mr.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fq.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kb.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vg.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uf.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xj.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://ey.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gk.yuexingan06.cn

[F04] 追加写入文件
来源：http://xb.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zn.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tq.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fh.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://od.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zs.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rx.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wa.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oq.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://qb.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://je.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://ej.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://ku.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://gt.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oe.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xv.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://yi.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://am.jianghongdianzi.cn

[F06] 删除文件
来源：http://lh.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://cb.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://xx.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://us.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lt.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vs.colortex.cn

Go:   os.Remove("a.txt")
来源：http://ib.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://pf.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://cr.colortex.cn

[F07] 创建目录（含多级）
来源：http://fi.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ra.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sn.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zp.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ba.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zw.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fv.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wz.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xe.colortex.cn

[F08] 遍历目录
来源：http://ki.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xo.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://db.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://ed.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://sh.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gn.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yf.hahajie.cn

Ruby: Dir.children("dir")
来源：http://vg.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://iq.wgjwhj.cn

[F09] 获取文件大小
来源：http://us.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://cg.asd995.cn

PHP:  filesize("a.txt");
来源：http://vs.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://jf.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://by.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sy.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rw.asd995.cn

Ruby: File.size("a.txt")
来源：http://gz.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://co.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ls.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://er.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://se.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nq.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://lw.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ho.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rn.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uw.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jr.shxzukj.cn

[F11] 复制与移动文件
来源：http://jp.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ux.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ic.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ct.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qy.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sp.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vm.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wf.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wf.newstarts.cn

[F12] CSV 读写
来源：http://ug.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hc.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bp.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ce.huanxung.cn

TS:   // 同上
来源：http://ui.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gl.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gj.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://va.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rr.hahajie.cn

================================================================================
来源：http://md.panjiajie.cn

G. 面向对象
来源：http://vj.haigaiapp.cn

================================================================================
来源：http://ws.521024.cn

[G01] 定义类
来源：http://sd.shtwfgs.cn

Py:   class User: pass
来源：http://ak.lnxyls.cn

PHP:  class User {}
来源：http://yj.panjiajie.cn

JS:   class User {}
来源：http://ra.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://ih.shxzskj.cn

Java: class User {}
来源：http://ok.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://xy.shxzskj.cn

Ruby: class User; end
来源：http://my.wgjwhj.cn

C#:   class User {}
来源：http://pm.shxzukj.cn

[G02] 构造函数
来源：http://ow.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://pg.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://se.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://zm.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://ay.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://mm.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nj.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://el.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ot.shxzukj.cn

[G03] 实例属性
来源：http://ra.shxzskj.cn

Py:   self.name = "x"
来源：http://ya.shxzskj.cn

PHP:  public string $name = "x";
来源：http://zf.haigaiapp.cn

JS:   this.name = "x";
来源：http://ak.huixiangedu.cn

TS:   name: string = "x";
来源：http://ic.wgjwhj.cn

Java: private String name;
来源：http://yl.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fc.shtwfgs.cn

Ruby: @name = "x"
来源：http://ll.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://kk.colortex.cn

[G04] 定义方法
来源：http://mh.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://in.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ze.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://qy.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://fm.haigaiapp.cn

Java: String greet() { return name; }
来源：http://fc.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jz.szxytkj.cn

Ruby: def greet; @name; end
来源：http://yl.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://lb.huanxung.cn

[G05] 继承
来源：http://ye.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://gv.asd995.cn

PHP:  class Admin extends User {}
来源：http://co.gzmigu.cn

JS:   class Admin extends User {}
来源：http://pk.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://lo.shxzukj.cn

Java: class Admin extends User {}
来源：http://lr.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://an.panjiajie.cn

Ruby: class Admin < User; end
来源：http://mc.szxytkj.cn

C#:   class Admin : User {}
来源：http://un.shxzskj.cn

[G06] 重写方法
来源：http://wr.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://vd.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yp.colortex.cn

JS:   greet() { return "admin"; }
来源：http://nu.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://dx.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ue.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ru.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://vb.521024.cn

C#:   public override string Greet() => "admin";
来源：http://tk.szsharing.cn

[G07] 调用父类方法
来源：http://ul.9csxet.cn

Py:   super().greet()
来源：http://al.panjiajie.cn

PHP:  parent::greet();
来源：http://cg.shxzskj.cn

JS:   super.greet();
来源：http://ld.panjiajie.cn

TS:   super.greet();
来源：http://rg.nicolike.cn

Java: super.greet();
来源：http://tw.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pr.jianghongdianzi.cn

Ruby: super
来源：http://yd.newstarts.cn

C#:   base.Greet();
来源：http://uz.huixiangedu.cn

[G08] 静态方法与属性
来源：http://ey.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://on.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://wf.lnxyls.cn

JS:   static f() {}
来源：http://nr.shtwfgs.cn

TS:   static f(): void {}
来源：http://tx.jianghongdianzi.cn

Java: static void f() {}
来源：http://sy.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vf.huanxung.cn

Ruby: def self.f; end
来源：http://as.shxzskj.cn

C#:   public static void F() {}
来源：http://cj.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://sj.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://ee.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nk.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eo.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://se.521024.cn

Java: interface Shape { double area(); }
来源：http://sr.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://vf.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yp.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://wz.shtwfgs.cn

[G10] 访问控制
来源：http://sd.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://tp.huanxung.cn

PHP:  public / protected / private
来源：http://sc.nicolike.cn

JS:   #private 字段；其余公开
来源：http://uv.newstarts.cn

TS:   public / protected / private
来源：http://hj.521024.cn

Java: public / protected / private / 默认包级
来源：http://sn.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ch.521024.cn

Ruby: public / protected / private
来源：http://lw.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://dr.jctech888.com.cn

[G11] getter / setter
来源：http://wf.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://mh.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://la.szsharing.cn


<!-- 参考信息 -->