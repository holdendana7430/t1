代发 wailian999

C#:   list.Insert(0, 0);
来源：http://gv.muxihuayi.cn

[D04] 删除元素
来源：http://xg.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lp.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://is.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dx.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://go.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cj.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cw.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bn.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hy.asd995.cn

[D05] 访问与修改元素
来源：http://km.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qd.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fx.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xh.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://es.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://ks.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://vm.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://af.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aa.muxihuayi.cn

[D06] 数组长度
来源：http://wp.jctech888.com.cn

Py:   len(arr)
来源：http://wz.huixiangedu.cn

PHP:  count($arr);
来源：http://wz.chemitech.net.cn

JS:   arr.length
来源：http://kf.jianghongdianzi.cn

TS:   arr.length
来源：http://zx.yuexingan06.cn

Java: list.size();
来源：http://mk.lnxyls.cn

Go:   len(arr)
来源：http://ti.521024.cn

Ruby: arr.length; arr.size
来源：http://hn.yuexingan06.cn

C#:   list.Count;
来源：http://tw.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://qh.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qg.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ut.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://cg.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ok.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://au.lnxyls.cn

Go:   arr[1:4]
来源：http://yl.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://zt.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://mw.newstarts.cn

[D08] 合并两个数组
来源：http://bm.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://ly.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://bw.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yf.huixiangedu.cn

TS:   [...a, ...b];
来源：http://xw.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mx.yuexingan06.cn

Go:   append(a, b...)
来源：http://lj.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://lb.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://nh.wgjwhj.cn

[D09] 排序（升序）
来源：http://vd.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ch.shtwfgs.cn

PHP:  sort($arr);
来源：http://px.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dk.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kx.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cd.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wr.jianghongdianzi.cn

Ruby: arr.sort
来源：http://jf.bookmarksfly.cn

C#:   list.Sort();
来源：http://vn.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kk.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://um.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yk.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://de.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ks.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pw.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://am.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://st.szxytkj.cn

[D11] 反转数组
来源：http://la.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iy.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://vt.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ac.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://xr.panjiajie.cn

Java: Collections.reverse(list);
来源：http://hx.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://hw.haigaiapp.cn

Ruby: arr.reverse
来源：http://xd.panjiajie.cn

C#:   list.Reverse();
来源：http://kp.huanxung.cn

[D12] 查找元素下标
来源：http://sc.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://qs.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pe.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iu.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ox.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://re.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://td.nszjky.cn

Ruby: arr.index(x)
来源：http://of.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://pf.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://kl.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gy.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nj.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://ku.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://ip.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ij.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vl.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zt.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sn.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://gd.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qc.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tc.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://nr.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://kv.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rj.shxzskj.cn

Go:   // 手写循环
来源：http://lf.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fy.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://th.hahajie.cn

[D15] 去重
来源：http://yd.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://no.gzmigu.cn

PHP:  array_unique($arr);
来源：http://ao.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://bd.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://bc.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jl.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ho.lnxyls.cn

Ruby: arr.uniq
来源：http://jo.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://uk.shtwfgs.cn

[D16] 求和与平均值
来源：http://rt.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qu.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://co.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mj.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://et.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fg.asd995.cn

Go:   // 手写循环累加
来源：http://qb.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zz.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://fi.newstarts.cn

[D17] 最大值与最小值
来源：http://tt.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://zn.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://tv.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kz.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://ef.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mq.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qj.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://mm.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://ht.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://pi.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ol.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ot.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fa.jctech888.com.cn

TS:   nested.flat();
来源：http://fr.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uq.panjiajie.cn

Go:   // 手写双层循环
来源：http://nm.9csxet.cn

Ruby: nested.flatten
来源：http://qh.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sr.huixiangedu.cn

[D19] 按字段分组
来源：http://bw.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hc.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rq.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tg.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lx.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://di.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://da.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kk.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gz.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://uh.shxzukj.cn

Py:   Counter(arr)
来源：http://wl.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://va.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ju.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uo.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xs.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://dv.panjiajie.cn

Ruby: arr.tally
来源：http://dx.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://re.huanxung.cn

[D21] 判断是否包含某元素
来源：http://wq.yuexingan06.cn

Py:   x in arr
来源：http://lr.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://pa.haigaiapp.cn

JS:   arr.includes(x)
来源：http://wx.nicolike.cn

TS:   arr.includes(x)
来源：http://ej.colortex.cn

Java: list.contains(x)
来源：http://bu.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://gg.huanxung.cn

Ruby: arr.include?(x)
来源：http://af.szsharing.cn

C#:   list.Contains(x)
来源：http://qm.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://vd.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ut.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qh.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://on.shxzskj.cn

TS:   [...arr];
来源：http://co.colortex.cn

Java: new ArrayList<>(list);
来源：http://pf.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kx.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://bd.muxihuayi.cn

C#:   new List<int>(list);
来源：http://pa.yuexingan06.cn

[D23] reduce 累积计算
来源：http://tr.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yw.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sv.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kv.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fm.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qd.newstarts.cn

Go:   // 手写循环
来源：http://sr.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rk.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ph.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://xk.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kr.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gp.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ry.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hh.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oi.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tl.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://za.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vt.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://no.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ni.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zn.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tj.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yi.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tj.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ce.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ih.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yw.colortex.cn

[D26] 数组转字符串
来源：http://ge.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://mt.asd995.cn

PHP:  implode(", ", $arr);
来源：http://hk.lnxyls.cn

JS:   arr.join(", ")
来源：http://nu.521024.cn

TS:   arr.join(", ")
来源：http://fi.newstarts.cn

Java: String.join(", ", list)
来源：http://oo.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://mf.nicolike.cn

Ruby: arr.join(", ")
来源：http://oy.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://oq.yuntaijiaju.cn

================================================================================
来源：http://fu.asd995.cn

E. 字符串处理
来源：http://bk.jctech888.com.cn

================================================================================
来源：http://ww.nicolike.cn

[E01] 拼接字符串
来源：http://iy.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ri.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pw.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ld.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mx.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gm.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://le.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kt.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ed.jianghongdianzi.cn

[E02] 重复字符串
来源：http://ll.chemitech.net.cn

Py:   "ab" * 3
来源：http://lb.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://ff.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://jr.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://wq.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://wz.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://re.hahajie.cn

Ruby: "ab" * 3
来源：http://op.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gk.panjiajie.cn

[E03] 截取子串
来源：http://cr.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yg.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hj.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mk.521024.cn

TS:   s.slice(1, 4)
来源：http://ye.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://oq.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hb.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mn.colortex.cn

C#:   s.Substring(1, 3)
来源：http://ub.hahajie.cn

[E04] 查找子串位置
来源：http://qk.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://ap.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://ay.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bd.asd995.cn

TS:   s.indexOf("x")
来源：http://my.lnxyls.cn

Java: s.indexOf("x")
来源：http://vl.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://ki.bjjhwx.cn

Ruby: s.index("x")
来源：http://jq.asd995.cn

C#:   s.IndexOf("x")
来源：http://wj.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bw.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cc.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wh.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ly.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oo.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ju.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hb.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uy.colortex.cn

[E06] 替换子串
来源：http://uz.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nj.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://jb.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sn.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://hw.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ic.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tw.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hy.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://we.521024.cn

[E07] 按分隔符拆分
来源：http://gc.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xn.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xg.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dh.asd995.cn

TS:   s.split(",")
来源：http://rb.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uk.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lu.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://me.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zg.huanxung.cn

[E08] 数组按分隔符合并
来源：http://qb.nicolike.cn

Py:   ",".join(items)
来源：http://bz.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://mv.asd995.cn

JS:   items.join(",")
来源：http://kc.521024.cn

TS:   items.join(",")
来源：http://au.521024.cn

Java: String.join(",", items)
来源：http://js.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://tc.521024.cn

Ruby: items.join(",")
来源：http://ms.hnjuh.cn

C#:   string.Join(",", items)
来源：http://hv.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://af.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ld.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hx.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://iu.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://hj.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://as.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zk.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wh.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ds.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://go.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wx.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gn.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://ue.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://ax.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://be.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bt.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pd.9csxet.cn


<!-- 参考信息 -->