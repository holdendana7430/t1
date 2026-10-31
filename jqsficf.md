代发 wailian999

TS:   [...new Set(arr)]
来源：http://tj.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bx.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ow.chemitech.net.cn

Ruby: arr.uniq
来源：http://di.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://qi.szsharing.cn

[D16] 求和与平均值
来源：http://nv.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fq.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fh.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wg.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fg.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cm.nicolike.cn

Go:   // 手写循环累加
来源：http://mi.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://au.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://ru.gzmigu.cn

[D17] 最大值与最小值
来源：http://ld.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://fc.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://op.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hn.colortex.cn

TS:   Math.max(...arr);
来源：http://fx.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xr.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dk.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://fg.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://rc.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://wi.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ye.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://wr.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sp.panjiajie.cn

TS:   nested.flat();
来源：http://ga.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pk.jctech888.com.cn

Go:   // 手写双层循环
来源：http://ux.lnxyls.cn

Ruby: nested.flatten
来源：http://ku.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hq.jctech888.com.cn

[D19] 按字段分组
来源：http://bc.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gu.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gi.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lp.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gx.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bt.521024.cn

Go:   // 手写 map[string][]T
来源：http://nb.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ek.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jj.colortex.cn

[D20] 统计每个元素出现次数
来源：http://hs.bookmarksfly.cn

Py:   Counter(arr)
来源：http://gb.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://vj.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zi.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bi.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ir.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://mv.gzmigu.cn

Ruby: arr.tally
来源：http://tv.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://li.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://yo.shxzukj.cn

Py:   x in arr
来源：http://yp.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://ne.wgjwhj.cn

JS:   arr.includes(x)
来源：http://pn.shxzukj.cn

TS:   arr.includes(x)
来源：http://rx.shtwfgs.cn

Java: list.contains(x)
来源：http://xs.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://yv.gzmigu.cn

Ruby: arr.include?(x)
来源：http://gp.521024.cn

C#:   list.Contains(x)
来源：http://ph.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://wr.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cy.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rd.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rn.newstarts.cn

TS:   [...arr];
来源：http://pk.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://hk.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pt.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://xk.nicolike.cn

C#:   new List<int>(list);
来源：http://rs.huanxung.cn

[D23] reduce 累积计算
来源：http://db.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kk.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bt.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tw.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nh.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mx.jianghongdianzi.cn

Go:   // 手写循环
来源：http://wq.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wb.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ws.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://pe.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zy.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jo.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fr.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zz.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pm.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ib.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://om.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nr.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://qa.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pm.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://az.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vm.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pw.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jj.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://no.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sd.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iw.asd995.cn

[D26] 数组转字符串
来源：http://ck.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://ny.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://qx.huixiangedu.cn

JS:   arr.join(", ")
来源：http://st.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://hh.bjjhwx.cn

Java: String.join(", ", list)
来源：http://ot.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://ra.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://dq.colortex.cn

C#:   string.Join(", ", list)
来源：http://ke.shxzukj.cn

================================================================================
来源：http://tt.muxihuayi.cn

E. 字符串处理
来源：http://zx.jctech888.com.cn

================================================================================
来源：http://cz.nicolike.cn

[E01] 拼接字符串
来源：http://be.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ec.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fa.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dz.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ou.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ck.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yx.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zj.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dv.szsharing.cn

[E02] 重复字符串
来源：http://sg.521024.cn

Py:   "ab" * 3
来源：http://mk.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://ja.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://bx.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://eb.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://xf.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://er.colortex.cn

Ruby: "ab" * 3
来源：http://fq.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yf.521024.cn

[E03] 截取子串
来源：http://zx.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vv.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ul.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ti.szsharing.cn

TS:   s.slice(1, 4)
来源：http://qp.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://je.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gk.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://km.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://ie.nicolike.cn

[E04] 查找子串位置
来源：http://yu.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://xg.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://gs.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://at.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://py.huixiangedu.cn

Java: s.indexOf("x")
来源：http://ln.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://it.lnxyls.cn

Ruby: s.index("x")
来源：http://ku.szsharing.cn

C#:   s.IndexOf("x")
来源：http://jw.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jb.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ul.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wg.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://il.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tf.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lq.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ym.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tn.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tv.shxzukj.cn

[E06] 替换子串
来源：http://sx.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yu.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://rs.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sf.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://mj.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mb.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://st.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oz.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://kd.panjiajie.cn

[E07] 按分隔符拆分
来源：http://id.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qu.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zl.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://id.newstarts.cn

TS:   s.split(",")
来源：http://yt.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ys.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mr.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://xe.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qe.newstarts.cn

[E08] 数组按分隔符合并
来源：http://cm.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://po.shxzukj.cn

PHP:  implode(",", $items);
来源：http://rj.szxytkj.cn

JS:   items.join(",")
来源：http://kv.jctech888.com.cn

TS:   items.join(",")
来源：http://rt.9csxet.cn

Java: String.join(",", items)
来源：http://xx.colortex.cn

Go:   strings.Join(items, ",")
来源：http://ww.shtwfgs.cn

Ruby: items.join(",")
来源：http://yf.colortex.cn

C#:   string.Join(",", items)
来源：http://dk.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://xq.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qg.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dy.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://nc.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://kc.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://pm.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nl.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fk.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zw.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ib.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dm.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lb.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://jg.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://vi.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://ba.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jv.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ve.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jk.jianghongdianzi.cn

[E11] 反转字符串
来源：http://eo.newstarts.cn

Py:   s[::-1]
来源：http://vu.szsharing.cn

PHP:  strrev($s);
来源：http://bb.521024.cn

JS:   [...s].reverse().join("")
来源：http://hc.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://ix.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ft.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ha.wgjwhj.cn

Ruby: s.reverse
来源：http://ir.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vw.szsharing.cn

[E12] 统计某字符出现次数
来源：http://fv.jctech888.com.cn

Py:   s.count("a")
来源：http://pz.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://es.huanxung.cn

JS:   s.split("a").length - 1
来源：http://nu.colortex.cn

TS:   s.split("a").length - 1
来源：http://wv.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pl.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://oj.wgjwhj.cn

Ruby: s.count("a")
来源：http://jw.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://ad.huixiangedu.cn

[E13] 逐字符遍历
来源：http://eu.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://to.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wd.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tr.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jt.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hw.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ci.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aq.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kl.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://py.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ll.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lb.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ee.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wr.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yz.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yz.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uz.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rl.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://op.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lj.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://st.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://by.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tz.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ul.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zq.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eb.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fm.panjiajie.cn

[E16] 数字千分位
来源：http://bw.521024.cn

Py:   f"{1234567:,}"
来源：http://kl.huanxung.cn

PHP:  number_format(1234567);
来源：http://fb.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ic.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://po.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mv.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qf.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uw.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://ag.muxihuayi.cn

[E17] 首字母大写
来源：http://vl.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wg.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qc.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uo.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lf.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cq.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ep.newstarts.cn

Ruby: s.capitalize
来源：http://zw.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sv.521024.cn

[E18] 模板占位符替换
来源：http://nj.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eu.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zd.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ht.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nr.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nf.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oq.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ok.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eo.colortex.cn

[E19] 多行文本按行拆分
来源：http://rm.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://vh.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rz.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://yu.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://pr.chemitech.net.cn

Java: s.lines().toList()
来源：http://ut.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://so.muxihuayi.cn

Ruby: s.lines
来源：http://em.szxytkj.cn

C#:   s.Split('\n')
来源：http://kv.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://so.hnjuh.cn

Py:   if not s:
来源：http://vy.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lt.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tr.haigaiapp.cn

TS:   if (s === "") {}
来源：http://xq.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://uk.panjiajie.cn

Go:   if s == "" {}
来源：http://ci.huanxung.cn

Ruby: if s.empty?
来源：http://fw.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nr.szsharing.cn

[E21] 超长截断加省略号
来源：http://oe.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qi.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://db.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qh.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tl.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oo.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://zi.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://al.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wq.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://nh.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dq.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rd.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ca.nicolike.cn


<!-- 参考信息 -->