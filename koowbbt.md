代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mp.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nz.gzmigu.cn

[D05] 访问与修改元素
来源：http://cv.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ds.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nc.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kk.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://tt.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://gy.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://dg.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dd.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://je.lnxyls.cn

[D06] 数组长度
来源：http://jl.panjiajie.cn

Py:   len(arr)
来源：http://ib.shtwfgs.cn

PHP:  count($arr);
来源：http://ns.nicolike.cn

JS:   arr.length
来源：http://jb.muxihuayi.cn

TS:   arr.length
来源：http://zf.nszjky.cn

Java: list.size();
来源：http://gf.9csxet.cn

Go:   len(arr)
来源：http://jz.521024.cn

Ruby: arr.length; arr.size
来源：http://ur.wgjwhj.cn

C#:   list.Count;
来源：http://ur.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://rn.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://az.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jx.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://au.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://fr.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://px.gzmigu.cn

Go:   arr[1:4]
来源：http://qm.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://xe.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://zl.jctech888.com.cn

[D08] 合并两个数组
来源：http://pe.521024.cn

Py:   a + b;  a.extend(b)
来源：http://mb.asd995.cn

PHP:  array_merge($a, $b);
来源：http://ha.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zm.szsharing.cn

TS:   [...a, ...b];
来源：http://wl.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yj.shxzukj.cn

Go:   append(a, b...)
来源：http://tu.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://vk.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://qr.shxzukj.cn

[D09] 排序（升序）
来源：http://uj.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://gx.gzmigu.cn

PHP:  sort($arr);
来源：http://aw.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://om.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pu.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://my.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wu.yuntaijiaju.cn

Ruby: arr.sort
来源：http://qd.jianghongdianzi.cn

C#:   list.Sort();
来源：http://lq.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lb.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pp.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jd.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fc.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vx.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://no.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mb.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cb.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uz.huanxung.cn

[D11] 反转数组
来源：http://gg.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://km.szsharing.cn

PHP:  array_reverse($arr);
来源：http://mp.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xw.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://rl.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://sl.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://qj.huixiangedu.cn

Ruby: arr.reverse
来源：http://ow.hnjuh.cn

C#:   list.Reverse();
来源：http://wx.nicolike.cn

[D12] 查找元素下标
来源：http://bo.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://do.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gy.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jr.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://so.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://un.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://il.newstarts.cn

Ruby: arr.index(x)
来源：http://vs.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://wl.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://eo.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nt.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ci.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://rj.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://rg.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xn.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hs.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yf.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://so.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://ex.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://id.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://br.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://yy.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://zk.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://su.nszjky.cn

Go:   // 手写循环
来源：http://dp.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mn.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gw.huixiangedu.cn

[D15] 去重
来源：http://uz.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qn.shxzskj.cn

PHP:  array_unique($arr);
来源：http://wz.nszjky.cn

JS:   [...new Set(arr)]
来源：http://fa.9csxet.cn

TS:   [...new Set(arr)]
来源：http://uo.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ov.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jb.szsharing.cn

Ruby: arr.uniq
来源：http://oe.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://sk.chemitech.net.cn

[D16] 求和与平均值
来源：http://vi.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pz.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jp.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tj.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xp.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ag.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://ff.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ke.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://ml.colortex.cn

[D17] 最大值与最小值
来源：http://bn.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://or.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://fb.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jr.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://lk.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mm.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ru.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://tz.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://we.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://vi.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fw.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://xj.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ys.yuntaijiaju.cn

TS:   nested.flat();
来源：http://sd.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fh.panjiajie.cn

Go:   // 手写双层循环
来源：http://dg.521024.cn

Ruby: nested.flatten
来源：http://zv.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://da.shtwfgs.cn

[D19] 按字段分组
来源：http://gi.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gk.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wi.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eh.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mr.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://se.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wh.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mp.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://mh.panjiajie.cn

Py:   Counter(arr)
来源：http://xn.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://qt.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fu.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hw.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cv.9csxet.cn

Go:   // 手写 map[T]int
来源：http://pn.asd995.cn

Ruby: arr.tally
来源：http://fc.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iz.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://vd.hahajie.cn

Py:   x in arr
来源：http://en.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://yw.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://je.haigaiapp.cn

TS:   arr.includes(x)
来源：http://uv.haigaiapp.cn

Java: list.contains(x)
来源：http://fl.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://fb.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://wd.521024.cn

C#:   list.Contains(x)
来源：http://us.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://wl.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ud.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vb.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kz.shxzskj.cn

TS:   [...arr];
来源：http://ej.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://lr.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kp.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://rk.nszjky.cn

C#:   new List<int>(list);
来源：http://iy.hahajie.cn

[D23] reduce 累积计算
来源：http://dg.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tc.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ci.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ok.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://si.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ew.szsharing.cn

Go:   // 手写循环
来源：http://nd.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dm.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pl.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://pr.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ha.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pm.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gn.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gh.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://je.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hk.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ce.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qt.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://rk.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qb.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ge.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wh.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ro.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ih.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uw.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ej.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oc.9csxet.cn

[D26] 数组转字符串
来源：http://zw.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://wl.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://ju.panjiajie.cn

JS:   arr.join(", ")
来源：http://we.nicolike.cn

TS:   arr.join(", ")
来源：http://on.huixiangedu.cn

Java: String.join(", ", list)
来源：http://ir.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://kz.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://gi.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://bm.wgjwhj.cn

================================================================================
来源：http://zr.huixiangedu.cn

E. 字符串处理
来源：http://zo.muxihuayi.cn

================================================================================
来源：http://ht.szxytkj.cn

[E01] 拼接字符串
来源：http://vw.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tk.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nb.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yz.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ih.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nl.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://va.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xw.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mq.colortex.cn

[E02] 重复字符串
来源：http://kf.jctech888.com.cn

Py:   "ab" * 3
来源：http://lx.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://fc.szsharing.cn

JS:   "ab".repeat(3)
来源：http://px.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://rh.colortex.cn

Java: "ab".repeat(3)
来源：http://ju.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://fw.szsharing.cn

Ruby: "ab" * 3
来源：http://hk.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vr.hahajie.cn

[E03] 截取子串
来源：http://sb.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mp.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rb.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dg.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://xn.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://cp.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pk.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tk.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://kx.shtwfgs.cn

[E04] 查找子串位置
来源：http://yt.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://bk.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://pq.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fc.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://xh.shtwfgs.cn

Java: s.indexOf("x")
来源：http://kb.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://wf.hnjuh.cn

Ruby: s.index("x")
来源：http://ew.asd995.cn

C#:   s.IndexOf("x")
来源：http://gd.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mj.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dd.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yt.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://un.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zi.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zz.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qw.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rp.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zd.nicolike.cn

[E06] 替换子串
来源：http://st.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ti.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://tm.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hv.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://hi.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wa.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kh.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ws.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://ef.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://kb.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nu.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ww.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ed.shtwfgs.cn

TS:   s.split(",")
来源：http://li.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kb.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bf.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://yo.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rc.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://we.gzmigu.cn

Py:   ",".join(items)
来源：http://qx.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://cf.nszjky.cn

JS:   items.join(",")
来源：http://qn.jianghongdianzi.cn

TS:   items.join(",")
来源：http://ah.shxzukj.cn

Java: String.join(",", items)
来源：http://qv.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://nf.shxzukj.cn

Ruby: items.join(",")
来源：http://bn.nicolike.cn

C#:   string.Join(",", items)
来源：http://fh.gzmigu.cn

[E09] 去除所有空白字符
来源：http://hp.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://de.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pr.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://wh.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://kw.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://fq.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mk.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fi.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kz.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://sq.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sp.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vx.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://nf.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://pa.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ut.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pq.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ww.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dp.haigaiapp.cn

[E11] 反转字符串
来源：http://kk.shxzukj.cn

Py:   s[::-1]
来源：http://gg.bookmarksfly.cn

PHP:  strrev($s);
来源：http://vo.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://tc.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://ba.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hh.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nq.panjiajie.cn


<!-- 参考信息 -->