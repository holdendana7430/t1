代发 wailian999

C#:   s.Replace("a", "b")
来源：http://pr.nicolike.cn

[E07] 按分隔符拆分
来源：http://xi.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qt.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zb.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fe.9csxet.cn

TS:   s.split(",")
来源：http://ab.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cs.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tr.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://dd.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bf.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://wf.newstarts.cn

Py:   ",".join(items)
来源：http://wd.szsharing.cn

PHP:  implode(",", $items);
来源：http://ll.haigaiapp.cn

JS:   items.join(",")
来源：http://ve.521024.cn

TS:   items.join(",")
来源：http://ig.shxzukj.cn

Java: String.join(",", items)
来源：http://xs.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://tm.shxzskj.cn

Ruby: items.join(",")
来源：http://we.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://sq.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://vv.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vd.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gu.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://io.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://qq.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://hc.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fb.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uv.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wy.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://bo.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mu.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hc.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://kp.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://rg.szsharing.cn

Java: String.format("%03d", 7)
来源：http://uj.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wb.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dx.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oh.nszjky.cn

[E11] 反转字符串
来源：http://ir.jctech888.com.cn

Py:   s[::-1]
来源：http://nf.newstarts.cn

PHP:  strrev($s);
来源：http://lx.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://zl.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://rd.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ho.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zj.colortex.cn

Ruby: s.reverse
来源：http://do.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pa.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://tc.9csxet.cn

Py:   s.count("a")
来源：http://jk.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://rl.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://xb.huanxung.cn

TS:   s.split("a").length - 1
来源：http://yr.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mo.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://tz.szxytkj.cn

Ruby: s.count("a")
来源：http://yd.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://if.521024.cn

[E13] 逐字符遍历
来源：http://bu.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://ni.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tk.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ux.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nq.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xs.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pa.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://io.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hv.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://uw.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sl.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kr.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ka.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ag.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uh.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qc.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ju.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mx.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://dg.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ng.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ec.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kd.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sn.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://on.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sl.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ki.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wh.jianghongdianzi.cn

[E16] 数字千分位
来源：http://vy.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://ir.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://wn.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ta.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zr.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ys.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ju.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jh.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://dd.asd995.cn

[E17] 首字母大写
来源：http://lz.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yp.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ze.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ks.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eu.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gj.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://su.asd995.cn

Ruby: s.capitalize
来源：http://qb.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ep.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://em.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cl.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ds.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ky.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ku.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xc.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kn.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ds.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rl.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://ww.bjjhwx.cn

Py:   s.splitlines()
来源：http://ua.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ru.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://vv.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://aq.9csxet.cn

Java: s.lines().toList()
来源：http://ne.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://hp.muxihuayi.cn

Ruby: s.lines
来源：http://dt.shtwfgs.cn

C#:   s.Split('\n')
来源：http://pj.nicolike.cn

[E20] 判断字符串是否为空
来源：http://oz.hnjuh.cn

Py:   if not s:
来源：http://tm.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ni.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cf.gzmigu.cn

TS:   if (s === "") {}
来源：http://lq.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://gv.bjjhwx.cn

Go:   if s == "" {}
来源：http://yz.colortex.cn

Ruby: if s.empty?
来源：http://wt.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pl.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://zc.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rl.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rp.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gh.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yb.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sr.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://af.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dr.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cb.asd995.cn

[E22] 字节长度与字符长度
来源：http://cs.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dl.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ih.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nu.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ct.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://du.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qv.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://bk.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nb.szxytkj.cn

================================================================================
来源：http://su.szxytkj.cn

F. 文件与目录
来源：http://ba.lnxyls.cn

================================================================================
来源：http://gd.nszjky.cn

[F01] 读取整个文件
来源：http://lg.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://va.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://tp.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gn.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ub.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://if.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ka.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://xv.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://oe.lnxyls.cn

[F02] 逐行读取文件
来源：http://cs.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zh.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cx.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://by.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://co.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://th.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mp.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ws.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://im.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://st.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jf.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pm.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jq.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bc.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wr.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lc.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://tr.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oe.shxzukj.cn

[F04] 追加写入文件
来源：http://uq.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jf.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xn.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cb.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iz.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sf.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yh.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pj.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iz.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://fz.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ci.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://en.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://zk.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://jn.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://od.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cv.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ci.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://sa.haigaiapp.cn

[F06] 删除文件
来源：http://cs.asd995.cn

Py:   os.remove("a.txt")
来源：http://fm.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://jg.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wf.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://io.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nf.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://xi.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://fe.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://bl.521024.cn

[F07] 创建目录（含多级）
来源：http://uy.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jh.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bd.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ni.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yi.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ro.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fa.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dw.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jd.jianghongdianzi.cn

[F08] 遍历目录
来源：http://bk.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bs.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://js.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://wa.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ei.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qq.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wj.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://cn.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://mq.shtwfgs.cn

[F09] 获取文件大小
来源：http://qk.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://ol.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://bw.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://eu.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://ej.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hd.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qx.colortex.cn

Ruby: File.size("a.txt")
来源：http://fj.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://qk.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://eg.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kl.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wa.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://po.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://rf.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jq.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://so.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://df.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uw.muxihuayi.cn

[F11] 复制与移动文件
来源：http://oy.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lf.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lk.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://no.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fg.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wn.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lf.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ha.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gk.haigaiapp.cn

[F12] CSV 读写
来源：http://ab.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tl.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ru.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://er.huixinmuqiang.cn

TS:   // 同上
来源：http://kw.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zk.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lp.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rd.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gs.newstarts.cn

================================================================================
来源：http://xm.bookmarksfly.cn

G. 面向对象
来源：http://kv.huanxung.cn

================================================================================
来源：http://yq.jianghongdianzi.cn

[G01] 定义类
来源：http://lw.shxzukj.cn

Py:   class User: pass
来源：http://yf.chemitech.net.cn

PHP:  class User {}
来源：http://pw.9csxet.cn

JS:   class User {}
来源：http://au.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://ea.muxihuayi.cn

Java: class User {}
来源：http://al.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://hi.521024.cn

Ruby: class User; end
来源：http://lg.wgjwhj.cn

C#:   class User {}
来源：http://ao.shxzskj.cn

[G02] 构造函数
来源：http://eh.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://xo.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://dk.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://qo.colortex.cn

TS:   constructor(public name: string) {}
来源：http://pc.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://yj.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bv.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://bg.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://io.asd995.cn

[G03] 实例属性
来源：http://yi.521024.cn

Py:   self.name = "x"
来源：http://mi.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://zi.wgjwhj.cn

JS:   this.name = "x";
来源：http://sm.jctech888.com.cn

TS:   name: string = "x";
来源：http://lj.jianghongdianzi.cn

Java: private String name;
来源：http://hs.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sp.hahajie.cn

Ruby: @name = "x"
来源：http://he.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://js.muxihuayi.cn

[G04] 定义方法
来源：http://mh.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://ip.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vj.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://mm.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://ze.nicolike.cn

Java: String greet() { return name; }
来源：http://dc.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://it.nszjky.cn

Ruby: def greet; @name; end
来源：http://su.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://ag.gzmigu.cn

[G05] 继承
来源：http://gi.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://os.newstarts.cn

PHP:  class Admin extends User {}
来源：http://uy.521024.cn

JS:   class Admin extends User {}
来源：http://px.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://jt.asd995.cn


<!-- 参考信息 -->