代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://ej.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ql.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://on.wgjwhj.cn

[D06] 数组长度
来源：http://fi.bjjhwx.cn

Py:   len(arr)
来源：http://oq.asd995.cn

PHP:  count($arr);
来源：http://rp.haigaiapp.cn

JS:   arr.length
来源：http://yr.panjiajie.cn

TS:   arr.length
来源：http://qu.bookmarksfly.cn

Java: list.size();
来源：http://du.colortex.cn

Go:   len(arr)
来源：http://kt.nszjky.cn

Ruby: arr.length; arr.size
来源：http://pn.lnxyls.cn

C#:   list.Count;
来源：http://jh.szsharing.cn

[D07] 切片 / 取子数组
来源：http://dl.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sv.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vu.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://bx.521024.cn

TS:   arr.slice(1, 4);
来源：http://bh.521024.cn

Java: list.subList(1, 4);
来源：http://bv.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ka.shxzukj.cn

Ruby: arr[1, 3]
来源：http://au.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://iv.panjiajie.cn

[D08] 合并两个数组
来源：http://vs.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://pl.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://qo.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yz.huanxung.cn

TS:   [...a, ...b];
来源：http://tn.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gw.chemitech.net.cn

Go:   append(a, b...)
来源：http://wl.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://yv.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://rc.jctech888.com.cn

[D09] 排序（升序）
来源：http://wf.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://bd.jctech888.com.cn

PHP:  sort($arr);
来源：http://dm.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://af.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://td.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cl.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sv.hahajie.cn

Ruby: arr.sort
来源：http://sw.szxytkj.cn

C#:   list.Sort();
来源：http://bv.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ad.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xe.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ru.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wf.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ed.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rg.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://em.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wb.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rg.chemitech.net.cn

[D11] 反转数组
来源：http://sy.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zx.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://qg.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://es.shxzskj.cn

TS:   [...arr].reverse();
来源：http://uc.colortex.cn

Java: Collections.reverse(list);
来源：http://nu.asd995.cn

Go:   slices.Reverse(arr)
来源：http://es.shxzukj.cn

Ruby: arr.reverse
来源：http://hq.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://lx.shtwfgs.cn

[D12] 查找元素下标
来源：http://tp.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://hd.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xw.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vp.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ki.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ee.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://gl.nicolike.cn

Ruby: arr.index(x)
来源：http://cn.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://aj.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://af.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lh.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mv.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://cd.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://in.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nb.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cu.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ic.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hv.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://vt.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sk.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fc.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ip.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://lt.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gx.jianghongdianzi.cn

Go:   // 手写循环
来源：http://xv.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yk.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://je.bjjhwx.cn

[D15] 去重
来源：http://jy.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lv.hnjuh.cn

PHP:  array_unique($arr);
来源：http://aq.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://ru.9csxet.cn

TS:   [...new Set(arr)]
来源：http://jv.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sq.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ot.hnjuh.cn

Ruby: arr.uniq
来源：http://qp.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://qn.hahajie.cn

[D16] 求和与平均值
来源：http://xc.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sk.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jq.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wp.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nr.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kb.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://dx.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ef.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://ub.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://my.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://sc.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://fj.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kt.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://wr.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://if.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xs.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://lp.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://vh.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://bn.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yn.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://le.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kd.colortex.cn

TS:   nested.flat();
来源：http://zw.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jz.shtwfgs.cn

Go:   // 手写双层循环
来源：http://qu.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://nr.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yj.9csxet.cn

[D19] 按字段分组
来源：http://qc.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fx.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pb.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ja.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hl.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jo.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://tc.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ye.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uy.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://lm.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://nt.521024.cn

PHP:  array_count_values($arr);
来源：http://vn.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dn.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://af.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://af.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://bd.yuexingan06.cn

Ruby: arr.tally
来源：http://je.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://as.521024.cn

[D21] 判断是否包含某元素
来源：http://jp.asd995.cn

Py:   x in arr
来源：http://ln.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://ys.hnjuh.cn

JS:   arr.includes(x)
来源：http://eo.nszjky.cn

TS:   arr.includes(x)
来源：http://xe.szsharing.cn

Java: list.contains(x)
来源：http://jw.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://dy.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://dk.yuexingan06.cn

C#:   list.Contains(x)
来源：http://cu.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://wa.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://af.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jr.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rr.nszjky.cn

TS:   [...arr];
来源：http://wu.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://tx.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yg.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://dg.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://gg.9csxet.cn

[D23] reduce 累积计算
来源：http://dt.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tu.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hc.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mb.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://si.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://an.huixinmuqiang.cn

Go:   // 手写循环
来源：http://vg.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yx.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vb.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://sa.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zu.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dw.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xy.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yi.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mo.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cd.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cp.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nu.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ar.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xx.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jr.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lv.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ff.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iz.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pk.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xi.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bv.hnjuh.cn

[D26] 数组转字符串
来源：http://ks.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://pf.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://bv.colortex.cn

JS:   arr.join(", ")
来源：http://mi.shxzskj.cn

TS:   arr.join(", ")
来源：http://ph.lnxyls.cn

Java: String.join(", ", list)
来源：http://xe.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://gb.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://iq.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://kw.shxzskj.cn

================================================================================
来源：http://ae.huanxung.cn

E. 字符串处理
来源：http://dl.chemitech.net.cn

================================================================================
来源：http://kz.lnxyls.cn

[E01] 拼接字符串
来源：http://wn.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yr.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bw.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wc.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vk.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kf.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hg.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ha.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qk.nicolike.cn

[E02] 重复字符串
来源：http://ru.colortex.cn

Py:   "ab" * 3
来源：http://rz.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://bh.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://vm.9csxet.cn

TS:   "ab".repeat(3)
来源：http://fj.colortex.cn

Java: "ab".repeat(3)
来源：http://jr.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://ua.bjjhwx.cn

Ruby: "ab" * 3
来源：http://uv.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ud.9csxet.cn

[E03] 截取子串
来源：http://xz.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://th.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://op.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bx.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://kd.asd995.cn

Java: s.substring(1, 4)
来源：http://cp.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fc.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sf.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://xr.shtwfgs.cn

[E04] 查找子串位置
来源：http://mh.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://wk.colortex.cn

PHP:  strpos($s, "x");
来源：http://hw.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oj.gzmigu.cn

TS:   s.indexOf("x")
来源：http://qf.521024.cn

Java: s.indexOf("x")
来源：http://fo.521024.cn

Go:   strings.Index(s, "x")
来源：http://tx.haigaiapp.cn

Ruby: s.index("x")
来源：http://zh.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://bt.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wn.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ny.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ez.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ao.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wc.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dk.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nk.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lf.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mu.huixinmuqiang.cn

[E06] 替换子串
来源：http://fj.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hu.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://lr.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pu.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://dn.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bs.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rt.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://my.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://ii.9csxet.cn

[E07] 按分隔符拆分
来源：http://no.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oe.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qk.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ol.asd995.cn

TS:   s.split(",")
来源：http://dx.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://to.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fh.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://yc.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ra.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://px.szxytkj.cn

Py:   ",".join(items)
来源：http://ub.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://vp.yuntaijiaju.cn

JS:   items.join(",")
来源：http://js.hahajie.cn

TS:   items.join(",")
来源：http://fh.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://vt.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://io.shxzukj.cn

Ruby: items.join(",")
来源：http://bw.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://lu.newstarts.cn

[E09] 去除所有空白字符
来源：http://xb.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pw.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wj.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://mo.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ng.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://og.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ak.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zu.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rx.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://ru.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mm.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://km.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://ws.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://zg.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://ca.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tb.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ww.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rt.panjiajie.cn

[E11] 反转字符串
来源：http://vk.jianghongdianzi.cn

Py:   s[::-1]
来源：http://sd.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://gl.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://hw.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://yu.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nd.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ep.bookmarksfly.cn

Ruby: s.reverse
来源：http://mv.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bv.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://an.szsharing.cn

Py:   s.count("a")
来源：http://an.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://iy.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://fq.colortex.cn

TS:   s.split("a").length - 1
来源：http://bi.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gx.shxzskj.cn


<!-- 参考信息 -->