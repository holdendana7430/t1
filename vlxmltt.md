代发 wailian999

TS:   arr.slice(1, 4);
来源：http://dc.nicolike.cn

Java: list.subList(1, 4);
来源：http://si.nszjky.cn

Go:   arr[1:4]
来源：http://mv.hnjuh.cn

Ruby: arr[1, 3]
来源：http://vc.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://xm.szxytkj.cn

[D08] 合并两个数组
来源：http://zs.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://ma.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://ow.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xj.colortex.cn

TS:   [...a, ...b];
来源：http://px.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dt.yuexingan06.cn

Go:   append(a, b...)
来源：http://pq.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://eh.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://vy.hahajie.cn

[D09] 排序（升序）
来源：http://zn.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://wf.bjjhwx.cn

PHP:  sort($arr);
来源：http://qk.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nn.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gw.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bc.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uw.9csxet.cn

Ruby: arr.sort
来源：http://ir.jianghongdianzi.cn

C#:   list.Sort();
来源：http://op.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yn.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aa.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://le.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vl.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qf.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://av.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dp.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kb.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rc.panjiajie.cn

[D11] 反转数组
来源：http://mn.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ew.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://rf.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kb.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://to.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://ju.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://hr.wgjwhj.cn

Ruby: arr.reverse
来源：http://pm.9csxet.cn

C#:   list.Reverse();
来源：http://pg.bjjhwx.cn

[D12] 查找元素下标
来源：http://ky.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://mx.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rw.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hu.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lc.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yr.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://tf.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://mr.colortex.cn

C#:   list.IndexOf(x);
来源：http://ao.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://bm.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://co.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ka.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://oz.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://it.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ng.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://br.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yw.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://id.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://zr.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dj.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jz.521024.cn

JS:   arr.map(x => x * 2)
来源：http://eu.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://rr.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cs.muxihuayi.cn

Go:   // 手写循环
来源：http://lw.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cu.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ol.bookmarksfly.cn

[D15] 去重
来源：http://vc.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xv.panjiajie.cn

PHP:  array_unique($arr);
来源：http://in.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://ij.asd995.cn

TS:   [...new Set(arr)]
来源：http://nq.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gy.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ad.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://wm.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://ws.hnjuh.cn

[D16] 求和与平均值
来源：http://lg.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fj.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ys.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kj.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wj.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zl.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://vv.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tg.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://cl.521024.cn

[D17] 最大值与最小值
来源：http://cc.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://nr.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://fz.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xf.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://eu.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tb.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sg.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://zf.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://lw.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://ha.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kd.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://dc.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xj.shxzskj.cn

TS:   nested.flat();
来源：http://ia.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://en.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://fp.yuexingan06.cn

Ruby: nested.flatten
来源：http://ad.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wq.szsharing.cn

[D19] 按字段分组
来源：http://xb.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sv.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://du.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vc.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rp.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oa.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://dd.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uf.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://in.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://sj.bjjhwx.cn

Py:   Counter(arr)
来源：http://mn.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://rq.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jz.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dw.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rm.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://so.shxzukj.cn

Ruby: arr.tally
来源：http://ps.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rg.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://ju.huanxung.cn

Py:   x in arr
来源：http://lv.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://va.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://sa.9csxet.cn

TS:   arr.includes(x)
来源：http://cs.521024.cn

Java: list.contains(x)
来源：http://ca.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://sk.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://od.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://pi.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://zz.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ak.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ce.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sh.yuexingan06.cn

TS:   [...arr];
来源：http://io.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://yy.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://se.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://qq.shxzukj.cn

C#:   new List<int>(list);
来源：http://xq.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://ca.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fb.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://de.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ql.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yz.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zi.nicolike.cn

Go:   // 手写循环
来源：http://si.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://le.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oh.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://zo.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bs.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xj.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://af.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://np.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ip.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xc.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uj.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yp.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://nf.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ra.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hc.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sw.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rf.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xl.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dl.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tq.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fb.wgjwhj.cn

[D26] 数组转字符串
来源：http://yb.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://wk.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://kr.szsharing.cn

JS:   arr.join(", ")
来源：http://ub.shxzukj.cn

TS:   arr.join(", ")
来源：http://mj.chemitech.net.cn

Java: String.join(", ", list)
来源：http://hz.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://yx.asd995.cn

Ruby: arr.join(", ")
来源：http://sa.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://uj.shxzukj.cn

================================================================================
来源：http://dv.szsharing.cn

E. 字符串处理
来源：http://lp.nszjky.cn

================================================================================
来源：http://wl.chemitech.net.cn

[E01] 拼接字符串
来源：http://dj.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gg.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://go.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lt.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ak.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ys.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ri.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oz.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://du.huixiangedu.cn

[E02] 重复字符串
来源：http://ip.jctech888.com.cn

Py:   "ab" * 3
来源：http://vu.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://qh.newstarts.cn

JS:   "ab".repeat(3)
来源：http://eg.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://lu.huanxung.cn

Java: "ab".repeat(3)
来源：http://co.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://dj.hnjuh.cn

Ruby: "ab" * 3
来源：http://wl.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yc.9csxet.cn

[E03] 截取子串
来源：http://zv.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nz.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iw.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qz.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://or.lnxyls.cn

Java: s.substring(1, 4)
来源：http://na.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lq.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ux.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://lo.shxzukj.cn

[E04] 查找子串位置
来源：http://tl.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://vi.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ig.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pk.shxzskj.cn

TS:   s.indexOf("x")
来源：http://il.szsharing.cn

Java: s.indexOf("x")
来源：http://pw.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ax.shxzukj.cn

Ruby: s.index("x")
来源：http://th.hahajie.cn

C#:   s.IndexOf("x")
来源：http://oy.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ig.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ky.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gc.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hv.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yb.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iv.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hc.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kn.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gb.wgjwhj.cn

[E06] 替换子串
来源：http://ya.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ux.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://sp.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mb.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://ao.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dg.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dj.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qr.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://rq.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://oe.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://al.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xy.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ex.muxihuayi.cn

TS:   s.split(",")
来源：http://em.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oc.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hw.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://vp.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uv.szsharing.cn

[E08] 数组按分隔符合并
来源：http://ro.chemitech.net.cn

Py:   ",".join(items)
来源：http://qe.newstarts.cn

PHP:  implode(",", $items);
来源：http://oe.muxihuayi.cn

JS:   items.join(",")
来源：http://ai.gzmigu.cn

TS:   items.join(",")
来源：http://mb.szxytkj.cn

Java: String.join(",", items)
来源：http://lc.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://rf.9csxet.cn

Ruby: items.join(",")
来源：http://tl.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://rv.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://ha.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yx.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ob.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://vw.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://ph.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://sn.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rv.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://aj.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bb.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://li.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ox.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://if.521024.cn

JS:   "7".padStart(3, "0")
来源：http://el.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://ca.asd995.cn

Java: String.format("%03d", 7)
来源：http://cr.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zz.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lz.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ic.huanxung.cn

[E11] 反转字符串
来源：http://sk.panjiajie.cn

Py:   s[::-1]
来源：http://tr.nszjky.cn

PHP:  strrev($s);
来源：http://wq.521024.cn

JS:   [...s].reverse().join("")
来源：http://az.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://ej.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ca.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kg.shxzukj.cn

Ruby: s.reverse
来源：http://xo.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fm.colortex.cn

[E12] 统计某字符出现次数
来源：http://nx.asd995.cn

Py:   s.count("a")
来源：http://us.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://cq.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://bp.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://af.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gl.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://xk.asd995.cn

Ruby: s.count("a")
来源：http://qo.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://un.chemitech.net.cn

[E13] 逐字符遍历
来源：http://hb.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://tm.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fy.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://no.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pr.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ex.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://st.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qi.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ha.colortex.cn

[E14] URL 编码与 Base64
来源：http://wv.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xz.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jv.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ab.huanxung.cn


<!-- 参考信息 -->