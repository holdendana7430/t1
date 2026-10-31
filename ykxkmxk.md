代发 wailian999

PHP:  implode(",", $items);
来源：http://th.shxzukj.cn

JS:   items.join(",")
来源：http://us.szxytkj.cn

TS:   items.join(",")
来源：http://cd.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://ev.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://pa.szxytkj.cn

Ruby: items.join(",")
来源：http://fy.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://hl.asd995.cn

[E09] 去除所有空白字符
来源：http://sa.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cz.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eo.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://kq.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://rl.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ln.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jx.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rw.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cg.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://lf.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xy.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ze.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://tt.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://mx.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://eq.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xb.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xs.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oe.hahajie.cn

[E11] 反转字符串
来源：http://ez.bjjhwx.cn

Py:   s[::-1]
来源：http://gf.bjjhwx.cn

PHP:  strrev($s);
来源：http://xt.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://sh.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://qi.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nc.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hk.asd995.cn

Ruby: s.reverse
来源：http://yd.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kx.colortex.cn

[E12] 统计某字符出现次数
来源：http://ru.haigaiapp.cn

Py:   s.count("a")
来源：http://qf.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://ed.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://mq.hahajie.cn

TS:   s.split("a").length - 1
来源：http://lv.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eq.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://ln.nszjky.cn

Ruby: s.count("a")
来源：http://bl.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://wb.panjiajie.cn

[E13] 逐字符遍历
来源：http://bn.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://vs.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nt.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bf.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ha.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ib.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wu.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hu.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ir.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://tx.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vz.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eo.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vf.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nd.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ze.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ip.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cc.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xa.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://vs.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qr.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mp.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sh.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pe.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zm.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ab.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tu.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aw.hahajie.cn

[E16] 数字千分位
来源：http://wf.newstarts.cn

Py:   f"{1234567:,}"
来源：http://qr.huanxung.cn

PHP:  number_format(1234567);
来源：http://ov.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tb.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mx.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qa.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rl.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vb.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://gs.szsharing.cn

[E17] 首字母大写
来源：http://wq.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://by.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ye.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lk.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ki.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://el.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://va.wgjwhj.cn

Ruby: s.capitalize
来源：http://vq.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ao.szsharing.cn

[E18] 模板占位符替换
来源：http://oz.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://km.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gs.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nv.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yn.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ug.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mc.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bu.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://go.521024.cn

[E19] 多行文本按行拆分
来源：http://ty.yuexingan06.cn

Py:   s.splitlines()
来源：http://qe.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nz.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://pk.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://nm.9csxet.cn

Java: s.lines().toList()
来源：http://zy.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ue.szsharing.cn

Ruby: s.lines
来源：http://rr.hahajie.cn

C#:   s.Split('\n')
来源：http://rp.9csxet.cn

[E20] 判断字符串是否为空
来源：http://az.newstarts.cn

Py:   if not s:
来源：http://qd.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cf.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://so.wgjwhj.cn

TS:   if (s === "") {}
来源：http://xv.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ek.yuexingan06.cn

Go:   if s == "" {}
来源：http://qf.hnjuh.cn

Ruby: if s.empty?
来源：http://fv.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sn.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://pd.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aw.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pz.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xu.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ew.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sj.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://tj.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sy.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dx.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://pd.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cg.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zi.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pf.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ck.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hh.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pr.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://jp.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vd.bjjhwx.cn

================================================================================
来源：http://ng.huixinmuqiang.cn

F. 文件与目录
来源：http://qo.gzmigu.cn

================================================================================
来源：http://qw.szsharing.cn

[F01] 读取整个文件
来源：http://qv.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kz.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://xd.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pz.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uk.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hq.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wu.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://fd.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://vz.shxzskj.cn

[F02] 逐行读取文件
来源：http://ki.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jh.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pv.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cs.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vj.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ds.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rx.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xf.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ud.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://jw.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rz.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fn.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hw.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ah.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vh.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ny.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://yc.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kv.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://wk.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fm.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zy.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bs.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ke.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jb.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ks.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://se.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ln.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://nc.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ca.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://tp.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://oz.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://rq.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nc.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iv.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://vb.colortex.cn

C#:   File.Exists("a.txt")
来源：http://ef.muxihuayi.cn

[F06] 删除文件
来源：http://zs.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://ao.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://jb.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fq.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mu.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yc.521024.cn

Go:   os.Remove("a.txt")
来源：http://qj.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://wz.521024.cn

C#:   File.Delete("a.txt");
来源：http://wv.huanxung.cn

[F07] 创建目录（含多级）
来源：http://kd.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nf.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zd.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ve.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://os.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fp.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://th.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lx.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vr.yuntaijiaju.cn

[F08] 遍历目录
来源：http://sy.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bx.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wv.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://nd.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://eq.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cm.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ny.521024.cn

Ruby: Dir.children("dir")
来源：http://cf.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://lz.panjiajie.cn

[F09] 获取文件大小
来源：http://dn.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://ed.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://cz.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://cx.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://bk.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nn.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wz.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://pl.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://qh.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ci.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dv.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mu.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ci.huanxung.cn

TS:   path.extname("a.txt")
来源：http://ei.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://li.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://of.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qu.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nd.hnjuh.cn

[F11] 复制与移动文件
来源：http://wh.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lq.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iv.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ty.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yq.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vq.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ho.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ur.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fz.hnjuh.cn

[F12] CSV 读写
来源：http://rm.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sm.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yr.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://or.haigaiapp.cn

TS:   // 同上
来源：http://mj.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ld.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jp.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mz.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://el.newstarts.cn

================================================================================
来源：http://zs.panjiajie.cn

G. 面向对象
来源：http://ze.huanxung.cn

================================================================================
来源：http://uf.colortex.cn

[G01] 定义类
来源：http://qm.szxytkj.cn

Py:   class User: pass
来源：http://rk.shxzskj.cn

PHP:  class User {}
来源：http://di.wgjwhj.cn

JS:   class User {}
来源：http://gq.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://aq.huanxung.cn

Java: class User {}
来源：http://hl.shxzskj.cn

Go:   type User struct { Name string }
来源：http://dk.newstarts.cn

Ruby: class User; end
来源：http://kl.shtwfgs.cn

C#:   class User {}
来源：http://vw.chemitech.net.cn

[G02] 构造函数
来源：http://cq.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://sc.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://bo.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://ie.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://re.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://eo.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://od.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ms.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://ql.colortex.cn

[G03] 实例属性
来源：http://vt.gzmigu.cn

Py:   self.name = "x"
来源：http://xc.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://rm.chemitech.net.cn

JS:   this.name = "x";
来源：http://li.huanxung.cn

TS:   name: string = "x";
来源：http://dp.yuexingan06.cn

Java: private String name;
来源：http://ur.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://em.panjiajie.cn

Ruby: @name = "x"
来源：http://xr.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://uy.huixiangedu.cn

[G04] 定义方法
来源：http://bg.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://xl.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yr.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://qs.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://vm.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://nw.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iz.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://nj.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://wo.hahajie.cn

[G05] 继承
来源：http://za.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://bo.521024.cn

PHP:  class Admin extends User {}
来源：http://ng.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://mi.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://eh.colortex.cn

Java: class Admin extends User {}
来源：http://jm.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ls.hahajie.cn

Ruby: class Admin < User; end
来源：http://ib.panjiajie.cn

C#:   class Admin : User {}
来源：http://rc.hahajie.cn

[G06] 重写方法
来源：http://ba.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://pc.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dl.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://et.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://ao.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://rc.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ic.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://cu.bookmarksfly.cn


<!-- 参考信息 -->