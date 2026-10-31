代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bk.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sj.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xm.9csxet.cn

[D26] 数组转字符串
来源：http://pn.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://tz.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://in.gzmigu.cn

JS:   arr.join(", ")
来源：http://os.lnxyls.cn

TS:   arr.join(", ")
来源：http://nh.bjjhwx.cn

Java: String.join(", ", list)
来源：http://tb.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://cl.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://vn.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://kq.newstarts.cn

================================================================================
来源：http://xz.szxytkj.cn

E. 字符串处理
来源：http://hp.521024.cn

================================================================================
来源：http://qx.9csxet.cn

[E01] 拼接字符串
来源：http://rc.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kg.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://la.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ze.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wi.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://np.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cv.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ff.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hw.panjiajie.cn

[E02] 重复字符串
来源：http://fh.newstarts.cn

Py:   "ab" * 3
来源：http://wy.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://nv.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://gt.521024.cn

TS:   "ab".repeat(3)
来源：http://xz.colortex.cn

Java: "ab".repeat(3)
来源：http://ti.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://bi.colortex.cn

Ruby: "ab" * 3
来源：http://zs.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xx.9csxet.cn

[E03] 截取子串
来源：http://tl.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hy.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rd.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ub.521024.cn

TS:   s.slice(1, 4)
来源：http://ly.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://bz.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xa.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ah.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://ca.panjiajie.cn

[E04] 查找子串位置
来源：http://lw.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://tf.9csxet.cn

PHP:  strpos($s, "x");
来源：http://nv.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://en.asd995.cn

TS:   s.indexOf("x")
来源：http://ls.szsharing.cn

Java: s.indexOf("x")
来源：http://yx.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://xi.hnjuh.cn

Ruby: s.index("x")
来源：http://nr.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://hg.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fa.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://td.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xq.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ty.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dv.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ee.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uf.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pp.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rr.szsharing.cn

[E06] 替换子串
来源：http://iz.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sa.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://hp.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wc.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://pg.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cl.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qv.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lc.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://yn.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://tk.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wq.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ow.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xu.wgjwhj.cn

TS:   s.split(",")
来源：http://ej.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sj.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pd.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://ip.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uw.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://kl.bookmarksfly.cn

Py:   ",".join(items)
来源：http://ef.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://su.szxytkj.cn

JS:   items.join(",")
来源：http://gn.szsharing.cn

TS:   items.join(",")
来源：http://oo.yuexingan06.cn

Java: String.join(",", items)
来源：http://ux.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ep.newstarts.cn

Ruby: items.join(",")
来源：http://fp.huanxung.cn

C#:   string.Join(",", items)
来源：http://gd.hahajie.cn

[E09] 去除所有空白字符
来源：http://ms.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://um.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ax.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://wq.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://bx.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://ph.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oy.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xz.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gc.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://rh.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zj.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dz.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://be.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://ay.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://mt.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rl.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jd.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kq.hahajie.cn

[E11] 反转字符串
来源：http://un.huanxung.cn

Py:   s[::-1]
来源：http://pz.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://iz.521024.cn

JS:   [...s].reverse().join("")
来源：http://on.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://qu.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pj.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sz.gzmigu.cn

Ruby: s.reverse
来源：http://xd.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xe.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://ao.huanxung.cn

Py:   s.count("a")
来源：http://gs.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://ha.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://kg.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://gs.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://na.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://rc.szxytkj.cn

Ruby: s.count("a")
来源：http://ei.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://ha.hnjuh.cn

[E13] 逐字符遍历
来源：http://vx.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://ud.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tt.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tv.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bz.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qs.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ec.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ts.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yx.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://ei.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pi.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ru.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tq.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vf.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aj.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wn.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vu.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xt.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://ns.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hx.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xf.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oe.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ii.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fe.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pu.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ql.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pe.muxihuayi.cn

[E16] 数字千分位
来源：http://ic.nszjky.cn

Py:   f"{1234567:,}"
来源：http://td.huanxung.cn

PHP:  number_format(1234567);
来源：http://wi.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wc.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lz.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tu.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jc.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://no.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://dg.bjjhwx.cn

[E17] 首字母大写
来源：http://vf.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ff.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dx.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kd.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wm.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qf.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zn.bjjhwx.cn

Ruby: s.capitalize
来源：http://ic.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mi.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://ey.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fh.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ge.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://en.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ff.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wr.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ig.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hc.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sz.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://fk.shxzukj.cn

Py:   s.splitlines()
来源：http://en.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wi.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://aq.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://bo.huanxung.cn

Java: s.lines().toList()
来源：http://ry.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://rc.shtwfgs.cn

Ruby: s.lines
来源：http://ud.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://nf.szsharing.cn

[E20] 判断字符串是否为空
来源：http://ja.huixiangedu.cn

Py:   if not s:
来源：http://ls.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vi.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cy.shtwfgs.cn

TS:   if (s === "") {}
来源：http://vi.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://mt.huanxung.cn

Go:   if s == "" {}
来源：http://jx.huanxung.cn

Ruby: if s.empty?
来源：http://nk.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://as.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://ld.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zg.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ju.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mu.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ad.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://px.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://uu.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gq.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tz.szsharing.cn

[E22] 字节长度与字符长度
来源：http://qr.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aj.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zn.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xv.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wa.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ay.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lt.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://sk.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wq.lnxyls.cn

================================================================================
来源：http://rw.hnjuh.cn

F. 文件与目录
来源：http://lr.gzmigu.cn

================================================================================
来源：http://vc.hnjuh.cn

[F01] 读取整个文件
来源：http://gq.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xz.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://bf.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pt.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xp.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bu.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ld.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://nn.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://hc.gzmigu.cn

[F02] 逐行读取文件
来源：http://fk.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ze.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dn.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wf.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gj.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lb.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ab.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://es.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mk.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://oo.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ug.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fc.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mr.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sl.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qm.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zd.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://sc.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sa.gzmigu.cn

[F04] 追加写入文件
来源：http://bu.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jp.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sb.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fa.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://op.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yu.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hm.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zy.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qm.521024.cn

[F05] 判断文件或目录是否存在
来源：http://mj.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://li.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://uy.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ih.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://ve.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://de.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ts.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://po.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://tb.colortex.cn

[F06] 删除文件
来源：http://mi.9csxet.cn

Py:   os.remove("a.txt")
来源：http://lz.nicolike.cn

PHP:  unlink("a.txt");
来源：http://rc.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xk.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ig.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yc.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://gz.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://wm.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://xt.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://uc.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qz.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sp.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tu.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uz.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oj.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gi.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tv.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bu.hahajie.cn

[F08] 遍历目录
来源：http://of.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ej.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rd.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://hg.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://zo.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fa.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://um.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://yq.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://cf.yuexingan06.cn

[F09] 获取文件大小
来源：http://vu.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://fo.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://wf.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://ob.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://qt.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ac.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gj.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://xk.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://ou.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://pi.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://na.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ft.jianghongdianzi.cn


<!-- 参考信息 -->