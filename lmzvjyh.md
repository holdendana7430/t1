代发 wailian999

Ruby: s.split(",");  s.split
来源：http://ew.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ms.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://mq.9csxet.cn

Py:   ",".join(items)
来源：http://ff.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://br.bjjhwx.cn

JS:   items.join(",")
来源：http://xo.shxzskj.cn

TS:   items.join(",")
来源：http://mw.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://xp.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://nn.muxihuayi.cn

Ruby: items.join(",")
来源：http://kt.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://kw.huanxung.cn

[E09] 去除所有空白字符
来源：http://tv.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uh.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rp.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://gh.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://ok.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://ln.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zt.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kr.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pu.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://vw.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gm.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ik.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://wz.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ix.szsharing.cn

Java: String.format("%03d", 7)
来源：http://sv.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bc.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dw.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://io.shtwfgs.cn

[E11] 反转字符串
来源：http://lj.nszjky.cn

Py:   s[::-1]
来源：http://qb.newstarts.cn

PHP:  strrev($s);
来源：http://lc.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://do.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://dv.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sg.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jx.nszjky.cn

Ruby: s.reverse
来源：http://lv.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zj.newstarts.cn

[E12] 统计某字符出现次数
来源：http://xb.szxytkj.cn

Py:   s.count("a")
来源：http://co.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ca.nszjky.cn

JS:   s.split("a").length - 1
来源：http://zc.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://nl.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://be.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://cv.szsharing.cn

Ruby: s.count("a")
来源：http://xs.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://zv.szsharing.cn

[E13] 逐字符遍历
来源：http://aj.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://mk.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vm.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://py.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vx.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jo.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ra.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ld.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ng.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://vk.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cr.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rt.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kz.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eb.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ps.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ex.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gh.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ln.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://ki.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ss.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ft.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lv.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oi.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lc.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ow.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jd.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wx.asd995.cn

[E16] 数字千分位
来源：http://mg.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://mo.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://yj.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qq.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rm.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hp.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xt.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://km.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://kh.szxytkj.cn

[E17] 首字母大写
来源：http://ic.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://px.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tb.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://be.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://is.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://be.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pj.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://sm.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xt.shxzukj.cn

[E18] 模板占位符替换
来源：http://om.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ae.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mi.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://di.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sl.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wg.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fd.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ty.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cg.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://wb.bookmarksfly.cn

Py:   s.splitlines()
来源：http://ii.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oe.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://aj.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://qg.szsharing.cn

Java: s.lines().toList()
来源：http://yo.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://bq.huanxung.cn

Ruby: s.lines
来源：http://ue.nicolike.cn

C#:   s.Split('\n')
来源：http://az.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://sb.chemitech.net.cn

Py:   if not s:
来源：http://pr.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aw.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ht.nicolike.cn

TS:   if (s === "") {}
来源：http://qh.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://jx.chemitech.net.cn

Go:   if s == "" {}
来源：http://ga.bjjhwx.cn

Ruby: if s.empty?
来源：http://yz.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xl.shxzskj.cn

[E21] 超长截断加省略号
来源：http://jb.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://id.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bu.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mz.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wj.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xe.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://qi.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mx.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mv.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://yh.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uy.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nq.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://es.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hd.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ex.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://ds.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sc.panjiajie.cn

================================================================================
来源：http://tw.asd995.cn

F. 文件与目录
来源：http://lr.asd995.cn

================================================================================
来源：http://zm.huanxung.cn

[F01] 读取整个文件
来源：http://fl.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xp.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://zf.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yx.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dm.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tv.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kg.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://ul.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://es.asd995.cn

[F02] 逐行读取文件
来源：http://pp.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://px.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bd.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rp.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vv.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xb.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ij.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fk.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://da.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://hd.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gp.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ho.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ru.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hr.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jg.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zk.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://iz.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ly.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://gb.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cv.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hg.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bg.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pv.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://js.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tt.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yq.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ey.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://ml.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tp.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://nx.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://rw.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ri.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gj.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://em.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://uw.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://kq.hahajie.cn

[F06] 删除文件
来源：http://px.nicolike.cn

Py:   os.remove("a.txt")
来源：http://am.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://sr.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dd.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fu.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kj.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://dw.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://ot.colortex.cn

C#:   File.Delete("a.txt");
来源：http://dp.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://wk.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xn.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pl.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mz.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bx.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fv.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ay.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ru.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aw.bjjhwx.cn

[F08] 遍历目录
来源：http://zm.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hc.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wm.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://xq.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://pr.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eg.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ln.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ob.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://ey.bjjhwx.cn

[F09] 获取文件大小
来源：http://cl.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://uz.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://rx.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://ak.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://po.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cy.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pm.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://mn.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://cm.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ad.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ex.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cs.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ls.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://ix.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://et.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wh.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ce.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xn.hahajie.cn

[F11] 复制与移动文件
来源：http://rj.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oc.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ts.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qp.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ao.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zb.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vz.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cy.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nk.huixinmuqiang.cn

[F12] CSV 读写
来源：http://va.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mq.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qr.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ea.shxzskj.cn

TS:   // 同上
来源：http://rw.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wp.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qu.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://la.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kt.jianghongdianzi.cn

================================================================================
来源：http://jm.chemitech.net.cn

G. 面向对象
来源：http://nn.haigaiapp.cn

================================================================================
来源：http://ld.huanxung.cn

[G01] 定义类
来源：http://tf.hahajie.cn

Py:   class User: pass
来源：http://eq.wgjwhj.cn

PHP:  class User {}
来源：http://we.jctech888.com.cn

JS:   class User {}
来源：http://pz.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://yx.9csxet.cn

Java: class User {}
来源：http://ib.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://qq.haigaiapp.cn

Ruby: class User; end
来源：http://wa.9csxet.cn

C#:   class User {}
来源：http://rj.huixinmuqiang.cn

[G02] 构造函数
来源：http://ed.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://tq.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://wo.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://hs.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://es.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://eq.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xg.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://sl.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://na.huixiangedu.cn

[G03] 实例属性
来源：http://vh.muxihuayi.cn

Py:   self.name = "x"
来源：http://gg.nszjky.cn

PHP:  public string $name = "x";
来源：http://om.shxzukj.cn

JS:   this.name = "x";
来源：http://oq.szsharing.cn

TS:   name: string = "x";
来源：http://kq.jctech888.com.cn

Java: private String name;
来源：http://ch.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hk.newstarts.cn

Ruby: @name = "x"
来源：http://ap.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://nw.hahajie.cn

[G04] 定义方法
来源：http://xg.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://co.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kt.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://ww.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://bo.chemitech.net.cn

Java: String greet() { return name; }
来源：http://sg.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cs.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://ny.9csxet.cn

C#:   public string Greet() => Name;
来源：http://zi.bjjhwx.cn

[G05] 继承
来源：http://qm.panjiajie.cn

Py:   class Admin(User): pass
来源：http://bi.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://ad.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://jw.nicolike.cn

TS:   class Admin extends User {}
来源：http://tc.muxihuayi.cn

Java: class Admin extends User {}
来源：http://qi.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hx.9csxet.cn

Ruby: class Admin < User; end
来源：http://tu.gzmigu.cn

C#:   class Admin : User {}
来源：http://dx.huixiangedu.cn

[G06] 重写方法
来源：http://km.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://sp.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://om.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://uw.newstarts.cn


<!-- 参考信息 -->