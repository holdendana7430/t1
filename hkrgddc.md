代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://op.huanxung.cn

TS:   s.split(",")
来源：http://hg.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://um.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pg.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://xi.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ms.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://ep.shxzukj.cn

Py:   ",".join(items)
来源：http://xo.colortex.cn

PHP:  implode(",", $items);
来源：http://yc.nicolike.cn

JS:   items.join(",")
来源：http://jc.panjiajie.cn

TS:   items.join(",")
来源：http://xf.nszjky.cn

Java: String.join(",", items)
来源：http://oj.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://sp.colortex.cn

Ruby: items.join(",")
来源：http://sv.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://so.9csxet.cn

[E09] 去除所有空白字符
来源：http://zn.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hb.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gk.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://kj.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://yq.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://oi.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qo.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kq.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gb.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://us.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yy.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jv.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://mq.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://rl.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://xq.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gt.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xz.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iw.szxytkj.cn

[E11] 反转字符串
来源：http://iw.hahajie.cn

Py:   s[::-1]
来源：http://lo.nszjky.cn

PHP:  strrev($s);
来源：http://qd.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://bb.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://cv.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hi.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fq.huanxung.cn

Ruby: s.reverse
来源：http://oo.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ds.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://bt.shtwfgs.cn

Py:   s.count("a")
来源：http://jo.huixiangedu.cn

PHP:  substr_count($s, "a");
来源：http://ia.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://vt.hahajie.cn

TS:   s.split("a").length - 1
来源：http://kt.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eu.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://ox.chemitech.net.cn

Ruby: s.count("a")
来源：http://ip.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://vt.asd995.cn

[E13] 逐字符遍历
来源：http://sk.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://xc.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nd.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fs.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://an.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://se.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pp.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eg.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bj.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://io.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://it.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ke.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jg.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://py.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ge.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dg.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rn.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://we.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://jy.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sw.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gs.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ml.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jt.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ud.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jt.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bk.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vp.jianghongdianzi.cn

[E16] 数字千分位
来源：http://od.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://ei.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://vz.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cl.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yg.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ih.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sx.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ib.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://sl.jctech888.com.cn

[E17] 首字母大写
来源：http://fv.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://su.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wk.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vw.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ij.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gg.huixiangedu.cn

Ruby: s.capitalize
来源：http://mo.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xj.newstarts.cn

[E18] 模板占位符替换
来源：http://tl.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xx.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ld.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jb.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gd.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://to.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ri.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wb.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ha.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://sl.chemitech.net.cn

Py:   s.splitlines()
来源：http://eb.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mr.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://rr.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://eh.lnxyls.cn

Java: s.lines().toList()
来源：http://zy.521024.cn

Go:   strings.Split(s, "\n")
来源：http://ou.wgjwhj.cn

Ruby: s.lines
来源：http://gc.panjiajie.cn

C#:   s.Split('\n')
来源：http://bc.newstarts.cn

[E20] 判断字符串是否为空
来源：http://lz.panjiajie.cn

Py:   if not s:
来源：http://sz.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mp.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pg.shtwfgs.cn

TS:   if (s === "") {}
来源：http://al.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://xe.colortex.cn

Go:   if s == "" {}
来源：http://dc.shtwfgs.cn

Ruby: if s.empty?
来源：http://zd.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ms.newstarts.cn

[E21] 超长截断加省略号
来源：http://vg.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bp.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tm.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ee.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tr.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nd.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://ql.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iv.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cb.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://zh.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://un.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ep.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qx.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fd.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bj.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cs.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://jw.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yk.szsharing.cn

================================================================================
来源：http://ix.jctech888.com.cn

F. 文件与目录
来源：http://ys.9csxet.cn

================================================================================
来源：http://pq.9csxet.cn

[F01] 读取整个文件
来源：http://zb.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cs.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://jq.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nh.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xu.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oh.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://so.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://bu.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://hy.wgjwhj.cn

[F02] 逐行读取文件
来源：http://hl.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kx.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bn.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://go.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://si.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ua.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nq.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gy.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xx.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://pu.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wp.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nd.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eb.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bn.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ov.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ap.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://sr.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oi.muxihuayi.cn

[F04] 追加写入文件
来源：http://bw.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yj.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ts.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iy.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qc.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cy.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ea.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://js.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wc.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://ad.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hd.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://jy.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://ie.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://xk.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://io.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iy.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://lg.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://up.muxihuayi.cn

[F06] 删除文件
来源：http://de.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://tu.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://ze.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wb.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vk.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gd.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://om.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://dq.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://si.szsharing.cn

[F07] 创建目录（含多级）
来源：http://uk.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mz.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rq.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://op.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://do.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zy.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ps.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wb.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gb.asd995.cn

[F08] 遍历目录
来源：http://no.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qp.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ug.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://ok.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://yn.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aj.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rv.huanxung.cn

Ruby: Dir.children("dir")
来源：http://tl.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://of.haigaiapp.cn

[F09] 获取文件大小
来源：http://vw.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://bx.szsharing.cn

PHP:  filesize("a.txt");
来源：http://en.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://rn.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://np.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mk.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zt.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://he.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://am.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://vf.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ft.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hm.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xr.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://pq.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bg.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nq.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tj.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oy.gzmigu.cn

[F11] 复制与移动文件
来源：http://sp.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vb.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pv.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pa.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://es.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oc.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zp.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rl.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sr.colortex.cn

[F12] CSV 读写
来源：http://ev.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zt.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ln.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://av.huixiangedu.cn

TS:   // 同上
来源：http://up.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mh.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ew.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lx.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ue.shtwfgs.cn

================================================================================
来源：http://bz.shxzskj.cn

G. 面向对象
来源：http://zq.jctech888.com.cn

================================================================================
来源：http://tb.shtwfgs.cn

[G01] 定义类
来源：http://ya.hnjuh.cn

Py:   class User: pass
来源：http://zd.newstarts.cn

PHP:  class User {}
来源：http://fh.hnjuh.cn

JS:   class User {}
来源：http://ok.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://at.shxzskj.cn

Java: class User {}
来源：http://zk.panjiajie.cn

Go:   type User struct { Name string }
来源：http://xb.asd995.cn

Ruby: class User; end
来源：http://dk.yuntaijiaju.cn

C#:   class User {}
来源：http://he.shtwfgs.cn

[G02] 构造函数
来源：http://qg.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://gk.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ej.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://kq.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://be.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://av.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ew.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://fx.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://hc.shxzukj.cn

[G03] 实例属性
来源：http://vz.lnxyls.cn

Py:   self.name = "x"
来源：http://kk.hahajie.cn

PHP:  public string $name = "x";
来源：http://ge.panjiajie.cn

JS:   this.name = "x";
来源：http://li.wgjwhj.cn

TS:   name: string = "x";
来源：http://lu.jianghongdianzi.cn

Java: private String name;
来源：http://zi.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://st.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://wq.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://en.szxytkj.cn

[G04] 定义方法
来源：http://bz.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://lo.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qc.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://dq.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://kr.colortex.cn

Java: String greet() { return name; }
来源：http://tw.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qy.lnxyls.cn

Ruby: def greet; @name; end
来源：http://di.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://qr.szsharing.cn

[G05] 继承
来源：http://yr.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://xv.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://fu.lnxyls.cn

JS:   class Admin extends User {}
来源：http://ur.panjiajie.cn

TS:   class Admin extends User {}
来源：http://pr.lnxyls.cn

Java: class Admin extends User {}
来源：http://ro.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ju.hahajie.cn

Ruby: class Admin < User; end
来源：http://xz.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://wo.gzmigu.cn


<!-- 参考信息 -->