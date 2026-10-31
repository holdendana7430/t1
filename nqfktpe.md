代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://zm.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ss.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://ln.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ge.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dy.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://bl.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://oa.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://hh.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tb.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://yd.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xj.huanxung.cn

TS:   nested.flat();
来源：http://ct.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qg.gzmigu.cn

Go:   // 手写双层循环
来源：http://nb.jctech888.com.cn

Ruby: nested.flatten
来源：http://ch.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rv.huixiangedu.cn

[D19] 按字段分组
来源：http://hd.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wq.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ir.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sc.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vl.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wf.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://bi.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lh.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yp.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://wv.jctech888.com.cn

Py:   Counter(arr)
来源：http://ri.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://if.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hj.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cg.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://on.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://bp.nszjky.cn

Ruby: arr.tally
来源：http://zm.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://up.nszjky.cn

[D21] 判断是否包含某元素
来源：http://ai.jianghongdianzi.cn

Py:   x in arr
来源：http://dy.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://bb.521024.cn

JS:   arr.includes(x)
来源：http://de.bjjhwx.cn

TS:   arr.includes(x)
来源：http://jb.shtwfgs.cn

Java: list.contains(x)
来源：http://gd.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://ws.colortex.cn

Ruby: arr.include?(x)
来源：http://pa.gzmigu.cn

C#:   list.Contains(x)
来源：http://tt.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://lj.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qh.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fc.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gy.yuexingan06.cn

TS:   [...arr];
来源：http://ou.szsharing.cn

Java: new ArrayList<>(list);
来源：http://yb.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fj.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://ez.gzmigu.cn

C#:   new List<int>(list);
来源：http://yv.newstarts.cn

[D23] reduce 累积计算
来源：http://vy.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wt.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ja.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nf.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mb.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tf.gzmigu.cn

Go:   // 手写循环
来源：http://cy.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kn.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cg.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://vb.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rd.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nw.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gt.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wc.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ri.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qd.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wl.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yk.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://lg.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ih.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zp.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gq.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ti.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uw.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wz.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uk.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hb.colortex.cn

[D26] 数组转字符串
来源：http://vl.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://fk.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://iw.shxzskj.cn

JS:   arr.join(", ")
来源：http://uc.szsharing.cn

TS:   arr.join(", ")
来源：http://um.hahajie.cn

Java: String.join(", ", list)
来源：http://zh.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://ne.hahajie.cn

Ruby: arr.join(", ")
来源：http://ke.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://bm.lnxyls.cn

================================================================================
来源：http://lf.wgjwhj.cn

E. 字符串处理
来源：http://op.huixinmuqiang.cn

================================================================================
来源：http://ms.nszjky.cn

[E01] 拼接字符串
来源：http://co.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nv.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ax.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ao.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bf.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://md.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yk.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zv.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nh.wgjwhj.cn

[E02] 重复字符串
来源：http://lw.panjiajie.cn

Py:   "ab" * 3
来源：http://fc.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://ox.huanxung.cn

JS:   "ab".repeat(3)
来源：http://cf.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://xy.asd995.cn

Java: "ab".repeat(3)
来源：http://bt.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://aq.newstarts.cn

Ruby: "ab" * 3
来源：http://hk.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ch.yuntaijiaju.cn

[E03] 截取子串
来源：http://pm.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iu.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ru.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fc.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://ia.szsharing.cn

Java: s.substring(1, 4)
来源：http://dx.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sf.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ww.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://on.nszjky.cn

[E04] 查找子串位置
来源：http://fx.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ls.szsharing.cn

PHP:  strpos($s, "x");
来源：http://xf.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ck.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://lt.shxzukj.cn

Java: s.indexOf("x")
来源：http://uc.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://oq.szxytkj.cn

Ruby: s.index("x")
来源：http://yh.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://ek.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ki.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zi.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://in.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mz.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tz.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gy.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ht.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://br.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lt.hahajie.cn

[E06] 替换子串
来源：http://cp.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://av.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://iy.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lc.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ic.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kf.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ta.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sa.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://kv.hnjuh.cn

[E07] 按分隔符拆分
来源：http://wr.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bb.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cf.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sq.muxihuayi.cn

TS:   s.split(",")
来源：http://jn.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cu.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wh.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://jd.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://za.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://gr.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://gy.colortex.cn

PHP:  implode(",", $items);
来源：http://vu.muxihuayi.cn

JS:   items.join(",")
来源：http://lm.szxytkj.cn

TS:   items.join(",")
来源：http://gw.lnxyls.cn

Java: String.join(",", items)
来源：http://ex.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://da.muxihuayi.cn

Ruby: items.join(",")
来源：http://zf.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://vq.521024.cn

[E09] 去除所有空白字符
来源：http://ab.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cv.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jt.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://pj.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://rs.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://vq.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vo.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fy.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fo.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://fe.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zu.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ak.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://xp.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://tw.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://ow.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lp.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ts.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dt.shxzskj.cn

[E11] 反转字符串
来源：http://rl.bookmarksfly.cn

Py:   s[::-1]
来源：http://ui.nicolike.cn

PHP:  strrev($s);
来源：http://pq.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://xi.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://rm.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xk.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ki.521024.cn

Ruby: s.reverse
来源：http://tt.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cz.nicolike.cn

[E12] 统计某字符出现次数
来源：http://yv.nszjky.cn

Py:   s.count("a")
来源：http://if.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://cc.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://og.nszjky.cn

TS:   s.split("a").length - 1
来源：http://cd.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gd.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://pm.wgjwhj.cn

Ruby: s.count("a")
来源：http://ly.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://jb.huixiangedu.cn

[E13] 逐字符遍历
来源：http://ai.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://wa.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iv.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xh.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kc.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ev.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://og.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ph.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vi.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://ll.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vv.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rd.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yi.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jc.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jt.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ko.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iz.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zo.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://of.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xm.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lb.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kz.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ha.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gv.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ei.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lr.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ec.colortex.cn

[E16] 数字千分位
来源：http://ye.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://zg.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://mz.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hv.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jh.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mj.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cg.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fh.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://pi.shxzukj.cn

[E17] 首字母大写
来源：http://cl.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vs.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ta.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kn.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ez.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dr.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vr.newstarts.cn

Ruby: s.capitalize
来源：http://cx.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cf.shtwfgs.cn

[E18] 模板占位符替换
来源：http://tt.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ni.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://su.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ep.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://th.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dq.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lr.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oe.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ei.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://mh.gzmigu.cn

Py:   s.splitlines()
来源：http://of.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vo.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://bt.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://lo.panjiajie.cn

Java: s.lines().toList()
来源：http://bs.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://rw.szsharing.cn

Ruby: s.lines
来源：http://kh.shtwfgs.cn

C#:   s.Split('\n')
来源：http://en.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://wv.muxihuayi.cn

Py:   if not s:
来源：http://cg.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ky.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xk.lnxyls.cn

TS:   if (s === "") {}
来源：http://tr.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://vi.szsharing.cn

Go:   if s == "" {}
来源：http://lp.huanxung.cn

Ruby: if s.empty?
来源：http://bi.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ms.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://gf.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ru.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oo.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wi.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ri.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wr.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://vs.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zf.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ve.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://tg.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bl.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gq.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oy.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mb.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xg.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wd.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://dx.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ff.nszjky.cn

================================================================================
来源：http://rd.muxihuayi.cn

F. 文件与目录
来源：http://nq.huixinmuqiang.cn

================================================================================
来源：http://so.hnjuh.cn

[F01] 读取整个文件
来源：http://uh.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qe.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://sg.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bg.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://in.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://as.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ku.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://hf.wgjwhj.cn


<!-- 参考信息 -->