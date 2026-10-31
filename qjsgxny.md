代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://tc.asd995.cn

PHP:  implode(", ", $arr);
来源：http://bb.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://zk.gzmigu.cn

TS:   arr.join(", ")
来源：http://zw.521024.cn

Java: String.join(", ", list)
来源：http://su.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://wk.newstarts.cn

Ruby: arr.join(", ")
来源：http://rq.colortex.cn

C#:   string.Join(", ", list)
来源：http://xg.hnjuh.cn

================================================================================
来源：http://ng.521024.cn

E. 字符串处理
来源：http://mx.9csxet.cn

================================================================================
来源：http://tn.shxzukj.cn

[E01] 拼接字符串
来源：http://jm.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zq.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://me.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ma.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mx.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ex.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fk.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oo.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uk.haigaiapp.cn

[E02] 重复字符串
来源：http://ry.gzmigu.cn

Py:   "ab" * 3
来源：http://vk.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://kk.nszjky.cn

JS:   "ab".repeat(3)
来源：http://eq.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://vd.shxzskj.cn

Java: "ab".repeat(3)
来源：http://xs.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://xa.chemitech.net.cn

Ruby: "ab" * 3
来源：http://nt.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pf.panjiajie.cn

[E03] 截取子串
来源：http://vu.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qr.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://im.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ge.shxzskj.cn

TS:   s.slice(1, 4)
来源：http://hr.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://lc.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xy.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tk.colortex.cn

C#:   s.Substring(1, 3)
来源：http://je.huixiangedu.cn

[E04] 查找子串位置
来源：http://sg.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://xp.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://qi.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://di.nszjky.cn

TS:   s.indexOf("x")
来源：http://fn.gzmigu.cn

Java: s.indexOf("x")
来源：http://ds.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://ns.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ih.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://ep.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zn.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rw.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cc.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mf.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xq.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vg.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xp.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oc.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hu.jianghongdianzi.cn

[E06] 替换子串
来源：http://ty.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mr.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://pg.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kc.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://xr.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ch.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://to.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dd.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://po.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://iw.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://da.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xd.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xy.9csxet.cn

TS:   s.split(",")
来源：http://no.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qh.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mn.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://py.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oi.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://ks.szsharing.cn

Py:   ",".join(items)
来源：http://ap.shxzskj.cn

PHP:  implode(",", $items);
来源：http://wn.bookmarksfly.cn

JS:   items.join(",")
来源：http://rj.jctech888.com.cn

TS:   items.join(",")
来源：http://lg.hnjuh.cn

Java: String.join(",", items)
来源：http://nb.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://tz.huixiangedu.cn

Ruby: items.join(",")
来源：http://jk.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://li.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ra.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://us.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lo.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://sz.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://qr.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://tl.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jm.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cg.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rv.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://mj.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://or.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vm.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://oz.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://hf.nicolike.cn

Java: String.format("%03d", 7)
来源：http://do.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vh.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ej.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lc.shtwfgs.cn

[E11] 反转字符串
来源：http://vl.shxzukj.cn

Py:   s[::-1]
来源：http://qe.nicolike.cn

PHP:  strrev($s);
来源：http://gr.asd995.cn

JS:   [...s].reverse().join("")
来源：http://qe.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://yt.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://in.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dy.muxihuayi.cn

Ruby: s.reverse
来源：http://bl.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sd.szsharing.cn

[E12] 统计某字符出现次数
来源：http://is.huanxung.cn

Py:   s.count("a")
来源：http://iy.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://ae.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://oh.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://ko.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tt.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://ce.newstarts.cn

Ruby: s.count("a")
来源：http://ux.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://sb.521024.cn

[E13] 逐字符遍历
来源：http://dz.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://lu.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cp.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ym.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aj.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gh.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sh.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xc.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zg.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://mi.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dk.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pm.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://py.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xe.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qe.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ax.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sj.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ut.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://op.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vt.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fc.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://an.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://be.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gj.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ib.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oh.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iy.muxihuayi.cn

[E16] 数字千分位
来源：http://uu.szsharing.cn

Py:   f"{1234567:,}"
来源：http://vw.shxzukj.cn

PHP:  number_format(1234567);
来源：http://bk.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cf.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fm.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wo.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gu.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ee.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://po.9csxet.cn

[E17] 首字母大写
来源：http://ci.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://um.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://re.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zd.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://au.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vs.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hf.shtwfgs.cn

Ruby: s.capitalize
来源：http://mi.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jd.wgjwhj.cn

[E18] 模板占位符替换
来源：http://rq.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jz.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sz.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ka.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kr.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bl.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://px.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hl.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pv.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://va.newstarts.cn

Py:   s.splitlines()
来源：http://yy.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nl.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://pv.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://ow.huixiangedu.cn

Java: s.lines().toList()
来源：http://im.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://qb.szxytkj.cn

Ruby: s.lines
来源：http://df.huanxung.cn

C#:   s.Split('\n')
来源：http://tw.nszjky.cn

[E20] 判断字符串是否为空
来源：http://nb.asd995.cn

Py:   if not s:
来源：http://oz.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://az.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://us.szxytkj.cn

TS:   if (s === "") {}
来源：http://an.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://nj.nicolike.cn

Go:   if s == "" {}
来源：http://lx.9csxet.cn

Ruby: if s.empty?
来源：http://ef.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rs.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://lq.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sj.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bg.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ik.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rj.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://be.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://us.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://is.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jl.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://io.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xk.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hl.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uc.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dy.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zy.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nx.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://ax.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ob.huixiangedu.cn

================================================================================
来源：http://wu.chemitech.net.cn

F. 文件与目录
来源：http://ns.gzmigu.cn

================================================================================
来源：http://nw.nicolike.cn

[F01] 读取整个文件
来源：http://ku.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qg.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://ga.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pn.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://il.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ps.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dg.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://gd.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://ec.hnjuh.cn

[F02] 逐行读取文件
来源：http://mh.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://na.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oj.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ay.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bp.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://my.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wd.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vx.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nq.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://qa.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vz.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qk.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vr.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://to.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://va.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eu.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://cb.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iu.9csxet.cn

[F04] 追加写入文件
来源：http://ai.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rc.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rw.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fh.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zr.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://il.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ls.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gu.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ea.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://ov.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uo.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://yz.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ex.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://po.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sx.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ph.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://le.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://mz.colortex.cn

[F06] 删除文件
来源：http://xi.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://bp.asd995.cn

PHP:  unlink("a.txt");
来源：http://dq.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yg.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xg.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qd.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://rd.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://dt.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://bh.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://ie.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qs.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ci.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ck.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dw.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uj.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eh.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iw.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zr.panjiajie.cn

[F08] 遍历目录
来源：http://nl.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kk.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kp.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://tk.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://ez.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sj.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://of.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://vv.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://tn.bookmarksfly.cn

[F09] 获取文件大小
来源：http://el.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://we.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://bu.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://xa.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://sz.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bz.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ka.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://jk.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://bd.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://wd.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xg.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kc.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://te.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://sv.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cq.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hw.nicolike.cn


<!-- 参考信息 -->