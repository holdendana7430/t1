代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yl.haigaiapp.cn

[E03] 截取子串
来源：http://cr.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jr.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://db.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gz.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://ip.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://er.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jd.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sy.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://oy.szsharing.cn

[E04] 查找子串位置
来源：http://dc.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://jm.nicolike.cn

PHP:  strpos($s, "x");
来源：http://gb.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eo.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://tn.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://kx.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://pi.wgjwhj.cn

Ruby: s.index("x")
来源：http://hr.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://ik.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bz.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vp.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bs.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jr.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://st.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ut.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kl.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ez.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ou.hahajie.cn

[E06] 替换子串
来源：http://xk.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sh.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://ml.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mq.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://em.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xl.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cr.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ar.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://zr.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://aq.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uy.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aj.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ff.newstarts.cn

TS:   s.split(",")
来源：http://ly.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nm.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nz.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://tj.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aa.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://qt.colortex.cn

Py:   ",".join(items)
来源：http://lk.shxzukj.cn

PHP:  implode(",", $items);
来源：http://gm.asd995.cn

JS:   items.join(",")
来源：http://fi.haigaiapp.cn

TS:   items.join(",")
来源：http://oh.szxytkj.cn

Java: String.join(",", items)
来源：http://za.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://vq.jctech888.com.cn

Ruby: items.join(",")
来源：http://dy.hahajie.cn

C#:   string.Join(",", items)
来源：http://wp.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://yd.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://le.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cc.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://rs.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://jb.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://wy.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cg.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eq.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vu.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://kt.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cy.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://em.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://sn.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://fe.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://lj.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ey.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dd.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cv.chemitech.net.cn

[E11] 反转字符串
来源：http://sl.jctech888.com.cn

Py:   s[::-1]
来源：http://nt.hnjuh.cn

PHP:  strrev($s);
来源：http://gw.asd995.cn

JS:   [...s].reverse().join("")
来源：http://it.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://yc.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fo.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zo.huanxung.cn

Ruby: s.reverse
来源：http://mh.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hq.colortex.cn

[E12] 统计某字符出现次数
来源：http://ff.colortex.cn

Py:   s.count("a")
来源：http://us.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://ji.nicolike.cn

JS:   s.split("a").length - 1
来源：http://vk.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://hg.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iy.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://du.szxytkj.cn

Ruby: s.count("a")
来源：http://ip.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://er.huixiangedu.cn

[E13] 逐字符遍历
来源：http://hm.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://zr.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pq.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fy.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nq.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vc.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qz.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kd.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gm.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://ej.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uf.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wt.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iq.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ms.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qo.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gc.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dq.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rf.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://xt.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ew.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sh.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pc.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jt.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vu.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dr.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bh.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vl.colortex.cn

[E16] 数字千分位
来源：http://lv.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://fg.asd995.cn

PHP:  number_format(1234567);
来源：http://ug.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jg.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ft.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kk.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rx.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://su.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://bg.yuexingan06.cn

[E17] 首字母大写
来源：http://rq.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hh.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://te.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sc.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rl.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xr.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pv.bookmarksfly.cn

Ruby: s.capitalize
来源：http://kt.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cn.lnxyls.cn

[E18] 模板占位符替换
来源：http://te.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tw.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nm.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uk.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sf.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jv.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pl.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ro.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eh.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://tw.hahajie.cn

Py:   s.splitlines()
来源：http://qn.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ta.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://oo.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://dl.9csxet.cn

Java: s.lines().toList()
来源：http://vj.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://mm.huanxung.cn

Ruby: s.lines
来源：http://xq.shxzskj.cn

C#:   s.Split('\n')
来源：http://un.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://ko.gzmigu.cn

Py:   if not s:
来源：http://mu.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zy.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yl.panjiajie.cn

TS:   if (s === "") {}
来源：http://xf.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://my.colortex.cn

Go:   if s == "" {}
来源：http://pu.9csxet.cn

Ruby: if s.empty?
来源：http://qq.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jn.shxzskj.cn

[E21] 超长截断加省略号
来源：http://ua.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gr.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qo.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mt.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://md.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tr.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ld.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tq.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vo.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://rm.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fk.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mh.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zw.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rm.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uv.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wv.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://op.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bo.huixiangedu.cn

================================================================================
来源：http://wx.huixiangedu.cn

F. 文件与目录
来源：http://mm.jianghongdianzi.cn

================================================================================
来源：http://rp.newstarts.cn

[F01] 读取整个文件
来源：http://uz.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fc.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://bl.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ms.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xi.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ls.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://at.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://io.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://vo.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ba.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ml.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rl.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://on.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qm.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dd.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xp.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zp.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zw.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://bq.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://on.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rk.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zw.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://em.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ra.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fk.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://cz.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ru.huanxung.cn

[F04] 追加写入文件
来源：http://aq.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yo.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rl.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://id.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wv.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ba.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sa.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jh.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ma.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://px.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aq.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://de.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://ow.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://al.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jc.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://li.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://ca.colortex.cn

C#:   File.Exists("a.txt")
来源：http://pt.yuexingan06.cn

[F06] 删除文件
来源：http://vq.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://or.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://ht.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://co.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aw.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nt.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://ve.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://si.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://do.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://hw.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rw.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://th.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jy.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lx.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://km.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://py.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ty.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ro.521024.cn

[F08] 遍历目录
来源：http://uw.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ll.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jf.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://jm.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://oz.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qx.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pk.nicolike.cn

Ruby: Dir.children("dir")
来源：http://di.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://tg.szsharing.cn

[F09] 获取文件大小
来源：http://rx.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://ce.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://gm.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://yr.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://qe.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mf.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kf.huanxung.cn

Ruby: File.size("a.txt")
来源：http://qk.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://vl.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://qd.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ia.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dq.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://en.colortex.cn

TS:   path.extname("a.txt")
来源：http://qi.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://in.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pk.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://af.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bq.colortex.cn

[F11] 复制与移动文件
来源：http://lo.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kf.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ia.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pg.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ev.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ki.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tv.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://er.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hf.shxzskj.cn

[F12] CSV 读写
来源：http://tu.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ze.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gp.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eo.asd995.cn

TS:   // 同上
来源：http://vb.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tg.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ge.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bu.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wf.hnjuh.cn

================================================================================
来源：http://uw.chemitech.net.cn

G. 面向对象
来源：http://zm.hahajie.cn

================================================================================
来源：http://uw.521024.cn

[G01] 定义类
来源：http://kq.szxytkj.cn

Py:   class User: pass
来源：http://dp.gzmigu.cn

PHP:  class User {}
来源：http://vk.newstarts.cn

JS:   class User {}
来源：http://fa.521024.cn

TS:   class User { name: string = ""; }
来源：http://qo.lnxyls.cn


<!-- 参考信息 -->