代发 wailian999

Ruby: s.split(",");  s.split
来源：http://ig.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://an.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://zt.szsharing.cn

Py:   ",".join(items)
来源：http://kv.colortex.cn

PHP:  implode(",", $items);
来源：http://gr.nicolike.cn

JS:   items.join(",")
来源：http://vh.szxytkj.cn

TS:   items.join(",")
来源：http://bf.szxytkj.cn

Java: String.join(",", items)
来源：http://fe.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://ws.hahajie.cn

Ruby: items.join(",")
来源：http://hd.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ay.9csxet.cn

[E09] 去除所有空白字符
来源：http://xy.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ss.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rq.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://xf.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ot.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://cv.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dw.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nk.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cm.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://jf.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ij.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qd.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://jk.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://wb.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://mv.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://td.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://op.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fj.nszjky.cn

[E11] 反转字符串
来源：http://iq.newstarts.cn

Py:   s[::-1]
来源：http://nc.wgjwhj.cn

PHP:  strrev($s);
来源：http://vc.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://jd.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://hp.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lp.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pz.panjiajie.cn

Ruby: s.reverse
来源：http://fe.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dt.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://gm.hahajie.cn

Py:   s.count("a")
来源：http://os.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://wt.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://me.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://wy.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lt.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://fe.bjjhwx.cn

Ruby: s.count("a")
来源：http://fw.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://uj.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://wp.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://xg.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dm.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xg.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kk.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xr.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://th.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rv.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fe.nszjky.cn

[E14] URL 编码与 Base64
来源：http://tr.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vq.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bc.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ms.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cd.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gu.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ff.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ed.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cf.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://gu.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ic.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pb.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rf.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ye.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://au.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jo.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xi.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zg.yuntaijiaju.cn

[E16] 数字千分位
来源：http://qs.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://do.shxzukj.cn

PHP:  number_format(1234567);
来源：http://gm.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hl.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ds.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sf.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rh.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pa.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://or.panjiajie.cn

[E17] 首字母大写
来源：http://hh.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://id.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ub.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hj.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ox.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jg.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://va.jctech888.com.cn

Ruby: s.capitalize
来源：http://tz.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vz.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://hb.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sk.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aq.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sn.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bi.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vs.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eb.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kl.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://td.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://ro.haigaiapp.cn

Py:   s.splitlines()
来源：http://qx.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nb.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://vx.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://fb.nicolike.cn

Java: s.lines().toList()
来源：http://jx.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://cn.wgjwhj.cn

Ruby: s.lines
来源：http://tk.wgjwhj.cn

C#:   s.Split('\n')
来源：http://qd.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://bn.wgjwhj.cn

Py:   if not s:
来源：http://gv.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ie.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qc.haigaiapp.cn

TS:   if (s === "") {}
来源：http://fj.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://vg.huixiangedu.cn

Go:   if s == "" {}
来源：http://sa.szxytkj.cn

Ruby: if s.empty?
来源：http://bt.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sq.gzmigu.cn

[E21] 超长截断加省略号
来源：http://mc.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mr.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kq.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zx.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zg.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wb.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://tx.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sp.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ym.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://hg.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jl.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xp.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jq.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://im.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gj.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cj.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://bl.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uv.hnjuh.cn

================================================================================
来源：http://na.jianghongdianzi.cn

F. 文件与目录
来源：http://xx.hahajie.cn

================================================================================
来源：http://rh.huixiangedu.cn

[F01] 读取整个文件
来源：http://py.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jd.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://ga.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hs.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kn.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eh.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ze.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://ji.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://fj.9csxet.cn

[F02] 逐行读取文件
来源：http://ah.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rz.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kg.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lr.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://us.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iz.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wx.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jb.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://le.521024.cn

[F03] 写入文件（覆盖）
来源：http://me.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vy.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vz.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://az.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pe.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bb.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ds.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://if.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cs.hahajie.cn

[F04] 追加写入文件
来源：http://zd.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ex.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fn.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hj.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://df.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rs.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dp.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rv.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hs.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://wt.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rk.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://jj.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://zd.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://it.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dw.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dx.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://qg.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://as.hahajie.cn

[F06] 删除文件
来源：http://bt.hahajie.cn

Py:   os.remove("a.txt")
来源：http://lb.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://cm.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qt.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ya.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yw.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://vy.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://bs.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://ze.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://vz.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tz.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xv.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mu.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mx.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oh.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yr.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wu.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ls.haigaiapp.cn

[F08] 遍历目录
来源：http://nv.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fv.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dm.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://co.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ia.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tw.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://et.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://ko.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://lb.szxytkj.cn

[F09] 获取文件大小
来源：http://oh.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://rs.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://ui.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://qz.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://jm.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sb.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yu.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://vb.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://pi.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ug.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xx.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vb.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fb.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://di.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qy.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zq.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gu.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vw.nicolike.cn

[F11] 复制与移动文件
来源：http://py.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cv.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nx.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lu.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jd.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xf.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dv.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://by.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vf.hnjuh.cn

[F12] CSV 读写
来源：http://yj.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vw.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://de.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ra.shtwfgs.cn

TS:   // 同上
来源：http://vn.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yn.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fc.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dy.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wf.bjjhwx.cn

================================================================================
来源：http://jp.szxytkj.cn

G. 面向对象
来源：http://hv.shtwfgs.cn

================================================================================
来源：http://pc.nicolike.cn

[G01] 定义类
来源：http://qx.hahajie.cn

Py:   class User: pass
来源：http://ly.szxytkj.cn

PHP:  class User {}
来源：http://fa.haigaiapp.cn

JS:   class User {}
来源：http://vh.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://mq.lnxyls.cn

Java: class User {}
来源：http://vj.lnxyls.cn

Go:   type User struct { Name string }
来源：http://hi.521024.cn

Ruby: class User; end
来源：http://im.huanxung.cn

C#:   class User {}
来源：http://ps.bookmarksfly.cn

[G02] 构造函数
来源：http://rv.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://fk.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://ep.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://pc.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://oa.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://yp.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sm.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://hy.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://nm.hnjuh.cn

[G03] 实例属性
来源：http://qj.haigaiapp.cn

Py:   self.name = "x"
来源：http://jr.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://gq.9csxet.cn

JS:   this.name = "x";
来源：http://jl.nszjky.cn

TS:   name: string = "x";
来源：http://qk.chemitech.net.cn

Java: private String name;
来源：http://bj.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xd.shtwfgs.cn

Ruby: @name = "x"
来源：http://sq.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://im.yuexingan06.cn

[G04] 定义方法
来源：http://ip.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://kq.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ai.hahajie.cn

JS:   greet() { return this.name; }
来源：http://mi.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://md.gzmigu.cn

Java: String greet() { return name; }
来源：http://pf.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qt.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://dj.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://uw.hahajie.cn

[G05] 继承
来源：http://pg.nszjky.cn

Py:   class Admin(User): pass
来源：http://aa.521024.cn

PHP:  class Admin extends User {}
来源：http://um.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://zp.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://qd.yuexingan06.cn

Java: class Admin extends User {}
来源：http://fy.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dh.huanxung.cn

Ruby: class Admin < User; end
来源：http://vf.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://py.9csxet.cn

[G06] 重写方法
来源：http://yd.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://pe.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tx.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://db.nicolike.cn


<!-- 参考信息 -->