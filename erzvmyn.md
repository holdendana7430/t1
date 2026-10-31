代发 wailian999

Ruby: s.split(",");  s.split
来源：http://uj.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sw.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://gu.9csxet.cn

Py:   ",".join(items)
来源：http://lu.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://wr.521024.cn

JS:   items.join(",")
来源：http://cw.nszjky.cn

TS:   items.join(",")
来源：http://sm.asd995.cn

Java: String.join(",", items)
来源：http://gt.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://wu.muxihuayi.cn

Ruby: items.join(",")
来源：http://ea.huanxung.cn

C#:   string.Join(",", items)
来源：http://mn.szxytkj.cn

[E09] 去除所有空白字符
来源：http://xk.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vu.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aw.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://mm.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ww.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://sk.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qp.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://by.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qg.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://cr.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cn.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zx.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://md.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://dd.nicolike.cn

Java: String.format("%03d", 7)
来源：http://of.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wx.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://le.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rz.chemitech.net.cn

[E11] 反转字符串
来源：http://hi.chemitech.net.cn

Py:   s[::-1]
来源：http://mr.nszjky.cn

PHP:  strrev($s);
来源：http://wm.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://oa.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://mq.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://at.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://va.lnxyls.cn

Ruby: s.reverse
来源：http://co.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wg.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://fa.gzmigu.cn

Py:   s.count("a")
来源：http://kb.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://kg.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://am.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://vr.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bx.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://rf.jctech888.com.cn

Ruby: s.count("a")
来源：http://hj.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://jq.9csxet.cn

[E13] 逐字符遍历
来源：http://jr.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://xd.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tj.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ka.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://es.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sk.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pw.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cm.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xx.huanxung.cn

[E14] URL 编码与 Base64
来源：http://or.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ao.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dq.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uj.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://my.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vm.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qs.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://es.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qf.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://ve.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dx.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ud.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ul.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://za.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://br.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xo.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ml.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://se.nszjky.cn

[E16] 数字千分位
来源：http://da.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://ph.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://lg.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jy.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ng.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zq.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fh.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fx.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://kf.panjiajie.cn

[E17] 首字母大写
来源：http://bn.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vo.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://he.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hs.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nb.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://av.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://as.panjiajie.cn

Ruby: s.capitalize
来源：http://os.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://id.panjiajie.cn

[E18] 模板占位符替换
来源：http://qs.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://je.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rm.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qt.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://by.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sy.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ax.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gs.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pc.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://ud.gzmigu.cn

Py:   s.splitlines()
来源：http://ak.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oi.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://hn.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://si.9csxet.cn

Java: s.lines().toList()
来源：http://dx.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://fq.bjjhwx.cn

Ruby: s.lines
来源：http://fy.chemitech.net.cn

C#:   s.Split('\n')
来源：http://yu.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://at.muxihuayi.cn

Py:   if not s:
来源：http://bz.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nr.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jo.haigaiapp.cn

TS:   if (s === "") {}
来源：http://vw.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://hy.shxzskj.cn

Go:   if s == "" {}
来源：http://oi.nicolike.cn

Ruby: if s.empty?
来源：http://wj.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dd.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://qd.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zz.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://np.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xg.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://br.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mp.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://xq.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uc.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dr.szsharing.cn

[E22] 字节长度与字符长度
来源：http://kx.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xo.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lv.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://te.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://az.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mi.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jp.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://qf.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kk.lnxyls.cn

================================================================================
来源：http://tq.yuexingan06.cn

F. 文件与目录
来源：http://zp.gzmigu.cn

================================================================================
来源：http://lk.newstarts.cn

[F01] 读取整个文件
来源：http://na.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yt.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://te.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vi.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gc.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hw.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lx.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://wn.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://ar.hahajie.cn

[F02] 逐行读取文件
来源：http://hk.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://so.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fx.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qm.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hk.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tj.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dz.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hm.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://es.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://hw.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fc.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sw.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ro.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bl.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tr.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xp.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://qz.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wv.yuexingan06.cn

[F04] 追加写入文件
来源：http://eb.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ys.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gn.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ro.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kz.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fw.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yr.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ou.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://fl.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sn.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://eg.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://rp.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://zi.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xa.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qo.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://mo.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://fy.muxihuayi.cn

[F06] 删除文件
来源：http://mw.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://nd.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://rk.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ek.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nf.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sj.asd995.cn

Go:   os.Remove("a.txt")
来源：http://wr.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://xk.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://ol.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://qh.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lr.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gh.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pv.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cu.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fq.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vw.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mt.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yp.jctech888.com.cn

[F08] 遍历目录
来源：http://zs.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qg.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uz.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://ob.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://hg.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iv.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kz.521024.cn

Ruby: Dir.children("dir")
来源：http://fo.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://gd.bjjhwx.cn

[F09] 获取文件大小
来源：http://yl.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://ke.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://jd.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://uc.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://rt.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ga.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ae.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://hn.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://xy.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://nf.jianghongdianzi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dq.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ai.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eu.szsharing.cn

TS:   path.extname("a.txt")
来源：http://bz.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rf.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://we.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eb.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tz.shxzukj.cn

[F11] 复制与移动文件
来源：http://mq.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wm.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bp.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yb.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://us.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wm.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sb.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tu.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ir.bjjhwx.cn

[F12] CSV 读写
来源：http://ty.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ep.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ot.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cv.colortex.cn

TS:   // 同上
来源：http://ua.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ci.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://li.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ka.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iv.9csxet.cn

================================================================================
来源：http://vj.9csxet.cn

G. 面向对象
来源：http://rb.asd995.cn

================================================================================
来源：http://rw.szsharing.cn

[G01] 定义类
来源：http://sw.9csxet.cn

Py:   class User: pass
来源：http://vg.gzmigu.cn

PHP:  class User {}
来源：http://vb.hahajie.cn

JS:   class User {}
来源：http://rp.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://hb.jianghongdianzi.cn

Java: class User {}
来源：http://fz.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://cp.bjjhwx.cn

Ruby: class User; end
来源：http://mk.521024.cn

C#:   class User {}
来源：http://ad.huixinmuqiang.cn

[G02] 构造函数
来源：http://zj.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://ri.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://td.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://zv.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://hl.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://bt.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ty.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://lc.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://hd.yuntaijiaju.cn

[G03] 实例属性
来源：http://om.wgjwhj.cn

Py:   self.name = "x"
来源：http://wy.asd995.cn

PHP:  public string $name = "x";
来源：http://il.hnjuh.cn

JS:   this.name = "x";
来源：http://ky.asd995.cn

TS:   name: string = "x";
来源：http://rn.chemitech.net.cn

Java: private String name;
来源：http://in.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vw.bookmarksfly.cn

Ruby: @name = "x"
来源：http://ha.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://kg.huixiangedu.cn

[G04] 定义方法
来源：http://mu.nicolike.cn

Py:   def greet(self): return self.name
来源：http://iu.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gq.huanxung.cn

JS:   greet() { return this.name; }
来源：http://kx.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://nt.muxihuayi.cn

Java: String greet() { return name; }
来源：http://cc.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://so.nicolike.cn

Ruby: def greet; @name; end
来源：http://qs.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://vi.yuntaijiaju.cn

[G05] 继承
来源：http://aw.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://bc.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://op.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://ci.huanxung.cn

TS:   class Admin extends User {}
来源：http://iw.nicolike.cn

Java: class Admin extends User {}
来源：http://wj.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tb.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://wi.gzmigu.cn

C#:   class Admin : User {}
来源：http://gu.szxytkj.cn

[G06] 重写方法
来源：http://kg.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://qe.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ho.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://ow.asd995.cn


<!-- 参考信息 -->