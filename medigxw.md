代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bc.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gu.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://nt.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://ma.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://cb.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wi.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fv.panjiajie.cn

[D06] 数组长度
来源：http://yg.nicolike.cn

Py:   len(arr)
来源：http://er.asd995.cn

PHP:  count($arr);
来源：http://iu.shxzukj.cn

JS:   arr.length
来源：http://ku.9csxet.cn

TS:   arr.length
来源：http://mp.bjjhwx.cn

Java: list.size();
来源：http://vw.chemitech.net.cn

Go:   len(arr)
来源：http://en.huanxung.cn

Ruby: arr.length; arr.size
来源：http://dy.szxytkj.cn

C#:   list.Count;
来源：http://jn.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://iy.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ur.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hh.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://bi.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://rj.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://tk.newstarts.cn

Go:   arr[1:4]
来源：http://gz.huanxung.cn

Ruby: arr[1, 3]
来源：http://cb.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://ee.hnjuh.cn

[D08] 合并两个数组
来源：http://km.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://tq.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://gj.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uq.shtwfgs.cn

TS:   [...a, ...b];
来源：http://ez.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pm.yuexingan06.cn

Go:   append(a, b...)
来源：http://br.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://hp.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://lt.szxytkj.cn

[D09] 排序（升序）
来源：http://sm.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://lt.jctech888.com.cn

PHP:  sort($arr);
来源：http://fp.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ry.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tp.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ai.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fd.hahajie.cn

Ruby: arr.sort
来源：http://mk.nicolike.cn

C#:   list.Sort();
来源：http://xb.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ld.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cb.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gk.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jr.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ow.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://co.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uy.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kt.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tt.szsharing.cn

[D11] 反转数组
来源：http://vc.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cm.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://yc.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hb.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://fh.hnjuh.cn

Java: Collections.reverse(list);
来源：http://bx.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://ea.newstarts.cn

Ruby: arr.reverse
来源：http://tf.panjiajie.cn

C#:   list.Reverse();
来源：http://sv.jctech888.com.cn

[D12] 查找元素下标
来源：http://xn.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://br.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kt.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eq.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ld.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oo.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://er.muxihuayi.cn

Ruby: arr.index(x)
来源：http://rk.huanxung.cn

C#:   list.IndexOf(x);
来源：http://vg.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://lk.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ym.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ye.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://om.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://yk.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sw.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dm.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nl.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ar.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://ro.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kl.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sz.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://kv.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://rv.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ki.huixiangedu.cn

Go:   // 手写循环
来源：http://ks.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jv.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ns.colortex.cn

[D15] 去重
来源：http://zc.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xr.521024.cn

PHP:  array_unique($arr);
来源：http://rz.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://yn.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://pq.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://df.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qr.muxihuayi.cn

Ruby: arr.uniq
来源：http://ac.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://vq.szxytkj.cn

[D16] 求和与平均值
来源：http://ej.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ui.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ll.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://za.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eh.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://py.9csxet.cn

Go:   // 手写循环累加
来源：http://nm.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wd.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://qw.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://vx.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://jp.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://lr.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ea.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://do.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pk.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pu.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://oc.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://bp.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://cg.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ep.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://pl.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nr.wgjwhj.cn

TS:   nested.flat();
来源：http://mr.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://do.huixiangedu.cn

Go:   // 手写双层循环
来源：http://al.9csxet.cn

Ruby: nested.flatten
来源：http://kp.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ck.nszjky.cn

[D19] 按字段分组
来源：http://dq.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://no.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hp.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lz.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nb.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ni.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://xb.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dn.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://em.521024.cn

[D20] 统计每个元素出现次数
来源：http://vr.9csxet.cn

Py:   Counter(arr)
来源：http://cc.nszjky.cn

PHP:  array_count_values($arr);
来源：http://jg.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mi.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tq.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://td.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://ja.lnxyls.cn

Ruby: arr.tally
来源：http://hb.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wr.asd995.cn

[D21] 判断是否包含某元素
来源：http://pb.9csxet.cn

Py:   x in arr
来源：http://nc.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://xo.nicolike.cn

JS:   arr.includes(x)
来源：http://jv.wgjwhj.cn

TS:   arr.includes(x)
来源：http://rm.szxytkj.cn

Java: list.contains(x)
来源：http://ji.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://yb.lnxyls.cn

Ruby: arr.include?(x)
来源：http://lr.szsharing.cn

C#:   list.Contains(x)
来源：http://gl.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://js.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ck.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wr.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://we.jctech888.com.cn

TS:   [...arr];
来源：http://qo.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://cc.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ym.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://nh.shxzskj.cn

C#:   new List<int>(list);
来源：http://xa.9csxet.cn

[D23] reduce 累积计算
来源：http://ki.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vt.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tf.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jd.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nr.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fv.chemitech.net.cn

Go:   // 手写循环
来源：http://rz.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yo.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pm.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://pg.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ep.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jj.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kz.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qb.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sk.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tv.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rt.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yz.colortex.cn

[D25] Set 集合去重与交并差
来源：http://zl.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wi.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vr.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nn.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fv.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cd.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zt.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jc.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wi.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://ce.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ql.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://ye.yuexingan06.cn

JS:   arr.join(", ")
来源：http://tk.colortex.cn

TS:   arr.join(", ")
来源：http://mt.szsharing.cn

Java: String.join(", ", list)
来源：http://jx.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://vh.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://wh.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://aj.wgjwhj.cn

================================================================================
来源：http://fg.wgjwhj.cn

E. 字符串处理
来源：http://ys.hahajie.cn

================================================================================
来源：http://nz.shxzskj.cn

[E01] 拼接字符串
来源：http://uj.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ou.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sb.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qd.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qf.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ib.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://go.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fh.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kh.szxytkj.cn

[E02] 重复字符串
来源：http://ln.panjiajie.cn

Py:   "ab" * 3
来源：http://ym.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://or.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://iu.huanxung.cn

TS:   "ab".repeat(3)
来源：http://fa.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://st.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://qs.shtwfgs.cn

Ruby: "ab" * 3
来源：http://ro.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wj.yuntaijiaju.cn

[E03] 截取子串
来源：http://uj.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dm.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gt.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sd.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://qv.shxzukj.cn

Java: s.substring(1, 4)
来源：http://ub.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hy.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tb.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ai.newstarts.cn

[E04] 查找子串位置
来源：http://qr.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://tw.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://xi.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fo.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://lj.chemitech.net.cn

Java: s.indexOf("x")
来源：http://ae.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://qn.nicolike.cn

Ruby: s.index("x")
来源：http://xz.newstarts.cn

C#:   s.IndexOf("x")
来源：http://up.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://po.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://he.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dh.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kc.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kh.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uv.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uk.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ov.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ko.hnjuh.cn

[E06] 替换子串
来源：http://hi.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tp.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://aj.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vz.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://zu.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lj.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hu.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://et.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://pp.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://hg.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ev.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://td.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jm.huanxung.cn

TS:   s.split(",")
来源：http://eu.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kl.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oq.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://ue.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yc.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://lu.panjiajie.cn

Py:   ",".join(items)
来源：http://gm.asd995.cn

PHP:  implode(",", $items);
来源：http://so.hahajie.cn

JS:   items.join(",")
来源：http://jl.colortex.cn

TS:   items.join(",")
来源：http://gc.gzmigu.cn

Java: String.join(",", items)
来源：http://xx.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://sp.jctech888.com.cn

Ruby: items.join(",")
来源：http://vu.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://lv.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://xy.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dk.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tu.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://tp.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://wj.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://fc.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cw.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lb.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vh.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://do.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://he.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xh.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://yv.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://pq.colortex.cn

Java: String.format("%03d", 7)
来源：http://fd.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pa.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rp.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uk.yuexingan06.cn

[E11] 反转字符串
来源：http://ok.jctech888.com.cn

Py:   s[::-1]
来源：http://mk.huixiangedu.cn

PHP:  strrev($s);
来源：http://kb.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://to.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://xv.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hl.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vo.9csxet.cn

Ruby: s.reverse
来源：http://pb.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ft.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://er.yuexingan06.cn

Py:   s.count("a")
来源：http://mo.chemitech.net.cn


<!-- 参考信息 -->