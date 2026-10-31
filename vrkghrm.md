代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cu.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://tx.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ng.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gc.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ja.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ip.muxihuayi.cn

[D05] 访问与修改元素
来源：http://lm.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bi.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://et.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ff.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://mq.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://dh.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ha.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ri.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zy.wgjwhj.cn

[D06] 数组长度
来源：http://de.muxihuayi.cn

Py:   len(arr)
来源：http://al.nszjky.cn

PHP:  count($arr);
来源：http://ht.hnjuh.cn

JS:   arr.length
来源：http://mq.wgjwhj.cn

TS:   arr.length
来源：http://qg.bookmarksfly.cn

Java: list.size();
来源：http://xn.colortex.cn

Go:   len(arr)
来源：http://lw.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://vp.nicolike.cn

C#:   list.Count;
来源：http://mb.hahajie.cn

[D07] 切片 / 取子数组
来源：http://lx.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ss.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oi.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://mx.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://zn.nszjky.cn

Java: list.subList(1, 4);
来源：http://uy.haigaiapp.cn

Go:   arr[1:4]
来源：http://yo.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://va.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://io.jctech888.com.cn

[D08] 合并两个数组
来源：http://co.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://am.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://as.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nn.szsharing.cn

TS:   [...a, ...b];
来源：http://lm.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bc.huixiangedu.cn

Go:   append(a, b...)
来源：http://wz.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://au.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://ik.9csxet.cn

[D09] 排序（升序）
来源：http://rs.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://km.colortex.cn

PHP:  sort($arr);
来源：http://dq.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ew.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ch.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nq.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hh.9csxet.cn

Ruby: arr.sort
来源：http://gr.muxihuayi.cn

C#:   list.Sort();
来源：http://fg.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rs.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://to.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zx.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qh.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ga.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://by.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ac.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bv.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nj.szsharing.cn

[D11] 反转数组
来源：http://ek.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ei.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://ti.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bc.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://nf.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://rl.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://ac.huanxung.cn

Ruby: arr.reverse
来源：http://xs.szsharing.cn

C#:   list.Reverse();
来源：http://sg.huanxung.cn

[D12] 查找元素下标
来源：http://uo.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://ee.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dx.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gq.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cb.521024.cn

Go:   slices.Index(arr, x)
来源：http://dy.shxzukj.cn

Ruby: arr.index(x)
来源：http://sl.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://fi.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://fy.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ur.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ma.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://sj.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://jo.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mf.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ol.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jv.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ma.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://no.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qx.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pn.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://me.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://ik.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wk.hnjuh.cn

Go:   // 手写循环
来源：http://ua.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qd.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ml.bjjhwx.cn

[D15] 去重
来源：http://kl.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rl.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://yo.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://im.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://wp.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://is.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ey.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://rr.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ip.chemitech.net.cn

[D16] 求和与平均值
来源：http://tf.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yh.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://de.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ja.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xi.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ad.nicolike.cn

Go:   // 手写循环累加
来源：http://kl.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dm.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://mr.hnjuh.cn

[D17] 最大值与最小值
来源：http://xf.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://cg.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://se.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xv.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://eh.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mg.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ci.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://hd.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://sy.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://rl.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fi.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://rd.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nx.huanxung.cn

TS:   nested.flat();
来源：http://wj.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gd.lnxyls.cn

Go:   // 手写双层循环
来源：http://pu.szsharing.cn

Ruby: nested.flatten
来源：http://ed.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iq.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ds.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ze.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jt.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rq.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uy.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pb.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://tq.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rh.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vh.colortex.cn

[D20] 统计每个元素出现次数
来源：http://jl.wgjwhj.cn

Py:   Counter(arr)
来源：http://zo.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ol.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dg.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qt.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bk.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://yn.szsharing.cn

Ruby: arr.tally
来源：http://su.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oo.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://gg.bookmarksfly.cn

Py:   x in arr
来源：http://wy.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://mq.szsharing.cn

JS:   arr.includes(x)
来源：http://zl.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://ku.nszjky.cn

Java: list.contains(x)
来源：http://zw.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://tk.nszjky.cn

Ruby: arr.include?(x)
来源：http://cs.hnjuh.cn

C#:   list.Contains(x)
来源：http://sy.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://bx.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jw.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ln.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://te.jianghongdianzi.cn

TS:   [...arr];
来源：http://rg.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://ic.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://er.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://jr.nszjky.cn

C#:   new List<int>(list);
来源：http://pg.9csxet.cn

[D23] reduce 累积计算
来源：http://xi.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vf.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kk.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ru.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ys.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ew.yuntaijiaju.cn

Go:   // 手写循环
来源：http://it.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yj.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cc.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://qx.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vr.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://up.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ji.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hd.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rk.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sx.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://we.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aw.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://my.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zr.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fu.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bu.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fy.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vz.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zn.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cn.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vc.szsharing.cn

[D26] 数组转字符串
来源：http://vk.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://pj.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://hx.shxzukj.cn

JS:   arr.join(", ")
来源：http://ha.newstarts.cn

TS:   arr.join(", ")
来源：http://xi.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://ma.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://ki.asd995.cn

Ruby: arr.join(", ")
来源：http://yq.szsharing.cn

C#:   string.Join(", ", list)
来源：http://eo.newstarts.cn

================================================================================
来源：http://sk.haigaiapp.cn

E. 字符串处理
来源：http://ri.colortex.cn

================================================================================
来源：http://oo.colortex.cn

[E01] 拼接字符串
来源：http://dq.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jr.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nm.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fh.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ge.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ha.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://km.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uy.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nf.9csxet.cn

[E02] 重复字符串
来源：http://rl.hahajie.cn

Py:   "ab" * 3
来源：http://aa.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://dv.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://ap.asd995.cn

TS:   "ab".repeat(3)
来源：http://fx.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://km.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://er.hnjuh.cn

Ruby: "ab" * 3
来源：http://nn.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jo.newstarts.cn

[E03] 截取子串
来源：http://au.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yv.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vh.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bi.asd995.cn

TS:   s.slice(1, 4)
来源：http://mt.nicolike.cn

Java: s.substring(1, 4)
来源：http://ox.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ly.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bq.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://os.colortex.cn

[E04] 查找子串位置
来源：http://ez.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://kh.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://tc.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rn.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://rk.hnjuh.cn

Java: s.indexOf("x")
来源：http://oc.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://rx.9csxet.cn

Ruby: s.index("x")
来源：http://op.asd995.cn

C#:   s.IndexOf("x")
来源：http://al.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ey.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zc.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://an.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://th.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tx.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://au.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ap.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mz.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wn.lnxyls.cn

[E06] 替换子串
来源：http://ky.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lm.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://kq.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ug.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://gq.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ke.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uk.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fl.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://po.hnjuh.cn

[E07] 按分隔符拆分
来源：http://kj.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://de.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xp.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jj.huixiangedu.cn

TS:   s.split(",")
来源：http://uv.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pa.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sw.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://ue.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gp.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://bx.yuexingan06.cn

Py:   ",".join(items)
来源：http://js.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://vn.jianghongdianzi.cn

JS:   items.join(",")
来源：http://aa.9csxet.cn

TS:   items.join(",")
来源：http://iz.huanxung.cn

Java: String.join(",", items)
来源：http://ng.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://ii.szsharing.cn

Ruby: items.join(",")
来源：http://ht.colortex.cn

C#:   string.Join(",", items)
来源：http://gp.hahajie.cn

[E09] 去除所有空白字符
来源：http://wr.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://be.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mh.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ym.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://dx.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://op.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://am.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nv.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://js.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://gf.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sh.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xs.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://mq.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://ue.newstarts.cn

Java: String.format("%03d", 7)
来源：http://hu.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vo.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nn.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ou.bjjhwx.cn

[E11] 反转字符串
来源：http://qa.lnxyls.cn

Py:   s[::-1]
来源：http://he.9csxet.cn

PHP:  strrev($s);
来源：http://mh.yuexingan06.cn


<!-- 参考信息 -->