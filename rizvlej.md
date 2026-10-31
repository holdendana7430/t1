代发 wailian999

Ruby: arr.tally
来源：http://rv.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tr.szsharing.cn

[D21] 判断是否包含某元素
来源：http://qy.bookmarksfly.cn

Py:   x in arr
来源：http://nl.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://se.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://rl.nszjky.cn

TS:   arr.includes(x)
来源：http://ua.shxzukj.cn

Java: list.contains(x)
来源：http://bb.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://dn.asd995.cn

Ruby: arr.include?(x)
来源：http://ae.gzmigu.cn

C#:   list.Contains(x)
来源：http://eq.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://bv.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://an.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jh.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pl.panjiajie.cn

TS:   [...arr];
来源：http://dh.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://md.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nz.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://jd.shtwfgs.cn

C#:   new List<int>(list);
来源：http://ev.nicolike.cn

[D23] reduce 累积计算
来源：http://xf.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gl.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jv.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qc.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cj.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://do.huanxung.cn

Go:   // 手写循环
来源：http://zi.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://up.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fm.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://kf.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tq.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ay.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fp.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oj.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://at.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sv.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qp.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://qy.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fc.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ng.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ii.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qs.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mz.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iy.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tt.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kw.huixiangedu.cn

[D26] 数组转字符串
来源：http://pe.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://vk.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://rb.hahajie.cn

JS:   arr.join(", ")
来源：http://eg.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ey.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://ew.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://qv.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://dr.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://aa.9csxet.cn

================================================================================
来源：http://oc.bookmarksfly.cn

E. 字符串处理
来源：http://vi.muxihuayi.cn

================================================================================
来源：http://zq.szxytkj.cn

[E01] 拼接字符串
来源：http://bb.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yw.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yb.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wv.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://af.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dv.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jv.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ou.chemitech.net.cn

[E02] 重复字符串
来源：http://bv.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://iw.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://gy.hahajie.cn

JS:   "ab".repeat(3)
来源：http://pl.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://ud.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://lk.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://eo.muxihuayi.cn

Ruby: "ab" * 3
来源：http://fk.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nh.szsharing.cn

[E03] 截取子串
来源：http://uc.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cg.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yh.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://of.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://dc.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://ns.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ae.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://is.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://sl.asd995.cn

[E04] 查找子串位置
来源：http://es.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://nb.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://cl.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lp.shxzukj.cn

TS:   s.indexOf("x")
来源：http://ri.521024.cn

Java: s.indexOf("x")
来源：http://iv.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://mg.hahajie.cn

Ruby: s.index("x")
来源：http://yq.colortex.cn

C#:   s.IndexOf("x")
来源：http://ni.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://as.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ay.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fr.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rz.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fu.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wr.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bh.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nt.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oi.huanxung.cn

[E06] 替换子串
来源：http://wg.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://go.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://vn.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ao.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://st.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eu.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ca.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rq.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://bi.newstarts.cn

[E07] 按分隔符拆分
来源：http://vl.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qj.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lw.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iw.szxytkj.cn

TS:   s.split(",")
来源：http://ff.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rk.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bj.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ne.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rc.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://nn.newstarts.cn

Py:   ",".join(items)
来源：http://ev.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://hm.muxihuayi.cn

JS:   items.join(",")
来源：http://vg.nszjky.cn

TS:   items.join(",")
来源：http://zg.muxihuayi.cn

Java: String.join(",", items)
来源：http://nx.521024.cn

Go:   strings.Join(items, ",")
来源：http://be.wgjwhj.cn

Ruby: items.join(",")
来源：http://gw.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://ao.szsharing.cn

[E09] 去除所有空白字符
来源：http://wk.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rl.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pj.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://vv.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://en.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://pw.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zu.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://es.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vs.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://ci.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ey.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eu.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://nl.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://qx.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://gu.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kq.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://go.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ar.chemitech.net.cn

[E11] 反转字符串
来源：http://ko.521024.cn

Py:   s[::-1]
来源：http://sd.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://sx.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://vs.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://uh.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yf.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tj.bjjhwx.cn

Ruby: s.reverse
来源：http://kh.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hx.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://qq.wgjwhj.cn

Py:   s.count("a")
来源：http://rb.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://to.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://yn.nicolike.cn

TS:   s.split("a").length - 1
来源：http://yw.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hd.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://bz.wgjwhj.cn

Ruby: s.count("a")
来源：http://fc.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://ko.yuexingan06.cn

[E13] 逐字符遍历
来源：http://gk.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://mh.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jc.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kb.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xo.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bc.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://go.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sy.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tu.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://nu.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nu.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dp.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://js.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bd.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ve.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://an.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hf.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hb.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://xm.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ab.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wn.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://si.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://om.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wl.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ww.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pl.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xc.szsharing.cn

[E16] 数字千分位
来源：http://rl.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://rz.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://mr.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jn.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nq.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wd.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xs.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qh.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://mm.yuexingan06.cn

[E17] 首字母大写
来源：http://nv.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://of.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ff.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://or.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qv.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gp.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rx.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://hc.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ws.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://qv.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://er.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nf.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ma.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kp.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pa.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://er.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ap.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dz.colortex.cn

[E19] 多行文本按行拆分
来源：http://fu.haigaiapp.cn

Py:   s.splitlines()
来源：http://ym.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hn.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://up.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://dp.hnjuh.cn

Java: s.lines().toList()
来源：http://it.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://za.521024.cn

Ruby: s.lines
来源：http://cz.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://tt.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://ya.shxzukj.cn

Py:   if not s:
来源：http://js.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mk.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ox.chemitech.net.cn

TS:   if (s === "") {}
来源：http://rw.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://ee.gzmigu.cn

Go:   if s == "" {}
来源：http://yv.gzmigu.cn

Ruby: if s.empty?
来源：http://ct.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gl.szsharing.cn

[E21] 超长截断加省略号
来源：http://cn.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mc.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zg.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rz.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eg.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dq.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://hw.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fo.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://at.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://vx.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pq.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eu.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fw.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xe.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hc.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yl.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://ik.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mq.nicolike.cn

================================================================================
来源：http://vp.gzmigu.cn

F. 文件与目录
来源：http://tp.szxytkj.cn

================================================================================
来源：http://yw.huanxung.cn

[F01] 读取整个文件
来源：http://md.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eu.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://qf.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pg.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fx.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nk.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gh.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://bx.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://yv.jctech888.com.cn

[F02] 逐行读取文件
来源：http://lr.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ka.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gu.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dn.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ha.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ad.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kd.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ya.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zq.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://su.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zv.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tl.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ys.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tw.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xg.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ax.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://wg.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mo.nicolike.cn

[F04] 追加写入文件
来源：http://xx.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dz.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nj.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wm.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pa.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wm.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yi.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nu.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ql.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://yt.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gx.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://jd.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://pi.bookmarksfly.cn


<!-- 参考信息 -->