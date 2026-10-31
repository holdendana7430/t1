代发 wailian999

PHP:  implode(",", $items);
来源：http://tk.szxytkj.cn

JS:   items.join(",")
来源：http://jn.szsharing.cn

TS:   items.join(",")
来源：http://jk.szxytkj.cn

Java: String.join(",", items)
来源：http://as.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://yl.muxihuayi.cn

Ruby: items.join(",")
来源：http://ce.nszjky.cn

C#:   string.Join(",", items)
来源：http://xl.asd995.cn

[E09] 去除所有空白字符
来源：http://yg.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xm.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ic.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://kr.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://bg.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://dp.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mj.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ub.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ge.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://jr.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://us.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zk.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://xb.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://qk.nszjky.cn

Java: String.format("%03d", 7)
来源：http://qc.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qc.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tu.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wt.gzmigu.cn

[E11] 反转字符串
来源：http://ef.huanxung.cn

Py:   s[::-1]
来源：http://cx.asd995.cn

PHP:  strrev($s);
来源：http://lg.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://dq.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://wu.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://za.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://im.yuexingan06.cn

Ruby: s.reverse
来源：http://cz.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lz.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://ry.asd995.cn

Py:   s.count("a")
来源：http://sx.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://zt.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://hz.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://hi.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qf.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://mh.shxzukj.cn

Ruby: s.count("a")
来源：http://kw.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ij.521024.cn

[E13] 逐字符遍历
来源：http://mg.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://vm.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://se.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bt.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hk.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pm.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ta.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vq.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ci.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://so.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gs.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yq.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gf.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ce.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vt.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dz.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ml.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hi.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://uw.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ql.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cy.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nr.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ck.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dh.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gn.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://or.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vv.huixinmuqiang.cn

[E16] 数字千分位
来源：http://ef.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://ea.hnjuh.cn

PHP:  number_format(1234567);
来源：http://pt.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tb.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bo.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ta.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xp.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pb.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://xu.muxihuayi.cn

[E17] 首字母大写
来源：http://cz.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cd.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ok.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://me.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rc.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pf.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qa.nicolike.cn

Ruby: s.capitalize
来源：http://su.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yd.wgjwhj.cn

[E18] 模板占位符替换
来源：http://cs.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wc.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ur.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oe.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pl.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vm.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ja.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ti.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://me.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://rd.yuexingan06.cn

Py:   s.splitlines()
来源：http://af.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pl.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://dl.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://mz.asd995.cn

Java: s.lines().toList()
来源：http://zd.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://zu.colortex.cn

Ruby: s.lines
来源：http://zt.chemitech.net.cn

C#:   s.Split('\n')
来源：http://vw.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://lk.9csxet.cn

Py:   if not s:
来源：http://oe.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vz.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xf.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://vz.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://kg.szxytkj.cn

Go:   if s == "" {}
来源：http://jd.chemitech.net.cn

Ruby: if s.empty?
来源：http://kg.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yx.shxzukj.cn

[E21] 超长截断加省略号
来源：http://vy.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tr.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zb.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uj.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xt.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fa.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://us.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jy.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eq.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://mo.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lm.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dj.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ia.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://of.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://do.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yu.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://xs.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uh.huixiangedu.cn

================================================================================
来源：http://xv.asd995.cn

F. 文件与目录
来源：http://bg.shxzskj.cn

================================================================================
来源：http://uq.bjjhwx.cn

[F01] 读取整个文件
来源：http://wa.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sa.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://ze.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ab.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vz.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cr.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hn.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://yp.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://dx.shxzskj.cn

[F02] 逐行读取文件
来源：http://to.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xz.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://al.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ps.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ki.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vz.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tf.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cw.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kj.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://hw.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cw.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rp.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gc.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ed.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sx.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bu.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://fc.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nq.lnxyls.cn

[F04] 追加写入文件
来源：http://oc.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wh.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vf.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ur.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kf.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uj.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wh.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mf.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ij.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://rk.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zw.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://mp.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://jk.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://kj.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ti.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nv.521024.cn

Ruby: File.exist?("a.txt")
来源：http://sa.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ki.hahajie.cn

[F06] 删除文件
来源：http://ss.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://um.szsharing.cn

PHP:  unlink("a.txt");
来源：http://vf.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://td.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cg.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wo.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://oy.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://vu.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://rb.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://oc.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jh.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://od.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sm.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fw.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ef.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pd.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gd.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pd.szsharing.cn

[F08] 遍历目录
来源：http://yc.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lw.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mp.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://yf.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://ra.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gg.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fb.nicolike.cn

Ruby: Dir.children("dir")
来源：http://sn.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://wf.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://eq.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://en.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://pc.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://pa.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://if.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qs.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oy.szsharing.cn

Ruby: File.size("a.txt")
来源：http://pq.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://pj.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://mc.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ig.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jz.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ob.9csxet.cn

TS:   path.extname("a.txt")
来源：http://wx.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lz.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uu.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ry.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jl.asd995.cn

[F11] 复制与移动文件
来源：http://uy.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pw.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dj.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ie.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zo.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eb.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dk.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fp.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ne.bookmarksfly.cn

[F12] CSV 读写
来源：http://pj.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oi.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sx.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://md.yuexingan06.cn

TS:   // 同上
来源：http://vi.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ax.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gt.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pu.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ug.muxihuayi.cn

================================================================================
来源：http://rd.nicolike.cn

G. 面向对象
来源：http://ka.bjjhwx.cn

================================================================================
来源：http://kw.yuntaijiaju.cn

[G01] 定义类
来源：http://qs.asd995.cn

Py:   class User: pass
来源：http://lo.haigaiapp.cn

PHP:  class User {}
来源：http://vs.panjiajie.cn

JS:   class User {}
来源：http://kt.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://mo.huixinmuqiang.cn

Java: class User {}
来源：http://vb.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://fu.yuntaijiaju.cn

Ruby: class User; end
来源：http://qs.bookmarksfly.cn

C#:   class User {}
来源：http://hp.huixiangedu.cn

[G02] 构造函数
来源：http://dt.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://an.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://fx.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://qj.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://vv.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://kf.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pj.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://dp.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://sn.hnjuh.cn

[G03] 实例属性
来源：http://ie.colortex.cn

Py:   self.name = "x"
来源：http://yt.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://wg.lnxyls.cn

JS:   this.name = "x";
来源：http://pv.asd995.cn

TS:   name: string = "x";
来源：http://qa.hnjuh.cn

Java: private String name;
来源：http://ke.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ts.huanxung.cn

Ruby: @name = "x"
来源：http://ir.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://te.jianghongdianzi.cn

[G04] 定义方法
来源：http://ry.szsharing.cn

Py:   def greet(self): return self.name
来源：http://re.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fi.szsharing.cn

JS:   greet() { return this.name; }
来源：http://fj.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ou.muxihuayi.cn

Java: String greet() { return name; }
来源：http://dd.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bd.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://su.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://tc.chemitech.net.cn

[G05] 继承
来源：http://ss.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://mw.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://kr.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://nf.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://ja.hnjuh.cn

Java: class Admin extends User {}
来源：http://os.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pl.asd995.cn

Ruby: class Admin < User; end
来源：http://zw.lnxyls.cn

C#:   class Admin : User {}
来源：http://kq.huixinmuqiang.cn

[G06] 重写方法
来源：http://rc.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://kn.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://in.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://oo.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://pb.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://jf.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vc.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://xh.huixinmuqiang.cn


<!-- 参考信息 -->