代发 wailian999

Ruby: arr.tally
来源：http://ah.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dx.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://da.shtwfgs.cn

Py:   x in arr
来源：http://yp.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://gd.huanxung.cn

JS:   arr.includes(x)
来源：http://bq.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://lu.chemitech.net.cn

Java: list.contains(x)
来源：http://nh.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://vy.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://xf.panjiajie.cn

C#:   list.Contains(x)
来源：http://wr.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://na.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kc.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kf.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://si.lnxyls.cn

TS:   [...arr];
来源：http://is.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://ex.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pz.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://gl.colortex.cn

C#:   new List<int>(list);
来源：http://ct.muxihuayi.cn

[D23] reduce 累积计算
来源：http://bm.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cz.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lr.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://al.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nv.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://km.panjiajie.cn

Go:   // 手写循环
来源：http://lo.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zw.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mm.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://gi.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://va.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dr.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uo.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yv.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qv.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://we.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ra.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pk.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://cb.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tz.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tk.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ym.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ay.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sf.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uc.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oj.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ul.colortex.cn

[D26] 数组转字符串
来源：http://sx.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://hw.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://aj.muxihuayi.cn

JS:   arr.join(", ")
来源：http://zd.shtwfgs.cn

TS:   arr.join(", ")
来源：http://tc.hahajie.cn

Java: String.join(", ", list)
来源：http://an.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://io.nicolike.cn

Ruby: arr.join(", ")
来源：http://wm.9csxet.cn

C#:   string.Join(", ", list)
来源：http://tc.colortex.cn

================================================================================
来源：http://jn.huanxung.cn

E. 字符串处理
来源：http://je.yuntaijiaju.cn

================================================================================
来源：http://va.gzmigu.cn

[E01] 拼接字符串
来源：http://op.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://et.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gn.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vt.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xn.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zj.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ro.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gi.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sa.hnjuh.cn

[E02] 重复字符串
来源：http://lw.haigaiapp.cn

Py:   "ab" * 3
来源：http://wt.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://tr.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://zy.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://og.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ho.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://kj.asd995.cn

Ruby: "ab" * 3
来源：http://vk.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ss.colortex.cn

[E03] 截取子串
来源：http://fa.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://it.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pl.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zq.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://im.colortex.cn

Java: s.substring(1, 4)
来源：http://ic.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dy.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uf.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://yn.colortex.cn

[E04] 查找子串位置
来源：http://sr.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://nd.huanxung.cn

PHP:  strpos($s, "x");
来源：http://al.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oa.nszjky.cn

TS:   s.indexOf("x")
来源：http://ew.muxihuayi.cn

Java: s.indexOf("x")
来源：http://jc.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://ru.9csxet.cn

Ruby: s.index("x")
来源：http://qr.colortex.cn

C#:   s.IndexOf("x")
来源：http://ec.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rc.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pd.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cz.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://on.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yo.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dr.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pd.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uf.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lr.gzmigu.cn

[E06] 替换子串
来源：http://uh.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bd.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://fp.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://us.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://bj.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fw.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jx.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ic.colortex.cn

C#:   s.Replace("a", "b")
来源：http://hp.shxzskj.cn

[E07] 按分隔符拆分
来源：http://lq.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wh.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ux.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xx.szsharing.cn

TS:   s.split(",")
来源：http://ck.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nf.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ws.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://qd.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sw.asd995.cn

[E08] 数组按分隔符合并
来源：http://ix.gzmigu.cn

Py:   ",".join(items)
来源：http://xe.nszjky.cn

PHP:  implode(",", $items);
来源：http://fz.haigaiapp.cn

JS:   items.join(",")
来源：http://xz.shtwfgs.cn

TS:   items.join(",")
来源：http://xw.nszjky.cn

Java: String.join(",", items)
来源：http://fi.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://ak.szxytkj.cn

Ruby: items.join(",")
来源：http://kq.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://fu.asd995.cn

[E09] 去除所有空白字符
来源：http://zh.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xw.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jd.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://id.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://nx.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://oq.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gc.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mh.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pp.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://bq.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lo.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oc.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://pe.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://gl.9csxet.cn

Java: String.format("%03d", 7)
来源：http://yk.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nk.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pd.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cl.jianghongdianzi.cn

[E11] 反转字符串
来源：http://jd.chemitech.net.cn

Py:   s[::-1]
来源：http://vx.gzmigu.cn

PHP:  strrev($s);
来源：http://uh.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://lv.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://ym.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://un.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hb.szxytkj.cn

Ruby: s.reverse
来源：http://cu.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://en.szsharing.cn

[E12] 统计某字符出现次数
来源：http://wk.yuexingan06.cn

Py:   s.count("a")
来源：http://pn.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://ub.asd995.cn

JS:   s.split("a").length - 1
来源：http://gn.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://wu.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kd.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://bs.muxihuayi.cn

Ruby: s.count("a")
来源：http://ww.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://lb.shxzskj.cn

[E13] 逐字符遍历
来源：http://gk.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://lr.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://po.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zb.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://el.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://py.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ej.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nc.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://im.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://yt.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tr.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fg.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qn.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jz.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ze.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tz.hnjuh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uz.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rs.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://di.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sb.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ju.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rv.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vc.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qj.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zj.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://es.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zp.asd995.cn

[E16] 数字千分位
来源：http://ve.newstarts.cn

Py:   f"{1234567:,}"
来源：http://iu.nicolike.cn

PHP:  number_format(1234567);
来源：http://ke.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://su.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fz.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wn.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://me.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ll.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://oj.shtwfgs.cn

[E17] 首字母大写
来源：http://lo.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ta.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://we.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ks.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jg.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://by.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ph.huanxung.cn

Ruby: s.capitalize
来源：http://rm.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dx.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://mz.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bu.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uk.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ll.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ko.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sj.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uy.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lv.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hy.huanxung.cn

[E19] 多行文本按行拆分
来源：http://pg.hnjuh.cn

Py:   s.splitlines()
来源：http://ov.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wj.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://zc.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://ub.shxzukj.cn

Java: s.lines().toList()
来源：http://qn.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://en.muxihuayi.cn

Ruby: s.lines
来源：http://ce.hnjuh.cn

C#:   s.Split('\n')
来源：http://ui.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://of.nszjky.cn

Py:   if not s:
来源：http://sk.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yw.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vx.nicolike.cn

TS:   if (s === "") {}
来源：http://ah.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://zm.shxzskj.cn

Go:   if s == "" {}
来源：http://tt.asd995.cn

Ruby: if s.empty?
来源：http://gb.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mm.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://av.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zn.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sw.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://th.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cp.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nz.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://zx.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kz.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ej.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://vd.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zn.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qy.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xc.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://df.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://to.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xp.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://qo.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://af.bjjhwx.cn

================================================================================
来源：http://vp.huixinmuqiang.cn

F. 文件与目录
来源：http://fa.haigaiapp.cn

================================================================================
来源：http://fk.newstarts.cn

[F01] 读取整个文件
来源：http://fz.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cc.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://xa.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oe.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pk.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tp.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ei.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://zv.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://kr.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://jp.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://od.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zt.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ie.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ew.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ay.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iy.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://be.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xk.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ss.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mz.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ii.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xo.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qd.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kw.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ve.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://lf.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bg.jctech888.com.cn

[F04] 追加写入文件
来源：http://bo.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dn.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pc.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fd.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jq.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ht.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://op.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qu.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iw.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://eo.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mk.521024.cn

PHP:  file_exists("a.txt");
来源：http://dk.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://mb.haigaiapp.cn


<!-- 参考信息 -->