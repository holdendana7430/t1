代发 wailian999

PHP:  implode(",", $items);
来源：http://fa.panjiajie.cn

JS:   items.join(",")
来源：http://la.huixiangedu.cn

TS:   items.join(",")
来源：http://zh.szxytkj.cn

Java: String.join(",", items)
来源：http://dz.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://nb.jctech888.com.cn

Ruby: items.join(",")
来源：http://mh.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://ms.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://rt.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ym.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ey.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://hj.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://zz.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://qz.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zl.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ua.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nt.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://qx.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lw.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rz.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://rg.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://vw.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://ys.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sx.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ty.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hl.szxytkj.cn

[E11] 反转字符串
来源：http://cw.bjjhwx.cn

Py:   s[::-1]
来源：http://ht.huixiangedu.cn

PHP:  strrev($s);
来源：http://lq.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ih.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://ot.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yd.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ha.bjjhwx.cn

Ruby: s.reverse
来源：http://yj.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yj.nszjky.cn

[E12] 统计某字符出现次数
来源：http://zn.chemitech.net.cn

Py:   s.count("a")
来源：http://ru.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://sa.nszjky.cn

JS:   s.split("a").length - 1
来源：http://ud.huanxung.cn

TS:   s.split("a").length - 1
来源：http://ym.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qj.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://oe.haigaiapp.cn

Ruby: s.count("a")
来源：http://vj.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://tk.gzmigu.cn

[E13] 逐字符遍历
来源：http://yn.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://qx.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fd.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zf.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fr.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://io.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zw.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kx.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vk.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ju.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fz.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ug.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kl.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bi.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ah.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bz.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dr.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://os.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://fw.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cx.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vz.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mn.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://se.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sk.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qk.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yb.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wx.jctech888.com.cn

[E16] 数字千分位
来源：http://ql.colortex.cn

Py:   f"{1234567:,}"
来源：http://rb.hnjuh.cn

PHP:  number_format(1234567);
来源：http://rb.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ke.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hm.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bq.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xe.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://st.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://fe.nszjky.cn

[E17] 首字母大写
来源：http://qm.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sc.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rt.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yf.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nj.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wt.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rr.jctech888.com.cn

Ruby: s.capitalize
来源：http://ke.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uc.asd995.cn

[E18] 模板占位符替换
来源：http://ye.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vo.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pu.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ij.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zu.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://um.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://da.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xy.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mz.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://pi.huanxung.cn

Py:   s.splitlines()
来源：http://ki.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ta.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://ih.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://pj.szxytkj.cn

Java: s.lines().toList()
来源：http://yo.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://gk.9csxet.cn

Ruby: s.lines
来源：http://hc.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://yh.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://mr.hnjuh.cn

Py:   if not s:
来源：http://za.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gn.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bl.huixiangedu.cn

TS:   if (s === "") {}
来源：http://xz.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://hz.bjjhwx.cn

Go:   if s == "" {}
来源：http://kl.shxzskj.cn

Ruby: if s.empty?
来源：http://xf.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xl.shxzskj.cn

[E21] 超长截断加省略号
来源：http://wd.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mh.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xp.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nc.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tg.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ne.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://cs.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wq.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://as.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://jj.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ib.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ag.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ys.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zl.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qq.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vo.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://rq.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fo.jianghongdianzi.cn

================================================================================
来源：http://bd.gzmigu.cn

F. 文件与目录
来源：http://zi.yuexingan06.cn

================================================================================
来源：http://ne.huixiangedu.cn

[F01] 读取整个文件
来源：http://sw.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jd.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://nn.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://an.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ye.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dq.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qg.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://yz.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://pk.chemitech.net.cn

[F02] 逐行读取文件
来源：http://dn.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hh.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ci.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zu.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pu.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oq.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oz.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ro.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://su.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://ou.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sj.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xq.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://et.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nt.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ee.521024.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pq.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://ft.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://md.nszjky.cn

[F04] 追加写入文件
来源：http://ng.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://op.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://id.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vq.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vp.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qd.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yv.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fv.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://si.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://we.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ww.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://im.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://mb.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://ro.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sq.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wv.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://lr.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://kh.shxzukj.cn

[F06] 删除文件
来源：http://ap.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://aj.newstarts.cn

PHP:  unlink("a.txt");
来源：http://pp.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://do.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nw.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ne.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ey.asd995.cn

Ruby: File.delete("a.txt")
来源：http://cq.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://ri.szsharing.cn

[F07] 创建目录（含多级）
来源：http://pp.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tz.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jv.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rm.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eg.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ga.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vf.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wq.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nl.wgjwhj.cn

[F08] 遍历目录
来源：http://ij.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zj.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yx.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://xk.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://sw.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qt.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ui.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://su.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://rn.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://mi.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://lc.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://np.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://ix.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://dv.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ox.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lv.9csxet.cn

Ruby: File.size("a.txt")
来源：http://zv.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://pf.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://sb.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dp.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://au.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://od.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://bw.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fm.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ea.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hx.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yd.hahajie.cn

[F11] 复制与移动文件
来源：http://xa.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cl.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oj.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vb.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ub.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cs.9csxet.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jd.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sc.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gu.9csxet.cn

[F12] CSV 读写
来源：http://io.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://io.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://it.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vr.haigaiapp.cn

TS:   // 同上
来源：http://hj.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ae.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nc.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://it.haigaiapp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gq.nicolike.cn

================================================================================
来源：http://mr.hahajie.cn

G. 面向对象
来源：http://ou.shtwfgs.cn

================================================================================
来源：http://uy.hnjuh.cn

[G01] 定义类
来源：http://am.hahajie.cn

Py:   class User: pass
来源：http://xs.haigaiapp.cn

PHP:  class User {}
来源：http://lm.yuexingan06.cn

JS:   class User {}
来源：http://zx.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://qr.jianghongdianzi.cn

Java: class User {}
来源：http://su.szxytkj.cn

Go:   type User struct { Name string }
来源：http://cc.shxzskj.cn

Ruby: class User; end
来源：http://al.huixinmuqiang.cn

C#:   class User {}
来源：http://hq.newstarts.cn

[G02] 构造函数
来源：http://ma.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://df.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://ei.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://yt.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ru.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://cm.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ho.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://cc.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://uf.hnjuh.cn

[G03] 实例属性
来源：http://ci.haigaiapp.cn

Py:   self.name = "x"
来源：http://du.newstarts.cn

PHP:  public string $name = "x";
来源：http://hx.szxytkj.cn

JS:   this.name = "x";
来源：http://rc.hahajie.cn

TS:   name: string = "x";
来源：http://sp.yuexingan06.cn

Java: private String name;
来源：http://bc.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vv.newstarts.cn

Ruby: @name = "x"
来源：http://dh.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://wz.jianghongdianzi.cn

[G04] 定义方法
来源：http://lm.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://ul.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vy.huanxung.cn

JS:   greet() { return this.name; }
来源：http://hm.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://rz.chemitech.net.cn

Java: String greet() { return name; }
来源：http://yl.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rb.huanxung.cn

Ruby: def greet; @name; end
来源：http://up.nicolike.cn

C#:   public string Greet() => Name;
来源：http://fc.yuexingan06.cn

[G05] 继承
来源：http://uz.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://qu.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://ga.521024.cn

JS:   class Admin extends User {}
来源：http://jj.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://sx.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ix.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ld.9csxet.cn

Ruby: class Admin < User; end
来源：http://zi.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://yf.asd995.cn

[G06] 重写方法
来源：http://of.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://hs.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xa.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://vo.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://tg.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ud.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qo.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://ev.yuntaijiaju.cn


<!-- 参考信息 -->