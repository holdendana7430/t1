代发 wailian999

Ruby: s.split(",");  s.split
来源：http://cu.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qd.521024.cn

[E08] 数组按分隔符合并
来源：http://ic.muxihuayi.cn

Py:   ",".join(items)
来源：http://pc.lnxyls.cn

PHP:  implode(",", $items);
来源：http://ld.panjiajie.cn

JS:   items.join(",")
来源：http://dj.yuexingan06.cn

TS:   items.join(",")
来源：http://yt.wgjwhj.cn

Java: String.join(",", items)
来源：http://et.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://ux.wgjwhj.cn

Ruby: items.join(",")
来源：http://ax.nicolike.cn

C#:   string.Join(",", items)
来源：http://wd.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://il.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hx.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mv.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://qs.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://qr.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://xd.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wh.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tg.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ao.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://aw.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xf.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rs.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://tl.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://nk.nszjky.cn

Java: String.format("%03d", 7)
来源：http://kk.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pb.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ec.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lt.wgjwhj.cn

[E11] 反转字符串
来源：http://ae.bjjhwx.cn

Py:   s[::-1]
来源：http://yz.521024.cn

PHP:  strrev($s);
来源：http://ak.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://pp.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://an.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uh.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sf.hahajie.cn

Ruby: s.reverse
来源：http://zr.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fd.9csxet.cn

[E12] 统计某字符出现次数
来源：http://iv.colortex.cn

Py:   s.count("a")
来源：http://ni.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://gv.szsharing.cn

JS:   s.split("a").length - 1
来源：http://jn.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://bk.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xz.asd995.cn

Go:   strings.Count(s, "a")
来源：http://xv.colortex.cn

Ruby: s.count("a")
来源：http://xx.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://vw.shxzukj.cn

[E13] 逐字符遍历
来源：http://sw.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://lo.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rx.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qm.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rd.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ly.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://la.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wb.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uc.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://lu.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kc.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mm.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ke.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rv.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zd.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lm.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jn.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gx.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://ne.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iq.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://me.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ka.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kp.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rv.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eo.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vc.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ed.huanxung.cn

[E16] 数字千分位
来源：http://mv.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://oh.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://vc.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oa.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://my.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ck.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://of.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ek.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://ww.muxihuayi.cn

[E17] 首字母大写
来源：http://yl.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ze.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xg.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tz.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://we.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ij.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lv.panjiajie.cn

Ruby: s.capitalize
来源：http://xx.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uk.haigaiapp.cn

[E18] 模板占位符替换
来源：http://qe.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ak.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yj.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ec.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bu.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hm.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vu.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://em.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pq.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://gs.521024.cn

Py:   s.splitlines()
来源：http://xg.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uo.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://dh.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://om.colortex.cn

Java: s.lines().toList()
来源：http://sl.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://zv.jctech888.com.cn

Ruby: s.lines
来源：http://cx.521024.cn

C#:   s.Split('\n')
来源：http://oz.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://ik.shxzskj.cn

Py:   if not s:
来源：http://gt.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://du.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pa.szsharing.cn

TS:   if (s === "") {}
来源：http://ls.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://bt.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://em.wgjwhj.cn

Ruby: if s.empty?
来源：http://oa.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xm.colortex.cn

[E21] 超长截断加省略号
来源：http://jy.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cz.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lk.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://le.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sv.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ro.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://yw.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://no.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ub.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://ce.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tr.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wt.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ew.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tv.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sd.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gi.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://nc.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://de.shtwfgs.cn

================================================================================
来源：http://pa.jianghongdianzi.cn

F. 文件与目录
来源：http://mb.muxihuayi.cn

================================================================================
来源：http://oj.lnxyls.cn

[F01] 读取整个文件
来源：http://bx.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://el.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://rl.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ed.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ew.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yq.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dk.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://hd.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://jz.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://wd.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vo.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ex.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hd.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ms.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lp.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iv.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sv.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dh.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://jj.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pa.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iw.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ht.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fx.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ci.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cv.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://kp.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ye.szxytkj.cn

[F04] 追加写入文件
来源：http://xt.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oh.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vs.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kb.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://st.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ot.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lc.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cx.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uv.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://mg.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qw.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://rj.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://bs.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://ee.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gk.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fi.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://ly.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://cr.shxzskj.cn

[F06] 删除文件
来源：http://pn.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://pi.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://nf.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://le.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ot.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uk.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://gq.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://gy.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://jk.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://jb.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ya.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yk.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ik.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sh.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://te.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://st.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://so.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sz.colortex.cn

[F08] 遍历目录
来源：http://ye.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zb.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ax.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://lq.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://ep.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yl.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vj.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://do.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://fy.hahajie.cn

[F09] 获取文件大小
来源：http://ux.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://wp.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://gx.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://ui.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://gp.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vq.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tk.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://qs.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://aa.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://kj.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nb.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://am.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ra.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://qv.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://po.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xb.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oc.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fa.shtwfgs.cn

[F11] 复制与移动文件
来源：http://qt.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uj.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ea.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sj.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sm.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yf.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lp.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cz.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kr.hnjuh.cn

[F12] CSV 读写
来源：http://qv.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ar.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jx.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wa.muxihuayi.cn

TS:   // 同上
来源：http://se.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cv.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jv.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://we.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ry.panjiajie.cn

================================================================================
来源：http://dn.huixiangedu.cn

G. 面向对象
来源：http://sr.521024.cn

================================================================================
来源：http://sa.wgjwhj.cn

[G01] 定义类
来源：http://np.colortex.cn

Py:   class User: pass
来源：http://ks.asd995.cn

PHP:  class User {}
来源：http://dh.nszjky.cn

JS:   class User {}
来源：http://ax.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://fq.jianghongdianzi.cn

Java: class User {}
来源：http://xt.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://gq.chemitech.net.cn

Ruby: class User; end
来源：http://be.wgjwhj.cn

C#:   class User {}
来源：http://vf.newstarts.cn

[G02] 构造函数
来源：http://to.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://tr.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://oz.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://tc.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://al.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://rz.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fi.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://fv.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://cv.szsharing.cn

[G03] 实例属性
来源：http://io.panjiajie.cn

Py:   self.name = "x"
来源：http://hx.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://lz.shxzukj.cn

JS:   this.name = "x";
来源：http://dd.colortex.cn

TS:   name: string = "x";
来源：http://vn.lnxyls.cn

Java: private String name;
来源：http://xy.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lb.szxytkj.cn

Ruby: @name = "x"
来源：http://ou.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://zq.hnjuh.cn

[G04] 定义方法
来源：http://cg.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://fb.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ex.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ye.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://xa.colortex.cn

Java: String greet() { return name; }
来源：http://pm.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gl.asd995.cn

Ruby: def greet; @name; end
来源：http://lv.newstarts.cn

C#:   public string Greet() => Name;
来源：http://qh.shtwfgs.cn

[G05] 继承
来源：http://zt.colortex.cn

Py:   class Admin(User): pass
来源：http://te.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://at.hnjuh.cn

JS:   class Admin extends User {}
来源：http://pv.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://ut.szsharing.cn

Java: class Admin extends User {}
来源：http://eq.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://az.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://jr.9csxet.cn

C#:   class Admin : User {}
来源：http://lb.shtwfgs.cn

[G06] 重写方法
来源：http://tr.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://fb.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jg.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://fu.colortex.cn


<!-- 参考信息 -->