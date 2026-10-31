代发 wailian999

Ruby: s.split(",");  s.split
来源：http://tb.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ic.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://to.colortex.cn

Py:   ",".join(items)
来源：http://ar.szsharing.cn

PHP:  implode(",", $items);
来源：http://qm.muxihuayi.cn

JS:   items.join(",")
来源：http://jk.jianghongdianzi.cn

TS:   items.join(",")
来源：http://wu.shxzukj.cn

Java: String.join(",", items)
来源：http://rc.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://mg.bjjhwx.cn

Ruby: items.join(",")
来源：http://di.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://nz.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://bp.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mq.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mh.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://hm.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://ra.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://no.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iq.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cq.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ao.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://db.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kt.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ul.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://ul.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://my.huanxung.cn

Java: String.format("%03d", 7)
来源：http://kj.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mw.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lr.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://av.chemitech.net.cn

[E11] 反转字符串
来源：http://er.newstarts.cn

Py:   s[::-1]
来源：http://az.szxytkj.cn

PHP:  strrev($s);
来源：http://am.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://se.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://cn.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kt.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ao.bookmarksfly.cn

Ruby: s.reverse
来源：http://ce.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vh.nszjky.cn

[E12] 统计某字符出现次数
来源：http://qq.muxihuayi.cn

Py:   s.count("a")
来源：http://vr.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://en.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://gs.521024.cn

TS:   s.split("a").length - 1
来源：http://on.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kl.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://rh.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://va.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://jz.asd995.cn

[E13] 逐字符遍历
来源：http://gq.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://pp.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mh.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rr.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lz.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kf.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rf.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rm.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vt.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://dr.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lk.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kl.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ei.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ks.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://td.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jl.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bi.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ci.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://cn.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pl.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zh.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xw.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nv.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jj.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://td.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sv.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dk.chemitech.net.cn

[E16] 数字千分位
来源：http://wv.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://jr.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://va.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wd.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iy.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yq.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ac.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zo.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://hi.huanxung.cn

[E17] 首字母大写
来源：http://fg.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ld.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dn.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ay.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wy.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://av.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://in.gzmigu.cn

Ruby: s.capitalize
来源：http://kd.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bt.szxytkj.cn

[E18] 模板占位符替换
来源：http://fp.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ys.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qg.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://en.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ay.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hi.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ez.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ze.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ne.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://lg.huanxung.cn

Py:   s.splitlines()
来源：http://sf.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kp.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://hr.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://xk.asd995.cn

Java: s.lines().toList()
来源：http://rt.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://ug.huixinmuqiang.cn

Ruby: s.lines
来源：http://re.asd995.cn

C#:   s.Split('\n')
来源：http://nm.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://jm.9csxet.cn

Py:   if not s:
来源：http://hj.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qm.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ee.bjjhwx.cn

TS:   if (s === "") {}
来源：http://sg.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://pp.panjiajie.cn

Go:   if s == "" {}
来源：http://on.newstarts.cn

Ruby: if s.empty?
来源：http://pt.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mp.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://uu.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zv.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lx.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bv.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yt.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gt.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://an.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rj.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fm.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://gk.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kf.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gy.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rb.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://od.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mz.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wa.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://ia.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lf.huixiangedu.cn

================================================================================
来源：http://pi.gzmigu.cn

F. 文件与目录
来源：http://vm.colortex.cn

================================================================================
来源：http://ce.yuexingan06.cn

[F01] 读取整个文件
来源：http://wo.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ts.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://ms.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jj.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ge.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lj.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gp.asd995.cn

Ruby: File.read("a.txt")
来源：http://op.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://ti.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://ln.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://th.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qh.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xh.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wz.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dw.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hl.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tq.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ks.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://rk.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ds.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vl.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sz.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ve.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ib.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ox.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://nw.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ed.hnjuh.cn

[F04] 追加写入文件
来源：http://lu.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mh.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ab.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cy.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://te.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bx.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jr.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zq.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gj.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://nk.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ds.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://qp.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://mi.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://az.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jt.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ow.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://vr.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://ah.chemitech.net.cn

[F06] 删除文件
来源：http://wa.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://bk.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://rg.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jg.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ai.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://br.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://qg.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://ou.521024.cn

C#:   File.Delete("a.txt");
来源：http://fx.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://qu.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fa.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ss.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zh.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jo.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://na.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eg.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ai.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fa.nicolike.cn

[F08] 遍历目录
来源：http://vv.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nn.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dd.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://fn.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://hn.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sh.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qo.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://hp.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://zm.colortex.cn

[F09] 获取文件大小
来源：http://nd.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://py.nszjky.cn

PHP:  filesize("a.txt");
来源：http://bc.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://fu.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://ae.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gc.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ux.szsharing.cn

Ruby: File.size("a.txt")
来源：http://nm.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://gq.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://hd.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kx.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vv.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zr.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://yk.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://um.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lx.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yo.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zb.panjiajie.cn

[F11] 复制与移动文件
来源：http://br.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sv.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bo.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ai.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ro.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ra.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zn.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pj.jianghongdianzi.cn

[F12] CSV 读写
来源：http://bx.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hm.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://at.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gt.shxzskj.cn

TS:   // 同上
来源：http://td.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mz.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fo.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nm.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fg.bjjhwx.cn

================================================================================
来源：http://we.nicolike.cn

G. 面向对象
来源：http://qp.panjiajie.cn

================================================================================
来源：http://od.bjjhwx.cn

[G01] 定义类
来源：http://ew.521024.cn

Py:   class User: pass
来源：http://fz.huanxung.cn

PHP:  class User {}
来源：http://zc.panjiajie.cn

JS:   class User {}
来源：http://mr.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://ze.hahajie.cn

Java: class User {}
来源：http://kv.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://nv.shxzukj.cn

Ruby: class User; end
来源：http://nz.panjiajie.cn

C#:   class User {}
来源：http://ts.panjiajie.cn

[G02] 构造函数
来源：http://dt.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://ox.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://sr.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://tz.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://sb.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://nr.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cl.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://jc.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://sl.hahajie.cn

[G03] 实例属性
来源：http://mj.gzmigu.cn

Py:   self.name = "x"
来源：http://mm.huanxung.cn

PHP:  public string $name = "x";
来源：http://gx.wgjwhj.cn

JS:   this.name = "x";
来源：http://iz.chemitech.net.cn

TS:   name: string = "x";
来源：http://pw.hnjuh.cn

Java: private String name;
来源：http://nz.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yu.muxihuayi.cn

Ruby: @name = "x"
来源：http://dx.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://bw.muxihuayi.cn

[G04] 定义方法
来源：http://jo.hahajie.cn

Py:   def greet(self): return self.name
来源：http://xv.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ny.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://hc.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://pl.huanxung.cn

Java: String greet() { return name; }
来源：http://lb.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yf.hnjuh.cn

Ruby: def greet; @name; end
来源：http://fv.asd995.cn

C#:   public string Greet() => Name;
来源：http://px.lnxyls.cn

[G05] 继承
来源：http://fq.szxytkj.cn

Py:   class Admin(User): pass
来源：http://pr.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://qi.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://uh.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://gg.wgjwhj.cn

Java: class Admin extends User {}
来源：http://uy.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dt.asd995.cn

Ruby: class Admin < User; end
来源：http://ro.yuexingan06.cn

C#:   class Admin : User {}
来源：http://od.shtwfgs.cn

[G06] 重写方法
来源：http://mj.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://cd.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oo.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://fb.chemitech.net.cn


<!-- 参考信息 -->