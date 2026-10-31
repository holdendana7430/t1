代发 wailian999

Java: new ArrayList<>(list);
来源：http://vr.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kp.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://qb.hahajie.cn

C#:   new List<int>(list);
来源：http://ai.jctech888.com.cn

[D23] reduce 累积计算
来源：http://dh.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gx.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://co.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ed.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vn.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dc.jctech888.com.cn

Go:   // 手写循环
来源：http://rt.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lh.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://de.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://zg.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fe.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cv.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tb.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tv.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zx.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bd.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zz.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://di.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://gv.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bh.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://si.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bo.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://so.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nn.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://md.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xm.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bv.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://az.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://op.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://qc.shxzukj.cn

JS:   arr.join(", ")
来源：http://kl.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ec.521024.cn

Java: String.join(", ", list)
来源：http://cm.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://fh.asd995.cn

Ruby: arr.join(", ")
来源：http://hz.nszjky.cn

C#:   string.Join(", ", list)
来源：http://nv.yuntaijiaju.cn

================================================================================
来源：http://qe.lnxyls.cn

E. 字符串处理
来源：http://fc.huanxung.cn

================================================================================
来源：http://qx.huixiangedu.cn

[E01] 拼接字符串
来源：http://bw.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://un.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bv.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uk.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fi.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ft.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fj.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bj.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bq.wgjwhj.cn

[E02] 重复字符串
来源：http://fp.bookmarksfly.cn

Py:   "ab" * 3
来源：http://vj.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://fi.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://jg.asd995.cn

TS:   "ab".repeat(3)
来源：http://ve.huanxung.cn

Java: "ab".repeat(3)
来源：http://fu.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://hr.shtwfgs.cn

Ruby: "ab" * 3
来源：http://zh.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yo.colortex.cn

[E03] 截取子串
来源：http://ar.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pm.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rz.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gb.newstarts.cn

TS:   s.slice(1, 4)
来源：http://vt.9csxet.cn

Java: s.substring(1, 4)
来源：http://bg.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dw.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bk.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://sj.9csxet.cn

[E04] 查找子串位置
来源：http://ez.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://gb.asd995.cn

PHP:  strpos($s, "x");
来源：http://ym.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xh.colortex.cn

TS:   s.indexOf("x")
来源：http://kw.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://to.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://en.nicolike.cn

Ruby: s.index("x")
来源：http://dq.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://nz.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kh.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ff.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wz.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jk.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mh.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://er.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wx.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ty.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xy.nszjky.cn

[E06] 替换子串
来源：http://pt.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kw.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://tc.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ke.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://mj.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yh.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mc.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tn.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://fp.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://ge.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eu.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ee.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rw.jctech888.com.cn

TS:   s.split(",")
来源：http://zu.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yb.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iu.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://wo.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ku.nszjky.cn

[E08] 数组按分隔符合并
来源：http://qc.521024.cn

Py:   ",".join(items)
来源：http://zz.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://fk.gzmigu.cn

JS:   items.join(",")
来源：http://sz.muxihuayi.cn

TS:   items.join(",")
来源：http://kx.panjiajie.cn

Java: String.join(",", items)
来源：http://wb.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://vg.newstarts.cn

Ruby: items.join(",")
来源：http://gk.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://rq.nicolike.cn

[E09] 去除所有空白字符
来源：http://vb.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jm.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ao.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ae.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://as.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://iu.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gc.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qp.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vs.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ix.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xj.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bv.521024.cn

JS:   "7".padStart(3, "0")
来源：http://ir.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://fi.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://hq.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cc.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tq.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fp.wgjwhj.cn

[E11] 反转字符串
来源：http://bq.shtwfgs.cn

Py:   s[::-1]
来源：http://wx.gzmigu.cn

PHP:  strrev($s);
来源：http://yg.colortex.cn

JS:   [...s].reverse().join("")
来源：http://lk.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://ug.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bc.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oh.colortex.cn

Ruby: s.reverse
来源：http://li.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ih.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://ie.muxihuayi.cn

Py:   s.count("a")
来源：http://ys.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://dx.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://sp.nicolike.cn

TS:   s.split("a").length - 1
来源：http://fu.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rp.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://pg.nszjky.cn

Ruby: s.count("a")
来源：http://tl.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://nu.chemitech.net.cn

[E13] 逐字符遍历
来源：http://iv.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://dm.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pu.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ks.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zc.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xe.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ub.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eb.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uj.521024.cn

[E14] URL 编码与 Base64
来源：http://rf.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tl.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vh.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jo.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ur.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qy.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://da.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kf.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://up.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://ql.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vl.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jb.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xy.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hy.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uf.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://up.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vt.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jf.haigaiapp.cn

[E16] 数字千分位
来源：http://tt.asd995.cn

Py:   f"{1234567:,}"
来源：http://bs.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://vg.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jo.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hx.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jz.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pz.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vg.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://tw.haigaiapp.cn

[E17] 首字母大写
来源：http://ow.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vk.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cx.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lx.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ef.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oy.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fk.521024.cn

Ruby: s.capitalize
来源：http://tj.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://av.nicolike.cn

[E18] 模板占位符替换
来源：http://zw.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ao.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bd.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vs.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://se.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bv.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kv.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://em.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sm.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://ol.9csxet.cn

Py:   s.splitlines()
来源：http://kw.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ky.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://oo.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://rt.szsharing.cn

Java: s.lines().toList()
来源：http://ca.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://dw.jctech888.com.cn

Ruby: s.lines
来源：http://tf.newstarts.cn

C#:   s.Split('\n')
来源：http://ym.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://bx.colortex.cn

Py:   if not s:
来源：http://mh.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qg.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kf.shxzskj.cn

TS:   if (s === "") {}
来源：http://yt.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://bv.9csxet.cn

Go:   if s == "" {}
来源：http://wc.huixiangedu.cn

Ruby: if s.empty?
来源：http://zs.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qx.hahajie.cn

[E21] 超长截断加省略号
来源：http://ts.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mg.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tf.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sx.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wm.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yb.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://ai.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://av.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gf.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://kr.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xy.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ic.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mz.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zq.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wi.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://on.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://cx.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aw.yuntaijiaju.cn

================================================================================
来源：http://qx.yuexingan06.cn

F. 文件与目录
来源：http://tz.shxzskj.cn

================================================================================
来源：http://ff.nszjky.cn

[F01] 读取整个文件
来源：http://ed.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dj.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://pe.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ol.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://je.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yf.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uj.nicolike.cn

Ruby: File.read("a.txt")
来源：http://ap.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://vb.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://gs.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bn.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ca.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dz.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qx.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cf.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://si.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uj.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cs.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://oy.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tn.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gt.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://an.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ok.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://na.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://em.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://if.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fv.newstarts.cn

[F04] 追加写入文件
来源：http://mq.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oh.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wp.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vs.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xz.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pv.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qo.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wr.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jh.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://mp.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hg.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://uc.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://go.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://zl.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xc.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kd.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://py.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://ca.wgjwhj.cn

[F06] 删除文件
来源：http://bt.nicolike.cn

Py:   os.remove("a.txt")
来源：http://ty.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://of.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qt.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fb.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yv.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://sf.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://qj.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://hb.hahajie.cn

[F07] 创建目录（含多级）
来源：http://oz.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uo.jctech888.com.cn


<!-- 参考信息 -->