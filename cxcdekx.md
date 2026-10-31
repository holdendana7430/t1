代发 wailian999

================================================================================
来源：http://nk.hahajie.cn

E. 字符串处理
来源：http://ud.bjjhwx.cn

================================================================================
来源：http://xc.9csxet.cn

[E01] 拼接字符串
来源：http://pn.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://po.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lk.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://be.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bv.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lr.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ne.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://de.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nl.shtwfgs.cn

[E02] 重复字符串
来源：http://fj.jctech888.com.cn

Py:   "ab" * 3
来源：http://td.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://fs.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://gk.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://vf.hahajie.cn

Java: "ab".repeat(3)
来源：http://lm.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://uy.panjiajie.cn

Ruby: "ab" * 3
来源：http://ai.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ya.shxzukj.cn

[E03] 截取子串
来源：http://yx.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sp.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ss.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://al.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://dp.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://jz.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://er.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://et.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://do.hahajie.cn

[E04] 查找子串位置
来源：http://ik.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://je.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://nt.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qj.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://ko.hnjuh.cn

Java: s.indexOf("x")
来源：http://fg.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://xv.521024.cn

Ruby: s.index("x")
来源：http://yg.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://pw.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://er.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lg.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yi.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cz.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gx.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ik.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zv.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ii.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://on.bookmarksfly.cn

[E06] 替换子串
来源：http://bp.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wb.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://uu.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cg.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://de.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vk.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oz.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://at.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://lm.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://vo.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lo.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mo.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sz.yuntaijiaju.cn

TS:   s.split(",")
来源：http://hw.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://on.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zo.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://nu.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hd.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://ow.lnxyls.cn

Py:   ",".join(items)
来源：http://mw.newstarts.cn

PHP:  implode(",", $items);
来源：http://lh.haigaiapp.cn

JS:   items.join(",")
来源：http://pg.huixiangedu.cn

TS:   items.join(",")
来源：http://ew.szsharing.cn

Java: String.join(",", items)
来源：http://ca.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://yr.wgjwhj.cn

Ruby: items.join(",")
来源：http://ie.szxytkj.cn

C#:   string.Join(",", items)
来源：http://xk.colortex.cn

[E09] 去除所有空白字符
来源：http://kx.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zf.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ki.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://yp.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://yy.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://hd.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ag.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fu.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gu.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://jo.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cl.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pq.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://wx.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://ib.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://eo.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pw.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gl.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jw.szsharing.cn

[E11] 反转字符串
来源：http://xa.muxihuayi.cn

Py:   s[::-1]
来源：http://gz.jctech888.com.cn

PHP:  strrev($s);
来源：http://sy.asd995.cn

JS:   [...s].reverse().join("")
来源：http://pu.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://kn.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tp.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oj.haigaiapp.cn

Ruby: s.reverse
来源：http://bq.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dw.huanxung.cn

[E12] 统计某字符出现次数
来源：http://ss.9csxet.cn

Py:   s.count("a")
来源：http://wy.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://sl.newstarts.cn

JS:   s.split("a").length - 1
来源：http://ix.szsharing.cn

TS:   s.split("a").length - 1
来源：http://wy.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wv.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://st.bookmarksfly.cn

Ruby: s.count("a")
来源：http://wt.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://ri.newstarts.cn

[E13] 逐字符遍历
来源：http://zo.colortex.cn

Py:   for ch in s: print(ch)
来源：http://gv.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vv.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xb.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gq.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sf.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vq.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bq.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kj.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://zl.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xo.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yw.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fu.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ob.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ry.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sl.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://du.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kp.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://zw.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://su.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qm.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ei.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ji.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rs.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://al.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mh.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tq.yuexingan06.cn

[E16] 数字千分位
来源：http://ns.newstarts.cn

Py:   f"{1234567:,}"
来源：http://af.szxytkj.cn

PHP:  number_format(1234567);
来源：http://al.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ui.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ap.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ur.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cx.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gp.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://pe.shxzskj.cn

[E17] 首字母大写
来源：http://gb.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rh.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zk.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pk.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dj.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xz.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hw.huixiangedu.cn

Ruby: s.capitalize
来源：http://yz.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nn.shxzskj.cn

[E18] 模板占位符替换
来源：http://vd.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xs.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kd.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pp.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ef.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mn.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dl.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mx.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://im.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://bb.szxytkj.cn

Py:   s.splitlines()
来源：http://al.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://br.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://mc.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://vj.panjiajie.cn

Java: s.lines().toList()
来源：http://qs.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://ga.szxytkj.cn

Ruby: s.lines
来源：http://hf.nicolike.cn

C#:   s.Split('\n')
来源：http://fk.nszjky.cn

[E20] 判断字符串是否为空
来源：http://yi.huixiangedu.cn

Py:   if not s:
来源：http://lf.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://op.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ms.9csxet.cn

TS:   if (s === "") {}
来源：http://ym.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://qx.gzmigu.cn

Go:   if s == "" {}
来源：http://hn.nicolike.cn

Ruby: if s.empty?
来源：http://co.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ju.521024.cn

[E21] 超长截断加省略号
来源：http://ly.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nc.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ua.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gt.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gm.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oa.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://fv.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jr.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pe.colortex.cn

[E22] 字节长度与字符长度
来源：http://rm.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://za.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bz.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://da.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tt.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vz.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rk.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://ma.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uw.huixiangedu.cn

================================================================================
来源：http://tt.shxzskj.cn

F. 文件与目录
来源：http://fc.huixiangedu.cn

================================================================================
来源：http://ii.asd995.cn

[F01] 读取整个文件
来源：http://fb.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mv.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://bh.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ev.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sf.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rj.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jl.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://dj.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://ip.shtwfgs.cn

[F02] 逐行读取文件
来源：http://mi.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zd.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rk.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://il.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cf.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fq.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zb.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mv.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ah.521024.cn

[F03] 写入文件（覆盖）
来源：http://pl.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zg.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rm.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vp.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oq.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://av.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zt.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ck.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qw.shxzukj.cn

[F04] 追加写入文件
来源：http://vw.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oy.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ip.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tc.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ed.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://do.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://es.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ur.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dp.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://rw.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kf.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://od.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://ad.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://fm.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fb.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ze.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://oo.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://fb.asd995.cn

[F06] 删除文件
来源：http://ck.nszjky.cn

Py:   os.remove("a.txt")
来源：http://le.colortex.cn

PHP:  unlink("a.txt");
来源：http://dx.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ra.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tj.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oo.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://nl.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://xr.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://ka.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://xz.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://my.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hh.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ey.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ro.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rx.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vr.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kp.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://au.bjjhwx.cn

[F08] 遍历目录
来源：http://nx.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bv.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xs.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://dv.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://vl.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://my.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fz.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://vv.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ky.nicolike.cn

[F09] 获取文件大小
来源：http://pk.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://al.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://mn.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://lg.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://dc.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://su.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kc.colortex.cn

Ruby: File.size("a.txt")
来源：http://qq.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://jz.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://qk.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bx.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yb.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://me.huanxung.cn

TS:   path.extname("a.txt")
来源：http://yh.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ib.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sb.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fr.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bp.nszjky.cn

[F11] 复制与移动文件
来源：http://yl.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pe.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cy.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hl.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tu.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://my.szsharing.cn


<!-- 参考信息 -->