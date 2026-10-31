代发 wailian999

Go:   strings.Join(items, ",")
来源：http://op.panjiajie.cn

Ruby: items.join(",")
来源：http://wr.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://rf.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://xi.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ot.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rx.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://su.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://tt.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://co.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bt.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mq.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jf.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://gx.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zl.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cw.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://mb.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://vb.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://qo.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vi.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gd.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kx.haigaiapp.cn

[E11] 反转字符串
来源：http://rn.hahajie.cn

Py:   s[::-1]
来源：http://id.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://ua.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://ie.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://mf.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://je.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sj.gzmigu.cn

Ruby: s.reverse
来源：http://vl.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ok.nicolike.cn

[E12] 统计某字符出现次数
来源：http://jx.szsharing.cn

Py:   s.count("a")
来源：http://fs.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://wp.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://ip.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://cw.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jn.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://tf.yuexingan06.cn

Ruby: s.count("a")
来源：http://vy.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://hy.haigaiapp.cn

[E13] 逐字符遍历
来源：http://tw.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://wm.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ps.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kd.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sf.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hy.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hx.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fr.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ju.colortex.cn

[E14] URL 编码与 Base64
来源：http://xn.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ri.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://by.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zi.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gm.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://af.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jr.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ht.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gh.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://cd.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://il.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ja.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xs.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sa.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gl.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ks.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hh.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jk.yuntaijiaju.cn

[E16] 数字千分位
来源：http://ze.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://mn.lnxyls.cn

PHP:  number_format(1234567);
来源：http://tq.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://og.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ab.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mr.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hu.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://el.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://rn.shxzskj.cn

[E17] 首字母大写
来源：http://wj.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vg.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ng.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://so.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mi.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bk.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mn.szxytkj.cn

Ruby: s.capitalize
来源：http://mw.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wu.colortex.cn

[E18] 模板占位符替换
来源：http://jb.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ix.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cc.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qv.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uq.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xe.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://al.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sj.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bu.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://li.szsharing.cn

Py:   s.splitlines()
来源：http://jm.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ay.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://jo.521024.cn

TS:   s.split(/\r?\n/)
来源：http://rv.huanxung.cn

Java: s.lines().toList()
来源：http://oj.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://wy.nszjky.cn

Ruby: s.lines
来源：http://wd.haigaiapp.cn

C#:   s.Split('\n')
来源：http://ez.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://fv.huixinmuqiang.cn

Py:   if not s:
来源：http://pf.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cx.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://da.huanxung.cn

TS:   if (s === "") {}
来源：http://ew.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ro.muxihuayi.cn

Go:   if s == "" {}
来源：http://mz.szxytkj.cn

Ruby: if s.empty?
来源：http://ew.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xy.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://sf.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xd.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://no.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yv.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gd.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vw.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://oz.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jf.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uv.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://gv.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tv.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dd.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yh.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yj.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bb.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eg.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://bq.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ba.panjiajie.cn

================================================================================
来源：http://yn.gzmigu.cn

F. 文件与目录
来源：http://dj.muxihuayi.cn

================================================================================
来源：http://vo.hahajie.cn

[F01] 读取整个文件
来源：http://jf.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cy.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://kx.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ef.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uh.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ps.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jw.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://lh.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://nn.521024.cn

[F02] 逐行读取文件
来源：http://mz.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wi.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fd.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xj.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hg.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hm.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://re.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://as.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ib.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://sc.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iq.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yp.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pu.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ar.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ch.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vn.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://my.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xf.muxihuayi.cn

[F04] 追加写入文件
来源：http://xx.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tr.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iw.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gu.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xf.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jb.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ep.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xo.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jy.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://pu.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sb.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://js.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://yd.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://ft.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uq.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vj.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://fu.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://jm.lnxyls.cn

[F06] 删除文件
来源：http://uf.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://kp.colortex.cn

PHP:  unlink("a.txt");
来源：http://dr.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://de.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sw.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ld.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://et.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://fa.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://nn.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://et.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ql.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xl.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yh.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ag.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qf.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xb.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qd.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qt.haigaiapp.cn

[F08] 遍历目录
来源：http://xr.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://np.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cn.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://jc.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ob.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yx.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xu.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://zq.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://qm.bjjhwx.cn

[F09] 获取文件大小
来源：http://ra.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://aw.9csxet.cn

PHP:  filesize("a.txt");
来源：http://qv.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://ry.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://qj.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zr.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fe.huanxung.cn

Ruby: File.size("a.txt")
来源：http://uo.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://yq.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://fw.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fy.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lz.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mp.nszjky.cn

TS:   path.extname("a.txt")
来源：http://zi.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ip.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://at.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rz.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ci.nszjky.cn

[F11] 复制与移动文件
来源：http://uw.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nc.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jz.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kj.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rv.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bs.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aq.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yw.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xz.bookmarksfly.cn

[F12] CSV 读写
来源：http://fm.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qv.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rc.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vh.hahajie.cn

TS:   // 同上
来源：http://aj.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tp.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jp.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tr.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://co.lnxyls.cn

================================================================================
来源：http://nu.colortex.cn

G. 面向对象
来源：http://nt.lnxyls.cn

================================================================================
来源：http://tk.521024.cn

[G01] 定义类
来源：http://ak.hnjuh.cn

Py:   class User: pass
来源：http://cj.nicolike.cn

PHP:  class User {}
来源：http://za.chemitech.net.cn

JS:   class User {}
来源：http://pt.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://li.huanxung.cn

Java: class User {}
来源：http://is.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://tx.chemitech.net.cn

Ruby: class User; end
来源：http://to.huixiangedu.cn

C#:   class User {}
来源：http://om.lnxyls.cn

[G02] 构造函数
来源：http://hn.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://va.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://se.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://zr.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://lz.521024.cn

Java: User(String name) { this.name = name; }
来源：http://aj.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sa.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://lo.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://nh.chemitech.net.cn

[G03] 实例属性
来源：http://zd.nszjky.cn

Py:   self.name = "x"
来源：http://qs.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://se.hnjuh.cn

JS:   this.name = "x";
来源：http://vb.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://gx.colortex.cn

Java: private String name;
来源：http://ga.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zc.szsharing.cn

Ruby: @name = "x"
来源：http://bc.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://fs.huanxung.cn

[G04] 定义方法
来源：http://qm.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://jf.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zv.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://oz.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://mf.shtwfgs.cn

Java: String greet() { return name; }
来源：http://ef.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zi.asd995.cn

Ruby: def greet; @name; end
来源：http://ho.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://ym.yuntaijiaju.cn

[G05] 继承
来源：http://uh.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://nq.huanxung.cn

PHP:  class Admin extends User {}
来源：http://ve.9csxet.cn

JS:   class Admin extends User {}
来源：http://yf.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://mr.bjjhwx.cn

Java: class Admin extends User {}
来源：http://bz.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bl.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://oz.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://yp.wgjwhj.cn

[G06] 重写方法
来源：http://am.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://mc.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bl.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://xh.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://jv.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://hx.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ff.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://tj.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://kn.huanxung.cn

[G07] 调用父类方法
来源：http://xq.asd995.cn

Py:   super().greet()
来源：http://yy.newstarts.cn

PHP:  parent::greet();
来源：http://kb.nszjky.cn


<!-- 参考信息 -->