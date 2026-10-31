代发 wailian999

[D15] 去重
来源：http://hc.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://he.szxytkj.cn

PHP:  array_unique($arr);
来源：http://eo.asd995.cn

JS:   [...new Set(arr)]
来源：http://uz.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://in.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zl.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wn.szxytkj.cn

Ruby: arr.uniq
来源：http://vt.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://nv.lnxyls.cn

[D16] 求和与平均值
来源：http://em.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fe.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yg.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tg.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gk.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ee.szxytkj.cn

Go:   // 手写循环累加
来源：http://kn.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bx.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://vl.nicolike.cn

[D17] 最大值与最小值
来源：http://bg.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://sf.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://rc.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://va.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://tf.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ct.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yu.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://qx.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://jn.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://as.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pt.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://ai.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gj.panjiajie.cn

TS:   nested.flat();
来源：http://gt.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vt.521024.cn

Go:   // 手写双层循环
来源：http://yh.bjjhwx.cn

Ruby: nested.flatten
来源：http://td.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nz.colortex.cn

[D19] 按字段分组
来源：http://li.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kd.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gs.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://at.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qj.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fq.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://zg.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vi.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ub.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://vo.jctech888.com.cn

Py:   Counter(arr)
来源：http://ar.huanxung.cn

PHP:  array_count_values($arr);
来源：http://lm.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xn.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cq.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ni.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://cq.szxytkj.cn

Ruby: arr.tally
来源：http://dm.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jd.szsharing.cn

[D21] 判断是否包含某元素
来源：http://gk.jctech888.com.cn

Py:   x in arr
来源：http://sm.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://gf.asd995.cn

JS:   arr.includes(x)
来源：http://gg.nszjky.cn

TS:   arr.includes(x)
来源：http://yi.shxzukj.cn

Java: list.contains(x)
来源：http://sh.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://vc.nicolike.cn

Ruby: arr.include?(x)
来源：http://fe.szxytkj.cn

C#:   list.Contains(x)
来源：http://qy.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ev.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ju.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gt.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ts.shxzskj.cn

TS:   [...arr];
来源：http://de.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://ks.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fp.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://nz.panjiajie.cn

C#:   new List<int>(list);
来源：http://hj.asd995.cn

[D23] reduce 累积计算
来源：http://tc.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zf.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ie.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cl.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tr.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qe.bjjhwx.cn

Go:   // 手写循环
来源：http://te.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nt.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jo.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://dy.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mw.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ad.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sc.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bk.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mb.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hg.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vg.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bj.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://dt.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bl.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://la.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rl.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gu.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://od.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iq.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xm.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xj.521024.cn

[D26] 数组转字符串
来源：http://hs.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://lk.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://gk.panjiajie.cn

JS:   arr.join(", ")
来源：http://le.asd995.cn

TS:   arr.join(", ")
来源：http://ij.hnjuh.cn

Java: String.join(", ", list)
来源：http://nl.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://wz.asd995.cn

Ruby: arr.join(", ")
来源：http://tw.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://ql.nicolike.cn

================================================================================
来源：http://if.nicolike.cn

E. 字符串处理
来源：http://oc.jctech888.com.cn

================================================================================
来源：http://fi.asd995.cn

[E01] 拼接字符串
来源：http://ys.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rr.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xl.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tj.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uy.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vu.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zb.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oh.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ka.nicolike.cn

[E02] 重复字符串
来源：http://rt.asd995.cn

Py:   "ab" * 3
来源：http://nx.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://px.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://uf.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://ch.shxzskj.cn

Java: "ab".repeat(3)
来源：http://og.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://sq.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://ck.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dq.asd995.cn

[E03] 截取子串
来源：http://my.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://og.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hu.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gl.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://ot.szsharing.cn

Java: s.substring(1, 4)
来源：http://qa.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rl.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ve.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://zd.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://ew.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://dy.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://yz.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zm.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://wg.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://ns.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://fd.szxytkj.cn

Ruby: s.index("x")
来源：http://xv.9csxet.cn

C#:   s.IndexOf("x")
来源：http://ls.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hv.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uv.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hy.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lf.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rg.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nf.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rc.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wq.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mf.asd995.cn

[E06] 替换子串
来源：http://lq.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iy.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://su.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yy.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://vx.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://na.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wj.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://is.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://pf.newstarts.cn

[E07] 按分隔符拆分
来源：http://um.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://df.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vk.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xo.asd995.cn

TS:   s.split(",")
来源：http://yj.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mr.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vx.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://if.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://up.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ll.colortex.cn

Py:   ",".join(items)
来源：http://pg.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://rt.nicolike.cn

JS:   items.join(",")
来源：http://un.jianghongdianzi.cn

TS:   items.join(",")
来源：http://wm.newstarts.cn

Java: String.join(",", items)
来源：http://lk.colortex.cn

Go:   strings.Join(items, ",")
来源：http://ge.colortex.cn

Ruby: items.join(",")
来源：http://ks.9csxet.cn

C#:   string.Join(",", items)
来源：http://qy.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://cd.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hy.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://en.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://zy.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://dz.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ip.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://je.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kx.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gn.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://dl.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ga.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ct.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://rg.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://qf.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://kq.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mm.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vc.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sx.hahajie.cn

[E11] 反转字符串
来源：http://ns.haigaiapp.cn

Py:   s[::-1]
来源：http://ln.huanxung.cn

PHP:  strrev($s);
来源：http://bg.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ru.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://ol.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pe.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://or.haigaiapp.cn

Ruby: s.reverse
来源：http://kh.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qu.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://ao.colortex.cn

Py:   s.count("a")
来源：http://bo.asd995.cn

PHP:  substr_count($s, "a");
来源：http://up.hahajie.cn

JS:   s.split("a").length - 1
来源：http://fq.nicolike.cn

TS:   s.split("a").length - 1
来源：http://tt.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ug.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://er.szxytkj.cn

Ruby: s.count("a")
来源：http://hk.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://zb.nicolike.cn

[E13] 逐字符遍历
来源：http://xs.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://ck.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://es.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wu.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cu.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kp.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bc.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cu.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cf.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://xq.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ze.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ln.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yv.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ds.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mr.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://db.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rm.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wg.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://te.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://px.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vj.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uv.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ni.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ly.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://go.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uz.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mj.szsharing.cn

[E16] 数字千分位
来源：http://uq.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://wa.szxytkj.cn

PHP:  number_format(1234567);
来源：http://dk.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cw.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pg.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sm.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pm.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cd.colortex.cn

C#:   1234567.ToString("N0")
来源：http://vb.hnjuh.cn

[E17] 首字母大写
来源：http://of.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://le.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://he.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ef.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mb.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kj.shtwfgs.cn

Ruby: s.capitalize
来源：http://ks.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pl.hnjuh.cn

[E18] 模板占位符替换
来源：http://wq.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ti.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zp.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xe.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://es.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aq.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xz.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ch.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dt.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://gz.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://kb.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nz.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://xl.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://fy.shtwfgs.cn

Java: s.lines().toList()
来源：http://dv.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://dz.szsharing.cn

Ruby: s.lines
来源：http://yi.panjiajie.cn

C#:   s.Split('\n')
来源：http://jh.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://nh.chemitech.net.cn

Py:   if not s:
来源：http://cf.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lp.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vj.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://kp.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://bv.huanxung.cn

Go:   if s == "" {}
来源：http://bp.bjjhwx.cn

Ruby: if s.empty?
来源：http://hl.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bf.9csxet.cn

[E21] 超长截断加省略号
来源：http://vt.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kk.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rx.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nd.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mr.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bp.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://qc.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ro.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qx.panjiajie.cn


<!-- 参考信息 -->