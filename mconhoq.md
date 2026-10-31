代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xu.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xk.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://ft.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ej.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qw.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qx.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hf.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qx.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gl.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ym.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qy.szsharing.cn

[D26] 数组转字符串
来源：http://vm.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://gs.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://zc.yuexingan06.cn

JS:   arr.join(", ")
来源：http://ol.shxzukj.cn

TS:   arr.join(", ")
来源：http://rz.521024.cn

Java: String.join(", ", list)
来源：http://so.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://az.lnxyls.cn

Ruby: arr.join(", ")
来源：http://hy.521024.cn

C#:   string.Join(", ", list)
来源：http://tb.shtwfgs.cn

================================================================================
来源：http://jt.shxzukj.cn

E. 字符串处理
来源：http://tw.yuntaijiaju.cn

================================================================================
来源：http://wu.szsharing.cn

[E01] 拼接字符串
来源：http://qw.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://re.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hl.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jk.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nk.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cf.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gy.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xv.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jb.newstarts.cn

[E02] 重复字符串
来源：http://yg.hahajie.cn

Py:   "ab" * 3
来源：http://gb.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://dr.9csxet.cn

JS:   "ab".repeat(3)
来源：http://ys.nszjky.cn

TS:   "ab".repeat(3)
来源：http://sy.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://cp.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://lp.hnjuh.cn

Ruby: "ab" * 3
来源：http://uk.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ph.jctech888.com.cn

[E03] 截取子串
来源：http://oq.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rq.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tv.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xx.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://qu.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://zl.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cp.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qv.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://ft.muxihuayi.cn

[E04] 查找子串位置
来源：http://bh.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://va.nszjky.cn

PHP:  strpos($s, "x");
来源：http://an.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ba.hnjuh.cn

TS:   s.indexOf("x")
来源：http://ag.yuexingan06.cn

Java: s.indexOf("x")
来源：http://os.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://qk.nicolike.cn

Ruby: s.index("x")
来源：http://ct.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://tx.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pd.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://az.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vv.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sk.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qu.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://np.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rh.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ww.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://en.muxihuayi.cn

[E06] 替换子串
来源：http://yb.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zp.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://kv.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jc.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ui.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://id.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pu.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dz.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://ll.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://hm.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://py.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lc.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wc.jianghongdianzi.cn

TS:   s.split(",")
来源：http://je.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dl.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zn.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://xh.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tk.huanxung.cn

[E08] 数组按分隔符合并
来源：http://kk.colortex.cn

Py:   ",".join(items)
来源：http://sy.shxzskj.cn

PHP:  implode(",", $items);
来源：http://bv.gzmigu.cn

JS:   items.join(",")
来源：http://ev.hnjuh.cn

TS:   items.join(",")
来源：http://io.nicolike.cn

Java: String.join(",", items)
来源：http://oj.colortex.cn

Go:   strings.Join(items, ",")
来源：http://oa.huixiangedu.cn

Ruby: items.join(",")
来源：http://xy.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://by.szxytkj.cn

[E09] 去除所有空白字符
来源：http://vp.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://du.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hu.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://ic.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://nh.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://ye.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oz.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ug.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kd.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://fq.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sn.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sk.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://hs.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://rm.hahajie.cn

Java: String.format("%03d", 7)
来源：http://to.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vk.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cz.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bm.szsharing.cn

[E11] 反转字符串
来源：http://yl.panjiajie.cn

Py:   s[::-1]
来源：http://ab.9csxet.cn

PHP:  strrev($s);
来源：http://gl.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://hk.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://cq.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zn.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ax.szsharing.cn

Ruby: s.reverse
来源：http://al.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ny.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://nm.bookmarksfly.cn

Py:   s.count("a")
来源：http://id.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://mt.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://pv.hahajie.cn

TS:   s.split("a").length - 1
来源：http://tq.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zc.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://qp.bookmarksfly.cn

Ruby: s.count("a")
来源：http://rq.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://uk.szsharing.cn

[E13] 逐字符遍历
来源：http://bp.colortex.cn

Py:   for ch in s: print(ch)
来源：http://nh.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yl.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rc.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vq.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ui.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ru.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lj.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jf.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://dk.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ap.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ll.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://io.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://we.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ws.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ld.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ri.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cb.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://rn.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yj.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xm.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nf.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ys.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lb.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dt.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ps.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uw.asd995.cn

[E16] 数字千分位
来源：http://yt.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://yo.nicolike.cn

PHP:  number_format(1234567);
来源：http://mb.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dx.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cm.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ld.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tg.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kv.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://rk.nicolike.cn

[E17] 首字母大写
来源：http://zd.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pv.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ty.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qz.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hb.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rh.muxihuayi.cn

Ruby: s.capitalize
来源：http://xb.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fx.jctech888.com.cn

[E18] 模板占位符替换
来源：http://hz.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lp.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zr.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wm.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cp.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ki.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qw.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fr.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yc.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://ea.hnjuh.cn

Py:   s.splitlines()
来源：http://ra.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mo.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://mk.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://sd.asd995.cn

Java: s.lines().toList()
来源：http://wo.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://wx.521024.cn

Ruby: s.lines
来源：http://ya.szxytkj.cn

C#:   s.Split('\n')
来源：http://ow.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://np.muxihuayi.cn

Py:   if not s:
来源：http://ee.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sn.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://am.lnxyls.cn

TS:   if (s === "") {}
来源：http://ks.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://xz.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://nm.colortex.cn

Ruby: if s.empty?
来源：http://fh.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gw.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://yh.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wb.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cl.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pr.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://he.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zw.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://ks.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qr.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oy.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://dd.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bj.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fz.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vj.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wn.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fy.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://me.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://pf.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wg.9csxet.cn

================================================================================
来源：http://te.shtwfgs.cn

F. 文件与目录
来源：http://jq.haigaiapp.cn

================================================================================
来源：http://oc.szsharing.cn

[F01] 读取整个文件
来源：http://un.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zk.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://xu.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wp.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cc.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uv.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wk.hahajie.cn

Ruby: File.read("a.txt")
来源：http://vq.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://cw.hahajie.cn

[F02] 逐行读取文件
来源：http://qx.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pu.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ax.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bc.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xo.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ow.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://za.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lk.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sx.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://jn.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gn.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ld.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ev.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rp.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xm.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dy.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://ks.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kw.shxzukj.cn

[F04] 追加写入文件
来源：http://il.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ti.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ht.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fe.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dg.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://em.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tl.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://py.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wp.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://gm.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mu.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://ot.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://zw.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://os.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qi.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ps.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://sq.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://bp.bjjhwx.cn

[F06] 删除文件
来源：http://se.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://eb.521024.cn

PHP:  unlink("a.txt");
来源：http://rs.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://go.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lc.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uh.colortex.cn

Go:   os.Remove("a.txt")
来源：http://ba.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://ak.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://vx.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://ez.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://en.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mm.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cd.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ch.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yg.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lx.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wl.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dz.asd995.cn

[F08] 遍历目录
来源：http://fj.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ih.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bc.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://gb.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://zz.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nw.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://th.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://co.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://ns.bjjhwx.cn

[F09] 获取文件大小
来源：http://bm.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://gf.9csxet.cn

PHP:  filesize("a.txt");
来源：http://ou.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://pw.haigaiapp.cn


<!-- 参考信息 -->