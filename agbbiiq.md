代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yk.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://ue.shtwfgs.cn

[D17] 最大值与最小值
来源：http://cb.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://af.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://gy.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fu.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://in.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://si.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ne.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://gb.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ey.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://gc.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mu.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://ho.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vb.9csxet.cn

TS:   nested.flat();
来源：http://pj.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xp.shxzskj.cn

Go:   // 手写双层循环
来源：http://px.gzmigu.cn

Ruby: nested.flatten
来源：http://uz.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cl.haigaiapp.cn

[D19] 按字段分组
来源：http://sr.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://la.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fr.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://et.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qx.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ll.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://iw.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tq.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zk.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://jb.shtwfgs.cn

Py:   Counter(arr)
来源：http://mx.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://up.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wk.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pj.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yp.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://zg.huixinmuqiang.cn

Ruby: arr.tally
来源：http://wk.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bg.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://lh.nicolike.cn

Py:   x in arr
来源：http://un.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://fa.jctech888.com.cn

JS:   arr.includes(x)
来源：http://wo.shtwfgs.cn

TS:   arr.includes(x)
来源：http://qc.jianghongdianzi.cn

Java: list.contains(x)
来源：http://fr.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://ks.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://sy.nszjky.cn

C#:   list.Contains(x)
来源：http://ma.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://xb.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ug.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tv.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vu.wgjwhj.cn

TS:   [...arr];
来源：http://jo.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://bm.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://az.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://be.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://zk.colortex.cn

[D23] reduce 累积计算
来源：http://hh.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xv.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pn.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mr.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bt.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pp.hahajie.cn

Go:   // 手写循环
来源：http://oo.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tw.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fq.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://ad.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kd.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yt.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uu.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cu.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://da.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zd.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gc.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lk.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://nn.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gt.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fe.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uc.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cv.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tm.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tm.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wq.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://em.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://wd.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://qn.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://bo.chemitech.net.cn

JS:   arr.join(", ")
来源：http://uo.hnjuh.cn

TS:   arr.join(", ")
来源：http://nj.nicolike.cn

Java: String.join(", ", list)
来源：http://ee.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://qz.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://am.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://xg.yuntaijiaju.cn

================================================================================
来源：http://kb.hahajie.cn

E. 字符串处理
来源：http://el.shxzukj.cn

================================================================================
来源：http://ud.bjjhwx.cn

[E01] 拼接字符串
来源：http://kr.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kh.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://my.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lh.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ij.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ku.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eq.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wy.hnjuh.cn

[E02] 重复字符串
来源：http://ez.lnxyls.cn

Py:   "ab" * 3
来源：http://rc.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://aw.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://al.asd995.cn

TS:   "ab".repeat(3)
来源：http://mv.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ub.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://qu.gzmigu.cn

Ruby: "ab" * 3
来源：http://ys.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lw.nicolike.cn

[E03] 截取子串
来源：http://zz.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cb.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xd.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vf.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://ad.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://br.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bi.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nr.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://zl.newstarts.cn

[E04] 查找子串位置
来源：http://qc.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://fz.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://sg.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ka.szxytkj.cn

TS:   s.indexOf("x")
来源：http://mm.jctech888.com.cn

Java: s.indexOf("x")
来源：http://ps.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://sn.shxzukj.cn

Ruby: s.index("x")
来源：http://vv.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://tc.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ms.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hk.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ru.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cs.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://el.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dx.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fp.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hg.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qw.muxihuayi.cn

[E06] 替换子串
来源：http://ty.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ar.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://bx.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zo.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://gn.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://un.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sv.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cf.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://me.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://vi.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pn.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dc.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pz.9csxet.cn

TS:   s.split(",")
来源：http://mv.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xl.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fe.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://yq.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tg.newstarts.cn

[E08] 数组按分隔符合并
来源：http://eg.panjiajie.cn

Py:   ",".join(items)
来源：http://pp.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://oy.jctech888.com.cn

JS:   items.join(",")
来源：http://ug.bjjhwx.cn

TS:   items.join(",")
来源：http://jp.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://im.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://sa.hnjuh.cn

Ruby: items.join(",")
来源：http://le.gzmigu.cn

C#:   string.Join(",", items)
来源：http://tx.hnjuh.cn

[E09] 去除所有空白字符
来源：http://bm.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gq.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ll.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://uv.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://rs.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://ew.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ln.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zk.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ic.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://ft.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vt.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nm.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://gn.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://ry.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://oz.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zq.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dk.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cs.nicolike.cn

[E11] 反转字符串
来源：http://yi.newstarts.cn

Py:   s[::-1]
来源：http://qt.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://fz.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://fi.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://qh.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gj.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ks.huanxung.cn

Ruby: s.reverse
来源：http://rj.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ew.huanxung.cn

[E12] 统计某字符出现次数
来源：http://qz.nicolike.cn

Py:   s.count("a")
来源：http://re.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://sl.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://vq.nicolike.cn

TS:   s.split("a").length - 1
来源：http://yq.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ng.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://kh.hnjuh.cn

Ruby: s.count("a")
来源：http://ny.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://yr.szxytkj.cn

[E13] 逐字符遍历
来源：http://rt.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://zq.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iu.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ey.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ei.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tu.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kl.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oc.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hr.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ay.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xh.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nv.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dr.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tg.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ml.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://em.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xl.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ec.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://bp.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ny.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ce.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kv.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gt.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ws.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://th.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pv.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lo.lnxyls.cn

[E16] 数字千分位
来源：http://se.nicolike.cn

Py:   f"{1234567:,}"
来源：http://oa.shxzskj.cn

PHP:  number_format(1234567);
来源：http://cs.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wv.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qx.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uy.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hf.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xd.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://px.jctech888.com.cn

[E17] 首字母大写
来源：http://ad.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bd.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aw.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tm.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vj.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xo.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://db.newstarts.cn

Ruby: s.capitalize
来源：http://es.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yg.shxzukj.cn

[E18] 模板占位符替换
来源：http://ow.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://df.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wj.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uv.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ru.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kc.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://to.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qj.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gs.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://au.bjjhwx.cn

Py:   s.splitlines()
来源：http://sp.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://up.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://mq.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://ec.huanxung.cn

Java: s.lines().toList()
来源：http://jp.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://bc.panjiajie.cn

Ruby: s.lines
来源：http://oh.jctech888.com.cn

C#:   s.Split('\n')
来源：http://ef.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://bt.wgjwhj.cn

Py:   if not s:
来源：http://js.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yk.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mx.wgjwhj.cn

TS:   if (s === "") {}
来源：http://gb.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://up.huanxung.cn

Go:   if s == "" {}
来源：http://ta.asd995.cn

Ruby: if s.empty?
来源：http://ow.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tt.gzmigu.cn

[E21] 超长截断加省略号
来源：http://yj.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sj.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xv.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://er.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fn.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ku.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://cy.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oe.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://he.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://mg.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fg.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xu.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iq.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ni.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gh.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gm.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://qp.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ph.wgjwhj.cn

================================================================================
来源：http://cx.bjjhwx.cn

F. 文件与目录
来源：http://sv.shxzukj.cn

================================================================================
来源：http://hv.nicolike.cn

[F01] 读取整个文件
来源：http://nd.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bl.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://lr.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dt.colortex.cn


<!-- 参考信息 -->