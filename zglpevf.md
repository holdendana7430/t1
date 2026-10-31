代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jk.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zf.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://en.panjiajie.cn

[D26] 数组转字符串
来源：http://pw.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://qx.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://pa.huanxung.cn

JS:   arr.join(", ")
来源：http://xq.bjjhwx.cn

TS:   arr.join(", ")
来源：http://hg.szxytkj.cn

Java: String.join(", ", list)
来源：http://vz.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://if.gzmigu.cn

Ruby: arr.join(", ")
来源：http://hg.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://nw.jianghongdianzi.cn

================================================================================
来源：http://uk.panjiajie.cn

E. 字符串处理
来源：http://ft.nicolike.cn

================================================================================
来源：http://qi.bookmarksfly.cn

[E01] 拼接字符串
来源：http://jt.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ya.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://po.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nv.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vv.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://en.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pl.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://du.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bw.chemitech.net.cn

[E02] 重复字符串
来源：http://mo.szxytkj.cn

Py:   "ab" * 3
来源：http://ej.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://dj.nszjky.cn

JS:   "ab".repeat(3)
来源：http://xi.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://rb.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://dv.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://tp.hahajie.cn

Ruby: "ab" * 3
来源：http://da.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ej.gzmigu.cn

[E03] 截取子串
来源：http://iz.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tw.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uf.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://me.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://ma.gzmigu.cn

Java: s.substring(1, 4)
来源：http://fl.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lb.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ym.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://sd.jctech888.com.cn

[E04] 查找子串位置
来源：http://tu.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://rc.hahajie.cn

PHP:  strpos($s, "x");
来源：http://wx.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wr.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://sb.shtwfgs.cn

Java: s.indexOf("x")
来源：http://tt.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://zu.lnxyls.cn

Ruby: s.index("x")
来源：http://lj.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://qw.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://di.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mn.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lw.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uv.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kt.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ks.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ax.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pz.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tv.huixinmuqiang.cn

[E06] 替换子串
来源：http://em.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ve.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://zu.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uh.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://qf.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sz.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://in.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ta.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://rr.szxytkj.cn

[E07] 按分隔符拆分
来源：http://rl.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nh.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ek.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ze.shtwfgs.cn

TS:   s.split(",")
来源：http://hx.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dl.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sp.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://av.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jp.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://ai.panjiajie.cn

Py:   ",".join(items)
来源：http://mc.hahajie.cn

PHP:  implode(",", $items);
来源：http://sq.gzmigu.cn

JS:   items.join(",")
来源：http://tk.shtwfgs.cn

TS:   items.join(",")
来源：http://of.asd995.cn

Java: String.join(",", items)
来源：http://cd.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://qk.huanxung.cn

Ruby: items.join(",")
来源：http://iw.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://ll.panjiajie.cn

[E09] 去除所有空白字符
来源：http://lx.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hb.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ue.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://fi.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ec.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://qr.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yp.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mi.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zn.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://kr.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vs.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://et.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://ub.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://yl.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://nh.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sb.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lx.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rc.haigaiapp.cn

[E11] 反转字符串
来源：http://yg.nicolike.cn

Py:   s[::-1]
来源：http://zh.shtwfgs.cn

PHP:  strrev($s);
来源：http://kj.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://ze.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://ro.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dh.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zs.yuexingan06.cn

Ruby: s.reverse
来源：http://wm.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hf.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://pj.jctech888.com.cn

Py:   s.count("a")
来源：http://je.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://rd.huanxung.cn

JS:   s.split("a").length - 1
来源：http://os.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://aw.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wk.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://ng.haigaiapp.cn

Ruby: s.count("a")
来源：http://zs.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://hm.hahajie.cn

[E13] 逐字符遍历
来源：http://yj.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://cd.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xc.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lm.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bu.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wa.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yo.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://of.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ow.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://pw.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yh.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://of.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ol.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ek.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yx.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sk.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fv.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dn.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://fu.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://js.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gi.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wy.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tq.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aw.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ut.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qt.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://db.huanxung.cn

[E16] 数字千分位
来源：http://ow.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://nk.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://zj.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cu.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hj.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oq.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qt.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oj.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://hl.lnxyls.cn

[E17] 首字母大写
来源：http://aw.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ep.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ak.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zn.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uw.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wa.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rf.panjiajie.cn

Ruby: s.capitalize
来源：http://sk.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nc.9csxet.cn

[E18] 模板占位符替换
来源：http://lf.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lg.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://te.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lu.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qf.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ca.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nd.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ow.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bd.colortex.cn

[E19] 多行文本按行拆分
来源：http://ki.asd995.cn

Py:   s.splitlines()
来源：http://xr.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ky.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://uq.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://pg.muxihuayi.cn

Java: s.lines().toList()
来源：http://xp.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://lp.huixinmuqiang.cn

Ruby: s.lines
来源：http://gg.hnjuh.cn

C#:   s.Split('\n')
来源：http://hw.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://jv.yuexingan06.cn

Py:   if not s:
来源：http://qd.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ee.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jp.9csxet.cn

TS:   if (s === "") {}
来源：http://jx.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://rj.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://do.yuexingan06.cn

Ruby: if s.empty?
来源：http://zx.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ny.newstarts.cn

[E21] 超长截断加省略号
来源：http://bq.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ii.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://os.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xk.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pu.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tr.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://aa.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dv.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iv.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://lt.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rk.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kw.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://io.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qf.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dk.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tt.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://zb.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rh.9csxet.cn

================================================================================
来源：http://be.nszjky.cn

F. 文件与目录
来源：http://ka.szxytkj.cn

================================================================================
来源：http://yl.gzmigu.cn

[F01] 读取整个文件
来源：http://ox.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ck.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://ld.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jg.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ch.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zk.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zk.nicolike.cn

Ruby: File.read("a.txt")
来源：http://tt.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://iq.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://zf.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gr.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cb.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wj.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zs.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pe.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rx.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zz.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yr.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://hc.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dv.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://an.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sx.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oe.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://we.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tl.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://hf.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ra.panjiajie.cn

[F04] 追加写入文件
来源：http://pi.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://of.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zn.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sa.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qk.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ph.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fk.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fe.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jd.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://gt.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://py.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://pb.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://da.wgjwhj.cn

TS:   fs.existsSync("a.txt")
来源：http://ua.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pv.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sb.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://jw.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://ku.haigaiapp.cn

[F06] 删除文件
来源：http://sr.9csxet.cn

Py:   os.remove("a.txt")
来源：http://kc.nicolike.cn

PHP:  unlink("a.txt");
来源：http://vl.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mu.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mz.asd995.cn

Go:   os.Remove("a.txt")
来源：http://ga.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://wu.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://kp.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://sf.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ql.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qw.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zl.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://se.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kj.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lv.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rg.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pk.shxzukj.cn

[F08] 遍历目录
来源：http://td.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vx.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sy.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://ry.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://tk.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gl.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sv.colortex.cn

Ruby: Dir.children("dir")
来源：http://uq.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://wn.szsharing.cn

[F09] 获取文件大小
来源：http://hi.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://da.huanxung.cn

PHP:  filesize("a.txt");
来源：http://nq.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://df.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://yx.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ho.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ng.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://ig.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://xe.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://nk.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vu.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dr.nicolike.cn


<!-- 参考信息 -->