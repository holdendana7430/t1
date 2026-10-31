代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xn.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://ng.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kv.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vy.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nj.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mq.asd995.cn

[D05] 访问与修改元素
来源：http://ho.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rs.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zo.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gq.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://cd.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://zy.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ta.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bu.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://an.huixinmuqiang.cn

[D06] 数组长度
来源：http://xe.panjiajie.cn

Py:   len(arr)
来源：http://pl.bjjhwx.cn

PHP:  count($arr);
来源：http://af.huixinmuqiang.cn

JS:   arr.length
来源：http://zf.gzmigu.cn

TS:   arr.length
来源：http://us.nicolike.cn

Java: list.size();
来源：http://jk.nicolike.cn

Go:   len(arr)
来源：http://vj.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://sz.9csxet.cn

C#:   list.Count;
来源：http://wd.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://ge.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nc.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ld.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://hn.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://ry.shxzukj.cn

Java: list.subList(1, 4);
来源：http://mq.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://tx.521024.cn

Ruby: arr[1, 3]
来源：http://kj.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://ag.hnjuh.cn

[D08] 合并两个数组
来源：http://yz.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://ab.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://rq.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wt.newstarts.cn

TS:   [...a, ...b];
来源：http://op.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://py.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://hc.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://yp.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://vy.nicolike.cn

[D09] 排序（升序）
来源：http://an.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://le.yuexingan06.cn

PHP:  sort($arr);
来源：http://zq.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wi.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fg.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sp.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://et.521024.cn

Ruby: arr.sort
来源：http://er.yuntaijiaju.cn

C#:   list.Sort();
来源：http://rs.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pn.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dv.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yw.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gi.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lj.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ay.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://se.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://me.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cr.9csxet.cn

[D11] 反转数组
来源：http://mn.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fd.colortex.cn

PHP:  array_reverse($arr);
来源：http://ap.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hv.colortex.cn

TS:   [...arr].reverse();
来源：http://ll.colortex.cn

Java: Collections.reverse(list);
来源：http://ce.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://lz.shxzukj.cn

Ruby: arr.reverse
来源：http://mz.shxzukj.cn

C#:   list.Reverse();
来源：http://jl.nicolike.cn

[D12] 查找元素下标
来源：http://wr.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://xd.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://re.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oa.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mp.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qr.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://pr.hnjuh.cn

Ruby: arr.index(x)
来源：http://nm.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ie.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://wu.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zv.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://io.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://lv.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://ak.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mk.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ws.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jy.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://va.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://fl.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://og.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ng.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://im.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://rh.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://py.hnjuh.cn

Go:   // 手写循环
来源：http://zi.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mo.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rv.jctech888.com.cn

[D15] 去重
来源：http://ak.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dz.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://hb.colortex.cn

JS:   [...new Set(arr)]
来源：http://wz.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://qa.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://im.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gf.shxzskj.cn

Ruby: arr.uniq
来源：http://gh.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://dh.bjjhwx.cn

[D16] 求和与平均值
来源：http://iz.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pn.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ms.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://db.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ti.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dd.haigaiapp.cn

Go:   // 手写循环累加
来源：http://hw.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yv.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://tm.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://ny.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://ni.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://zd.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uq.huanxung.cn

TS:   Math.max(...arr);
来源：http://ik.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sm.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ct.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://jv.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://qe.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://ys.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ev.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://no.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xh.bookmarksfly.cn

TS:   nested.flat();
来源：http://vb.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wl.lnxyls.cn

Go:   // 手写双层循环
来源：http://es.shxzukj.cn

Ruby: nested.flatten
来源：http://rn.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pn.newstarts.cn

[D19] 按字段分组
来源：http://nr.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ow.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mt.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rk.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://th.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tm.521024.cn

Go:   // 手写 map[string][]T
来源：http://tt.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yg.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jj.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://do.huixiangedu.cn

Py:   Counter(arr)
来源：http://lf.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://vu.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ur.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fe.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fb.hahajie.cn

Go:   // 手写 map[T]int
来源：http://pk.gzmigu.cn

Ruby: arr.tally
来源：http://ak.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cl.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://yd.nicolike.cn

Py:   x in arr
来源：http://ej.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://wk.hnjuh.cn

JS:   arr.includes(x)
来源：http://wu.gzmigu.cn

TS:   arr.includes(x)
来源：http://ci.bookmarksfly.cn

Java: list.contains(x)
来源：http://yd.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://em.lnxyls.cn

Ruby: arr.include?(x)
来源：http://sw.huixiangedu.cn

C#:   list.Contains(x)
来源：http://ao.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://re.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qz.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qs.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ba.colortex.cn

TS:   [...arr];
来源：http://cd.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://yw.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bw.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://rd.chemitech.net.cn

C#:   new List<int>(list);
来源：http://ka.lnxyls.cn

[D23] reduce 累积计算
来源：http://he.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yq.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wc.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ju.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qj.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ze.muxihuayi.cn

Go:   // 手写循环
来源：http://pd.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vm.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sx.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://ns.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bp.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tu.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cp.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tv.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uw.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xb.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dq.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://za.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://nf.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://io.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jv.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uy.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iu.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vb.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pw.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fa.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dz.shxzskj.cn

[D26] 数组转字符串
来源：http://ua.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://mj.521024.cn

PHP:  implode(", ", $arr);
来源：http://xp.521024.cn

JS:   arr.join(", ")
来源：http://qe.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://uk.nszjky.cn

Java: String.join(", ", list)
来源：http://pg.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://ya.panjiajie.cn

Ruby: arr.join(", ")
来源：http://th.newstarts.cn

C#:   string.Join(", ", list)
来源：http://ye.bjjhwx.cn

================================================================================
来源：http://vn.haigaiapp.cn

E. 字符串处理
来源：http://cz.nszjky.cn

================================================================================
来源：http://yr.panjiajie.cn

[E01] 拼接字符串
来源：http://nq.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://am.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://me.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bj.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://up.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yv.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wu.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kh.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zd.hahajie.cn

[E02] 重复字符串
来源：http://fk.yuexingan06.cn

Py:   "ab" * 3
来源：http://pn.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://yv.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://se.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://gx.szxytkj.cn

Java: "ab".repeat(3)
来源：http://pd.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://xj.colortex.cn

Ruby: "ab" * 3
来源：http://qk.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sw.shxzukj.cn

[E03] 截取子串
来源：http://sp.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zo.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fr.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ps.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://sz.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://hj.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://me.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fd.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://wv.chemitech.net.cn

[E04] 查找子串位置
来源：http://af.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://zw.colortex.cn

PHP:  strpos($s, "x");
来源：http://oh.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gy.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://pi.newstarts.cn

Java: s.indexOf("x")
来源：http://uj.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://gh.asd995.cn

Ruby: s.index("x")
来源：http://qh.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ay.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bf.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kq.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ka.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rg.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ge.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ep.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lv.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ya.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ke.szsharing.cn

[E06] 替换子串
来源：http://hu.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iw.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ub.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xy.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://un.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://et.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://as.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ki.521024.cn

C#:   s.Replace("a", "b")
来源：http://mf.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://og.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aw.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xm.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xr.9csxet.cn

TS:   s.split(",")
来源：http://cu.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mr.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cr.colortex.cn

Ruby: s.split(",");  s.split
来源：http://kk.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jg.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://ks.colortex.cn

Py:   ",".join(items)
来源：http://yy.hnjuh.cn

PHP:  implode(",", $items);
来源：http://qd.muxihuayi.cn

JS:   items.join(",")
来源：http://vp.yuexingan06.cn

TS:   items.join(",")
来源：http://mz.haigaiapp.cn

Java: String.join(",", items)
来源：http://yj.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://gq.asd995.cn

Ruby: items.join(",")
来源：http://dn.colortex.cn

C#:   string.Join(",", items)
来源：http://vc.lnxyls.cn

[E09] 去除所有空白字符
来源：http://va.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://up.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tl.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://bb.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ig.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://nk.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aw.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yo.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vh.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://sd.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xx.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xd.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://na.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://vf.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://vd.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ab.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ia.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nf.huixinmuqiang.cn

[E11] 反转字符串
来源：http://pq.bookmarksfly.cn

Py:   s[::-1]
来源：http://cw.521024.cn

PHP:  strrev($s);
来源：http://iu.muxihuayi.cn


<!-- 参考信息 -->