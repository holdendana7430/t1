代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yp.bookmarksfly.cn

[E03] 截取子串
来源：http://bt.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vx.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gr.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rp.521024.cn

TS:   s.slice(1, 4)
来源：http://so.hnjuh.cn

Java: s.substring(1, 4)
来源：http://st.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ja.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qn.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://ez.newstarts.cn

[E04] 查找子串位置
来源：http://xr.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://tx.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://nz.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hq.shxzskj.cn

TS:   s.indexOf("x")
来源：http://py.jctech888.com.cn

Java: s.indexOf("x")
来源：http://vo.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://px.szsharing.cn

Ruby: s.index("x")
来源：http://uf.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://vp.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yh.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rp.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://el.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bm.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vx.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ha.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iq.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ze.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kf.colortex.cn

[E06] 替换子串
来源：http://ba.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lt.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://nz.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yw.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://jx.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://je.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kx.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cw.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://pt.szxytkj.cn

[E07] 按分隔符拆分
来源：http://ue.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qf.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://im.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://be.lnxyls.cn

TS:   s.split(",")
来源：http://hs.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fm.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ja.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://de.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wc.521024.cn

[E08] 数组按分隔符合并
来源：http://tk.shxzskj.cn

Py:   ",".join(items)
来源：http://qq.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://qs.hnjuh.cn

JS:   items.join(",")
来源：http://wd.nicolike.cn

TS:   items.join(",")
来源：http://se.huixiangedu.cn

Java: String.join(",", items)
来源：http://qn.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ew.nszjky.cn

Ruby: items.join(",")
来源：http://dq.asd995.cn

C#:   string.Join(",", items)
来源：http://cd.newstarts.cn

[E09] 去除所有空白字符
来源：http://am.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pv.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://et.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://gn.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://gg.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://fg.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ni.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bz.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://up.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://ba.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hv.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cl.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://hs.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://hb.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://gn.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://za.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rs.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gt.9csxet.cn

[E11] 反转字符串
来源：http://jy.szsharing.cn

Py:   s[::-1]
来源：http://gq.szsharing.cn

PHP:  strrev($s);
来源：http://fj.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://oj.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://sb.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gf.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jj.shxzskj.cn

Ruby: s.reverse
来源：http://qh.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mb.nszjky.cn

[E12] 统计某字符出现次数
来源：http://uq.nicolike.cn

Py:   s.count("a")
来源：http://av.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://pq.colortex.cn

JS:   s.split("a").length - 1
来源：http://rj.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://ap.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fi.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://jp.szsharing.cn

Ruby: s.count("a")
来源：http://jo.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://nu.nicolike.cn

[E13] 逐字符遍历
来源：http://oe.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://mn.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jr.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xp.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yg.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mu.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sf.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qi.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rf.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://ed.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://at.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uy.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ut.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aq.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fw.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nx.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bk.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fb.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://yl.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uy.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qx.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://it.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pg.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lq.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jh.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gn.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yh.szxytkj.cn

[E16] 数字千分位
来源：http://kz.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://tf.hnjuh.cn

PHP:  number_format(1234567);
来源：http://fs.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ms.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ox.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rl.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://on.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ly.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://dz.muxihuayi.cn

[E17] 首字母大写
来源：http://ud.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dy.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qe.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lu.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ae.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ty.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yd.nszjky.cn

Ruby: s.capitalize
来源：http://qu.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ua.jctech888.com.cn

[E18] 模板占位符替换
来源：http://qu.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mn.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ec.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sx.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bd.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dv.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tm.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://st.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dz.asd995.cn

[E19] 多行文本按行拆分
来源：http://dg.huixiangedu.cn

Py:   s.splitlines()
来源：http://ts.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pp.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://wz.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://ih.shxzukj.cn

Java: s.lines().toList()
来源：http://nt.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://mm.huixiangedu.cn

Ruby: s.lines
来源：http://jk.shtwfgs.cn

C#:   s.Split('\n')
来源：http://sc.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://ry.jianghongdianzi.cn

Py:   if not s:
来源：http://we.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lp.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lr.gzmigu.cn

TS:   if (s === "") {}
来源：http://fm.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://zx.hahajie.cn

Go:   if s == "" {}
来源：http://st.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://lh.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tp.shxzskj.cn

[E21] 超长截断加省略号
来源：http://th.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wq.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://br.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ec.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nq.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bk.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://zm.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hj.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ml.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://rw.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xk.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lx.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://de.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yv.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wb.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bg.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://uc.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lj.szxytkj.cn

================================================================================
来源：http://iw.nicolike.cn

F. 文件与目录
来源：http://yn.huixinmuqiang.cn

================================================================================
来源：http://hc.asd995.cn

[F01] 读取整个文件
来源：http://qp.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hn.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://zr.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wc.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rw.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://we.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ot.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://nr.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://lw.haigaiapp.cn

[F02] 逐行读取文件
来源：http://hc.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cr.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://um.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fh.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ir.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mn.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://of.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://so.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tf.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://qo.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lr.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yr.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ea.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sd.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mu.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lv.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://sv.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ef.jctech888.com.cn

[F04] 追加写入文件
来源：http://mr.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wb.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tb.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ce.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://op.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ah.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://md.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zc.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://is.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://kc.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tw.colortex.cn

PHP:  file_exists("a.txt");
来源：http://ee.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://xf.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://ir.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vq.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lo.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ub.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://un.yuexingan06.cn

[F06] 删除文件
来源：http://nr.huanxung.cn

Py:   os.remove("a.txt")
来源：http://ps.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://wq.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vf.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bu.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bi.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://mw.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://ie.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://qs.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://uu.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bu.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yo.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nl.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gb.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ys.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ux.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hp.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kn.muxihuayi.cn

[F08] 遍历目录
来源：http://on.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ck.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hm.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://tn.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://mg.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qw.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bh.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://iv.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://fr.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://mc.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://ig.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://lg.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://gz.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://sy.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jl.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zy.colortex.cn

Ruby: File.size("a.txt")
来源：http://zm.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://gw.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://ms.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kl.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oz.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yc.hahajie.cn

TS:   path.extname("a.txt")
来源：http://as.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://em.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://or.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tq.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://en.muxihuayi.cn

[F11] 复制与移动文件
来源：http://cb.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cg.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gw.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vg.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zb.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uy.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xh.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yj.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gc.muxihuayi.cn

[F12] CSV 读写
来源：http://zh.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ag.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ug.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zu.521024.cn

TS:   // 同上
来源：http://bm.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://up.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jv.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://st.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pb.szxytkj.cn

================================================================================
来源：http://wl.shxzskj.cn

G. 面向对象
来源：http://zx.521024.cn

================================================================================
来源：http://cp.chemitech.net.cn

[G01] 定义类
来源：http://wo.asd995.cn

Py:   class User: pass
来源：http://mp.wgjwhj.cn

PHP:  class User {}
来源：http://xb.yuexingan06.cn

JS:   class User {}
来源：http://dq.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://lo.shxzskj.cn


<!-- 参考信息 -->