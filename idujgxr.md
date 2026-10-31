代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ie.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://to.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://ny.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://vm.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://jr.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ay.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://df.szsharing.cn

[D06] 数组长度
来源：http://wc.newstarts.cn

Py:   len(arr)
来源：http://cf.huixinmuqiang.cn

PHP:  count($arr);
来源：http://gz.shxzukj.cn

JS:   arr.length
来源：http://am.jctech888.com.cn

TS:   arr.length
来源：http://jk.shxzskj.cn

Java: list.size();
来源：http://mf.bjjhwx.cn

Go:   len(arr)
来源：http://rv.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://xc.jctech888.com.cn

C#:   list.Count;
来源：http://wt.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://le.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dz.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gc.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://zk.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://my.asd995.cn

Java: list.subList(1, 4);
来源：http://ah.haigaiapp.cn

Go:   arr[1:4]
来源：http://zb.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://li.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://rx.9csxet.cn

[D08] 合并两个数组
来源：http://iw.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://bq.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://lm.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wi.hnjuh.cn

TS:   [...a, ...b];
来源：http://be.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iv.yuexingan06.cn

Go:   append(a, b...)
来源：http://ze.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://zh.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://im.muxihuayi.cn

[D09] 排序（升序）
来源：http://wf.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ll.lnxyls.cn

PHP:  sort($arr);
来源：http://ic.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wl.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qc.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aj.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rm.huanxung.cn

Ruby: arr.sort
来源：http://dt.yuexingan06.cn

C#:   list.Sort();
来源：http://qe.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sn.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qo.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bt.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rw.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xo.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aj.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mz.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sa.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mv.shxzukj.cn

[D11] 反转数组
来源：http://uv.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://il.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://iq.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fc.hnjuh.cn

TS:   [...arr].reverse();
来源：http://ta.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://hj.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://df.lnxyls.cn

Ruby: arr.reverse
来源：http://zo.gzmigu.cn

C#:   list.Reverse();
来源：http://xl.bjjhwx.cn

[D12] 查找元素下标
来源：http://rp.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://of.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ji.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://in.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ji.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bg.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://cb.shxzukj.cn

Ruby: arr.index(x)
来源：http://av.nszjky.cn

C#:   list.IndexOf(x);
来源：http://sc.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://nt.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ko.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://it.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://di.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://nl.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jv.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ti.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pz.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lk.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://zr.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wd.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yh.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://es.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://sa.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qi.huixiangedu.cn

Go:   // 手写循环
来源：http://og.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zh.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xy.bjjhwx.cn

[D15] 去重
来源：http://ua.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vf.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://qx.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://fp.newstarts.cn

TS:   [...new Set(arr)]
来源：http://hu.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mv.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ic.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://js.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://sd.nszjky.cn

[D16] 求和与平均值
来源：http://gq.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ht.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fr.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sl.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tz.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yz.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://vx.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://su.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://dm.shxzukj.cn

[D17] 最大值与最小值
来源：http://yz.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://il.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://bw.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bg.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://lz.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mx.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fe.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://tf.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://qx.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://np.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gr.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://jz.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rm.panjiajie.cn

TS:   nested.flat();
来源：http://mr.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sa.gzmigu.cn

Go:   // 手写双层循环
来源：http://ve.521024.cn

Ruby: nested.flatten
来源：http://ul.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vz.bjjhwx.cn

[D19] 按字段分组
来源：http://ke.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mx.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uu.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://np.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jf.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mx.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://bw.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ms.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://le.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://pn.chemitech.net.cn

Py:   Counter(arr)
来源：http://zm.colortex.cn

PHP:  array_count_values($arr);
来源：http://zb.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ca.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zn.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hg.9csxet.cn

Go:   // 手写 map[T]int
来源：http://wx.szsharing.cn

Ruby: arr.tally
来源：http://js.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nz.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://ln.panjiajie.cn

Py:   x in arr
来源：http://bp.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://vg.colortex.cn

JS:   arr.includes(x)
来源：http://it.haigaiapp.cn

TS:   arr.includes(x)
来源：http://tu.hahajie.cn

Java: list.contains(x)
来源：http://co.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://vv.newstarts.cn

Ruby: arr.include?(x)
来源：http://kh.chemitech.net.cn

C#:   list.Contains(x)
来源：http://rx.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://yh.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sp.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mr.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ph.yuexingan06.cn

TS:   [...arr];
来源：http://oc.asd995.cn

Java: new ArrayList<>(list);
来源：http://qa.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fc.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://zu.colortex.cn

C#:   new List<int>(list);
来源：http://zh.huanxung.cn

[D23] reduce 累积计算
来源：http://pr.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wd.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rv.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rd.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qc.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://in.shxzskj.cn

Go:   // 手写循环
来源：http://jp.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gw.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gg.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://hw.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zy.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tw.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ce.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://os.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ro.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dz.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://be.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gf.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://mv.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gr.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xn.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jd.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qj.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cb.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dq.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gg.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mq.huixiangedu.cn

[D26] 数组转字符串
来源：http://fz.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://vt.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://as.shxzskj.cn

JS:   arr.join(", ")
来源：http://vu.chemitech.net.cn

TS:   arr.join(", ")
来源：http://uf.521024.cn

Java: String.join(", ", list)
来源：http://gn.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://px.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://hq.521024.cn

C#:   string.Join(", ", list)
来源：http://mi.nszjky.cn

================================================================================
来源：http://hy.gzmigu.cn

E. 字符串处理
来源：http://xz.newstarts.cn

================================================================================
来源：http://fn.szxytkj.cn

[E01] 拼接字符串
来源：http://uz.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kt.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cu.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ml.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ht.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rd.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fb.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lw.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hi.szxytkj.cn

[E02] 重复字符串
来源：http://kj.shtwfgs.cn

Py:   "ab" * 3
来源：http://zg.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://dw.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://oi.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://yj.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://hj.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://gt.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://wd.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vw.9csxet.cn

[E03] 截取子串
来源：http://bi.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vf.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zn.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bz.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://px.9csxet.cn

Java: s.substring(1, 4)
来源：http://af.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jp.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jk.colortex.cn

C#:   s.Substring(1, 3)
来源：http://sk.szxytkj.cn

[E04] 查找子串位置
来源：http://dg.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://ha.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://fh.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mx.nicolike.cn

TS:   s.indexOf("x")
来源：http://bu.muxihuayi.cn

Java: s.indexOf("x")
来源：http://yb.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://gv.jctech888.com.cn

Ruby: s.index("x")
来源：http://ly.huanxung.cn

C#:   s.IndexOf("x")
来源：http://fa.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gm.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bf.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ht.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nv.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://we.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zb.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lg.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kp.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vr.yuntaijiaju.cn

[E06] 替换子串
来源：http://nv.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kq.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ps.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ry.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://nu.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kp.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xl.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sc.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://na.szxytkj.cn

[E07] 按分隔符拆分
来源：http://nn.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fj.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dj.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xx.newstarts.cn

TS:   s.split(",")
来源：http://ay.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pm.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jx.521024.cn

Ruby: s.split(",");  s.split
来源：http://wt.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://so.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://yi.shxzskj.cn

Py:   ",".join(items)
来源：http://qy.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://ek.shxzukj.cn

JS:   items.join(",")
来源：http://xr.bookmarksfly.cn

TS:   items.join(",")
来源：http://lq.jctech888.com.cn

Java: String.join(",", items)
来源：http://hq.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://xj.chemitech.net.cn

Ruby: items.join(",")
来源：http://gg.lnxyls.cn

C#:   string.Join(",", items)
来源：http://to.newstarts.cn

[E09] 去除所有空白字符
来源：http://rz.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fa.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fh.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://tv.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://mt.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://si.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://og.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qg.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ld.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://ri.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ho.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kz.521024.cn

JS:   "7".padStart(3, "0")
来源：http://sh.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://wy.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://zw.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eg.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fl.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://my.nszjky.cn

[E11] 反转字符串
来源：http://wo.asd995.cn

Py:   s[::-1]
来源：http://tq.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://xj.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://hc.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://le.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lq.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://es.panjiajie.cn

Ruby: s.reverse
来源：http://cz.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://va.9csxet.cn

[E12] 统计某字符出现次数
来源：http://ek.521024.cn

Py:   s.count("a")
来源：http://gq.jctech888.com.cn


<!-- 参考信息 -->