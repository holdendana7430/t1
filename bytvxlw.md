代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://os.chemitech.net.cn

TS:   s.split(",")
来源：http://ae.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ab.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xz.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://yj.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mo.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://dl.haigaiapp.cn

Py:   ",".join(items)
来源：http://rd.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://qe.gzmigu.cn

JS:   items.join(",")
来源：http://ke.jctech888.com.cn

TS:   items.join(",")
来源：http://jt.panjiajie.cn

Java: String.join(",", items)
来源：http://cz.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://am.gzmigu.cn

Ruby: items.join(",")
来源：http://kz.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://wg.nszjky.cn

[E09] 去除所有空白字符
来源：http://lo.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://al.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://to.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://hb.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://ub.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://ge.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eo.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xn.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://op.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ty.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mr.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bc.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://ti.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://wl.nicolike.cn

Java: String.format("%03d", 7)
来源：http://os.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qd.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mx.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ct.nszjky.cn

[E11] 反转字符串
来源：http://fz.colortex.cn

Py:   s[::-1]
来源：http://rj.jctech888.com.cn

PHP:  strrev($s);
来源：http://gq.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ub.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://xx.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vf.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qw.nszjky.cn

Ruby: s.reverse
来源：http://ya.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ab.nszjky.cn

[E12] 统计某字符出现次数
来源：http://pt.wgjwhj.cn

Py:   s.count("a")
来源：http://pv.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://uk.9csxet.cn

JS:   s.split("a").length - 1
来源：http://iu.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ou.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vm.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://jc.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://fj.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://ll.9csxet.cn

[E13] 逐字符遍历
来源：http://tz.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://mo.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xl.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ut.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wx.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gb.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cy.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://re.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gw.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://sd.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pe.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kj.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yz.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yl.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aj.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rq.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yl.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ob.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://tq.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xk.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://md.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zg.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://me.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yl.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eb.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wu.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uj.gzmigu.cn

[E16] 数字千分位
来源：http://sy.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://is.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://ck.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pt.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wt.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nz.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kq.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eq.colortex.cn

C#:   1234567.ToString("N0")
来源：http://zi.521024.cn

[E17] 首字母大写
来源：http://hr.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xr.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cf.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lb.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ue.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://te.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ts.nicolike.cn

Ruby: s.capitalize
来源：http://mk.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mx.szxytkj.cn

[E18] 模板占位符替换
来源：http://wj.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sl.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jl.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cn.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ht.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nj.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gp.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gw.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kw.colortex.cn

[E19] 多行文本按行拆分
来源：http://gw.panjiajie.cn

Py:   s.splitlines()
来源：http://ud.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yy.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://qo.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://xg.gzmigu.cn

Java: s.lines().toList()
来源：http://wi.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://yq.shxzukj.cn

Ruby: s.lines
来源：http://kz.yuexingan06.cn

C#:   s.Split('\n')
来源：http://uz.hahajie.cn

[E20] 判断字符串是否为空
来源：http://qs.yuexingan06.cn

Py:   if not s:
来源：http://gi.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ns.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ja.colortex.cn

TS:   if (s === "") {}
来源：http://ki.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://wu.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://nj.wgjwhj.cn

Ruby: if s.empty?
来源：http://sj.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mf.shxzskj.cn

[E21] 超长截断加省略号
来源：http://gj.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ko.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gv.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tc.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yz.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ej.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://iq.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hb.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aa.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://mu.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://an.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tt.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hb.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wk.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tk.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bf.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ha.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cb.nszjky.cn

================================================================================
来源：http://nv.panjiajie.cn

F. 文件与目录
来源：http://fr.jianghongdianzi.cn

================================================================================
来源：http://tg.chemitech.net.cn

[F01] 读取整个文件
来源：http://ie.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oj.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://hy.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dj.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yl.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cp.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wf.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://tk.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://vb.panjiajie.cn

[F02] 逐行读取文件
来源：http://ui.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ea.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qd.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://em.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ue.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lz.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uz.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ey.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qt.asd995.cn

[F03] 写入文件（覆盖）
来源：http://qv.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sh.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xz.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kr.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fq.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bg.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jf.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://ts.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://si.lnxyls.cn

[F04] 追加写入文件
来源：http://gx.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yn.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aj.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ie.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ns.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jb.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pk.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://km.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sa.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://xf.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://di.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://qr.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://kr.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://pk.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wv.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ew.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://nq.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://sc.panjiajie.cn

[F06] 删除文件
来源：http://im.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://lh.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://sl.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yw.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ej.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pq.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://lu.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://dm.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://ej.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://sm.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jo.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ix.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://an.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ad.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jo.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yy.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fy.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gz.yuexingan06.cn

[F08] 遍历目录
来源：http://qm.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xa.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dm.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://pr.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://rd.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zp.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tb.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://og.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://cz.panjiajie.cn

[F09] 获取文件大小
来源：http://vi.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://aa.newstarts.cn

PHP:  filesize("a.txt");
来源：http://wc.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://lr.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://lv.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sf.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ju.szsharing.cn

Ruby: File.size("a.txt")
来源：http://mf.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://ic.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://rn.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bm.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aq.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mi.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://wh.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yw.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ak.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tr.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kh.colortex.cn

[F11] 复制与移动文件
来源：http://jk.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vh.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cu.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://km.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wj.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ib.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lg.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yx.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yl.521024.cn

[F12] CSV 读写
来源：http://ad.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hj.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oo.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jh.yuexingan06.cn

TS:   // 同上
来源：http://ms.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fc.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ps.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vf.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nv.szxytkj.cn

================================================================================
来源：http://ge.huixiangedu.cn

G. 面向对象
来源：http://yu.colortex.cn

================================================================================
来源：http://cq.shxzukj.cn

[G01] 定义类
来源：http://pq.bookmarksfly.cn

Py:   class User: pass
来源：http://yv.panjiajie.cn

PHP:  class User {}
来源：http://xu.lnxyls.cn

JS:   class User {}
来源：http://hi.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://eb.gzmigu.cn

Java: class User {}
来源：http://bq.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://kz.asd995.cn

Ruby: class User; end
来源：http://vw.colortex.cn

C#:   class User {}
来源：http://gu.hahajie.cn

[G02] 构造函数
来源：http://ps.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://pf.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://ur.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://fu.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://kg.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://tz.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ic.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://ax.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://et.bookmarksfly.cn

[G03] 实例属性
来源：http://ah.shtwfgs.cn

Py:   self.name = "x"
来源：http://hk.colortex.cn

PHP:  public string $name = "x";
来源：http://xl.muxihuayi.cn

JS:   this.name = "x";
来源：http://iu.szxytkj.cn

TS:   name: string = "x";
来源：http://jx.szxytkj.cn

Java: private String name;
来源：http://hp.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ot.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://gp.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ry.haigaiapp.cn

[G04] 定义方法
来源：http://ny.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://qs.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pn.9csxet.cn

JS:   greet() { return this.name; }
来源：http://he.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://vo.huanxung.cn

Java: String greet() { return name; }
来源：http://nf.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vb.panjiajie.cn

Ruby: def greet; @name; end
来源：http://xk.newstarts.cn

C#:   public string Greet() => Name;
来源：http://pn.jctech888.com.cn

[G05] 继承
来源：http://th.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://jr.521024.cn

PHP:  class Admin extends User {}
来源：http://ew.521024.cn

JS:   class Admin extends User {}
来源：http://pa.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://zk.521024.cn

Java: class Admin extends User {}
来源：http://vy.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hp.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://fp.shxzukj.cn

C#:   class Admin : User {}
来源：http://cz.wgjwhj.cn


<!-- 参考信息 -->