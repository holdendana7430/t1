代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wf.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://ay.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://cu.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://gk.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ea.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://pz.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rm.asd995.cn

TS:   nested.flat();
来源：http://ce.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rj.bjjhwx.cn

Go:   // 手写双层循环
来源：http://ez.huanxung.cn

Ruby: nested.flatten
来源：http://as.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ae.shxzskj.cn

[D19] 按字段分组
来源：http://qm.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wr.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rz.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cd.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wk.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xs.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://bh.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hg.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zd.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://fx.shxzskj.cn

Py:   Counter(arr)
来源：http://lo.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://kh.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gh.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://km.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ql.hahajie.cn

Go:   // 手写 map[T]int
来源：http://nr.szsharing.cn

Ruby: arr.tally
来源：http://tu.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ko.hahajie.cn

[D21] 判断是否包含某元素
来源：http://vr.wgjwhj.cn

Py:   x in arr
来源：http://hc.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://ny.hnjuh.cn

JS:   arr.includes(x)
来源：http://jx.muxihuayi.cn

TS:   arr.includes(x)
来源：http://mn.haigaiapp.cn

Java: list.contains(x)
来源：http://xa.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://mp.521024.cn

Ruby: arr.include?(x)
来源：http://bo.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://cn.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://bx.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ju.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ko.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://or.huanxung.cn

TS:   [...arr];
来源：http://vn.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://wr.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sq.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://fp.nicolike.cn

C#:   new List<int>(list);
来源：http://mw.hahajie.cn

[D23] reduce 累积计算
来源：http://xl.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zw.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uk.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jc.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cn.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cf.bookmarksfly.cn

Go:   // 手写循环
来源：http://bc.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hu.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yv.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://nq.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ap.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rc.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ox.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iw.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://om.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hh.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gu.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://il.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://vn.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pi.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dx.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hw.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://is.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zy.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fy.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gy.shtwfgs.cn

[D26] 数组转字符串
来源：http://ek.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://on.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://st.shxzskj.cn

JS:   arr.join(", ")
来源：http://vk.asd995.cn

TS:   arr.join(", ")
来源：http://be.huanxung.cn

Java: String.join(", ", list)
来源：http://jc.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://xy.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://kv.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://kt.521024.cn

================================================================================
来源：http://bv.nszjky.cn

E. 字符串处理
来源：http://dj.huixiangedu.cn

================================================================================
来源：http://ng.colortex.cn

[E01] 拼接字符串
来源：http://yy.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ts.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ij.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oc.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ku.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hu.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ny.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yo.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ej.shxzukj.cn

[E02] 重复字符串
来源：http://vd.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://ru.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://eb.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://to.newstarts.cn

TS:   "ab".repeat(3)
来源：http://kf.shxzskj.cn

Java: "ab".repeat(3)
来源：http://pe.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://hz.huanxung.cn

Ruby: "ab" * 3
来源：http://op.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mn.muxihuayi.cn

[E03] 截取子串
来源：http://be.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tf.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jw.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pl.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://dj.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://pv.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://po.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yq.colortex.cn

C#:   s.Substring(1, 3)
来源：http://cd.gzmigu.cn

[E04] 查找子串位置
来源：http://kb.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://cj.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ps.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ev.shxzukj.cn

TS:   s.indexOf("x")
来源：http://nl.521024.cn

Java: s.indexOf("x")
来源：http://jk.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://ei.gzmigu.cn

Ruby: s.index("x")
来源：http://nt.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://zy.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nh.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ou.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ny.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bd.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://su.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yi.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lw.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iz.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://im.jianghongdianzi.cn

[E06] 替换子串
来源：http://vs.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hk.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://je.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pb.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://yo.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kw.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xx.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qs.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://bj.szsharing.cn

[E07] 按分隔符拆分
来源：http://vh.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://au.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aa.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oo.muxihuayi.cn

TS:   s.split(",")
来源：http://jo.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hs.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lk.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://ma.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://js.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ho.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://af.asd995.cn

PHP:  implode(",", $items);
来源：http://ky.colortex.cn

JS:   items.join(",")
来源：http://qt.gzmigu.cn

TS:   items.join(",")
来源：http://qn.asd995.cn

Java: String.join(",", items)
来源：http://xf.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://zh.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://mx.9csxet.cn

C#:   string.Join(",", items)
来源：http://as.9csxet.cn

[E09] 去除所有空白字符
来源：http://ho.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dl.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tg.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://kb.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://pl.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://pt.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jm.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kb.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ea.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://gz.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qo.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sn.521024.cn

JS:   "7".padStart(3, "0")
来源：http://go.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://ya.nicolike.cn

Java: String.format("%03d", 7)
来源：http://si.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dt.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cn.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xh.szxytkj.cn

[E11] 反转字符串
来源：http://yv.huixiangedu.cn

Py:   s[::-1]
来源：http://vw.szxytkj.cn

PHP:  strrev($s);
来源：http://gl.colortex.cn

JS:   [...s].reverse().join("")
来源：http://la.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://ch.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://an.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ik.shxzskj.cn

Ruby: s.reverse
来源：http://zi.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vq.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://rn.haigaiapp.cn

Py:   s.count("a")
来源：http://hg.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://tl.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://vz.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://sf.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lc.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://dt.wgjwhj.cn

Ruby: s.count("a")
来源：http://vx.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://qh.shxzskj.cn

[E13] 逐字符遍历
来源：http://ho.521024.cn

Py:   for ch in s: print(ch)
来源：http://dm.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ul.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qn.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sa.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://if.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pq.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jt.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ey.huanxung.cn

[E14] URL 编码与 Base64
来源：http://bs.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gd.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pa.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lb.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ie.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fu.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://av.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zw.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jx.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ys.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://di.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kq.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yv.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yp.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bq.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yz.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ot.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ts.chemitech.net.cn

[E16] 数字千分位
来源：http://ir.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://qa.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://ba.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kk.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wm.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qf.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nq.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://so.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://hs.bookmarksfly.cn

[E17] 首字母大写
来源：http://bn.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jo.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sm.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ve.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lg.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://io.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vv.nicolike.cn

Ruby: s.capitalize
来源：http://yz.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rz.bjjhwx.cn

[E18] 模板占位符替换
来源：http://gj.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://is.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uq.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bt.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qz.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gs.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yx.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ot.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oa.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://cb.hnjuh.cn

Py:   s.splitlines()
来源：http://gx.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ba.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://cw.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://sz.jctech888.com.cn

Java: s.lines().toList()
来源：http://wx.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://wt.lnxyls.cn

Ruby: s.lines
来源：http://sq.shxzskj.cn

C#:   s.Split('\n')
来源：http://ef.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://mn.newstarts.cn

Py:   if not s:
来源：http://ry.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ds.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cx.521024.cn

TS:   if (s === "") {}
来源：http://yc.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://hq.gzmigu.cn

Go:   if s == "" {}
来源：http://ql.yuexingan06.cn

Ruby: if s.empty?
来源：http://gk.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://by.nszjky.cn

[E21] 超长截断加省略号
来源：http://gf.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ed.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fu.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qx.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ou.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rs.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://jp.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ex.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ti.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://np.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rc.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ig.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wh.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sd.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mp.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qt.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://um.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xy.bjjhwx.cn

================================================================================
来源：http://aq.szsharing.cn

F. 文件与目录
来源：http://jn.jianghongdianzi.cn

================================================================================
来源：http://mt.521024.cn

[F01] 读取整个文件
来源：http://wt.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uc.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ty.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fh.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sk.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fk.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dy.nszjky.cn

Ruby: File.read("a.txt")
来源：http://hs.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://hq.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://ao.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://na.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://or.huixiangedu.cn


<!-- 参考信息 -->