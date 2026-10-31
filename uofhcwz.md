代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yy.colortex.cn

TS:   arr.splice(0, 1);
来源：http://jr.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wh.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ok.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ni.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rn.hahajie.cn

[D05] 访问与修改元素
来源：http://ib.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tc.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gu.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://as.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ey.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://an.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://zc.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uo.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gc.colortex.cn

[D06] 数组长度
来源：http://ui.nicolike.cn

Py:   len(arr)
来源：http://gt.shxzukj.cn

PHP:  count($arr);
来源：http://ow.wgjwhj.cn

JS:   arr.length
来源：http://xv.shxzukj.cn

TS:   arr.length
来源：http://cr.huanxung.cn

Java: list.size();
来源：http://hn.szsharing.cn

Go:   len(arr)
来源：http://hn.newstarts.cn

Ruby: arr.length; arr.size
来源：http://wp.newstarts.cn

C#:   list.Count;
来源：http://xn.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://bc.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bv.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://po.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://vx.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://ai.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://aw.nszjky.cn

Go:   arr[1:4]
来源：http://ty.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://iv.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://tm.nicolike.cn

[D08] 合并两个数组
来源：http://ed.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://vt.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://ms.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nq.shxzskj.cn

TS:   [...a, ...b];
来源：http://qm.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gn.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://oz.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://uo.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://tp.newstarts.cn

[D09] 排序（升序）
来源：http://rh.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://ga.shtwfgs.cn

PHP:  sort($arr);
来源：http://pj.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kk.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://at.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tn.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xd.gzmigu.cn

Ruby: arr.sort
来源：http://ei.szxytkj.cn

C#:   list.Sort();
来源：http://gg.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zz.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://it.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ue.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nx.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pt.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ql.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hg.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ch.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sq.szsharing.cn

[D11] 反转数组
来源：http://ja.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uu.newstarts.cn

PHP:  array_reverse($arr);
来源：http://nr.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yu.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ii.shxzskj.cn

Java: Collections.reverse(list);
来源：http://yz.521024.cn

Go:   slices.Reverse(arr)
来源：http://lo.shtwfgs.cn

Ruby: arr.reverse
来源：http://ca.jctech888.com.cn

C#:   list.Reverse();
来源：http://vs.chemitech.net.cn

[D12] 查找元素下标
来源：http://lr.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://lr.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dp.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://al.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oi.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zw.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://dt.shtwfgs.cn

Ruby: arr.index(x)
来源：http://in.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://pd.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://hm.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fe.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ad.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://nj.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://ho.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tv.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mx.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uh.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yr.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://wf.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bu.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yg.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://bq.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://kh.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cc.huanxung.cn

Go:   // 手写循环
来源：http://go.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ss.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bv.shxzskj.cn

[D15] 去重
来源：http://pq.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ay.hnjuh.cn

PHP:  array_unique($arr);
来源：http://xf.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://fw.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ct.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kf.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://go.chemitech.net.cn

Ruby: arr.uniq
来源：http://yu.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://cu.bookmarksfly.cn

[D16] 求和与平均值
来源：http://th.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pe.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ma.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kz.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lw.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bt.colortex.cn

Go:   // 手写循环累加
来源：http://yp.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wt.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://le.wgjwhj.cn

[D17] 最大值与最小值
来源：http://ni.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://bk.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://uj.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qm.lnxyls.cn

TS:   Math.max(...arr);
来源：http://yj.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ac.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jf.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://wm.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://uh.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://xn.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fb.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://rm.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xh.huixinmuqiang.cn

TS:   nested.flat();
来源：http://mr.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oi.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://qo.nicolike.cn

Ruby: nested.flatten
来源：http://iz.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yu.colortex.cn

[D19] 按字段分组
来源：http://ha.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dx.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uj.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wq.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ky.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jk.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://dn.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://np.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://os.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://dc.9csxet.cn

Py:   Counter(arr)
来源：http://kp.szsharing.cn

PHP:  array_count_values($arr);
来源：http://jy.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sq.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dk.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yk.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://qg.wgjwhj.cn

Ruby: arr.tally
来源：http://uh.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://en.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://kn.panjiajie.cn

Py:   x in arr
来源：http://xx.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://zi.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://fl.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://dm.lnxyls.cn

Java: list.contains(x)
来源：http://xv.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://jm.huanxung.cn

Ruby: arr.include?(x)
来源：http://qs.wgjwhj.cn

C#:   list.Contains(x)
来源：http://ji.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://oi.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qh.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://an.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jv.asd995.cn

TS:   [...arr];
来源：http://kg.asd995.cn

Java: new ArrayList<>(list);
来源：http://ty.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vs.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://my.9csxet.cn

C#:   new List<int>(list);
来源：http://pb.521024.cn

[D23] reduce 累积计算
来源：http://id.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://it.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ms.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xz.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://em.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://el.huixiangedu.cn

Go:   // 手写循环
来源：http://dl.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vd.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hh.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://vb.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eo.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lz.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ef.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cq.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hy.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pp.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://be.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://do.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://fu.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rx.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gc.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tg.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gf.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eo.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hw.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kw.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://il.9csxet.cn

[D26] 数组转字符串
来源：http://xi.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://iq.asd995.cn

PHP:  implode(", ", $arr);
来源：http://iz.asd995.cn

JS:   arr.join(", ")
来源：http://tc.shtwfgs.cn

TS:   arr.join(", ")
来源：http://uq.asd995.cn

Java: String.join(", ", list)
来源：http://jd.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://zo.hahajie.cn

Ruby: arr.join(", ")
来源：http://py.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://zv.panjiajie.cn

================================================================================
来源：http://kg.szsharing.cn

E. 字符串处理
来源：http://gl.521024.cn

================================================================================
来源：http://vs.huanxung.cn

[E01] 拼接字符串
来源：http://du.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jj.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ob.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cf.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tv.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ta.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jf.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mg.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ee.huixiangedu.cn

[E02] 重复字符串
来源：http://rh.shtwfgs.cn

Py:   "ab" * 3
来源：http://hm.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://td.hahajie.cn

JS:   "ab".repeat(3)
来源：http://sc.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://in.shxzukj.cn

Java: "ab".repeat(3)
来源：http://qw.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ie.9csxet.cn

Ruby: "ab" * 3
来源：http://pj.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oa.yuntaijiaju.cn

[E03] 截取子串
来源：http://ex.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xf.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xy.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://my.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://bk.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://nu.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cd.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wj.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://on.haigaiapp.cn

[E04] 查找子串位置
来源：http://yw.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://oy.colortex.cn

PHP:  strpos($s, "x");
来源：http://yl.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qk.panjiajie.cn

TS:   s.indexOf("x")
来源：http://qb.shtwfgs.cn

Java: s.indexOf("x")
来源：http://sc.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://az.yuexingan06.cn

Ruby: s.index("x")
来源：http://jh.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://su.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nw.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zj.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dw.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pu.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xh.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yj.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ey.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ks.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yj.yuexingan06.cn

[E06] 替换子串
来源：http://xj.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wq.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://pc.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://re.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://yo.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://am.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nu.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qu.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://fq.huanxung.cn

[E07] 按分隔符拆分
来源：http://gl.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cv.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rb.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gr.haigaiapp.cn

TS:   s.split(",")
来源：http://gh.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sf.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yk.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://nf.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ax.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://xq.9csxet.cn

Py:   ",".join(items)
来源：http://xr.huanxung.cn

PHP:  implode(",", $items);
来源：http://yc.hnjuh.cn

JS:   items.join(",")
来源：http://rj.shxzskj.cn

TS:   items.join(",")
来源：http://xg.521024.cn

Java: String.join(",", items)
来源：http://mf.asd995.cn

Go:   strings.Join(items, ",")
来源：http://ff.szxytkj.cn

Ruby: items.join(",")
来源：http://ap.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://cs.hnjuh.cn

[E09] 去除所有空白字符
来源：http://dx.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://de.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pm.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://nh.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://xa.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://xj.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sc.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://id.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ls.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://fn.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aq.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zt.521024.cn

JS:   "7".padStart(3, "0")
来源：http://mm.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://sr.521024.cn

Java: String.format("%03d", 7)
来源：http://sv.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qp.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wu.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jw.szxytkj.cn

[E11] 反转字符串
来源：http://jw.yuntaijiaju.cn

Py:   s[::-1]
来源：http://fr.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://cn.szxytkj.cn


<!-- 参考信息 -->