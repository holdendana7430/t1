代发 wailian999

Ruby: s.split(",");  s.split
来源：http://pc.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qx.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://wz.bookmarksfly.cn

Py:   ",".join(items)
来源：http://do.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://zz.shxzukj.cn

JS:   items.join(",")
来源：http://ke.bjjhwx.cn

TS:   items.join(",")
来源：http://je.huanxung.cn

Java: String.join(",", items)
来源：http://jy.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://lb.szxytkj.cn

Ruby: items.join(",")
来源：http://kv.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://if.panjiajie.cn

[E09] 去除所有空白字符
来源：http://cj.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fz.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dt.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://qn.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://zg.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://lb.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ah.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://is.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://un.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://eb.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ca.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qs.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://ut.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ec.hahajie.cn

Java: String.format("%03d", 7)
来源：http://fw.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ho.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ks.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xt.shxzskj.cn

[E11] 反转字符串
来源：http://be.muxihuayi.cn

Py:   s[::-1]
来源：http://fq.jctech888.com.cn

PHP:  strrev($s);
来源：http://fl.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://tk.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://hw.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kt.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wx.jctech888.com.cn

Ruby: s.reverse
来源：http://ox.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://it.szsharing.cn

[E12] 统计某字符出现次数
来源：http://lv.huixiangedu.cn

Py:   s.count("a")
来源：http://zj.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://ox.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://ji.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://sj.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vh.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://zl.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://ri.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://uy.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://qj.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://ew.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sc.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vi.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zo.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://db.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vw.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jf.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://re.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://wp.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xs.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ju.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yp.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://km.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ep.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hu.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bd.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rg.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://qw.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dn.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pl.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cz.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://de.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wu.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ai.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zo.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zs.bjjhwx.cn

[E16] 数字千分位
来源：http://pn.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://ab.newstarts.cn

PHP:  number_format(1234567);
来源：http://zm.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yj.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wa.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wt.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vl.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ad.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://sk.huixinmuqiang.cn

[E17] 首字母大写
来源：http://sd.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ns.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://al.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xs.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xr.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qq.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oi.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://ss.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ss.huixiangedu.cn

[E18] 模板占位符替换
来源：http://ap.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mr.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://we.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bu.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fy.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nk.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mg.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ds.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qh.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://wm.hnjuh.cn

Py:   s.splitlines()
来源：http://pc.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wz.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://bn.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://af.huixiangedu.cn

Java: s.lines().toList()
来源：http://vn.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://fp.huixiangedu.cn

Ruby: s.lines
来源：http://mq.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://zo.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://zy.jctech888.com.cn

Py:   if not s:
来源：http://rr.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xp.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ms.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://em.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://yi.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://mc.colortex.cn

Ruby: if s.empty?
来源：http://lz.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xq.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://vy.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dx.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pd.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ke.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hy.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://th.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://rs.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kq.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://av.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://eo.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hi.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kq.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sm.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://da.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jp.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ld.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://ku.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mz.yuexingan06.cn

================================================================================
来源：http://jd.lnxyls.cn

F. 文件与目录
来源：http://jp.huixinmuqiang.cn

================================================================================
来源：http://ml.shtwfgs.cn

[F01] 读取整个文件
来源：http://ty.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://an.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://uo.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dn.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ls.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cs.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vj.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://yf.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://es.newstarts.cn

[F02] 逐行读取文件
来源：http://hl.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gy.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bn.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fa.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ks.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sa.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sr.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gj.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xp.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://uz.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xu.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kq.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pa.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ze.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fk.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://it.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://sf.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ig.szsharing.cn

[F04] 追加写入文件
来源：http://ev.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gn.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ts.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qt.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://en.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cg.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wh.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cp.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mk.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://hd.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wc.colortex.cn

PHP:  file_exists("a.txt");
来源：http://lb.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://ay.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://vu.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cy.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yz.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://lw.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ox.muxihuayi.cn

[F06] 删除文件
来源：http://gm.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ni.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://yc.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ol.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wl.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wc.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ey.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://uq.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://ur.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://rl.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wv.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ts.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xk.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gp.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wd.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://co.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://em.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vg.nicolike.cn

[F08] 遍历目录
来源：http://yv.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uj.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tw.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://lb.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ry.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ap.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mp.nicolike.cn

Ruby: Dir.children("dir")
来源：http://jq.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://xw.hnjuh.cn

[F09] 获取文件大小
来源：http://wv.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://op.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://cm.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://sb.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://dk.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kf.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dw.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://sr.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://sk.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ml.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qv.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lj.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://el.newstarts.cn

TS:   path.extname("a.txt")
来源：http://kr.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rm.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ze.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bt.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cy.521024.cn

[F11] 复制与移动文件
来源：http://ao.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://us.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mh.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pw.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vz.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uc.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wu.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cs.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jr.bjjhwx.cn

[F12] CSV 读写
来源：http://wn.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yd.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ih.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vq.szxytkj.cn

TS:   // 同上
来源：http://js.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sx.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nk.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zm.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wf.chemitech.net.cn

================================================================================
来源：http://rp.gzmigu.cn

G. 面向对象
来源：http://mc.wgjwhj.cn

================================================================================
来源：http://ar.shxzukj.cn

[G01] 定义类
来源：http://ss.hahajie.cn

Py:   class User: pass
来源：http://pu.huixiangedu.cn

PHP:  class User {}
来源：http://tv.colortex.cn

JS:   class User {}
来源：http://bt.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://qy.huixinmuqiang.cn

Java: class User {}
来源：http://bg.colortex.cn

Go:   type User struct { Name string }
来源：http://wk.yuexingan06.cn

Ruby: class User; end
来源：http://mn.bookmarksfly.cn

C#:   class User {}
来源：http://jx.nszjky.cn

[G02] 构造函数
来源：http://tp.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://zw.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://wn.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://bo.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://qx.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://st.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rr.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://yu.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://ok.huixiangedu.cn

[G03] 实例属性
来源：http://vl.shxzskj.cn

Py:   self.name = "x"
来源：http://lj.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://yj.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://wm.bjjhwx.cn

TS:   name: string = "x";
来源：http://ai.huixiangedu.cn

Java: private String name;
来源：http://ne.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rx.newstarts.cn

Ruby: @name = "x"
来源：http://fw.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://qb.muxihuayi.cn

[G04] 定义方法
来源：http://db.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://ei.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kx.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://wb.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://yb.521024.cn

Java: String greet() { return name; }
来源：http://uf.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://al.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://sk.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://wc.haigaiapp.cn

[G05] 继承
来源：http://mx.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://eg.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://ed.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://at.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://st.muxihuayi.cn

Java: class Admin extends User {}
来源：http://te.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rf.huanxung.cn

Ruby: class Admin < User; end
来源：http://vm.chemitech.net.cn

C#:   class Admin : User {}
来源：http://qo.panjiajie.cn

[G06] 重写方法
来源：http://rm.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://vp.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eq.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://qc.yuntaijiaju.cn


<!-- 参考信息 -->