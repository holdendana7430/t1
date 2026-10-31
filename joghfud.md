代发 wailian999

[E06] 替换子串
来源：http://fs.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ka.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://cp.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://og.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://df.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ro.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ba.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ut.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://wc.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://zw.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ov.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xx.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hc.hahajie.cn

TS:   s.split(",")
来源：http://or.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zz.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rw.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://uu.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cp.huanxung.cn

[E08] 数组按分隔符合并
来源：http://qb.shtwfgs.cn

Py:   ",".join(items)
来源：http://ux.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://gc.bookmarksfly.cn

JS:   items.join(",")
来源：http://un.yuntaijiaju.cn

TS:   items.join(",")
来源：http://cg.yuexingan06.cn

Java: String.join(",", items)
来源：http://sr.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://xq.szxytkj.cn

Ruby: items.join(",")
来源：http://hz.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://ts.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://an.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lr.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bx.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://yd.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://xx.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://sv.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ia.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rr.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vj.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://vb.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ko.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cu.521024.cn

JS:   "7".padStart(3, "0")
来源：http://nq.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://cw.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://eq.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tm.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bb.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ja.huixinmuqiang.cn

[E11] 反转字符串
来源：http://nr.newstarts.cn

Py:   s[::-1]
来源：http://yo.shxzskj.cn

PHP:  strrev($s);
来源：http://hb.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://nz.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://vp.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://re.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ib.yuntaijiaju.cn

Ruby: s.reverse
来源：http://zq.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nx.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://fz.haigaiapp.cn

Py:   s.count("a")
来源：http://zt.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://fs.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://ao.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://jw.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ja.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://dk.9csxet.cn

Ruby: s.count("a")
来源：http://ap.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://gn.wgjwhj.cn

[E13] 逐字符遍历
来源：http://nv.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://hq.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ac.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dk.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fe.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jm.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sq.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qm.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sb.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://jl.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jn.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fy.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://st.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hq.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mj.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://me.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xs.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wk.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://gw.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yp.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yn.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ug.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gi.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sr.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gq.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bf.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xh.521024.cn

[E16] 数字千分位
来源：http://xj.colortex.cn

Py:   f"{1234567:,}"
来源：http://ge.colortex.cn

PHP:  number_format(1234567);
来源：http://tc.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://za.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oi.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xj.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pk.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sw.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://qk.colortex.cn

[E17] 首字母大写
来源：http://jp.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://js.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://is.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://om.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wn.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wb.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hq.9csxet.cn

Ruby: s.capitalize
来源：http://er.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://np.chemitech.net.cn

[E18] 模板占位符替换
来源：http://dl.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mh.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zl.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wj.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qo.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ve.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mo.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://ii.9csxet.cn

Py:   s.splitlines()
来源：http://th.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nv.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://po.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://jx.huanxung.cn

Java: s.lines().toList()
来源：http://tf.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://gi.panjiajie.cn

Ruby: s.lines
来源：http://wx.gzmigu.cn

C#:   s.Split('\n')
来源：http://br.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://yk.huixiangedu.cn

Py:   if not s:
来源：http://lj.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hj.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gh.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://si.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://fd.muxihuayi.cn

Go:   if s == "" {}
来源：http://tu.9csxet.cn

Ruby: if s.empty?
来源：http://vq.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ag.szsharing.cn

[E21] 超长截断加省略号
来源：http://as.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tm.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ar.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zw.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ip.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://py.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://wf.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ac.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xp.szsharing.cn

[E22] 字节长度与字符长度
来源：http://pp.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nz.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qe.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uh.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fq.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ua.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zm.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://bn.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://da.colortex.cn

================================================================================
来源：http://fq.huixinmuqiang.cn

F. 文件与目录
来源：http://li.shxzskj.cn

================================================================================
来源：http://rm.shxzskj.cn

[F01] 读取整个文件
来源：http://em.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yo.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://la.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tn.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dy.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dg.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mx.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://pv.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://qz.shtwfgs.cn

[F02] 逐行读取文件
来源：http://hw.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ah.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ro.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rx.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xt.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ch.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jc.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ev.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jr.colortex.cn

[F03] 写入文件（覆盖）
来源：http://xj.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qf.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vk.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ej.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kx.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ng.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cv.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://xf.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ov.newstarts.cn

[F04] 追加写入文件
来源：http://uh.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://te.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cf.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hp.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gd.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bz.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mw.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ll.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uo.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://jn.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pu.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://jk.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://cv.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://ej.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yg.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kc.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://me.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://fi.yuntaijiaju.cn

[F06] 删除文件
来源：http://gu.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://kk.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://hb.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nd.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zv.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jt.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://pa.521024.cn

Ruby: File.delete("a.txt")
来源：http://or.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://ha.asd995.cn

[F07] 创建目录（含多级）
来源：http://uk.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rk.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xl.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://us.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jp.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cz.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ri.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jb.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wd.chemitech.net.cn

[F08] 遍历目录
来源：http://uc.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rm.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wh.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://fk.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://ia.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gi.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jv.521024.cn

Ruby: Dir.children("dir")
来源：http://if.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://tt.muxihuayi.cn

[F09] 获取文件大小
来源：http://za.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://rg.9csxet.cn

PHP:  filesize("a.txt");
来源：http://zj.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://po.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://gh.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ot.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gq.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://pe.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ib.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://zc.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fv.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ir.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lu.nszjky.cn

TS:   path.extname("a.txt")
来源：http://cj.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ss.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yp.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gr.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://db.haigaiapp.cn

[F11] 复制与移动文件
来源：http://cj.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yn.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://as.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wp.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mp.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kt.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://st.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ge.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tu.jianghongdianzi.cn

[F12] CSV 读写
来源：http://fx.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hh.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ap.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bg.bjjhwx.cn

TS:   // 同上
来源：http://sv.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vh.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cg.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ch.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://be.yuexingan06.cn

================================================================================
来源：http://pv.9csxet.cn

G. 面向对象
来源：http://nw.newstarts.cn

================================================================================
来源：http://eg.shxzukj.cn

[G01] 定义类
来源：http://xs.gzmigu.cn

Py:   class User: pass
来源：http://ae.521024.cn

PHP:  class User {}
来源：http://vs.panjiajie.cn

JS:   class User {}
来源：http://as.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://fw.lnxyls.cn

Java: class User {}
来源：http://hz.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://qc.yuntaijiaju.cn

Ruby: class User; end
来源：http://ho.jctech888.com.cn

C#:   class User {}
来源：http://cg.shxzskj.cn

[G02] 构造函数
来源：http://zg.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://of.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ic.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://zy.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://dy.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://fu.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xt.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://el.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://zr.lnxyls.cn

[G03] 实例属性
来源：http://um.bookmarksfly.cn

Py:   self.name = "x"
来源：http://fc.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://dx.521024.cn

JS:   this.name = "x";
来源：http://ko.panjiajie.cn

TS:   name: string = "x";
来源：http://dz.yuexingan06.cn

Java: private String name;
来源：http://gp.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ai.nszjky.cn

Ruby: @name = "x"
来源：http://wi.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ym.jianghongdianzi.cn

[G04] 定义方法
来源：http://ek.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://qz.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kp.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://lm.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://oz.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://hg.szxytkj.cn


<!-- 参考信息 -->