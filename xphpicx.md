代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kv.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vk.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oi.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://se.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ps.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bo.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vo.szxytkj.cn

[D26] 数组转字符串
来源：http://cg.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://tx.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://iz.szxytkj.cn

JS:   arr.join(", ")
来源：http://vv.hahajie.cn

TS:   arr.join(", ")
来源：http://fn.asd995.cn

Java: String.join(", ", list)
来源：http://ew.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://ml.521024.cn

Ruby: arr.join(", ")
来源：http://lm.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://ak.haigaiapp.cn

================================================================================
来源：http://ei.szsharing.cn

E. 字符串处理
来源：http://ye.hnjuh.cn

================================================================================
来源：http://qf.lnxyls.cn

[E01] 拼接字符串
来源：http://zg.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ts.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nv.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hl.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gl.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ku.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ef.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tv.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hq.wgjwhj.cn

[E02] 重复字符串
来源：http://jw.newstarts.cn

Py:   "ab" * 3
来源：http://nj.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://wt.asd995.cn

JS:   "ab".repeat(3)
来源：http://mm.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://lo.lnxyls.cn

Java: "ab".repeat(3)
来源：http://kb.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://nm.lnxyls.cn

Ruby: "ab" * 3
来源：http://vf.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zo.newstarts.cn

[E03] 截取子串
来源：http://iq.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qe.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://so.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ui.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://cl.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://ys.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aq.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ku.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ki.jctech888.com.cn

[E04] 查找子串位置
来源：http://np.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://tn.szsharing.cn

PHP:  strpos($s, "x");
来源：http://sc.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://og.colortex.cn

TS:   s.indexOf("x")
来源：http://zi.muxihuayi.cn

Java: s.indexOf("x")
来源：http://fo.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://xe.521024.cn

Ruby: s.index("x")
来源：http://cf.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://wv.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zv.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://au.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nm.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zu.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ib.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hj.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rs.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ib.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sj.muxihuayi.cn

[E06] 替换子串
来源：http://rm.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lv.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://lq.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://me.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://pt.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ih.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sb.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vg.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://eg.lnxyls.cn

[E07] 按分隔符拆分
来源：http://ot.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gi.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zz.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sw.yuexingan06.cn

TS:   s.split(",")
来源：http://ad.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ve.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wz.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://ta.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ba.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://ii.newstarts.cn

Py:   ",".join(items)
来源：http://ic.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://cr.huanxung.cn

JS:   items.join(",")
来源：http://ho.newstarts.cn

TS:   items.join(",")
来源：http://ca.lnxyls.cn

Java: String.join(",", items)
来源：http://vp.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://el.haigaiapp.cn

Ruby: items.join(",")
来源：http://we.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://lx.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://oa.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mv.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ys.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://wn.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://zk.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://nk.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vx.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://il.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ue.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://lf.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uc.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xi.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://kj.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://nz.szsharing.cn

Java: String.format("%03d", 7)
来源：http://xi.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://um.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sj.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zl.shxzskj.cn

[E11] 反转字符串
来源：http://yn.muxihuayi.cn

Py:   s[::-1]
来源：http://rh.wgjwhj.cn

PHP:  strrev($s);
来源：http://la.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://eg.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://fz.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wl.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kd.haigaiapp.cn

Ruby: s.reverse
来源：http://kz.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://te.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://bn.shtwfgs.cn

Py:   s.count("a")
来源：http://ks.asd995.cn

PHP:  substr_count($s, "a");
来源：http://zk.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://bp.521024.cn

TS:   s.split("a").length - 1
来源：http://ul.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ee.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://tz.chemitech.net.cn

Ruby: s.count("a")
来源：http://ry.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://hw.bjjhwx.cn

[E13] 逐字符遍历
来源：http://im.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://fc.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lb.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tq.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xl.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yp.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hp.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://er.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wb.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://ew.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sl.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ll.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yo.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jo.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jt.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sj.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://os.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wp.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://fa.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wd.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wg.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vz.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oq.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zr.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rq.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vy.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wo.521024.cn

[E16] 数字千分位
来源：http://yo.asd995.cn

Py:   f"{1234567:,}"
来源：http://qs.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://ro.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mt.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kc.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fv.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ly.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hq.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://xp.szsharing.cn

[E17] 首字母大写
来源：http://co.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nx.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ni.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nf.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lg.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tn.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vc.lnxyls.cn

Ruby: s.capitalize
来源：http://cf.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ps.newstarts.cn

[E18] 模板占位符替换
来源：http://dg.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bd.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gt.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tu.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hm.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dh.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gk.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xc.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ce.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://sb.szxytkj.cn

Py:   s.splitlines()
来源：http://bw.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vb.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://on.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://sa.nszjky.cn

Java: s.lines().toList()
来源：http://aw.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://vi.lnxyls.cn

Ruby: s.lines
来源：http://dk.asd995.cn

C#:   s.Split('\n')
来源：http://sx.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://xl.huanxung.cn

Py:   if not s:
来源：http://jj.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ks.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mv.521024.cn

TS:   if (s === "") {}
来源：http://cn.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://qq.wgjwhj.cn

Go:   if s == "" {}
来源：http://pk.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://rp.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uy.nszjky.cn

[E21] 超长截断加省略号
来源：http://yr.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pl.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://up.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uu.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zz.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://db.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://fq.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sc.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uf.colortex.cn

[E22] 字节长度与字符长度
来源：http://ee.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wd.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bl.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uq.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ex.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jc.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ol.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://mt.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rr.newstarts.cn

================================================================================
来源：http://nm.521024.cn

F. 文件与目录
来源：http://nn.lnxyls.cn

================================================================================
来源：http://ie.521024.cn

[F01] 读取整个文件
来源：http://je.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ae.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://bx.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jk.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xj.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ju.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cd.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ds.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://vd.shtwfgs.cn

[F02] 逐行读取文件
来源：http://vr.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tv.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kt.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cx.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mb.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xs.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wm.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eo.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bj.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://xf.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://df.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vx.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vk.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bs.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aj.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zh.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://hc.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wk.wgjwhj.cn

[F04] 追加写入文件
来源：http://av.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oz.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gs.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rs.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hb.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yp.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zp.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gi.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://or.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://at.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://md.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://qr.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://rg.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://nb.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nf.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zh.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://sc.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://ro.lnxyls.cn

[F06] 删除文件
来源：http://vs.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://qx.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://gi.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zi.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://be.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vh.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://ex.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://bo.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://rf.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://al.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mw.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vb.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gr.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mq.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xb.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sc.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hq.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xq.lnxyls.cn

[F08] 遍历目录
来源：http://lc.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://on.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yf.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://xm.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://nk.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://on.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yb.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://bt.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://rw.newstarts.cn

[F09] 获取文件大小
来源：http://uo.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://nn.nszjky.cn

PHP:  filesize("a.txt");
来源：http://vq.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://mq.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://yu.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nu.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ql.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://un.jianghongdianzi.cn


<!-- 参考信息 -->