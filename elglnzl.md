代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://md.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xd.haigaiapp.cn

[D05] 访问与修改元素
来源：http://zr.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ct.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pu.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uf.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://lz.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://kx.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://cs.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rf.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qg.huixiangedu.cn

[D06] 数组长度
来源：http://pd.szsharing.cn

Py:   len(arr)
来源：http://ai.huanxung.cn

PHP:  count($arr);
来源：http://wn.hahajie.cn

JS:   arr.length
来源：http://fy.gzmigu.cn

TS:   arr.length
来源：http://yq.nicolike.cn

Java: list.size();
来源：http://hd.lnxyls.cn

Go:   len(arr)
来源：http://jl.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://we.nicolike.cn

C#:   list.Count;
来源：http://es.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://ag.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yx.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cd.colortex.cn

JS:   arr.slice(1, 4);
来源：http://zi.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://st.9csxet.cn

Java: list.subList(1, 4);
来源：http://ov.wgjwhj.cn

Go:   arr[1:4]
来源：http://hd.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://jg.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://oc.521024.cn

[D08] 合并两个数组
来源：http://ui.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://ss.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://in.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hx.shxzskj.cn

TS:   [...a, ...b];
来源：http://ep.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wk.bjjhwx.cn

Go:   append(a, b...)
来源：http://cd.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://os.521024.cn

C#:   a.Concat(b).ToList()
来源：http://ml.newstarts.cn

[D09] 排序（升序）
来源：http://hy.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://ic.colortex.cn

PHP:  sort($arr);
来源：http://gn.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://st.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zi.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://la.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mx.nszjky.cn

Ruby: arr.sort
来源：http://lk.huanxung.cn

C#:   list.Sort();
来源：http://st.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ty.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://go.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://or.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gl.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://in.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rp.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sg.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yo.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vn.nszjky.cn

[D11] 反转数组
来源：http://za.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xx.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://wk.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ce.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://ny.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://zu.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://lw.yuexingan06.cn

Ruby: arr.reverse
来源：http://wx.szxytkj.cn

C#:   list.Reverse();
来源：http://ah.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://su.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://xj.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ju.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dq.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ux.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xi.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://ng.lnxyls.cn

Ruby: arr.index(x)
来源：http://kr.9csxet.cn

C#:   list.IndexOf(x);
来源：http://iw.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://gm.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tj.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mp.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://rx.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://yd.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xe.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kp.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ck.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ap.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://wz.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sv.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vg.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://sm.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ks.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fy.bjjhwx.cn

Go:   // 手写循环
来源：http://jf.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ip.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://if.newstarts.cn

[D15] 去重
来源：http://lb.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ki.9csxet.cn

PHP:  array_unique($arr);
来源：http://iu.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://cd.521024.cn

TS:   [...new Set(arr)]
来源：http://vz.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zh.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ey.szsharing.cn

Ruby: arr.uniq
来源：http://zc.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://qc.chemitech.net.cn

[D16] 求和与平均值
来源：http://xj.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gk.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lr.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ln.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wt.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mr.huanxung.cn

Go:   // 手写循环累加
来源：http://cr.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lh.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://hq.hnjuh.cn

[D17] 最大值与最小值
来源：http://wa.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://sc.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://xu.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vu.huanxung.cn

TS:   Math.max(...arr);
来源：http://ef.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rd.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ax.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://tp.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://dg.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://ke.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rf.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://xo.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gd.bjjhwx.cn

TS:   nested.flat();
来源：http://md.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vd.asd995.cn

Go:   // 手写双层循环
来源：http://vm.shxzskj.cn

Ruby: nested.flatten
来源：http://tc.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fq.colortex.cn

[D19] 按字段分组
来源：http://zs.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zx.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kn.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fw.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lu.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ix.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://pj.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ot.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://id.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://tp.colortex.cn

Py:   Counter(arr)
来源：http://cz.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://rk.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sp.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zh.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://th.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://bq.panjiajie.cn

Ruby: arr.tally
来源：http://xv.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://km.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://jo.bookmarksfly.cn

Py:   x in arr
来源：http://dm.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://ki.gzmigu.cn

JS:   arr.includes(x)
来源：http://if.huanxung.cn

TS:   arr.includes(x)
来源：http://ig.huixiangedu.cn

Java: list.contains(x)
来源：http://bn.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://zg.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://je.shtwfgs.cn

C#:   list.Contains(x)
来源：http://qx.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://kg.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ru.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pd.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qt.nicolike.cn

TS:   [...arr];
来源：http://vz.hahajie.cn

Java: new ArrayList<>(list);
来源：http://sz.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yx.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://hu.nszjky.cn

C#:   new List<int>(list);
来源：http://lw.newstarts.cn

[D23] reduce 累积计算
来源：http://ri.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nt.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ds.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jg.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qc.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dx.9csxet.cn

Go:   // 手写循环
来源：http://lg.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hp.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zd.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://yz.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wb.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lf.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ie.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dj.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sf.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mp.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lx.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bb.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://su.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lf.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xt.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yw.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bg.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://go.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ys.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kl.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dc.nicolike.cn

[D26] 数组转字符串
来源：http://jw.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://dw.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://xx.panjiajie.cn

JS:   arr.join(", ")
来源：http://nw.nicolike.cn

TS:   arr.join(", ")
来源：http://fl.lnxyls.cn

Java: String.join(", ", list)
来源：http://vp.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://eq.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://jk.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://bb.bookmarksfly.cn

================================================================================
来源：http://wa.shtwfgs.cn

E. 字符串处理
来源：http://zm.hnjuh.cn

================================================================================
来源：http://om.shxzskj.cn

[E01] 拼接字符串
来源：http://gs.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kr.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vd.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rz.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kh.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ze.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uw.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tb.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rh.huanxung.cn

[E02] 重复字符串
来源：http://uf.bjjhwx.cn

Py:   "ab" * 3
来源：http://vh.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://ru.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://ah.szsharing.cn

TS:   "ab".repeat(3)
来源：http://gq.huanxung.cn

Java: "ab".repeat(3)
来源：http://ef.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://og.wgjwhj.cn

Ruby: "ab" * 3
来源：http://zm.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sb.jianghongdianzi.cn

[E03] 截取子串
来源：http://sz.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ao.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://du.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://qc.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://vf.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sr.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hm.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://gx.gzmigu.cn

[E04] 查找子串位置
来源：http://rz.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://bg.colortex.cn

PHP:  strpos($s, "x");
来源：http://yv.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jx.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://wc.huixiangedu.cn

Java: s.indexOf("x")
来源：http://fg.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://ol.shxzukj.cn

Ruby: s.index("x")
来源：http://sr.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://yb.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://em.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bl.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fu.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rj.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cb.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qq.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cx.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xp.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mn.asd995.cn

[E06] 替换子串
来源：http://gf.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ez.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://jc.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hp.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://sz.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hs.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bb.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xp.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://lc.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://js.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mr.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://by.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sc.hahajie.cn

TS:   s.split(",")
来源：http://ow.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gg.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aq.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://jv.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oj.szsharing.cn

[E08] 数组按分隔符合并
来源：http://ld.huixiangedu.cn

Py:   ",".join(items)
来源：http://yq.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://sx.521024.cn

JS:   items.join(",")
来源：http://fz.panjiajie.cn

TS:   items.join(",")
来源：http://fs.hnjuh.cn

Java: String.join(",", items)
来源：http://jx.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://yl.newstarts.cn

Ruby: items.join(",")
来源：http://yz.hnjuh.cn

C#:   string.Join(",", items)
来源：http://cz.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ur.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uy.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wm.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://ef.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://bc.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://mu.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gs.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://va.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uz.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://hl.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oh.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sh.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://fs.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://rx.nszjky.cn

Java: String.format("%03d", 7)
来源：http://fu.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ty.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ek.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vt.muxihuayi.cn

[E11] 反转字符串
来源：http://on.wgjwhj.cn

Py:   s[::-1]
来源：http://uv.gzmigu.cn

PHP:  strrev($s);
来源：http://wk.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ss.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://lm.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xe.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gz.shtwfgs.cn


<!-- 参考信息 -->