代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://gw.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vj.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bg.lnxyls.cn

[D06] 数组长度
来源：http://og.hnjuh.cn

Py:   len(arr)
来源：http://xe.bookmarksfly.cn

PHP:  count($arr);
来源：http://wg.jianghongdianzi.cn

JS:   arr.length
来源：http://bz.panjiajie.cn

TS:   arr.length
来源：http://jw.colortex.cn

Java: list.size();
来源：http://cw.huixinmuqiang.cn

Go:   len(arr)
来源：http://na.szsharing.cn

Ruby: arr.length; arr.size
来源：http://ss.szsharing.cn

C#:   list.Count;
来源：http://fn.9csxet.cn

[D07] 切片 / 取子数组
来源：http://ie.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rh.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nh.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://wl.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://yz.asd995.cn

Java: list.subList(1, 4);
来源：http://ph.gzmigu.cn

Go:   arr[1:4]
来源：http://mn.nicolike.cn

Ruby: arr[1, 3]
来源：http://lx.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://te.wgjwhj.cn

[D08] 合并两个数组
来源：http://bk.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://xb.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://uu.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lt.jctech888.com.cn

TS:   [...a, ...b];
来源：http://qr.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pa.gzmigu.cn

Go:   append(a, b...)
来源：http://gf.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://xd.521024.cn

C#:   a.Concat(b).ToList()
来源：http://sa.shxzukj.cn

[D09] 排序（升序）
来源：http://ce.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://er.shxzskj.cn

PHP:  sort($arr);
来源：http://ja.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sk.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ra.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kz.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zu.jctech888.com.cn

Ruby: arr.sort
来源：http://az.bookmarksfly.cn

C#:   list.Sort();
来源：http://sm.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zu.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mm.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dk.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://er.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qq.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wc.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vd.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nw.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bn.hnjuh.cn

[D11] 反转数组
来源：http://go.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gr.huanxung.cn

PHP:  array_reverse($arr);
来源：http://da.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hk.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://hc.szxytkj.cn

Java: Collections.reverse(list);
来源：http://zf.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://pf.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://va.panjiajie.cn

C#:   list.Reverse();
来源：http://uc.bookmarksfly.cn

[D12] 查找元素下标
来源：http://if.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://ie.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://la.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vj.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wr.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://az.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://as.asd995.cn

Ruby: arr.index(x)
来源：http://gg.nszjky.cn

C#:   list.IndexOf(x);
来源：http://km.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://xu.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://da.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://am.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://iy.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://xc.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cp.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kq.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lh.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cs.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://qk.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zo.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ok.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://xh.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://qn.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qs.nszjky.cn

Go:   // 手写循环
来源：http://eb.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nu.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://po.huixinmuqiang.cn

[D15] 去重
来源：http://vs.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sx.panjiajie.cn

PHP:  array_unique($arr);
来源：http://ns.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://vb.huanxung.cn

TS:   [...new Set(arr)]
来源：http://pl.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hk.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zz.shtwfgs.cn

Ruby: arr.uniq
来源：http://kc.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://va.panjiajie.cn

[D16] 求和与平均值
来源：http://qb.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ye.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://md.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wi.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wj.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fd.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ti.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ux.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://ag.bjjhwx.cn

[D17] 最大值与最小值
来源：http://go.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://se.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://nr.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uw.asd995.cn

TS:   Math.max(...arr);
来源：http://bu.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://or.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ad.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://nb.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://kv.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://mo.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cr.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://ii.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vj.bjjhwx.cn

TS:   nested.flat();
来源：http://ss.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jr.jctech888.com.cn

Go:   // 手写双层循环
来源：http://lx.szxytkj.cn

Ruby: nested.flatten
来源：http://gc.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jh.jianghongdianzi.cn

[D19] 按字段分组
来源：http://zh.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gb.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pt.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gq.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iy.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hd.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://ct.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://px.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rs.colortex.cn

[D20] 统计每个元素出现次数
来源：http://mb.bookmarksfly.cn

Py:   Counter(arr)
来源：http://ow.newstarts.cn

PHP:  array_count_values($arr);
来源：http://zx.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xm.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://on.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zz.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://ux.huixinmuqiang.cn

Ruby: arr.tally
来源：http://da.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ij.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://er.shxzskj.cn

Py:   x in arr
来源：http://yt.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://hq.hnjuh.cn

JS:   arr.includes(x)
来源：http://hq.yuexingan06.cn

TS:   arr.includes(x)
来源：http://gv.szsharing.cn

Java: list.contains(x)
来源：http://wp.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://wc.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://pe.jctech888.com.cn

C#:   list.Contains(x)
来源：http://rm.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://ik.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vq.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ua.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vm.szsharing.cn

TS:   [...arr];
来源：http://ma.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://wq.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zb.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://by.jctech888.com.cn

C#:   new List<int>(list);
来源：http://cv.shtwfgs.cn

[D23] reduce 累积计算
来源：http://tb.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tf.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sn.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cs.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cp.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ml.nicolike.cn

Go:   // 手写循环
来源：http://cd.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bq.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mz.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://hq.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iq.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sy.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ps.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hk.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zc.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fe.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mk.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uq.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://sc.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ag.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pz.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tf.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cy.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cq.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jo.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://us.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://np.wgjwhj.cn

[D26] 数组转字符串
来源：http://qo.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://iv.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://lq.newstarts.cn

JS:   arr.join(", ")
来源：http://yw.huanxung.cn

TS:   arr.join(", ")
来源：http://wq.hnjuh.cn

Java: String.join(", ", list)
来源：http://zs.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://vt.gzmigu.cn

Ruby: arr.join(", ")
来源：http://yb.huanxung.cn

C#:   string.Join(", ", list)
来源：http://us.jianghongdianzi.cn

================================================================================
来源：http://qh.shxzukj.cn

E. 字符串处理
来源：http://nq.yuexingan06.cn

================================================================================
来源：http://tf.shxzskj.cn

[E01] 拼接字符串
来源：http://am.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ry.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vf.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jv.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vj.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jt.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nm.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yv.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hc.gzmigu.cn

[E02] 重复字符串
来源：http://zr.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://kw.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://uk.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://uy.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ch.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://vc.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://cv.szsharing.cn

Ruby: "ab" * 3
来源：http://ex.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hv.nszjky.cn

[E03] 截取子串
来源：http://gu.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zx.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yj.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dg.szsharing.cn

TS:   s.slice(1, 4)
来源：http://hx.huanxung.cn

Java: s.substring(1, 4)
来源：http://zn.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ht.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tb.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://ea.haigaiapp.cn

[E04] 查找子串位置
来源：http://em.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://pb.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://uz.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ia.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://en.muxihuayi.cn

Java: s.indexOf("x")
来源：http://ep.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://zw.muxihuayi.cn

Ruby: s.index("x")
来源：http://ju.huanxung.cn

C#:   s.IndexOf("x")
来源：http://qb.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qt.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vk.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mm.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vs.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fd.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://db.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gv.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tr.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gc.panjiajie.cn

[E06] 替换子串
来源：http://te.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xu.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://hk.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ai.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://pl.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ix.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vx.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://go.asd995.cn

C#:   s.Replace("a", "b")
来源：http://wz.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://zb.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bt.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://io.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mb.yuexingan06.cn

TS:   s.split(",")
来源：http://bs.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dh.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nm.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://hz.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://it.szsharing.cn

[E08] 数组按分隔符合并
来源：http://hw.shxzskj.cn

Py:   ",".join(items)
来源：http://ns.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://uy.szsharing.cn

JS:   items.join(",")
来源：http://gc.bookmarksfly.cn

TS:   items.join(",")
来源：http://np.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://ia.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://px.panjiajie.cn

Ruby: items.join(",")
来源：http://kx.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://kj.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://ko.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ag.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dh.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://cg.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ub.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://ig.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jv.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xf.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zx.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://ou.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fx.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cy.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://zu.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://vr.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://nj.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nq.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hf.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lc.9csxet.cn

[E11] 反转字符串
来源：http://iy.shxzukj.cn

Py:   s[::-1]
来源：http://cx.gzmigu.cn

PHP:  strrev($s);
来源：http://wn.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://mj.colortex.cn

TS:   [...s].reverse().join("")
来源：http://ms.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wb.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uq.chemitech.net.cn

Ruby: s.reverse
来源：http://vv.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://et.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://ch.huixiangedu.cn

Py:   s.count("a")
来源：http://il.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://df.nicolike.cn

JS:   s.split("a").length - 1
来源：http://ea.521024.cn

TS:   s.split("a").length - 1
来源：http://ud.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qq.yuntaijiaju.cn


<!-- 参考信息 -->