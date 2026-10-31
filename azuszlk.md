代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mw.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vc.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qe.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://ih.hahajie.cn

Ruby: arr.index(x)
来源：http://ch.nszjky.cn

C#:   list.IndexOf(x);
来源：http://fd.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://fn.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ak.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vh.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://dk.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://cr.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eh.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bg.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ur.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bu.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://nn.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xv.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://us.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://tp.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://kr.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ob.szsharing.cn

Go:   // 手写循环
来源：http://hg.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://al.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ki.haigaiapp.cn

[D15] 去重
来源：http://dw.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://id.panjiajie.cn

PHP:  array_unique($arr);
来源：http://uq.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://br.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://ak.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wn.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ls.521024.cn

Ruby: arr.uniq
来源：http://sd.521024.cn

C#:   list.Distinct().ToList()
来源：http://zi.szsharing.cn

[D16] 求和与平均值
来源：http://zm.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xo.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://li.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tn.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qj.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jq.hahajie.cn

Go:   // 手写循环累加
来源：http://dj.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bt.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://kj.asd995.cn

[D17] 最大值与最小值
来源：http://db.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://ls.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://dp.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ww.lnxyls.cn

TS:   Math.max(...arr);
来源：http://cb.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kf.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mi.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://bj.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://na.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://xv.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fx.521024.cn

PHP:  array_merge(...$nested);
来源：http://op.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fu.colortex.cn

TS:   nested.flat();
来源：http://vv.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sa.gzmigu.cn

Go:   // 手写双层循环
来源：http://hk.jctech888.com.cn

Ruby: nested.flatten
来源：http://mu.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ux.newstarts.cn

[D19] 按字段分组
来源：http://xm.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ll.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://la.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yw.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zz.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qk.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://yt.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ab.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zm.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://fy.chemitech.net.cn

Py:   Counter(arr)
来源：http://bx.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://rx.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://th.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ms.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://za.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://wj.wgjwhj.cn

Ruby: arr.tally
来源：http://iw.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ma.521024.cn

[D21] 判断是否包含某元素
来源：http://wx.muxihuayi.cn

Py:   x in arr
来源：http://ut.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ww.hnjuh.cn

JS:   arr.includes(x)
来源：http://xf.hahajie.cn

TS:   arr.includes(x)
来源：http://xv.huixinmuqiang.cn

Java: list.contains(x)
来源：http://eq.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://kl.szsharing.cn

Ruby: arr.include?(x)
来源：http://ny.nszjky.cn

C#:   list.Contains(x)
来源：http://mq.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ag.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ic.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dd.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wj.yuexingan06.cn

TS:   [...arr];
来源：http://ug.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://tw.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ig.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://rw.colortex.cn

C#:   new List<int>(list);
来源：http://ls.colortex.cn

[D23] reduce 累积计算
来源：http://qy.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ws.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cb.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zz.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nb.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://et.huixinmuqiang.cn

Go:   // 手写循环
来源：http://xt.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xa.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://io.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://ji.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yb.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lk.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ux.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vr.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cb.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ud.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kc.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lw.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://am.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kh.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bb.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nw.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zd.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ng.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xu.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gw.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://op.szxytkj.cn

[D26] 数组转字符串
来源：http://wz.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://ag.521024.cn

PHP:  implode(", ", $arr);
来源：http://vk.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://qu.panjiajie.cn

TS:   arr.join(", ")
来源：http://zp.hnjuh.cn

Java: String.join(", ", list)
来源：http://lu.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://wh.nszjky.cn

Ruby: arr.join(", ")
来源：http://eh.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://sq.shxzukj.cn

================================================================================
来源：http://ly.chemitech.net.cn

E. 字符串处理
来源：http://iv.szsharing.cn

================================================================================
来源：http://jn.lnxyls.cn

[E01] 拼接字符串
来源：http://af.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ii.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kq.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rb.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://md.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ew.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fa.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qh.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://je.haigaiapp.cn

[E02] 重复字符串
来源：http://ju.muxihuayi.cn

Py:   "ab" * 3
来源：http://uh.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ye.521024.cn

JS:   "ab".repeat(3)
来源：http://nw.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://vj.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://el.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://ay.huanxung.cn

Ruby: "ab" * 3
来源：http://qr.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qj.521024.cn

[E03] 截取子串
来源：http://ug.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aq.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fu.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ae.hahajie.cn

TS:   s.slice(1, 4)
来源：http://rr.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://gn.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dg.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rs.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://qr.521024.cn

[E04] 查找子串位置
来源：http://xo.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://vd.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://gq.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://da.panjiajie.cn

TS:   s.indexOf("x")
来源：http://jq.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://kf.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://bt.shxzukj.cn

Ruby: s.index("x")
来源：http://li.szsharing.cn

C#:   s.IndexOf("x")
来源：http://ua.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nu.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ol.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ic.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bl.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zt.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hd.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hp.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vr.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ws.shtwfgs.cn

[E06] 替换子串
来源：http://um.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sk.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://yp.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xi.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://jz.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ej.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pr.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lg.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://sg.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://sf.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vu.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nb.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://it.gzmigu.cn

TS:   s.split(",")
来源：http://na.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sh.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mt.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://bf.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rd.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://sl.521024.cn

Py:   ",".join(items)
来源：http://jf.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://yr.bjjhwx.cn

JS:   items.join(",")
来源：http://iz.hahajie.cn

TS:   items.join(",")
来源：http://ez.jctech888.com.cn

Java: String.join(",", items)
来源：http://wk.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://sm.521024.cn

Ruby: items.join(",")
来源：http://bn.panjiajie.cn

C#:   string.Join(",", items)
来源：http://je.shxzukj.cn

[E09] 去除所有空白字符
来源：http://ym.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ln.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tj.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://sc.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://mt.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://wr.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zs.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jx.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lk.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://jw.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kx.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wi.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://ec.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://al.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://je.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://or.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ag.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yl.hnjuh.cn

[E11] 反转字符串
来源：http://eh.nicolike.cn

Py:   s[::-1]
来源：http://pl.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://up.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://qv.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://om.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dk.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jf.chemitech.net.cn

Ruby: s.reverse
来源：http://he.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jb.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://qy.521024.cn

Py:   s.count("a")
来源：http://ig.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://wk.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://ry.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://ll.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pt.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://jf.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://rx.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://ud.lnxyls.cn

[E13] 逐字符遍历
来源：http://qp.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://ti.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://li.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hx.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dt.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jh.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lr.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jj.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ni.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://nc.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mm.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zf.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://px.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kq.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dc.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fg.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nr.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xz.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://gc.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ij.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zw.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rm.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ed.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hs.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ts.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://im.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ci.panjiajie.cn

[E16] 数字千分位
来源：http://cs.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://su.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://av.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sj.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://px.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cu.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kk.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sq.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://hu.yuexingan06.cn

[E17] 首字母大写
来源：http://sw.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qr.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://es.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ca.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vz.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jt.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fj.shtwfgs.cn

Ruby: s.capitalize
来源：http://nv.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rw.shtwfgs.cn

[E18] 模板占位符替换
来源：http://el.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lj.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uh.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zg.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bu.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ho.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ox.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sg.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kc.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://jk.bookmarksfly.cn

Py:   s.splitlines()
来源：http://lb.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sc.jianghongdianzi.cn


<!-- 参考信息 -->