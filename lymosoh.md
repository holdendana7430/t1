代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iy.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xd.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://nu.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://qy.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://gk.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ta.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zt.panjiajie.cn

[D06] 数组长度
来源：http://eo.haigaiapp.cn

Py:   len(arr)
来源：http://jq.jctech888.com.cn

PHP:  count($arr);
来源：http://zg.gzmigu.cn

JS:   arr.length
来源：http://ei.huixinmuqiang.cn

TS:   arr.length
来源：http://vs.colortex.cn

Java: list.size();
来源：http://ai.9csxet.cn

Go:   len(arr)
来源：http://uk.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://ax.huixiangedu.cn

C#:   list.Count;
来源：http://rh.nicolike.cn

[D07] 切片 / 取子数组
来源：http://th.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qu.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://th.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://bl.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ua.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://nz.muxihuayi.cn

Go:   arr[1:4]
来源：http://ac.nicolike.cn

Ruby: arr[1, 3]
来源：http://fp.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://fj.newstarts.cn

[D08] 合并两个数组
来源：http://vp.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://xx.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://ha.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jz.szxytkj.cn

TS:   [...a, ...b];
来源：http://dx.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nf.asd995.cn

Go:   append(a, b...)
来源：http://si.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://ki.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://em.szsharing.cn

[D09] 排序（升序）
来源：http://sz.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://sn.huixiangedu.cn

PHP:  sort($arr);
来源：http://js.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oj.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rz.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yh.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fi.bookmarksfly.cn

Ruby: arr.sort
来源：http://pq.huixinmuqiang.cn

C#:   list.Sort();
来源：http://cp.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://py.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gf.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tx.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bx.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rx.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ar.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cp.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lb.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://of.jctech888.com.cn

[D11] 反转数组
来源：http://hc.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gf.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://vo.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lh.shxzskj.cn

TS:   [...arr].reverse();
来源：http://sz.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://oy.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://ah.shxzukj.cn

Ruby: arr.reverse
来源：http://dq.bookmarksfly.cn

C#:   list.Reverse();
来源：http://fg.muxihuayi.cn

[D12] 查找元素下标
来源：http://pd.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://mz.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hn.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sc.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sw.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sb.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://ns.asd995.cn

Ruby: arr.index(x)
来源：http://xn.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://oe.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://sg.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sw.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yg.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://pt.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://ja.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dy.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bc.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wp.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qp.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://im.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nf.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lq.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://zd.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://if.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yr.yuntaijiaju.cn

Go:   // 手写循环
来源：http://it.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xc.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hp.nszjky.cn

[D15] 去重
来源：http://kj.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ev.nszjky.cn

PHP:  array_unique($arr);
来源：http://vh.nicolike.cn

JS:   [...new Set(arr)]
来源：http://ow.9csxet.cn

TS:   [...new Set(arr)]
来源：http://rl.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jt.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ds.muxihuayi.cn

Ruby: arr.uniq
来源：http://hr.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://ye.nszjky.cn

[D16] 求和与平均值
来源：http://wf.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sl.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gf.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mw.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lq.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nx.szsharing.cn

Go:   // 手写循环累加
来源：http://dw.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://as.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://be.colortex.cn

[D17] 最大值与最小值
来源：http://ld.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://fh.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://rh.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://or.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://pa.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rb.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ds.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://wq.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://df.521024.cn

[D18] 扁平化嵌套数组
来源：http://pp.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wd.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://pb.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kc.yuntaijiaju.cn

TS:   nested.flat();
来源：http://gx.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wo.gzmigu.cn

Go:   // 手写双层循环
来源：http://vq.bjjhwx.cn

Ruby: nested.flatten
来源：http://bk.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qd.muxihuayi.cn

[D19] 按字段分组
来源：http://hx.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nt.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dt.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kb.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ps.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ko.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://rt.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kg.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://es.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://de.hahajie.cn

Py:   Counter(arr)
来源：http://aa.nicolike.cn

PHP:  array_count_values($arr);
来源：http://ic.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bo.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ne.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kz.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://rp.huanxung.cn

Ruby: arr.tally
来源：http://by.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sp.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://lj.9csxet.cn

Py:   x in arr
来源：http://aj.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://uu.9csxet.cn

JS:   arr.includes(x)
来源：http://rf.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://fy.nicolike.cn

Java: list.contains(x)
来源：http://kc.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://ik.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://ro.nicolike.cn

C#:   list.Contains(x)
来源：http://wu.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://si.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xi.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ta.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jm.shxzskj.cn

TS:   [...arr];
来源：http://yb.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://hd.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bi.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://fg.asd995.cn

C#:   new List<int>(list);
来源：http://pt.szxytkj.cn

[D23] reduce 累积计算
来源：http://ha.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mh.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jv.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ph.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ks.wgjwhj.cn

Go:   // 手写循环
来源：http://ue.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gs.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ih.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://tr.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ew.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ea.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ng.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hm.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vw.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jg.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wl.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ib.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://zu.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hh.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nd.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wj.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vj.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pa.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://md.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yc.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sa.bookmarksfly.cn

[D26] 数组转字符串
来源：http://rg.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://mr.colortex.cn

PHP:  implode(", ", $arr);
来源：http://jd.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://dk.nicolike.cn

TS:   arr.join(", ")
来源：http://xv.bjjhwx.cn

Java: String.join(", ", list)
来源：http://ve.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://uw.shxzskj.cn

Ruby: arr.join(", ")
来源：http://hf.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://iv.huixinmuqiang.cn

================================================================================
来源：http://at.huanxung.cn

E. 字符串处理
来源：http://wi.521024.cn

================================================================================
来源：http://hf.muxihuayi.cn

[E01] 拼接字符串
来源：http://hy.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fl.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://za.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bt.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oo.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wy.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pv.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iv.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://op.szsharing.cn

[E02] 重复字符串
来源：http://kj.huanxung.cn

Py:   "ab" * 3
来源：http://wj.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://ic.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://tr.521024.cn

TS:   "ab".repeat(3)
来源：http://ts.newstarts.cn

Java: "ab".repeat(3)
来源：http://ns.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://lk.nszjky.cn

Ruby: "ab" * 3
来源：http://wb.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xg.shtwfgs.cn

[E03] 截取子串
来源：http://lm.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zy.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hd.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://er.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://uv.shxzskj.cn

Java: s.substring(1, 4)
来源：http://ce.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qt.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ha.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://ln.521024.cn

[E04] 查找子串位置
来源：http://mg.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://mr.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://ni.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tu.shxzukj.cn

TS:   s.indexOf("x")
来源：http://zu.wgjwhj.cn

Java: s.indexOf("x")
来源：http://dw.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://vs.9csxet.cn

Ruby: s.index("x")
来源：http://fr.newstarts.cn

C#:   s.IndexOf("x")
来源：http://md.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ns.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hq.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sv.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fj.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lx.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ic.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ce.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ct.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fj.wgjwhj.cn

[E06] 替换子串
来源：http://mj.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://te.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://jp.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aa.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://xq.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pg.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ob.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qr.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://vl.szxytkj.cn

[E07] 按分隔符拆分
来源：http://li.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cv.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://it.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ft.colortex.cn

TS:   s.split(",")
来源：http://cn.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hn.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nw.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://eb.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cy.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://dc.shxzukj.cn

Py:   ",".join(items)
来源：http://ae.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://ld.asd995.cn

JS:   items.join(",")
来源：http://bh.shtwfgs.cn

TS:   items.join(",")
来源：http://ox.asd995.cn

Java: String.join(",", items)
来源：http://vo.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://sg.szsharing.cn

Ruby: items.join(",")
来源：http://nb.nicolike.cn

C#:   string.Join(",", items)
来源：http://cw.nicolike.cn

[E09] 去除所有空白字符
来源：http://pv.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xz.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://im.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://ni.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://wd.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://qk.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kh.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cl.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://je.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://zg.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kt.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ll.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://re.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://el.asd995.cn

Java: String.format("%03d", 7)
来源：http://mt.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rc.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kj.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qh.huanxung.cn

[E11] 反转字符串
来源：http://rd.jianghongdianzi.cn

Py:   s[::-1]
来源：http://yd.panjiajie.cn

PHP:  strrev($s);
来源：http://db.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://am.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://sf.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://re.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sr.panjiajie.cn

Ruby: s.reverse
来源：http://vg.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hu.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://sw.asd995.cn

Py:   s.count("a")
来源：http://tu.shxzskj.cn


<!-- 参考信息 -->