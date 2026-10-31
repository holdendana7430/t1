代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uz.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qb.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ea.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vr.huanxung.cn

[E02] 重复字符串
来源：http://kf.newstarts.cn

Py:   "ab" * 3
来源：http://oh.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://kk.newstarts.cn

JS:   "ab".repeat(3)
来源：http://pv.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://pw.gzmigu.cn

Java: "ab".repeat(3)
来源：http://zb.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://tz.9csxet.cn

Ruby: "ab" * 3
来源：http://fs.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kn.haigaiapp.cn

[E03] 截取子串
来源：http://jk.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pm.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lo.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://by.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://pz.szsharing.cn

Java: s.substring(1, 4)
来源：http://zy.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yo.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iv.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://ih.newstarts.cn

[E04] 查找子串位置
来源：http://ew.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://ih.newstarts.cn

PHP:  strpos($s, "x");
来源：http://oo.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wz.hahajie.cn

TS:   s.indexOf("x")
来源：http://km.hnjuh.cn

Java: s.indexOf("x")
来源：http://jl.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://mv.shxzukj.cn

Ruby: s.index("x")
来源：http://ht.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://gf.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ob.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oq.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ml.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cj.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rx.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oa.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ae.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mx.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hu.bjjhwx.cn

[E06] 替换子串
来源：http://vz.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bx.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://qj.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vy.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://eg.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qk.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vv.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qv.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://oy.asd995.cn

[E07] 按分隔符拆分
来源：http://dj.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ag.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cm.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ap.huixinmuqiang.cn

TS:   s.split(",")
来源：http://hj.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fk.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://li.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://cm.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dl.nicolike.cn

[E08] 数组按分隔符合并
来源：http://zq.hnjuh.cn

Py:   ",".join(items)
来源：http://os.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://js.muxihuayi.cn

JS:   items.join(",")
来源：http://cf.hnjuh.cn

TS:   items.join(",")
来源：http://nq.hnjuh.cn

Java: String.join(",", items)
来源：http://xf.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://el.lnxyls.cn

Ruby: items.join(",")
来源：http://by.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://wj.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ar.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://su.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mj.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://qp.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://wt.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://iu.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mo.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xw.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oo.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://vc.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bw.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tw.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://rh.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://xb.nszjky.cn

Java: String.format("%03d", 7)
来源：http://bf.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://od.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ws.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qq.wgjwhj.cn

[E11] 反转字符串
来源：http://cn.shxzukj.cn

Py:   s[::-1]
来源：http://hx.9csxet.cn

PHP:  strrev($s);
来源：http://ac.asd995.cn

JS:   [...s].reverse().join("")
来源：http://sp.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://iq.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wj.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vm.wgjwhj.cn

Ruby: s.reverse
来源：http://dp.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ea.huanxung.cn

[E12] 统计某字符出现次数
来源：http://hj.colortex.cn

Py:   s.count("a")
来源：http://ob.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://xw.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://uq.9csxet.cn

TS:   s.split("a").length - 1
来源：http://cx.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xk.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://li.9csxet.cn

Ruby: s.count("a")
来源：http://ux.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://jq.szsharing.cn

[E13] 逐字符遍历
来源：http://st.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://lt.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uf.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lo.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://an.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wv.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ce.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lj.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vq.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://nm.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mt.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mf.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mx.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vd.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lg.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gn.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://it.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nw.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://vx.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hj.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ik.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://je.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://is.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jn.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cz.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tp.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pj.panjiajie.cn

[E16] 数字千分位
来源：http://zb.nszjky.cn

Py:   f"{1234567:,}"
来源：http://qu.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://tb.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cq.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sc.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://by.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ea.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zs.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://op.yuntaijiaju.cn

[E17] 首字母大写
来源：http://cv.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wu.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nq.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gw.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zx.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rs.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zx.huanxung.cn

Ruby: s.capitalize
来源：http://eh.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fb.muxihuayi.cn

[E18] 模板占位符替换
来源：http://al.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cw.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fa.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rp.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jy.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ru.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pu.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xq.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ar.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://rm.panjiajie.cn

Py:   s.splitlines()
来源：http://ck.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uo.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://rn.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://gd.gzmigu.cn

Java: s.lines().toList()
来源：http://pg.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://hd.shxzskj.cn

Ruby: s.lines
来源：http://gv.huanxung.cn

C#:   s.Split('\n')
来源：http://dc.newstarts.cn

[E20] 判断字符串是否为空
来源：http://ia.huanxung.cn

Py:   if not s:
来源：http://vh.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xu.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bk.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://lb.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://vw.bookmarksfly.cn

Go:   if s == "" {}
来源：http://zb.yuexingan06.cn

Ruby: if s.empty?
来源：http://xp.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yv.asd995.cn

[E21] 超长截断加省略号
来源：http://be.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pj.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lv.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ov.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ct.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kv.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://hd.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qf.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qc.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://qy.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tm.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vu.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gn.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wn.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eg.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hq.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://fx.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mr.wgjwhj.cn

================================================================================
来源：http://et.bookmarksfly.cn

F. 文件与目录
来源：http://nb.lnxyls.cn

================================================================================
来源：http://ql.panjiajie.cn

[F01] 读取整个文件
来源：http://et.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rs.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://vu.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ih.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wd.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xf.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rf.nszjky.cn

Ruby: File.read("a.txt")
来源：http://px.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://jr.szxytkj.cn

[F02] 逐行读取文件
来源：http://bw.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ct.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wh.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wr.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ui.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dg.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hl.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dh.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mo.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://wn.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ne.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fa.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fz.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yc.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bj.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fl.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://mf.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://by.jctech888.com.cn

[F04] 追加写入文件
来源：http://qd.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ry.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://da.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://co.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://of.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lv.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ws.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vs.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yw.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://ci.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ux.521024.cn

PHP:  file_exists("a.txt");
来源：http://ss.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://me.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://id.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ah.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yk.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://bo.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://oe.panjiajie.cn

[F06] 删除文件
来源：http://jq.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://dy.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://dx.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yf.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sm.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xt.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://ms.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://jd.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://bf.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://qp.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qy.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tj.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://op.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://to.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wb.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://if.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iy.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dr.hahajie.cn

[F08] 遍历目录
来源：http://gz.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ez.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mf.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://xl.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://yr.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bt.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lu.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://nl.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://ek.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://ix.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://fn.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://ji.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://kb.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://ix.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ip.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ya.9csxet.cn

Ruby: File.size("a.txt")
来源：http://be.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://sr.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://jx.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cx.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cx.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://en.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://st.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cy.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ux.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iq.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ae.bjjhwx.cn

[F11] 复制与移动文件
来源：http://nl.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sr.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mt.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tq.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bh.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bz.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cd.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://or.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mz.chemitech.net.cn

[F12] CSV 读写
来源：http://xv.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ie.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eo.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gj.huixiangedu.cn

TS:   // 同上
来源：http://xa.gzmigu.cn


<!-- 参考信息 -->