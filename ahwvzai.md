代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xl.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zr.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ly.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://gi.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://hh.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ub.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bz.newstarts.cn

[D06] 数组长度
来源：http://xb.huanxung.cn

Py:   len(arr)
来源：http://fc.hahajie.cn

PHP:  count($arr);
来源：http://th.9csxet.cn

JS:   arr.length
来源：http://jo.asd995.cn

TS:   arr.length
来源：http://yz.521024.cn

Java: list.size();
来源：http://pq.yuntaijiaju.cn

Go:   len(arr)
来源：http://rf.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://ha.huanxung.cn

C#:   list.Count;
来源：http://mw.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://zl.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://he.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zx.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://xi.521024.cn

TS:   arr.slice(1, 4);
来源：http://kr.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://ro.colortex.cn

Go:   arr[1:4]
来源：http://ms.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://gb.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://am.newstarts.cn

[D08] 合并两个数组
来源：http://qp.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://xy.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ha.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nn.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://qv.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nw.wgjwhj.cn

Go:   append(a, b...)
来源：http://oe.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://bx.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://kl.shxzskj.cn

[D09] 排序（升序）
来源：http://bl.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://lp.hahajie.cn

PHP:  sort($arr);
来源：http://xw.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://md.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dx.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pj.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ii.hahajie.cn

Ruby: arr.sort
来源：http://ku.yuexingan06.cn

C#:   list.Sort();
来源：http://fx.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ox.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ix.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://az.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ly.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fj.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ue.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uk.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://et.jianghongdianzi.cn

[D11] 反转数组
来源：http://ic.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uc.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://wf.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qp.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://el.lnxyls.cn

Java: Collections.reverse(list);
来源：http://yl.colortex.cn

Go:   slices.Reverse(arr)
来源：http://qw.shxzskj.cn

Ruby: arr.reverse
来源：http://wx.szxytkj.cn

C#:   list.Reverse();
来源：http://zl.asd995.cn

[D12] 查找元素下标
来源：http://bf.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://nn.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vj.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eh.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hy.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ic.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://kf.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://bd.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://kl.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://oe.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eb.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ii.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://vv.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://wl.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dc.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jf.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nz.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kt.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://de.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ep.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rj.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://dh.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://vo.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xi.huixinmuqiang.cn

Go:   // 手写循环
来源：http://pg.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tq.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hx.chemitech.net.cn

[D15] 去重
来源：http://rx.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ak.nszjky.cn

PHP:  array_unique($arr);
来源：http://el.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://qk.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://mn.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kx.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ht.jctech888.com.cn

Ruby: arr.uniq
来源：http://nt.asd995.cn

C#:   list.Distinct().ToList()
来源：http://xj.wgjwhj.cn

[D16] 求和与平均值
来源：http://na.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aw.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hc.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pb.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://at.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lg.panjiajie.cn

Go:   // 手写循环累加
来源：http://ax.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zg.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://qv.bjjhwx.cn

[D17] 最大值与最小值
来源：http://tc.521024.cn

Py:   max(arr);  min(arr)
来源：http://vs.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://va.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dl.szxytkj.cn

TS:   Math.max(...arr);
来源：http://hj.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zm.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://do.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://jh.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://uo.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://ml.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://os.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://bh.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lf.chemitech.net.cn

TS:   nested.flat();
来源：http://ey.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wz.panjiajie.cn

Go:   // 手写双层循环
来源：http://ea.asd995.cn

Ruby: nested.flatten
来源：http://dg.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dq.9csxet.cn

[D19] 按字段分组
来源：http://hq.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ge.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fb.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aj.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pd.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lw.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://dk.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ol.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cx.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://my.hnjuh.cn

Py:   Counter(arr)
来源：http://fr.9csxet.cn

PHP:  array_count_values($arr);
来源：http://ya.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dt.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ne.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ki.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://nc.szsharing.cn

Ruby: arr.tally
来源：http://me.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yk.newstarts.cn

[D21] 判断是否包含某元素
来源：http://wq.huanxung.cn

Py:   x in arr
来源：http://pq.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://yt.9csxet.cn

JS:   arr.includes(x)
来源：http://fi.gzmigu.cn

TS:   arr.includes(x)
来源：http://pt.wgjwhj.cn

Java: list.contains(x)
来源：http://sc.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://fj.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://yy.haigaiapp.cn

C#:   list.Contains(x)
来源：http://kg.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://oj.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uc.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vz.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://av.bookmarksfly.cn

TS:   [...arr];
来源：http://yy.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ss.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gi.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://ky.jctech888.com.cn

C#:   new List<int>(list);
来源：http://ih.newstarts.cn

[D23] reduce 累积计算
来源：http://jo.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nz.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xh.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bj.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://il.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lm.wgjwhj.cn

Go:   // 手写循环
来源：http://vv.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ba.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fx.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://vh.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://je.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ie.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kr.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ke.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ch.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uz.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cz.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xq.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://fq.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://io.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ii.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dd.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://od.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dr.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mi.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kb.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ny.nicolike.cn

[D26] 数组转字符串
来源：http://zp.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://mt.asd995.cn

PHP:  implode(", ", $arr);
来源：http://sw.hahajie.cn

JS:   arr.join(", ")
来源：http://tj.bjjhwx.cn

TS:   arr.join(", ")
来源：http://ed.bjjhwx.cn

Java: String.join(", ", list)
来源：http://py.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://re.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://pw.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://oj.9csxet.cn

================================================================================
来源：http://pl.colortex.cn

E. 字符串处理
来源：http://tw.jctech888.com.cn

================================================================================
来源：http://yl.chemitech.net.cn

[E01] 拼接字符串
来源：http://tu.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ms.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bo.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kp.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bj.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mm.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mn.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xj.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.bookmarksfly.cn

[E02] 重复字符串
来源：http://ou.521024.cn

Py:   "ab" * 3
来源：http://og.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://zm.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://kn.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://ct.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://jf.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://nn.panjiajie.cn

Ruby: "ab" * 3
来源：http://yh.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fy.shxzukj.cn

[E03] 截取子串
来源：http://ms.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vz.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ns.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ij.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://ph.szsharing.cn

Java: s.substring(1, 4)
来源：http://eh.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qh.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ha.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://yd.hahajie.cn

[E04] 查找子串位置
来源：http://pd.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://bp.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://dt.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lu.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://tv.9csxet.cn

Java: s.indexOf("x")
来源：http://xg.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ku.hahajie.cn

Ruby: s.index("x")
来源：http://dx.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://zq.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xx.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wq.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cj.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mi.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xd.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sy.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cd.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kl.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ge.bookmarksfly.cn

[E06] 替换子串
来源：http://eb.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dz.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://ox.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iq.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://bi.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xb.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dw.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bi.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://di.colortex.cn

[E07] 按分隔符拆分
来源：http://tz.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cn.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ws.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kp.jctech888.com.cn

TS:   s.split(",")
来源：http://xj.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zd.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yj.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://mh.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rq.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://vx.hahajie.cn

Py:   ",".join(items)
来源：http://lh.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://ey.jctech888.com.cn

JS:   items.join(",")
来源：http://xj.bookmarksfly.cn

TS:   items.join(",")
来源：http://gy.colortex.cn

Java: String.join(",", items)
来源：http://pt.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ss.nszjky.cn

Ruby: items.join(",")
来源：http://zo.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://js.panjiajie.cn

[E09] 去除所有空白字符
来源：http://si.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jt.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://px.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://vp.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://hk.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://st.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://iw.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://de.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rh.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://bd.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jj.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uj.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://ib.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://jj.szsharing.cn

Java: String.format("%03d", 7)
来源：http://ve.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vp.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://az.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lq.hnjuh.cn

[E11] 反转字符串
来源：http://zj.asd995.cn

Py:   s[::-1]
来源：http://ui.wgjwhj.cn

PHP:  strrev($s);
来源：http://dj.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://dq.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://gg.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sx.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://la.jctech888.com.cn

Ruby: s.reverse
来源：http://un.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://im.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://sa.lnxyls.cn

Py:   s.count("a")
来源：http://hj.nicolike.cn


<!-- 参考信息 -->