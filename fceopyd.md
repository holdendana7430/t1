代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://rj.gzmigu.cn

Java: list.add(0, 0);
来源：http://zz.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ys.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://to.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://kv.gzmigu.cn

[D04] 删除元素
来源：http://di.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hu.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ni.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wc.521024.cn

TS:   arr.splice(0, 1);
来源：http://vi.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fz.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ar.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hh.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xr.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://wi.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ot.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://be.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eu.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://kl.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://lv.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://wc.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mw.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bn.chemitech.net.cn

[D06] 数组长度
来源：http://fy.jianghongdianzi.cn

Py:   len(arr)
来源：http://cb.nszjky.cn

PHP:  count($arr);
来源：http://hq.hnjuh.cn

JS:   arr.length
来源：http://zp.shtwfgs.cn

TS:   arr.length
来源：http://au.newstarts.cn

Java: list.size();
来源：http://al.bjjhwx.cn

Go:   len(arr)
来源：http://ol.9csxet.cn

Ruby: arr.length; arr.size
来源：http://bj.newstarts.cn

C#:   list.Count;
来源：http://iu.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://dj.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fb.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ex.asd995.cn

JS:   arr.slice(1, 4);
来源：http://hv.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://bs.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://sm.bookmarksfly.cn

Go:   arr[1:4]
来源：http://dg.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://tu.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://ts.bookmarksfly.cn

[D08] 合并两个数组
来源：http://jv.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://xe.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://aw.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rl.huanxung.cn

TS:   [...a, ...b];
来源：http://af.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ox.haigaiapp.cn

Go:   append(a, b...)
来源：http://qv.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://cj.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://li.szsharing.cn

[D09] 排序（升序）
来源：http://un.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://pc.bookmarksfly.cn

PHP:  sort($arr);
来源：http://wn.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wm.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uz.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vn.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qa.huanxung.cn

Ruby: arr.sort
来源：http://ow.shtwfgs.cn

C#:   list.Sort();
来源：http://ag.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dr.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kf.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lg.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qk.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bn.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lp.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uz.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yg.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zr.muxihuayi.cn

[D11] 反转数组
来源：http://sl.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ev.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://nt.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wf.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://mg.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://xt.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://ju.yuexingan06.cn

Ruby: arr.reverse
来源：http://wo.muxihuayi.cn

C#:   list.Reverse();
来源：http://rx.9csxet.cn

[D12] 查找元素下标
来源：http://hr.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://va.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tr.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kj.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://om.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fq.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://ef.colortex.cn

Ruby: arr.index(x)
来源：http://nt.hahajie.cn

C#:   list.IndexOf(x);
来源：http://on.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://xf.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ss.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ts.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://ie.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://yb.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gb.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dk.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rc.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lh.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://ca.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xl.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mf.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://sp.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://ky.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ba.bookmarksfly.cn

Go:   // 手写循环
来源：http://yt.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wc.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ls.yuntaijiaju.cn

[D15] 去重
来源：http://tz.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ga.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://np.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://ra.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://xl.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yh.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gx.yuexingan06.cn

Ruby: arr.uniq
来源：http://us.asd995.cn

C#:   list.Distinct().ToList()
来源：http://je.huixiangedu.cn

[D16] 求和与平均值
来源：http://vk.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oc.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pp.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cp.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ka.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://et.hahajie.cn

Go:   // 手写循环累加
来源：http://ci.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gh.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://bd.9csxet.cn

[D17] 最大值与最小值
来源：http://gt.asd995.cn

Py:   max(arr);  min(arr)
来源：http://em.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://we.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zq.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://gn.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uw.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ds.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://qj.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ug.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://sr.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nd.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://kh.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pq.panjiajie.cn

TS:   nested.flat();
来源：http://gk.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dd.huanxung.cn

Go:   // 手写双层循环
来源：http://wk.nicolike.cn

Ruby: nested.flatten
来源：http://ek.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bk.asd995.cn

[D19] 按字段分组
来源：http://rm.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xk.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oa.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lh.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sh.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gi.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://wt.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qw.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vb.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://cf.chemitech.net.cn

Py:   Counter(arr)
来源：http://nj.asd995.cn

PHP:  array_count_values($arr);
来源：http://yq.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hd.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pf.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dj.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://ro.panjiajie.cn

Ruby: arr.tally
来源：http://kk.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ic.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://dl.9csxet.cn

Py:   x in arr
来源：http://sa.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://ae.hahajie.cn

JS:   arr.includes(x)
来源：http://aq.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://iw.gzmigu.cn

Java: list.contains(x)
来源：http://xq.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://wk.shxzskj.cn

Ruby: arr.include?(x)
来源：http://ce.wgjwhj.cn

C#:   list.Contains(x)
来源：http://fr.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://dl.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ly.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ca.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tp.huixiangedu.cn

TS:   [...arr];
来源：http://hk.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://vv.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vp.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ls.bjjhwx.cn

C#:   new List<int>(list);
来源：http://wr.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://jp.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bm.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pi.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uc.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ya.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oy.gzmigu.cn

Go:   // 手写循环
来源：http://px.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vl.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qz.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://mz.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iw.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ga.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gs.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mj.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://um.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qx.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nj.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ms.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://gt.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hi.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gs.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sv.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vg.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jp.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vt.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lu.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yo.bjjhwx.cn

[D26] 数组转字符串
来源：http://at.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://xr.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://xu.jctech888.com.cn

JS:   arr.join(", ")
来源：http://gc.shxzukj.cn

TS:   arr.join(", ")
来源：http://fx.szsharing.cn

Java: String.join(", ", list)
来源：http://lb.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://rx.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://qf.newstarts.cn

C#:   string.Join(", ", list)
来源：http://lx.shtwfgs.cn

================================================================================
来源：http://wd.shxzukj.cn

E. 字符串处理
来源：http://wt.jctech888.com.cn

================================================================================
来源：http://sg.newstarts.cn

[E01] 拼接字符串
来源：http://ak.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ao.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vd.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xu.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://te.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yr.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pi.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ly.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ei.newstarts.cn

[E02] 重复字符串
来源：http://ei.chemitech.net.cn

Py:   "ab" * 3
来源：http://fe.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://ob.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ln.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://gh.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://up.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://hz.gzmigu.cn

Ruby: "ab" * 3
来源：http://ln.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kz.hnjuh.cn

[E03] 截取子串
来源：http://zq.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ky.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ax.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gr.asd995.cn

TS:   s.slice(1, 4)
来源：http://fx.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://cm.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ec.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://as.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://rr.muxihuayi.cn

[E04] 查找子串位置
来源：http://rl.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://jn.nicolike.cn

PHP:  strpos($s, "x");
来源：http://gj.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://id.nszjky.cn

TS:   s.indexOf("x")
来源：http://hi.muxihuayi.cn

Java: s.indexOf("x")
来源：http://wv.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://rm.szxytkj.cn

Ruby: s.index("x")
来源：http://iz.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://qe.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zq.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dh.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vc.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tq.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yj.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sg.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ed.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cd.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mm.lnxyls.cn

[E06] 替换子串
来源：http://ku.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mb.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://hy.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ba.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://cr.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xg.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uh.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cj.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://gv.szsharing.cn

[E07] 按分隔符拆分
来源：http://yg.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wh.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wn.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://im.yuexingan06.cn

TS:   s.split(",")
来源：http://ji.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://if.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dm.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://cq.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jx.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://um.newstarts.cn

Py:   ",".join(items)
来源：http://sx.colortex.cn

PHP:  implode(",", $items);
来源：http://vv.newstarts.cn

JS:   items.join(",")
来源：http://yk.521024.cn

TS:   items.join(",")
来源：http://mr.asd995.cn

Java: String.join(",", items)
来源：http://tf.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://sn.hnjuh.cn

Ruby: items.join(",")
来源：http://xi.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://vv.huanxung.cn

[E09] 去除所有空白字符
来源：http://lx.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hy.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kf.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://vi.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://hq.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://ri.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tc.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hk.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lj.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://jg.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wm.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kv.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://yz.muxihuayi.cn


<!-- 参考信息 -->