代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gs.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yf.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mt.521024.cn

[D26] 数组转字符串
来源：http://yp.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://cr.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://tv.hnjuh.cn

JS:   arr.join(", ")
来源：http://wa.lnxyls.cn

TS:   arr.join(", ")
来源：http://hx.colortex.cn

Java: String.join(", ", list)
来源：http://pf.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://ld.gzmigu.cn

Ruby: arr.join(", ")
来源：http://ub.szsharing.cn

C#:   string.Join(", ", list)
来源：http://ft.szsharing.cn

================================================================================
来源：http://tv.newstarts.cn

E. 字符串处理
来源：http://de.huanxung.cn

================================================================================
来源：http://ou.yuexingan06.cn

[E01] 拼接字符串
来源：http://hr.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://av.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lh.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://px.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bj.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gm.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bg.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xp.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rr.bjjhwx.cn

[E02] 重复字符串
来源：http://ri.newstarts.cn

Py:   "ab" * 3
来源：http://ju.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://ir.9csxet.cn

JS:   "ab".repeat(3)
来源：http://xh.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://lg.shxzukj.cn

Java: "ab".repeat(3)
来源：http://fv.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://oh.nszjky.cn

Ruby: "ab" * 3
来源：http://ru.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hr.gzmigu.cn

[E03] 截取子串
来源：http://nj.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ie.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xq.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yu.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://xd.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://in.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yj.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zi.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://yv.jctech888.com.cn

[E04] 查找子串位置
来源：http://ur.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://pg.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://rr.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bh.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://ka.521024.cn

Java: s.indexOf("x")
来源：http://ap.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://fp.huanxung.cn

Ruby: s.index("x")
来源：http://vn.asd995.cn

C#:   s.IndexOf("x")
来源：http://le.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lz.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ls.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://km.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xn.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://os.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yx.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sz.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jz.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uo.gzmigu.cn

[E06] 替换子串
来源：http://sk.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ks.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://fc.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ck.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://mp.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wp.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://se.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fk.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://pb.521024.cn

[E07] 按分隔符拆分
来源：http://en.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ok.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zg.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ve.chemitech.net.cn

TS:   s.split(",")
来源：http://un.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ys.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ei.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://re.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://of.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://qu.shxzskj.cn

Py:   ",".join(items)
来源：http://vc.nszjky.cn

PHP:  implode(",", $items);
来源：http://ez.521024.cn

JS:   items.join(",")
来源：http://nc.newstarts.cn

TS:   items.join(",")
来源：http://ys.szsharing.cn

Java: String.join(",", items)
来源：http://th.colortex.cn

Go:   strings.Join(items, ",")
来源：http://ce.nicolike.cn

Ruby: items.join(",")
来源：http://hp.shxzukj.cn

C#:   string.Join(",", items)
来源：http://xl.szxytkj.cn

[E09] 去除所有空白字符
来源：http://am.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ty.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eh.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://xu.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://yd.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://yu.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ml.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jn.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tc.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://cx.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lm.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tp.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://kt.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://pq.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://rx.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kn.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pt.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uf.shtwfgs.cn

[E11] 反转字符串
来源：http://es.huixinmuqiang.cn

Py:   s[::-1]
来源：http://qe.muxihuayi.cn

PHP:  strrev($s);
来源：http://vq.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://kg.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://kl.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cj.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ln.shxzskj.cn

Ruby: s.reverse
来源：http://jo.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lk.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://rq.shxzukj.cn

Py:   s.count("a")
来源：http://zf.colortex.cn

PHP:  substr_count($s, "a");
来源：http://ua.nicolike.cn

JS:   s.split("a").length - 1
来源：http://bg.9csxet.cn

TS:   s.split("a").length - 1
来源：http://dh.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yj.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://bz.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://ry.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://vf.wgjwhj.cn

[E13] 逐字符遍历
来源：http://mj.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://qf.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kx.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hv.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kc.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ty.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fd.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qs.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ux.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://tp.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ww.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pd.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hj.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ox.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mt.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ha.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mf.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jj.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ph.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lu.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ha.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sy.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ea.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ll.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fp.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tt.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zc.muxihuayi.cn

[E16] 数字千分位
来源：http://ok.colortex.cn

Py:   f"{1234567:,}"
来源：http://hc.hahajie.cn

PHP:  number_format(1234567);
来源：http://qo.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qo.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eq.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pd.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uh.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oc.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://wa.szxytkj.cn

[E17] 首字母大写
来源：http://do.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eh.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fd.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pe.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dq.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://af.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ox.huixiangedu.cn

Ruby: s.capitalize
来源：http://xb.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mo.hahajie.cn

[E18] 模板占位符替换
来源：http://oh.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vm.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ul.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ri.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sz.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wm.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oc.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hi.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uk.szsharing.cn

[E19] 多行文本按行拆分
来源：http://zn.nicolike.cn

Py:   s.splitlines()
来源：http://ab.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://st.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://vb.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://tn.521024.cn

Java: s.lines().toList()
来源：http://fk.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://is.wgjwhj.cn

Ruby: s.lines
来源：http://qa.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://gq.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://eu.nszjky.cn

Py:   if not s:
来源：http://sh.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qq.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xv.jctech888.com.cn

TS:   if (s === "") {}
来源：http://gl.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://rr.chemitech.net.cn

Go:   if s == "" {}
来源：http://oa.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://tv.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nf.huanxung.cn

[E21] 超长截断加省略号
来源：http://sg.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rj.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zo.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fm.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sh.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ob.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://qm.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yv.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ym.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://ud.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ch.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qn.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pe.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://em.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tj.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cs.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://zs.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dl.nszjky.cn

================================================================================
来源：http://dm.wgjwhj.cn

F. 文件与目录
来源：http://js.colortex.cn

================================================================================
来源：http://qs.wgjwhj.cn

[F01] 读取整个文件
来源：http://vb.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://co.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://bb.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gc.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qk.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zw.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oh.szsharing.cn

Ruby: File.read("a.txt")
来源：http://km.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://nu.wgjwhj.cn

[F02] 逐行读取文件
来源：http://km.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vt.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yy.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sv.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ug.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bm.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bg.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sm.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gg.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://cg.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gi.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nz.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ty.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fb.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zf.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zh.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://hs.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ga.gzmigu.cn

[F04] 追加写入文件
来源：http://lh.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cf.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pn.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://un.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mi.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fn.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://es.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yk.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hi.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://hw.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zm.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://bj.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://xo.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://ln.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ci.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ha.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://cs.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://jr.szxytkj.cn

[F06] 删除文件
来源：http://mj.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://al.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://yr.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nw.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mi.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dr.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://ih.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://me.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://ts.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://co.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ng.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://so.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uv.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kc.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aq.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cp.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ep.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tu.lnxyls.cn

[F08] 遍历目录
来源：http://xp.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://is.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lx.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://pe.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://ak.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zo.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ol.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://te.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://rf.shtwfgs.cn

[F09] 获取文件大小
来源：http://cw.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://hn.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://bi.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://ee.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://ze.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ur.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gr.asd995.cn

Ruby: File.size("a.txt")
来源：http://pg.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://an.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://aq.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ky.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ti.shxzukj.cn


<!-- 参考信息 -->