代发 wailian999

Ruby: s.split(",");  s.split
来源：http://jo.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ua.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://cx.colortex.cn

Py:   ",".join(items)
来源：http://qx.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://ip.huixiangedu.cn

JS:   items.join(",")
来源：http://le.lnxyls.cn

TS:   items.join(",")
来源：http://ec.nszjky.cn

Java: String.join(",", items)
来源：http://tf.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://ao.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://qh.szsharing.cn

C#:   string.Join(",", items)
来源：http://ep.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://fl.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dw.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ry.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://xx.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://iw.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://qu.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://na.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sd.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mz.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://tj.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eg.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ak.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://tw.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://jx.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://rz.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gl.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zk.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jj.shxzskj.cn

[E11] 反转字符串
来源：http://ew.yuntaijiaju.cn

Py:   s[::-1]
来源：http://bp.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://on.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://ee.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://vm.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://np.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ic.521024.cn

Ruby: s.reverse
来源：http://wi.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ar.colortex.cn

[E12] 统计某字符出现次数
来源：http://az.jctech888.com.cn

Py:   s.count("a")
来源：http://sl.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://dc.asd995.cn

JS:   s.split("a").length - 1
来源：http://oz.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://pi.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ww.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://mf.gzmigu.cn

Ruby: s.count("a")
来源：http://vj.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://on.hahajie.cn

[E13] 逐字符遍历
来源：http://jl.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://fo.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hr.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ld.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zm.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://og.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yd.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://la.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ei.nszjky.cn

[E14] URL 编码与 Base64
来源：http://dc.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qk.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jl.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ni.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rx.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kh.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wu.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mh.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ia.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://pu.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sc.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sp.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jo.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tr.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yi.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yo.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qt.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sl.9csxet.cn

[E16] 数字千分位
来源：http://lv.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://vp.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://qx.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sx.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yw.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uv.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uk.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hs.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://rf.asd995.cn

[E17] 首字母大写
来源：http://pe.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oy.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sk.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ej.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ob.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wm.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hu.bjjhwx.cn

Ruby: s.capitalize
来源：http://pr.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uo.nszjky.cn

[E18] 模板占位符替换
来源：http://dx.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oe.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pt.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cx.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://by.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ze.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xa.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://th.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://of.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://gd.hnjuh.cn

Py:   s.splitlines()
来源：http://pn.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jx.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://bt.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ul.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://aj.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://vw.jctech888.com.cn

Ruby: s.lines
来源：http://jk.shxzukj.cn

C#:   s.Split('\n')
来源：http://rm.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://fs.hahajie.cn

Py:   if not s:
来源：http://nm.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yx.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lp.bjjhwx.cn

TS:   if (s === "") {}
来源：http://sy.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://ay.panjiajie.cn

Go:   if s == "" {}
来源：http://jm.chemitech.net.cn

Ruby: if s.empty?
来源：http://dg.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fx.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://qw.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lb.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tt.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kz.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cb.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uk.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://sw.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ul.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fg.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://rn.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oj.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nu.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yz.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://po.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jx.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ds.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://tc.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pr.muxihuayi.cn

================================================================================
来源：http://kl.shtwfgs.cn

F. 文件与目录
来源：http://ti.szsharing.cn

================================================================================
来源：http://dw.newstarts.cn

[F01] 读取整个文件
来源：http://om.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fj.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://xe.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nt.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ks.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hr.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://do.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://dh.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://cq.szxytkj.cn

[F02] 逐行读取文件
来源：http://wx.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yj.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lr.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hn.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mn.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ik.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ll.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kx.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://od.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://na.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yy.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jf.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hy.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ab.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://in.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pt.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://zs.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ul.nszjky.cn

[F04] 追加写入文件
来源：http://un.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xn.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://et.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xr.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://og.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gz.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rb.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cu.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hb.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://nk.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ea.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://sa.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://qm.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://fh.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yn.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ee.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://fn.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://vy.szxytkj.cn

[F06] 删除文件
来源：http://ha.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://ou.asd995.cn

PHP:  unlink("a.txt");
来源：http://ii.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xx.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mn.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xs.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://dn.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://za.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://ed.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ev.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rt.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jv.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lh.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vz.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lb.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://of.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mk.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yl.chemitech.net.cn

[F08] 遍历目录
来源：http://td.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uj.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gd.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://kx.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://gi.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jb.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lk.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://yn.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://dy.nicolike.cn

[F09] 获取文件大小
来源：http://tz.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://da.huanxung.cn

PHP:  filesize("a.txt");
来源：http://fu.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://oc.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://td.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ez.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uu.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://wn.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://vk.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://kl.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ou.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lg.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cr.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://yr.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jx.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eb.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ed.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mt.gzmigu.cn

[F11] 复制与移动文件
来源：http://er.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://el.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vb.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zn.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ft.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ru.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jh.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://df.bookmarksfly.cn

[F12] CSV 读写
来源：http://yl.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ui.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jh.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yl.colortex.cn

TS:   // 同上
来源：http://ea.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qy.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xz.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oc.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dp.bookmarksfly.cn

================================================================================
来源：http://ef.chemitech.net.cn

G. 面向对象
来源：http://jx.haigaiapp.cn

================================================================================
来源：http://cw.huixinmuqiang.cn

[G01] 定义类
来源：http://kp.haigaiapp.cn

Py:   class User: pass
来源：http://ix.huixinmuqiang.cn

PHP:  class User {}
来源：http://br.shxzukj.cn

JS:   class User {}
来源：http://uz.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://gb.yuexingan06.cn

Java: class User {}
来源：http://mb.hnjuh.cn

Go:   type User struct { Name string }
来源：http://qo.haigaiapp.cn

Ruby: class User; end
来源：http://th.szxytkj.cn

C#:   class User {}
来源：http://kb.shxzukj.cn

[G02] 构造函数
来源：http://ct.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://qz.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://gc.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://da.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://tv.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://zt.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://im.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://ei.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://fi.gzmigu.cn

[G03] 实例属性
来源：http://hp.nicolike.cn

Py:   self.name = "x"
来源：http://ub.szxytkj.cn

PHP:  public string $name = "x";
来源：http://em.lnxyls.cn

JS:   this.name = "x";
来源：http://rs.muxihuayi.cn

TS:   name: string = "x";
来源：http://mg.521024.cn

Java: private String name;
来源：http://zu.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ij.lnxyls.cn

Ruby: @name = "x"
来源：http://vf.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://pj.gzmigu.cn

[G04] 定义方法
来源：http://er.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://hq.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lu.asd995.cn

JS:   greet() { return this.name; }
来源：http://af.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://hh.szsharing.cn

Java: String greet() { return name; }
来源：http://qn.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fd.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://tg.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://my.szsharing.cn

[G05] 继承
来源：http://dw.newstarts.cn

Py:   class Admin(User): pass
来源：http://hv.9csxet.cn

PHP:  class Admin extends User {}
来源：http://ru.panjiajie.cn

JS:   class Admin extends User {}
来源：http://ax.szxytkj.cn

TS:   class Admin extends User {}
来源：http://wb.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://xe.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hd.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://go.colortex.cn

C#:   class Admin : User {}
来源：http://ki.nszjky.cn

[G06] 重写方法
来源：http://kg.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://zd.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wy.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://bm.shxzukj.cn


<!-- 参考信息 -->