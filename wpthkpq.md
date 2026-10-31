代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://fm.colortex.cn

Go:   // 手写循环
来源：http://eb.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pe.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zf.hahajie.cn

[D15] 去重
来源：http://bs.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://db.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://md.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://ce.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ze.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gu.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hx.gzmigu.cn

Ruby: arr.uniq
来源：http://tu.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://oj.nicolike.cn

[D16] 求和与平均值
来源：http://dr.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kz.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tc.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ik.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ze.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kx.nicolike.cn

Go:   // 手写循环累加
来源：http://oj.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fl.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://wv.bjjhwx.cn

[D17] 最大值与最小值
来源：http://kn.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://ga.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://ap.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pc.nszjky.cn

TS:   Math.max(...arr);
来源：http://yw.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://si.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ej.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://zk.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://nr.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://mq.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ba.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://qe.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qr.shxzukj.cn

TS:   nested.flat();
来源：http://rg.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vv.nicolike.cn

Go:   // 手写双层循环
来源：http://bf.bjjhwx.cn

Ruby: nested.flatten
来源：http://hv.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ra.521024.cn

[D19] 按字段分组
来源：http://ni.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://al.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zs.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ys.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tg.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ck.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://gd.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sm.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://so.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://vc.yuexingan06.cn

Py:   Counter(arr)
来源：http://ke.newstarts.cn

PHP:  array_count_values($arr);
来源：http://gy.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sj.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dh.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yd.colortex.cn

Go:   // 手写 map[T]int
来源：http://mc.muxihuayi.cn

Ruby: arr.tally
来源：http://lw.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xg.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://jh.hahajie.cn

Py:   x in arr
来源：http://pi.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://ca.haigaiapp.cn

JS:   arr.includes(x)
来源：http://hv.521024.cn

TS:   arr.includes(x)
来源：http://bj.huixiangedu.cn

Java: list.contains(x)
来源：http://hx.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://zf.szxytkj.cn

Ruby: arr.include?(x)
来源：http://vq.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://ko.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://pp.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fc.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jp.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jf.shtwfgs.cn

TS:   [...arr];
来源：http://jn.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://zi.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nw.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://dc.lnxyls.cn

C#:   new List<int>(list);
来源：http://kr.asd995.cn

[D23] reduce 累积计算
来源：http://ht.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ls.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hu.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sl.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cl.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ih.hnjuh.cn

Go:   // 手写循环
来源：http://dj.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jq.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://to.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://fk.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tt.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://go.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qo.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jc.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vt.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hf.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aq.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tz.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://vk.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rw.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xx.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sj.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://up.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dt.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nb.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rf.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oq.huixiangedu.cn

[D26] 数组转字符串
来源：http://cv.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://hq.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://sp.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://ee.chemitech.net.cn

TS:   arr.join(", ")
来源：http://ze.jctech888.com.cn

Java: String.join(", ", list)
来源：http://vg.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://zq.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://hm.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://ru.bookmarksfly.cn

================================================================================
来源：http://es.hnjuh.cn

E. 字符串处理
来源：http://mj.hahajie.cn

================================================================================
来源：http://ev.huanxung.cn

[E01] 拼接字符串
来源：http://kh.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wn.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ht.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hg.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dx.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zq.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zy.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qs.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fj.bookmarksfly.cn

[E02] 重复字符串
来源：http://xi.hahajie.cn

Py:   "ab" * 3
来源：http://it.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ys.szsharing.cn

JS:   "ab".repeat(3)
来源：http://is.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://gl.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://bj.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://em.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://rf.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vg.newstarts.cn

[E03] 截取子串
来源：http://ik.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sm.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ao.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yh.newstarts.cn

TS:   s.slice(1, 4)
来源：http://vg.colortex.cn

Java: s.substring(1, 4)
来源：http://tk.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bc.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sv.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://ys.bjjhwx.cn

[E04] 查找子串位置
来源：http://qo.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://mq.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://ce.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tn.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://sx.colortex.cn

Java: s.indexOf("x")
来源：http://lj.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://pg.asd995.cn

Ruby: s.index("x")
来源：http://ig.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://wm.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tq.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cm.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zz.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zb.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gm.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://np.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iv.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dn.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ia.newstarts.cn

[E06] 替换子串
来源：http://db.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aa.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://hr.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://av.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://xt.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wb.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ws.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gr.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://rz.asd995.cn

[E07] 按分隔符拆分
来源：http://ms.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ph.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zs.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ey.nszjky.cn

TS:   s.split(",")
来源：http://cu.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hk.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zb.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://vj.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hf.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://no.bookmarksfly.cn

Py:   ",".join(items)
来源：http://wt.colortex.cn

PHP:  implode(",", $items);
来源：http://yi.colortex.cn

JS:   items.join(",")
来源：http://pn.gzmigu.cn

TS:   items.join(",")
来源：http://my.panjiajie.cn

Java: String.join(",", items)
来源：http://zz.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://lz.9csxet.cn

Ruby: items.join(",")
来源：http://mm.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://ms.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://tn.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hw.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wj.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://zm.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://ka.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://gw.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://de.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wn.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bd.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://tn.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://um.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sq.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://tf.521024.cn

TS:   "7".padStart(3, "0")
来源：http://nx.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://du.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rz.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zv.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yv.panjiajie.cn

[E11] 反转字符串
来源：http://vt.gzmigu.cn

Py:   s[::-1]
来源：http://fv.szsharing.cn

PHP:  strrev($s);
来源：http://fm.colortex.cn

JS:   [...s].reverse().join("")
来源：http://bd.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://at.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ex.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qk.yuntaijiaju.cn

Ruby: s.reverse
来源：http://gj.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://az.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://io.gzmigu.cn

Py:   s.count("a")
来源：http://dv.asd995.cn

PHP:  substr_count($s, "a");
来源：http://pr.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://rq.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://jn.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yz.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://eq.bookmarksfly.cn

Ruby: s.count("a")
来源：http://yx.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://ka.szxytkj.cn

[E13] 逐字符遍历
来源：http://dq.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://de.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tq.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tz.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gj.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dr.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rs.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://us.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ov.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://zg.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xn.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fr.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qu.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kd.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lw.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hx.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://om.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gm.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://cm.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hv.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gq.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ls.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sk.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hs.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://aw.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bg.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nx.muxihuayi.cn

[E16] 数字千分位
来源：http://nr.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://ok.nszjky.cn

PHP:  number_format(1234567);
来源：http://yw.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rm.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ep.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tg.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cm.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vz.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://yk.newstarts.cn

[E17] 首字母大写
来源：http://ap.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vh.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://na.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ws.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wc.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xf.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rj.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://jy.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bg.lnxyls.cn

[E18] 模板占位符替换
来源：http://jy.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ky.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yn.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qe.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ua.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xm.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dg.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yw.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://se.asd995.cn

[E19] 多行文本按行拆分
来源：http://pc.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://rf.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pa.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://fx.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://gl.hnjuh.cn

Java: s.lines().toList()
来源：http://ao.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://ps.huixiangedu.cn

Ruby: s.lines
来源：http://lv.lnxyls.cn

C#:   s.Split('\n')
来源：http://go.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://ga.jctech888.com.cn

Py:   if not s:
来源：http://pc.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gy.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sa.hahajie.cn

TS:   if (s === "") {}
来源：http://ch.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://jc.bookmarksfly.cn

Go:   if s == "" {}
来源：http://xb.hnjuh.cn

Ruby: if s.empty?
来源：http://yu.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://em.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://pw.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fg.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lw.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cw.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iv.muxihuayi.cn


<!-- 参考信息 -->