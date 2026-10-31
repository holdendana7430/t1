代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oa.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jw.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vk.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vj.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wk.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://to.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://od.muxihuayi.cn

[D26] 数组转字符串
来源：http://cd.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://hi.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://we.9csxet.cn

JS:   arr.join(", ")
来源：http://fo.shtwfgs.cn

TS:   arr.join(", ")
来源：http://ol.huanxung.cn

Java: String.join(", ", list)
来源：http://in.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://dk.asd995.cn

Ruby: arr.join(", ")
来源：http://vp.asd995.cn

C#:   string.Join(", ", list)
来源：http://qb.9csxet.cn

================================================================================
来源：http://zd.hahajie.cn

E. 字符串处理
来源：http://cn.shtwfgs.cn

================================================================================
来源：http://ul.shxzskj.cn

[E01] 拼接字符串
来源：http://mv.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dn.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://il.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zc.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hb.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bj.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hm.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hl.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yi.newstarts.cn

[E02] 重复字符串
来源：http://zz.521024.cn

Py:   "ab" * 3
来源：http://zf.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://yl.nszjky.cn

JS:   "ab".repeat(3)
来源：http://pz.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://wi.szsharing.cn

Java: "ab".repeat(3)
来源：http://cn.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://aq.chemitech.net.cn

Ruby: "ab" * 3
来源：http://ee.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fn.bjjhwx.cn

[E03] 截取子串
来源：http://tx.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wr.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pg.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hu.hahajie.cn

TS:   s.slice(1, 4)
来源：http://gr.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://qe.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nv.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bu.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://uj.hnjuh.cn

[E04] 查找子串位置
来源：http://ty.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://ep.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://ii.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cv.huanxung.cn

TS:   s.indexOf("x")
来源：http://tv.yuexingan06.cn

Java: s.indexOf("x")
来源：http://sr.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ye.shtwfgs.cn

Ruby: s.index("x")
来源：http://nn.9csxet.cn

C#:   s.IndexOf("x")
来源：http://yl.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://op.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mf.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lz.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://td.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ad.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qw.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sl.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lb.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yk.nszjky.cn

[E06] 替换子串
来源：http://gr.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dw.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://nn.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ct.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://vz.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xn.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ln.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tn.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://li.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://ls.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fp.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dl.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zr.lnxyls.cn

TS:   s.split(",")
来源：http://zt.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://by.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fe.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://gu.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ys.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://ng.bjjhwx.cn

Py:   ",".join(items)
来源：http://os.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://bk.gzmigu.cn

JS:   items.join(",")
来源：http://ap.muxihuayi.cn

TS:   items.join(",")
来源：http://sl.szxytkj.cn

Java: String.join(",", items)
来源：http://wb.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://on.szxytkj.cn

Ruby: items.join(",")
来源：http://ko.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://uf.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://fh.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cz.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://om.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://jm.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://vv.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://ly.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hu.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jo.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wo.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://qw.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ks.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gf.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://ab.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://yi.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://zw.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cx.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kk.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://he.szsharing.cn

[E11] 反转字符串
来源：http://br.jianghongdianzi.cn

Py:   s[::-1]
来源：http://nl.shtwfgs.cn

PHP:  strrev($s);
来源：http://gy.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://cn.colortex.cn

TS:   [...s].reverse().join("")
来源：http://uc.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wk.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tf.huixinmuqiang.cn

Ruby: s.reverse
来源：http://ll.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vq.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://rm.lnxyls.cn

Py:   s.count("a")
来源：http://er.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://co.521024.cn

JS:   s.split("a").length - 1
来源：http://fd.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://wm.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zy.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://yd.szxytkj.cn

Ruby: s.count("a")
来源：http://uf.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://vm.hahajie.cn

[E13] 逐字符遍历
来源：http://vp.521024.cn

Py:   for ch in s: print(ch)
来源：http://vt.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xl.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pa.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zs.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yb.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cf.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rb.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://py.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://uh.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bl.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ee.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cu.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rt.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xv.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://um.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pq.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bd.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://vp.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bv.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mt.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gf.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zu.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ja.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ls.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wf.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wk.panjiajie.cn

[E16] 数字千分位
来源：http://rf.521024.cn

Py:   f"{1234567:,}"
来源：http://wq.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://ft.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jk.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hf.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gt.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oy.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ca.asd995.cn

C#:   1234567.ToString("N0")
来源：http://eb.nszjky.cn

[E17] 首字母大写
来源：http://br.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://av.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ti.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gm.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dk.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pi.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nd.nszjky.cn

Ruby: s.capitalize
来源：http://dh.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oe.szxytkj.cn

[E18] 模板占位符替换
来源：http://hh.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vj.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xq.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://az.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mp.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oh.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tq.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ke.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bd.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://gj.yuexingan06.cn

Py:   s.splitlines()
来源：http://sy.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gz.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://ct.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://ln.colortex.cn

Java: s.lines().toList()
来源：http://sx.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://tl.9csxet.cn

Ruby: s.lines
来源：http://fm.bjjhwx.cn

C#:   s.Split('\n')
来源：http://gw.hahajie.cn

[E20] 判断字符串是否为空
来源：http://hd.szxytkj.cn

Py:   if not s:
来源：http://ot.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lf.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wc.521024.cn

TS:   if (s === "") {}
来源：http://fl.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ym.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://db.nicolike.cn

Ruby: if s.empty?
来源：http://gy.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://du.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://am.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xj.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qo.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gm.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ll.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vf.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://ud.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cb.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fn.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://ff.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yl.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cj.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hv.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xg.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ru.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pg.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ym.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mm.9csxet.cn

================================================================================
来源：http://ua.szxytkj.cn

F. 文件与目录
来源：http://ay.yuexingan06.cn

================================================================================
来源：http://ca.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://kd.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xe.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://vt.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ox.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://id.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ec.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://im.huanxung.cn

Ruby: File.read("a.txt")
来源：http://gn.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://dx.nicolike.cn

[F02] 逐行读取文件
来源：http://in.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wn.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ql.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rq.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ep.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vq.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hr.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ot.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dt.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://rt.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ij.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zk.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xu.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tw.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jv.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bf.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://aq.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ri.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://jy.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mo.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gs.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zf.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rq.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ur.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qe.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jj.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cj.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://rd.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vu.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://el.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://eh.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://xs.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xf.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fi.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://kq.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://sx.nicolike.cn

[F06] 删除文件
来源：http://hp.9csxet.cn

Py:   os.remove("a.txt")
来源：http://lk.huanxung.cn

PHP:  unlink("a.txt");
来源：http://wy.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uj.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ux.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mm.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://ka.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://vd.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://uf.hahajie.cn

[F07] 创建目录（含多级）
来源：http://xn.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gz.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ks.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://js.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gr.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fr.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ki.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yy.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ef.521024.cn

[F08] 遍历目录
来源：http://os.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ox.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oo.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://of.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://ck.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ux.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fa.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://jt.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://jg.nicolike.cn

[F09] 获取文件大小
来源：http://mw.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://ib.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://pp.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://jg.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://he.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://or.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zz.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://hn.shxzukj.cn


<!-- 参考信息 -->