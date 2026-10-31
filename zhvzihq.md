代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pl.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gw.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iu.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://zv.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://pt.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://ko.521024.cn

JS:   arr.join(", ")
来源：http://me.szxytkj.cn

TS:   arr.join(", ")
来源：http://yw.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://pf.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://tg.nicolike.cn

Ruby: arr.join(", ")
来源：http://tm.nicolike.cn

C#:   string.Join(", ", list)
来源：http://tr.yuexingan06.cn

================================================================================
来源：http://rc.haigaiapp.cn

E. 字符串处理
来源：http://ki.521024.cn

================================================================================
来源：http://fr.szxytkj.cn

[E01] 拼接字符串
来源：http://fv.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nu.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ou.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nj.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sz.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gs.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ws.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gn.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ul.shtwfgs.cn

[E02] 重复字符串
来源：http://fa.jctech888.com.cn

Py:   "ab" * 3
来源：http://dr.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://er.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://nz.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://wo.nszjky.cn

Java: "ab".repeat(3)
来源：http://ri.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://fr.hnjuh.cn

Ruby: "ab" * 3
来源：http://md.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pa.shxzukj.cn

[E03] 截取子串
来源：http://ox.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uq.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ow.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fg.hahajie.cn

TS:   s.slice(1, 4)
来源：http://ka.shxzukj.cn

Java: s.substring(1, 4)
来源：http://ko.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ys.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hz.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://gv.szxytkj.cn

[E04] 查找子串位置
来源：http://le.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://uj.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://jt.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tk.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://xy.bjjhwx.cn

Java: s.indexOf("x")
来源：http://eo.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://bf.newstarts.cn

Ruby: s.index("x")
来源：http://wx.asd995.cn

C#:   s.IndexOf("x")
来源：http://dq.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rc.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ok.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hv.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eg.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mt.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vc.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rr.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qi.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bp.shtwfgs.cn

[E06] 替换子串
来源：http://ri.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://te.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://im.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cn.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://ny.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gc.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mi.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ab.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://ns.szxytkj.cn

[E07] 按分隔符拆分
来源：http://ol.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tw.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zj.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ip.nszjky.cn

TS:   s.split(",")
来源：http://ag.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ad.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mt.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://rs.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hv.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://vv.shxzskj.cn

Py:   ",".join(items)
来源：http://yj.nicolike.cn

PHP:  implode(",", $items);
来源：http://op.jianghongdianzi.cn

JS:   items.join(",")
来源：http://vv.nicolike.cn

TS:   items.join(",")
来源：http://sj.lnxyls.cn

Java: String.join(",", items)
来源：http://fz.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://ds.asd995.cn

Ruby: items.join(",")
来源：http://sg.lnxyls.cn

C#:   string.Join(",", items)
来源：http://bs.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://qi.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://md.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ty.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://pn.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ip.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://wc.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://px.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sg.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fo.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://lm.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ho.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ha.521024.cn

JS:   "7".padStart(3, "0")
来源：http://bj.521024.cn

TS:   "7".padStart(3, "0")
来源：http://db.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://gd.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xt.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uj.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zb.colortex.cn

[E11] 反转字符串
来源：http://xz.nszjky.cn

Py:   s[::-1]
来源：http://qi.newstarts.cn

PHP:  strrev($s);
来源：http://ju.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://lx.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://bx.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qk.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xs.nszjky.cn

Ruby: s.reverse
来源：http://el.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qe.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://ub.panjiajie.cn

Py:   s.count("a")
来源：http://zi.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://dj.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://ug.521024.cn

TS:   s.split("a").length - 1
来源：http://gg.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kd.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://xe.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://rc.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://il.chemitech.net.cn

[E13] 逐字符遍历
来源：http://rm.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://wk.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nw.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nt.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ez.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jk.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aa.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dp.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://to.9csxet.cn

[E14] URL 编码与 Base64
来源：http://wu.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yf.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vr.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lz.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rt.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aw.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://re.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ke.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hg.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://io.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ms.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jz.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nf.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://va.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jc.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tu.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ti.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cp.shxzukj.cn

[E16] 数字千分位
来源：http://pv.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://ck.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://et.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ev.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lo.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://za.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://af.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mv.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://wg.nszjky.cn

[E17] 首字母大写
来源：http://ki.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tp.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tb.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ol.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ny.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://do.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uj.asd995.cn

Ruby: s.capitalize
来源：http://md.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cp.newstarts.cn

[E18] 模板占位符替换
来源：http://iu.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ep.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qs.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ed.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cq.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ub.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wn.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bb.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pw.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://vi.9csxet.cn

Py:   s.splitlines()
来源：http://km.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xw.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://if.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://ci.szsharing.cn

Java: s.lines().toList()
来源：http://nf.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://zk.huixiangedu.cn

Ruby: s.lines
来源：http://po.9csxet.cn

C#:   s.Split('\n')
来源：http://ul.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://qf.bookmarksfly.cn

Py:   if not s:
来源：http://gh.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://co.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fr.shtwfgs.cn

TS:   if (s === "") {}
来源：http://ea.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://nm.panjiajie.cn

Go:   if s == "" {}
来源：http://sq.newstarts.cn

Ruby: if s.empty?
来源：http://mp.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iy.colortex.cn

[E21] 超长截断加省略号
来源：http://nh.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qe.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pq.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xv.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lh.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ya.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nt.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tk.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nq.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://zq.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vm.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fp.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gz.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kp.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zx.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fh.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://wd.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ie.hahajie.cn

================================================================================
来源：http://lz.yuntaijiaju.cn

F. 文件与目录
来源：http://dn.bjjhwx.cn

================================================================================
来源：http://em.nicolike.cn

[F01] 读取整个文件
来源：http://nr.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://or.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://jk.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fd.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qc.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cd.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ut.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://so.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://rk.huanxung.cn

[F02] 逐行读取文件
来源：http://ew.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jl.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gx.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mw.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qx.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pt.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kq.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jb.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://nr.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ou.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xr.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mq.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sv.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ms.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hd.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ga.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bs.hnjuh.cn

[F04] 追加写入文件
来源：http://fa.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nb.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wa.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tv.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nk.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://su.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kf.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sk.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://dt.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lo.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://ob.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://no.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://ma.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ee.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rf.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://ld.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://zg.bookmarksfly.cn

[F06] 删除文件
来源：http://rz.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://qx.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://sw.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xw.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bx.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://np.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://rr.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://ef.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://ba.nicolike.cn

[F07] 创建目录（含多级）
来源：http://wl.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rp.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rl.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rr.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jq.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mf.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://te.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://od.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oi.huixinmuqiang.cn

[F08] 遍历目录
来源：http://up.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hu.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aw.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://qw.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://ak.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fo.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://py.nicolike.cn

Ruby: Dir.children("dir")
来源：http://dp.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://et.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://ii.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://vg.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://hn.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://js.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://ge.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mh.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lo.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://dz.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://hm.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://dq.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zh.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://je.gzmigu.cn


<!-- 参考信息 -->