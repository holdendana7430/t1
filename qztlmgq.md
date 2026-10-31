代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sn.newstarts.cn

[E11] 反转字符串
来源：http://gw.newstarts.cn

Py:   s[::-1]
来源：http://bq.panjiajie.cn

PHP:  strrev($s);
来源：http://iy.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://dw.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://aq.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ti.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gn.newstarts.cn

Ruby: s.reverse
来源：http://hh.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dl.szsharing.cn

[E12] 统计某字符出现次数
来源：http://zj.9csxet.cn

Py:   s.count("a")
来源：http://so.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://uf.colortex.cn

JS:   s.split("a").length - 1
来源：http://dy.huanxung.cn

TS:   s.split("a").length - 1
来源：http://vm.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rw.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://wv.huanxung.cn

Ruby: s.count("a")
来源：http://xa.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://mr.newstarts.cn

[E13] 逐字符遍历
来源：http://cz.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://eh.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pf.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aq.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gq.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kq.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ao.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dt.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://np.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://yx.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://su.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ym.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://my.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://de.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bc.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lw.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wr.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ph.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://lr.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xj.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oq.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jp.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ab.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://of.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qt.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hr.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cn.wgjwhj.cn

[E16] 数字千分位
来源：http://dy.szsharing.cn

Py:   f"{1234567:,}"
来源：http://mi.shxzskj.cn

PHP:  number_format(1234567);
来源：http://xd.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://va.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fq.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ci.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zi.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://er.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://cd.wgjwhj.cn

[E17] 首字母大写
来源：http://kc.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mj.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qq.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wx.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sr.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hs.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ng.gzmigu.cn

Ruby: s.capitalize
来源：http://uj.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gc.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ma.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ia.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ts.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lh.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tz.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zm.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://su.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rt.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nq.nszjky.cn

[E19] 多行文本按行拆分
来源：http://np.szsharing.cn

Py:   s.splitlines()
来源：http://bs.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pf.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://ae.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://hs.bookmarksfly.cn

Java: s.lines().toList()
来源：http://nk.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://fy.jianghongdianzi.cn

Ruby: s.lines
来源：http://qa.asd995.cn

C#:   s.Split('\n')
来源：http://oo.newstarts.cn

[E20] 判断字符串是否为空
来源：http://os.jctech888.com.cn

Py:   if not s:
来源：http://dt.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pm.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yq.szsharing.cn

TS:   if (s === "") {}
来源：http://ju.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://qr.shtwfgs.cn

Go:   if s == "" {}
来源：http://nz.bjjhwx.cn

Ruby: if s.empty?
来源：http://cd.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lc.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://qr.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lm.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wm.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gs.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tu.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xh.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://xp.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uk.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gd.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://pr.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cz.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ug.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vj.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fv.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kv.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mt.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://cm.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fo.shtwfgs.cn

================================================================================
来源：http://mn.bjjhwx.cn

F. 文件与目录
来源：http://im.muxihuayi.cn

================================================================================
来源：http://bo.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://qo.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vv.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://vg.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://si.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yf.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jq.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kd.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://ys.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://vz.shtwfgs.cn

[F02] 逐行读取文件
来源：http://uv.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eg.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qs.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nw.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ej.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mv.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ag.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pb.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yu.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://qy.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ol.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xf.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mx.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lf.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lk.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rq.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://rc.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ys.jctech888.com.cn

[F04] 追加写入文件
来源：http://sq.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ns.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xp.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ym.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ld.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vp.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pw.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pz.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yg.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://tk.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oa.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://yy.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://fz.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://sb.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zh.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vw.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://jp.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://cc.yuexingan06.cn

[F06] 删除文件
来源：http://tn.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://sm.colortex.cn

PHP:  unlink("a.txt");
来源：http://zk.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hd.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hq.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bv.colortex.cn

Go:   os.Remove("a.txt")
来源：http://ju.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://qs.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://qk.9csxet.cn

[F07] 创建目录（含多级）
来源：http://bt.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cb.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vf.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ln.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mc.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sj.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kq.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cg.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://je.521024.cn

[F08] 遍历目录
来源：http://ol.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cl.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dy.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://xd.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://en.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tl.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iq.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://qa.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://ls.lnxyls.cn

[F09] 获取文件大小
来源：http://zj.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://fq.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://fa.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://tx.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://vq.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rr.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ui.asd995.cn

Ruby: File.size("a.txt")
来源：http://bu.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://sn.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://hi.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://om.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jb.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gs.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://vr.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://na.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ru.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ev.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rf.nicolike.cn

[F11] 复制与移动文件
来源：http://wu.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bz.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ur.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pl.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ck.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dw.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ll.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ml.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ge.9csxet.cn

[F12] CSV 读写
来源：http://si.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wl.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ks.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ig.szxytkj.cn

TS:   // 同上
来源：http://hg.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ag.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tj.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://om.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oo.9csxet.cn

================================================================================
来源：http://fh.nszjky.cn

G. 面向对象
来源：http://vh.shxzskj.cn

================================================================================
来源：http://uz.haigaiapp.cn

[G01] 定义类
来源：http://ic.wgjwhj.cn

Py:   class User: pass
来源：http://jt.asd995.cn

PHP:  class User {}
来源：http://zz.jctech888.com.cn

JS:   class User {}
来源：http://nh.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://ee.nicolike.cn

Java: class User {}
来源：http://ld.gzmigu.cn

Go:   type User struct { Name string }
来源：http://js.jianghongdianzi.cn

Ruby: class User; end
来源：http://ig.wgjwhj.cn

C#:   class User {}
来源：http://im.szxytkj.cn

[G02] 构造函数
来源：http://vt.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://wo.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://rs.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://ur.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://ac.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://ay.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mi.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://ms.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://sx.nicolike.cn

[G03] 实例属性
来源：http://uc.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://yf.colortex.cn

PHP:  public string $name = "x";
来源：http://jt.chemitech.net.cn

JS:   this.name = "x";
来源：http://ej.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://na.newstarts.cn

Java: private String name;
来源：http://fy.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://se.hahajie.cn

Ruby: @name = "x"
来源：http://bv.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://kk.shxzskj.cn

[G04] 定义方法
来源：http://tx.newstarts.cn

Py:   def greet(self): return self.name
来源：http://wh.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lm.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://do.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://vx.yuexingan06.cn

Java: String greet() { return name; }
来源：http://yf.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://va.szxytkj.cn

Ruby: def greet; @name; end
来源：http://ff.hahajie.cn

C#:   public string Greet() => Name;
来源：http://ry.yuexingan06.cn

[G05] 继承
来源：http://rv.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://bq.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://kv.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://xr.shxzskj.cn

TS:   class Admin extends User {}
来源：http://nf.haigaiapp.cn

Java: class Admin extends User {}
来源：http://pb.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ix.asd995.cn

Ruby: class Admin < User; end
来源：http://tv.shtwfgs.cn

C#:   class Admin : User {}
来源：http://qn.jianghongdianzi.cn

[G06] 重写方法
来源：http://dl.colortex.cn

Py:   def greet(self): return "admin"
来源：http://px.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wb.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://im.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://te.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://pw.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nx.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://zj.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://kc.wgjwhj.cn

[G07] 调用父类方法
来源：http://xo.asd995.cn

Py:   super().greet()
来源：http://hh.bookmarksfly.cn

PHP:  parent::greet();
来源：http://am.haigaiapp.cn

JS:   super.greet();
来源：http://ex.huixiangedu.cn

TS:   super.greet();
来源：http://es.colortex.cn

Java: super.greet();
来源：http://uj.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ut.shxzukj.cn

Ruby: super
来源：http://mv.yuexingan06.cn

C#:   base.Greet();
来源：http://ww.szsharing.cn

[G08] 静态方法与属性
来源：http://dy.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hq.asd995.cn

PHP:  public static function f() {}
来源：http://mf.huanxung.cn

JS:   static f() {}
来源：http://ny.newstarts.cn

TS:   static f(): void {}
来源：http://ei.colortex.cn

Java: static void f() {}
来源：http://ej.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sl.nicolike.cn

Ruby: def self.f; end
来源：http://jg.bjjhwx.cn

C#:   public static void F() {}
来源：http://tl.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://nq.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://bc.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cu.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qi.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://aj.bookmarksfly.cn


<!-- 参考信息 -->