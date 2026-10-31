代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nd.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xz.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xy.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jt.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gx.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wa.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ry.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ll.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ee.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cb.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ho.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://in.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ih.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://co.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oo.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://vb.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://vj.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ah.szxytkj.cn

JS:   arr.join(", ")
来源：http://mz.huanxung.cn

TS:   arr.join(", ")
来源：http://by.colortex.cn

Java: String.join(", ", list)
来源：http://xt.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://nk.newstarts.cn

Ruby: arr.join(", ")
来源：http://rg.szsharing.cn

C#:   string.Join(", ", list)
来源：http://qo.yuntaijiaju.cn

================================================================================
来源：http://pd.shxzskj.cn

E. 字符串处理
来源：http://kh.9csxet.cn

================================================================================
来源：http://lm.szxytkj.cn

[E01] 拼接字符串
来源：http://vb.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://we.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sh.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ka.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qo.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fj.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://am.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ah.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yo.jctech888.com.cn

[E02] 重复字符串
来源：http://bu.panjiajie.cn

Py:   "ab" * 3
来源：http://dy.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://ae.9csxet.cn

JS:   "ab".repeat(3)
来源：http://xy.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://zx.colortex.cn

Java: "ab".repeat(3)
来源：http://vu.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://hf.muxihuayi.cn

Ruby: "ab" * 3
来源：http://aw.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ut.muxihuayi.cn

[E03] 截取子串
来源：http://jd.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gr.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fm.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xx.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://yg.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://zh.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ap.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iu.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://hw.szxytkj.cn

[E04] 查找子串位置
来源：http://ff.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://zj.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://sr.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iy.gzmigu.cn

TS:   s.indexOf("x")
来源：http://bq.lnxyls.cn

Java: s.indexOf("x")
来源：http://ox.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://ib.nicolike.cn

Ruby: s.index("x")
来源：http://dl.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://de.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gc.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://te.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lx.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ks.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mh.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fj.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://af.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ya.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dh.hahajie.cn

[E06] 替换子串
来源：http://yj.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sr.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://yp.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bc.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ld.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ur.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pf.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nw.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://ki.shxzukj.cn

[E07] 按分隔符拆分
来源：http://jn.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kv.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bb.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mt.lnxyls.cn

TS:   s.split(",")
来源：http://jn.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yf.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ju.521024.cn

Ruby: s.split(",");  s.split
来源：http://yl.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jt.nicolike.cn

[E08] 数组按分隔符合并
来源：http://zb.shtwfgs.cn

Py:   ",".join(items)
来源：http://sb.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://zb.huixiangedu.cn

JS:   items.join(",")
来源：http://qt.bookmarksfly.cn

TS:   items.join(",")
来源：http://bo.lnxyls.cn

Java: String.join(",", items)
来源：http://ut.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://wx.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://xf.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://yp.hnjuh.cn

[E09] 去除所有空白字符
来源：http://yk.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jf.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://un.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://mr.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://ky.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://gg.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gb.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://va.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vz.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://ep.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xj.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://en.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://sl.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://ta.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://es.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kc.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xx.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://of.hahajie.cn

[E11] 反转字符串
来源：http://pa.newstarts.cn

Py:   s[::-1]
来源：http://jk.panjiajie.cn

PHP:  strrev($s);
来源：http://yf.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://yk.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://qk.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mh.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xg.panjiajie.cn

Ruby: s.reverse
来源：http://rd.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jf.szsharing.cn

[E12] 统计某字符出现次数
来源：http://wd.colortex.cn

Py:   s.count("a")
来源：http://vr.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://bn.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://wc.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://xe.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://up.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://jx.lnxyls.cn

Ruby: s.count("a")
来源：http://fa.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://si.nicolike.cn

[E13] 逐字符遍历
来源：http://tk.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://aj.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cr.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nh.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bb.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xz.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wr.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nh.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lj.huanxung.cn

[E14] URL 编码与 Base64
来源：http://wq.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jf.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tr.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lr.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ct.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ae.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qe.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fa.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xb.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://ri.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://in.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vu.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bh.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ps.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oi.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://te.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wu.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ck.asd995.cn

[E16] 数字千分位
来源：http://nj.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://dw.colortex.cn

PHP:  number_format(1234567);
来源：http://kz.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nq.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pl.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zl.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kw.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ra.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://dv.jctech888.com.cn

[E17] 首字母大写
来源：http://on.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xo.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pr.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oz.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ri.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jo.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jz.nicolike.cn

Ruby: s.capitalize
来源：http://bp.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://du.9csxet.cn

[E18] 模板占位符替换
来源：http://dc.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mr.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://me.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://aw.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xj.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aq.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kt.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uv.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lo.hahajie.cn

[E19] 多行文本按行拆分
来源：http://fj.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://sw.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xm.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://kq.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://qj.huanxung.cn

Java: s.lines().toList()
来源：http://wc.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ji.panjiajie.cn

Ruby: s.lines
来源：http://re.haigaiapp.cn

C#:   s.Split('\n')
来源：http://qs.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://yp.yuntaijiaju.cn

Py:   if not s:
来源：http://ot.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zo.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tu.hahajie.cn

TS:   if (s === "") {}
来源：http://lr.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://er.hnjuh.cn

Go:   if s == "" {}
来源：http://rk.yuexingan06.cn

Ruby: if s.empty?
来源：http://wy.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xs.hahajie.cn

[E21] 超长截断加省略号
来源：http://wa.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vo.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wh.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://te.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iq.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bs.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://cu.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ru.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lv.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://rv.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vt.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tv.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ve.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aj.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mj.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rz.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://sg.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tx.jianghongdianzi.cn

================================================================================
来源：http://qq.haigaiapp.cn

F. 文件与目录
来源：http://kq.jctech888.com.cn

================================================================================
来源：http://ap.521024.cn

[F01] 读取整个文件
来源：http://wz.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dw.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://qf.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cu.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vh.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dp.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ov.hahajie.cn

Ruby: File.read("a.txt")
来源：http://sj.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://eu.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://bz.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oe.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sk.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ug.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jy.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nu.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ap.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dv.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sk.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://et.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ne.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dg.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gs.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pj.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://am.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ds.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://tp.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nd.chemitech.net.cn

[F04] 追加写入文件
来源：http://cj.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gg.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dp.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vd.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sg.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sl.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uk.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ts.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tk.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://vm.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xp.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://ci.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://sg.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://hj.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bj.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hx.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://jc.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://ji.huanxung.cn

[F06] 删除文件
来源：http://hz.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://nr.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://wp.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qa.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ae.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yi.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://zn.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://lr.521024.cn

C#:   File.Delete("a.txt");
来源：http://dq.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://jz.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hu.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hu.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ca.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tn.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ly.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ut.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wd.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://np.szsharing.cn

[F08] 遍历目录
来源：http://kr.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jh.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hg.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://gx.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://ad.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://un.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://su.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://lz.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://xo.shxzukj.cn


<!-- 参考信息 -->