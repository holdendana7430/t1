代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ug.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jb.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://qr.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://oi.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://va.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://al.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wk.shxzukj.cn

[D06] 数组长度
来源：http://ss.asd995.cn

Py:   len(arr)
来源：http://dn.panjiajie.cn

PHP:  count($arr);
来源：http://dy.colortex.cn

JS:   arr.length
来源：http://jv.asd995.cn

TS:   arr.length
来源：http://lc.jctech888.com.cn

Java: list.size();
来源：http://vp.gzmigu.cn

Go:   len(arr)
来源：http://ro.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://ya.yuntaijiaju.cn

C#:   list.Count;
来源：http://lv.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://wz.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ih.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ha.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://mn.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://di.9csxet.cn

Java: list.subList(1, 4);
来源：http://eg.shtwfgs.cn

Go:   arr[1:4]
来源：http://ec.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://mg.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://hn.nszjky.cn

[D08] 合并两个数组
来源：http://gn.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://rk.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://mn.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kl.shtwfgs.cn

TS:   [...a, ...b];
来源：http://rb.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rk.hnjuh.cn

Go:   append(a, b...)
来源：http://qn.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://ck.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://tb.lnxyls.cn

[D09] 排序（升序）
来源：http://jj.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://uh.newstarts.cn

PHP:  sort($arr);
来源：http://pc.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sv.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yo.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ep.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://na.yuexingan06.cn

Ruby: arr.sort
来源：http://gd.yuexingan06.cn

C#:   list.Sort();
来源：http://zj.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qn.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dp.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pj.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vv.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rd.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uz.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fb.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zc.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ig.muxihuayi.cn

[D11] 反转数组
来源：http://ir.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xd.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://nu.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hl.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://ta.panjiajie.cn

Java: Collections.reverse(list);
来源：http://cp.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://vs.huanxung.cn

Ruby: arr.reverse
来源：http://kr.521024.cn

C#:   list.Reverse();
来源：http://vw.panjiajie.cn

[D12] 查找元素下标
来源：http://hs.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://vy.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eh.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wf.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yg.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fn.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://hk.shxzskj.cn

Ruby: arr.index(x)
来源：http://ms.colortex.cn

C#:   list.IndexOf(x);
来源：http://ge.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://gy.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pj.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gp.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://zc.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://zi.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lq.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kd.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sd.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://en.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://fp.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://je.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ng.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://ou.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://xm.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ka.shxzskj.cn

Go:   // 手写循环
来源：http://kx.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jz.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zb.huanxung.cn

[D15] 去重
来源：http://so.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ds.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://sw.hahajie.cn

JS:   [...new Set(arr)]
来源：http://az.asd995.cn

TS:   [...new Set(arr)]
来源：http://dm.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xj.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ip.521024.cn

Ruby: arr.uniq
来源：http://zq.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://rd.asd995.cn

[D16] 求和与平均值
来源：http://nn.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://we.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ug.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qh.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sk.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mc.chemitech.net.cn

Go:   // 手写循环累加
来源：http://vv.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hb.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ol.nicolike.cn

[D17] 最大值与最小值
来源：http://et.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://ip.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://dw.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rf.lnxyls.cn

TS:   Math.max(...arr);
来源：http://oh.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ot.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vk.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://vq.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://is.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://ll.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gi.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://lm.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rq.bjjhwx.cn

TS:   nested.flat();
来源：http://nm.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ti.chemitech.net.cn

Go:   // 手写双层循环
来源：http://gw.gzmigu.cn

Ruby: nested.flatten
来源：http://ot.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cn.gzmigu.cn

[D19] 按字段分组
来源：http://ut.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ip.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kv.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mw.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://am.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ti.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://jr.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rp.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fm.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://ty.yuexingan06.cn

Py:   Counter(arr)
来源：http://lq.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://ku.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ls.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://js.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lw.colortex.cn

Go:   // 手写 map[T]int
来源：http://vu.9csxet.cn

Ruby: arr.tally
来源：http://sf.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xh.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://km.9csxet.cn

Py:   x in arr
来源：http://mq.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://bm.yuexingan06.cn

JS:   arr.includes(x)
来源：http://dj.shtwfgs.cn

TS:   arr.includes(x)
来源：http://nx.muxihuayi.cn

Java: list.contains(x)
来源：http://sp.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://sm.nicolike.cn

Ruby: arr.include?(x)
来源：http://ud.muxihuayi.cn

C#:   list.Contains(x)
来源：http://wh.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://pn.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qu.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uj.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tz.asd995.cn

TS:   [...arr];
来源：http://fn.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://xi.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jm.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://av.shxzukj.cn

C#:   new List<int>(list);
来源：http://lv.wgjwhj.cn

[D23] reduce 累积计算
来源：http://gk.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ab.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cr.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ju.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mq.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zp.szsharing.cn

Go:   // 手写循环
来源：http://rf.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lq.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ut.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://wq.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://us.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wm.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rt.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hj.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gl.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mp.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gc.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://si.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://ax.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qz.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://up.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pd.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ky.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lc.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mu.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://um.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uo.lnxyls.cn

[D26] 数组转字符串
来源：http://ak.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://au.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://fy.nszjky.cn

JS:   arr.join(", ")
来源：http://bk.bjjhwx.cn

TS:   arr.join(", ")
来源：http://bx.huixiangedu.cn

Java: String.join(", ", list)
来源：http://od.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://fg.nszjky.cn

Ruby: arr.join(", ")
来源：http://ei.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://gm.yuntaijiaju.cn

================================================================================
来源：http://xx.haigaiapp.cn

E. 字符串处理
来源：http://hk.colortex.cn

================================================================================
来源：http://oa.jctech888.com.cn

[E01] 拼接字符串
来源：http://oo.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sw.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lq.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gt.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eh.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gl.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hl.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bs.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rc.shxzukj.cn

[E02] 重复字符串
来源：http://av.bjjhwx.cn

Py:   "ab" * 3
来源：http://yj.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://lk.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://ys.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ui.huanxung.cn

Java: "ab".repeat(3)
来源：http://wq.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://sc.lnxyls.cn

Ruby: "ab" * 3
来源：http://lv.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rh.bjjhwx.cn

[E03] 截取子串
来源：http://hc.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ry.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://np.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nm.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://bb.9csxet.cn

Java: s.substring(1, 4)
来源：http://sd.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kb.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://of.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://zm.jctech888.com.cn

[E04] 查找子串位置
来源：http://ci.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://pp.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://fb.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shxzskj.cn

TS:   s.indexOf("x")
来源：http://eo.shxzskj.cn

Java: s.indexOf("x")
来源：http://tc.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://dd.muxihuayi.cn

Ruby: s.index("x")
来源：http://tc.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://du.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uv.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bd.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vl.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zx.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sd.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://to.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wz.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mn.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dc.jianghongdianzi.cn

[E06] 替换子串
来源：http://cd.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vh.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://hx.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ac.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://ij.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ft.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fj.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dl.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://cf.shxzskj.cn

[E07] 按分隔符拆分
来源：http://wb.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://az.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pj.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nz.asd995.cn

TS:   s.split(",")
来源：http://si.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gm.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://id.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://om.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nd.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://ht.panjiajie.cn

Py:   ",".join(items)
来源：http://jp.asd995.cn

PHP:  implode(",", $items);
来源：http://zz.yuexingan06.cn

JS:   items.join(",")
来源：http://yv.nszjky.cn

TS:   items.join(",")
来源：http://pk.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://lu.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://mi.lnxyls.cn

Ruby: items.join(",")
来源：http://oc.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://zu.lnxyls.cn

[E09] 去除所有空白字符
来源：http://ue.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ag.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cl.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://gw.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ss.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://yr.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zv.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fv.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mf.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://yd.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wp.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wu.521024.cn

JS:   "7".padStart(3, "0")
来源：http://zo.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://wx.nszjky.cn

Java: String.format("%03d", 7)
来源：http://on.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fj.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ad.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://to.haigaiapp.cn

[E11] 反转字符串
来源：http://uo.bjjhwx.cn

Py:   s[::-1]
来源：http://jz.huixiangedu.cn

PHP:  strrev($s);
来源：http://ml.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://fn.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://se.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zf.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pe.lnxyls.cn

Ruby: s.reverse
来源：http://wr.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://km.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://ol.lnxyls.cn

Py:   s.count("a")
来源：http://gc.nicolike.cn


<!-- 参考信息 -->