代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://lj.haigaiapp.cn

TS:   s.split(",")
来源：http://mp.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nt.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pk.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://jy.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wv.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://cq.hahajie.cn

Py:   ",".join(items)
来源：http://xb.shxzskj.cn

PHP:  implode(",", $items);
来源：http://xx.huixiangedu.cn

JS:   items.join(",")
来源：http://em.shtwfgs.cn

TS:   items.join(",")
来源：http://ad.9csxet.cn

Java: String.join(",", items)
来源：http://jn.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ln.chemitech.net.cn

Ruby: items.join(",")
来源：http://mr.colortex.cn

C#:   string.Join(",", items)
来源：http://rk.gzmigu.cn

[E09] 去除所有空白字符
来源：http://kw.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zk.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wm.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://ul.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ff.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://jl.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ik.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iw.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sd.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://vf.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gi.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rk.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://gx.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://lw.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://ik.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nb.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ah.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ms.shtwfgs.cn

[E11] 反转字符串
来源：http://vc.shtwfgs.cn

Py:   s[::-1]
来源：http://sc.asd995.cn

PHP:  strrev($s);
来源：http://mu.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://mo.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://sk.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ay.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vj.asd995.cn

Ruby: s.reverse
来源：http://hq.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iw.szsharing.cn

[E12] 统计某字符出现次数
来源：http://qb.jianghongdianzi.cn

Py:   s.count("a")
来源：http://dl.asd995.cn

PHP:  substr_count($s, "a");
来源：http://ta.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://ye.521024.cn

TS:   s.split("a").length - 1
来源：http://dx.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qj.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://jw.hnjuh.cn

Ruby: s.count("a")
来源：http://yo.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://bh.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://ru.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://kv.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yu.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zv.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jr.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mu.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pq.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gb.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gw.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://nf.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yi.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bj.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ll.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tm.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qa.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nq.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wu.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dq.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://jy.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qr.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zi.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://te.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nx.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cr.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ij.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pr.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://td.muxihuayi.cn

[E16] 数字千分位
来源：http://iw.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://rx.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://pi.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fl.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zi.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vo.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://td.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dq.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://uy.gzmigu.cn

[E17] 首字母大写
来源：http://db.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://he.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wa.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://an.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qz.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://om.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xv.gzmigu.cn

Ruby: s.capitalize
来源：http://ie.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gn.asd995.cn

[E18] 模板占位符替换
来源：http://po.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iw.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ec.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xe.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pb.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://za.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://on.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wd.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wo.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://xb.haigaiapp.cn

Py:   s.splitlines()
来源：http://zj.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ug.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://gh.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://eo.bookmarksfly.cn

Java: s.lines().toList()
来源：http://er.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://at.panjiajie.cn

Ruby: s.lines
来源：http://bi.lnxyls.cn

C#:   s.Split('\n')
来源：http://ez.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ps.colortex.cn

Py:   if not s:
来源：http://wq.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sf.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ac.colortex.cn

TS:   if (s === "") {}
来源：http://oo.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://aj.shxzukj.cn

Go:   if s == "" {}
来源：http://da.hnjuh.cn

Ruby: if s.empty?
来源：http://rh.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://az.huanxung.cn

[E21] 超长截断加省略号
来源：http://hf.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zp.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ws.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gk.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xj.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kv.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://wv.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cy.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://db.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://gy.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ja.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kn.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ay.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fw.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hx.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zv.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ye.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nt.newstarts.cn

================================================================================
来源：http://jr.asd995.cn

F. 文件与目录
来源：http://zp.9csxet.cn

================================================================================
来源：http://nf.szxytkj.cn

[F01] 读取整个文件
来源：http://ca.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vt.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://hc.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gx.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://we.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ac.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ai.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://dw.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://va.lnxyls.cn

[F02] 逐行读取文件
来源：http://je.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dr.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gy.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ug.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ly.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ne.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://or.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rd.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cr.colortex.cn

[F03] 写入文件（覆盖）
来源：http://bg.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ig.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qr.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yr.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fy.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mj.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qk.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://vo.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zt.9csxet.cn

[F04] 追加写入文件
来源：http://dy.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gz.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vz.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ou.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fh.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cv.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gg.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hy.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wx.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://aa.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fx.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://vg.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ho.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://xx.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://is.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cn.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://qd.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://rg.szsharing.cn

[F06] 删除文件
来源：http://uj.wgjwhj.cn

Py:   os.remove("a.txt")
来源：http://mc.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://ea.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gd.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gk.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dm.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://qs.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://rw.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://cz.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://fx.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://th.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jc.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xn.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vu.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zw.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lj.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jp.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://do.hnjuh.cn

[F08] 遍历目录
来源：http://ry.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mq.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lv.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://cw.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://dk.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xx.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nf.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://kg.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ad.colortex.cn

[F09] 获取文件大小
来源：http://ov.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://hz.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ik.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://fd.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://tx.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ln.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://en.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://vz.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://lo.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://jm.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yh.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pa.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gr.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ls.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zh.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mx.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ua.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nm.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://sz.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fy.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://up.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kz.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zl.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ig.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jk.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dq.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yb.bookmarksfly.cn

[F12] CSV 读写
来源：http://bs.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uh.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ik.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aq.shtwfgs.cn

TS:   // 同上
来源：http://ha.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gk.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://or.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jt.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kt.huixiangedu.cn

================================================================================
来源：http://hz.szsharing.cn

G. 面向对象
来源：http://mq.521024.cn

================================================================================
来源：http://nk.huixiangedu.cn

[G01] 定义类
来源：http://am.newstarts.cn

Py:   class User: pass
来源：http://tb.huixiangedu.cn

PHP:  class User {}
来源：http://vs.szsharing.cn

JS:   class User {}
来源：http://sd.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://lt.yuexingan06.cn

Java: class User {}
来源：http://bj.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://ab.bookmarksfly.cn

Ruby: class User; end
来源：http://nv.bjjhwx.cn

C#:   class User {}
来源：http://fz.bjjhwx.cn

[G02] 构造函数
来源：http://hi.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://st.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://fp.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://yr.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://td.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://uz.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://is.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://iq.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://ky.nicolike.cn

[G03] 实例属性
来源：http://lk.bjjhwx.cn

Py:   self.name = "x"
来源：http://eh.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://nw.nszjky.cn

JS:   this.name = "x";
来源：http://ne.colortex.cn

TS:   name: string = "x";
来源：http://fc.yuntaijiaju.cn

Java: private String name;
来源：http://ol.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cd.gzmigu.cn

Ruby: @name = "x"
来源：http://la.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ly.huixinmuqiang.cn

[G04] 定义方法
来源：http://ze.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://hj.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cv.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://yk.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://rx.jctech888.com.cn

Java: String greet() { return name; }
来源：http://bu.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ze.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://iv.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://fn.huixiangedu.cn

[G05] 继承
来源：http://nq.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://nt.szsharing.cn

PHP:  class Admin extends User {}
来源：http://ps.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://sr.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://xh.szxytkj.cn

Java: class Admin extends User {}
来源：http://hb.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kr.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://hg.nszjky.cn

C#:   class Admin : User {}
来源：http://tl.jctech888.com.cn


<!-- 参考信息 -->