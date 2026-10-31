代发 wailian999

[D19] 按字段分组
来源：http://eu.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nm.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qd.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cb.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ad.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sa.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://sp.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ir.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dz.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://zw.chemitech.net.cn

Py:   Counter(arr)
来源：http://sw.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://il.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eo.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hv.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ue.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://wx.521024.cn

Ruby: arr.tally
来源：http://ej.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wh.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://tn.lnxyls.cn

Py:   x in arr
来源：http://zl.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://lt.muxihuayi.cn

JS:   arr.includes(x)
来源：http://zw.asd995.cn

TS:   arr.includes(x)
来源：http://to.gzmigu.cn

Java: list.contains(x)
来源：http://yx.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://nx.nszjky.cn

Ruby: arr.include?(x)
来源：http://sq.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://gw.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://ad.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qb.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gx.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jy.lnxyls.cn

TS:   [...arr];
来源：http://le.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://mj.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ze.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://cu.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://zi.newstarts.cn

[D23] reduce 累积计算
来源：http://ht.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oj.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ef.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ku.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yn.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ba.shxzskj.cn

Go:   // 手写循环
来源：http://zn.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://is.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mh.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://ul.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bl.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wd.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bp.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wt.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://as.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hl.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kg.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pt.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://nu.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tn.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ov.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ec.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ji.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sj.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jh.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uy.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cu.521024.cn

[D26] 数组转字符串
来源：http://jt.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://vm.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://kg.gzmigu.cn

JS:   arr.join(", ")
来源：http://cv.asd995.cn

TS:   arr.join(", ")
来源：http://tc.shxzukj.cn

Java: String.join(", ", list)
来源：http://dc.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://vl.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://in.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://wt.lnxyls.cn

================================================================================
来源：http://uy.shxzskj.cn

E. 字符串处理
来源：http://oy.9csxet.cn

================================================================================
来源：http://ma.gzmigu.cn

[E01] 拼接字符串
来源：http://lu.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fj.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nm.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ln.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ap.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sr.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gz.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lq.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://he.shxzskj.cn

[E02] 重复字符串
来源：http://pf.huixiangedu.cn

Py:   "ab" * 3
来源：http://cv.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://cd.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://qc.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://mc.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://ys.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://gb.jctech888.com.cn

Ruby: "ab" * 3
来源：http://gr.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lw.521024.cn

[E03] 截取子串
来源：http://ig.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ej.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yr.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ij.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://um.nicolike.cn

Java: s.substring(1, 4)
来源：http://kg.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mc.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://th.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://fu.hnjuh.cn

[E04] 查找子串位置
来源：http://tg.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://xn.hahajie.cn

PHP:  strpos($s, "x");
来源：http://oe.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bm.lnxyls.cn

TS:   s.indexOf("x")
来源：http://kf.gzmigu.cn

Java: s.indexOf("x")
来源：http://oj.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ex.nszjky.cn

Ruby: s.index("x")
来源：http://ku.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://xq.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kl.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://le.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fd.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gz.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://in.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sk.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pj.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bk.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://po.szsharing.cn

[E06] 替换子串
来源：http://ad.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gz.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ur.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://df.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://hd.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ry.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sp.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qn.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://cq.huanxung.cn

[E07] 按分隔符拆分
来源：http://tr.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ug.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ph.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sx.hahajie.cn

TS:   s.split(",")
来源：http://co.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dq.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wy.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://pp.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ly.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://oc.wgjwhj.cn

Py:   ",".join(items)
来源：http://gv.nszjky.cn

PHP:  implode(",", $items);
来源：http://th.chemitech.net.cn

JS:   items.join(",")
来源：http://bl.nicolike.cn

TS:   items.join(",")
来源：http://ck.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://qm.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://bp.nicolike.cn

Ruby: items.join(",")
来源：http://xy.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://hl.colortex.cn

[E09] 去除所有空白字符
来源：http://dr.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://az.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ay.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://sw.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://ul.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://fe.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ao.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fq.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vx.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://mc.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://su.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ou.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ks.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://tn.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://ja.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nw.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yj.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iy.huixiangedu.cn

[E11] 反转字符串
来源：http://vk.chemitech.net.cn

Py:   s[::-1]
来源：http://xl.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://tm.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://dz.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://rv.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oy.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ah.szsharing.cn

Ruby: s.reverse
来源：http://xv.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vh.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://lb.wgjwhj.cn

Py:   s.count("a")
来源：http://py.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://bj.nicolike.cn

JS:   s.split("a").length - 1
来源：http://wa.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://le.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://up.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://wv.szsharing.cn

Ruby: s.count("a")
来源：http://ji.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://gz.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://km.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://rl.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ee.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gd.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qu.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gv.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fi.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ii.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ch.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://zy.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bt.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gu.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zs.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zg.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wm.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jo.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ta.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dk.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://yk.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://he.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://im.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iv.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zf.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kb.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wh.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qd.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vp.muxihuayi.cn

[E16] 数字千分位
来源：http://cp.szsharing.cn

Py:   f"{1234567:,}"
来源：http://vp.asd995.cn

PHP:  number_format(1234567);
来源：http://tv.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://th.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ae.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ub.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://id.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mi.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://tr.nszjky.cn

[E17] 首字母大写
来源：http://ju.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lf.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sa.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ct.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oj.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hj.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ai.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ur.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lk.hahajie.cn

[E18] 模板占位符替换
来源：http://ev.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kx.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ls.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://en.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wp.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sh.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xa.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aj.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lc.nicolike.cn

[E19] 多行文本按行拆分
来源：http://dg.szsharing.cn

Py:   s.splitlines()
来源：http://er.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://db.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://qj.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://sn.huixiangedu.cn

Java: s.lines().toList()
来源：http://hm.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://cj.jctech888.com.cn

Ruby: s.lines
来源：http://lx.panjiajie.cn

C#:   s.Split('\n')
来源：http://wz.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://pv.lnxyls.cn

Py:   if not s:
来源：http://kv.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cg.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mz.nszjky.cn

TS:   if (s === "") {}
来源：http://cv.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://lj.chemitech.net.cn

Go:   if s == "" {}
来源：http://aa.shtwfgs.cn

Ruby: if s.empty?
来源：http://hz.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hn.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://uz.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qg.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bi.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iy.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eh.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://we.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://vd.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://he.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dz.szsharing.cn

[E22] 字节长度与字符长度
来源：http://um.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cm.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://od.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ra.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tm.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ch.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aw.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://ut.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://df.wgjwhj.cn

================================================================================
来源：http://rn.jctech888.com.cn

F. 文件与目录
来源：http://os.yuexingan06.cn

================================================================================
来源：http://yu.huixiangedu.cn

[F01] 读取整个文件
来源：http://ao.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ti.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://qs.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wr.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dl.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hb.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cf.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://kw.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ek.chemitech.net.cn

[F02] 逐行读取文件
来源：http://bm.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://to.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://av.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lk.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bh.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uw.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jn.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sj.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uw.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://td.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://we.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rr.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gj.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fr.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ib.shtwfgs.cn


<!-- 参考信息 -->