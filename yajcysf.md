代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ts.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://pp.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cc.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ug.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fb.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yb.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vy.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mt.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vp.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sb.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://ak.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vn.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ny.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vx.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ao.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dt.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hf.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yf.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pl.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://xe.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://wz.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://nm.jctech888.com.cn

JS:   arr.join(", ")
来源：http://kk.hahajie.cn

TS:   arr.join(", ")
来源：http://eq.huixiangedu.cn

Java: String.join(", ", list)
来源：http://ip.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://eq.shxzskj.cn

Ruby: arr.join(", ")
来源：http://wo.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://ms.9csxet.cn

================================================================================
来源：http://bs.colortex.cn

E. 字符串处理
来源：http://oy.yuexingan06.cn

================================================================================
来源：http://nq.hahajie.cn

[E01] 拼接字符串
来源：http://bd.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pb.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hs.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qq.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uo.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nn.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zq.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dw.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yq.yuexingan06.cn

[E02] 重复字符串
来源：http://pb.szxytkj.cn

Py:   "ab" * 3
来源：http://ep.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ha.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://lr.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://mf.panjiajie.cn

Java: "ab".repeat(3)
来源：http://jh.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://tb.haigaiapp.cn

Ruby: "ab" * 3
来源：http://dy.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uz.521024.cn

[E03] 截取子串
来源：http://ch.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vd.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dw.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fl.9csxet.cn

TS:   s.slice(1, 4)
来源：http://ju.szxytkj.cn

Java: s.substring(1, 4)
来源：http://ly.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ox.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oy.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://rs.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://qp.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://bz.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://wn.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oj.newstarts.cn

TS:   s.indexOf("x")
来源：http://oc.muxihuayi.cn

Java: s.indexOf("x")
来源：http://xd.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://oc.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://tr.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://fs.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wt.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cv.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wm.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qr.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jo.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hl.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fx.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aw.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ea.yuntaijiaju.cn

[E06] 替换子串
来源：http://uf.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yq.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://ou.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ve.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://pb.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jb.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hj.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dq.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://sx.panjiajie.cn

[E07] 按分隔符拆分
来源：http://vl.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ta.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ds.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ov.nszjky.cn

TS:   s.split(",")
来源：http://bh.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vi.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ko.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://bc.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://de.nicolike.cn

[E08] 数组按分隔符合并
来源：http://jk.shxzskj.cn

Py:   ",".join(items)
来源：http://rj.szsharing.cn

PHP:  implode(",", $items);
来源：http://dn.yuexingan06.cn

JS:   items.join(",")
来源：http://ls.wgjwhj.cn

TS:   items.join(",")
来源：http://cn.bookmarksfly.cn

Java: String.join(",", items)
来源：http://ky.colortex.cn

Go:   strings.Join(items, ",")
来源：http://uh.9csxet.cn

Ruby: items.join(",")
来源：http://if.asd995.cn

C#:   string.Join(",", items)
来源：http://ef.nszjky.cn

[E09] 去除所有空白字符
来源：http://aj.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xu.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zt.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://js.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://pq.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://iw.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yp.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fk.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mo.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://qa.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uo.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wl.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://xa.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://fx.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://bm.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fi.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wn.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fg.muxihuayi.cn

[E11] 反转字符串
来源：http://rp.szxytkj.cn

Py:   s[::-1]
来源：http://tw.wgjwhj.cn

PHP:  strrev($s);
来源：http://jt.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://jj.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://ab.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tc.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://or.haigaiapp.cn

Ruby: s.reverse
来源：http://ko.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ym.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://xn.panjiajie.cn

Py:   s.count("a")
来源：http://ut.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://oe.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://ps.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://kv.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zi.colortex.cn

Go:   strings.Count(s, "a")
来源：http://vl.shxzukj.cn

Ruby: s.count("a")
来源：http://kq.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://yf.asd995.cn

[E13] 逐字符遍历
来源：http://mr.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://mg.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oh.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gb.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wp.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fn.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ni.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dm.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hd.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://yn.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qo.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://id.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ro.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://em.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vr.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://my.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tv.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://su.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://rk.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xn.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zo.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oi.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vo.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fo.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mn.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oc.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pi.jianghongdianzi.cn

[E16] 数字千分位
来源：http://tz.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://nj.nicolike.cn

PHP:  number_format(1234567);
来源：http://cz.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://it.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://so.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fs.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://go.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ot.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://nm.shtwfgs.cn

[E17] 首字母大写
来源：http://zz.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ld.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hi.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gy.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qg.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qb.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hq.szxytkj.cn

Ruby: s.capitalize
来源：http://qn.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qk.9csxet.cn

[E18] 模板占位符替换
来源：http://ob.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sb.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tc.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ph.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yt.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sc.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cz.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qe.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gp.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://sh.shtwfgs.cn

Py:   s.splitlines()
来源：http://sk.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vh.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://js.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://yf.bookmarksfly.cn

Java: s.lines().toList()
来源：http://tb.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://fi.shxzskj.cn

Ruby: s.lines
来源：http://tj.yuexingan06.cn

C#:   s.Split('\n')
来源：http://aw.newstarts.cn

[E20] 判断字符串是否为空
来源：http://lb.9csxet.cn

Py:   if not s:
来源：http://xd.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://od.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sn.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://rf.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://wl.9csxet.cn

Go:   if s == "" {}
来源：http://zf.jctech888.com.cn

Ruby: if s.empty?
来源：http://ft.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sh.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://gd.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lr.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hi.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kx.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://su.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ac.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://bl.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ef.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ui.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://vk.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qq.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mx.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gl.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ta.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lz.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pq.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://jg.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bb.panjiajie.cn

================================================================================
来源：http://ib.shxzukj.cn

F. 文件与目录
来源：http://xe.szsharing.cn

================================================================================
来源：http://lb.szxytkj.cn

[F01] 读取整个文件
来源：http://yr.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zb.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://xm.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hd.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mp.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iv.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fo.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://kx.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://mv.shxzskj.cn

[F02] 逐行读取文件
来源：http://eb.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fa.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://al.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uf.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uk.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rl.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hs.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zg.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rv.colortex.cn

[F03] 写入文件（覆盖）
来源：http://ay.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hq.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wj.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xg.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uo.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fp.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ng.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://in.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ij.shxzukj.cn

[F04] 追加写入文件
来源：http://fg.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hm.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dy.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wq.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pv.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ad.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zi.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ps.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://if.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://aj.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kd.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://cl.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://wy.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://zx.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ho.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xk.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://nj.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://mo.huanxung.cn

[F06] 删除文件
来源：http://aa.nicolike.cn

Py:   os.remove("a.txt")
来源：http://hz.9csxet.cn

PHP:  unlink("a.txt");
来源：http://yy.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://az.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://va.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gy.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://ig.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://fc.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://ei.asd995.cn

[F07] 创建目录（含多级）
来源：http://ak.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jd.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xb.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://px.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ef.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ss.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://on.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ne.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://by.521024.cn

[F08] 遍历目录
来源：http://wz.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rt.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hu.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://ol.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://av.newstarts.cn


<!-- 参考信息 -->