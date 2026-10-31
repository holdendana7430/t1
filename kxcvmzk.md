代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lu.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fp.shxzskj.cn

[D05] 访问与修改元素
来源：http://af.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bg.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ht.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yr.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://jz.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://vw.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://li.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ab.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ux.muxihuayi.cn

[D06] 数组长度
来源：http://nn.wgjwhj.cn

Py:   len(arr)
来源：http://ja.chemitech.net.cn

PHP:  count($arr);
来源：http://fz.newstarts.cn

JS:   arr.length
来源：http://vl.szxytkj.cn

TS:   arr.length
来源：http://vv.shtwfgs.cn

Java: list.size();
来源：http://xk.newstarts.cn

Go:   len(arr)
来源：http://ay.9csxet.cn

Ruby: arr.length; arr.size
来源：http://rr.huixinmuqiang.cn

C#:   list.Count;
来源：http://ue.asd995.cn

[D07] 切片 / 取子数组
来源：http://ec.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pv.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://of.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://hn.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://yb.hnjuh.cn

Java: list.subList(1, 4);
来源：http://kw.wgjwhj.cn

Go:   arr[1:4]
来源：http://ai.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://pt.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://au.9csxet.cn

[D08] 合并两个数组
来源：http://fc.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://kt.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://lu.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jz.yuexingan06.cn

TS:   [...a, ...b];
来源：http://nl.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bg.bjjhwx.cn

Go:   append(a, b...)
来源：http://fm.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://no.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://qy.shtwfgs.cn

[D09] 排序（升序）
来源：http://ie.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://fl.shtwfgs.cn

PHP:  sort($arr);
来源：http://qq.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vz.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gv.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ok.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cm.muxihuayi.cn

Ruby: arr.sort
来源：http://ce.shxzukj.cn

C#:   list.Sort();
来源：http://qx.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ri.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rd.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://in.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zw.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://on.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gc.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xb.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://do.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ph.bookmarksfly.cn

[D11] 反转数组
来源：http://wj.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qt.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://uw.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://om.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://ws.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://hf.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://gy.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://fu.gzmigu.cn

C#:   list.Reverse();
来源：http://rv.lnxyls.cn

[D12] 查找元素下标
来源：http://js.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://ks.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://az.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kk.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://to.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sv.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://fo.hahajie.cn

Ruby: arr.index(x)
来源：http://zx.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://vi.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://hy.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://or.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pk.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://or.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://kn.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://so.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ya.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ig.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kn.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://xr.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wx.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mh.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://zc.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://yb.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qb.shxzukj.cn

Go:   // 手写循环
来源：http://im.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ke.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nl.bookmarksfly.cn

[D15] 去重
来源：http://kb.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tx.gzmigu.cn

PHP:  array_unique($arr);
来源：http://ut.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://cp.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://sa.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cy.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ap.bjjhwx.cn

Ruby: arr.uniq
来源：http://do.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://pl.9csxet.cn

[D16] 求和与平均值
来源：http://fp.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fe.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vd.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://je.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zu.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qd.hnjuh.cn

Go:   // 手写循环累加
来源：http://sd.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sx.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://pv.huixiangedu.cn

[D17] 最大值与最小值
来源：http://yn.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://hk.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://gg.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xk.hnjuh.cn

TS:   Math.max(...arr);
来源：http://sj.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://en.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://ku.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://sv.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://jg.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://os.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://wh.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vu.yuexingan06.cn

TS:   nested.flat();
来源：http://ey.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pf.yuexingan06.cn

Go:   // 手写双层循环
来源：http://hd.muxihuayi.cn

Ruby: nested.flatten
来源：http://eq.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pu.szxytkj.cn

[D19] 按字段分组
来源：http://ln.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ci.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hw.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xo.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ai.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yb.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://mq.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iv.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mq.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://lc.bookmarksfly.cn

Py:   Counter(arr)
来源：http://eu.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://mb.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kh.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vo.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uz.nszjky.cn

Go:   // 手写 map[T]int
来源：http://gi.chemitech.net.cn

Ruby: arr.tally
来源：http://ip.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mi.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://tv.shxzskj.cn

Py:   x in arr
来源：http://bf.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://jn.nszjky.cn

JS:   arr.includes(x)
来源：http://gq.9csxet.cn

TS:   arr.includes(x)
来源：http://qc.colortex.cn

Java: list.contains(x)
来源：http://cu.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://zj.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://wm.521024.cn

C#:   list.Contains(x)
来源：http://wt.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://me.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ag.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xg.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ms.chemitech.net.cn

TS:   [...arr];
来源：http://os.newstarts.cn

Java: new ArrayList<>(list);
来源：http://mn.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://he.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://cn.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://hk.9csxet.cn

[D23] reduce 累积计算
来源：http://cc.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ri.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lk.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cm.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ga.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ky.huixinmuqiang.cn

Go:   // 手写循环
来源：http://oa.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mz.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iy.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://zl.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://br.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iv.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vt.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jv.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xj.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nb.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jy.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ke.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://us.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ra.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hl.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wv.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iv.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uu.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ir.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nf.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pk.haigaiapp.cn

[D26] 数组转字符串
来源：http://ch.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://sl.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ir.colortex.cn

JS:   arr.join(", ")
来源：http://dc.newstarts.cn

TS:   arr.join(", ")
来源：http://ub.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://vo.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://uk.panjiajie.cn

Ruby: arr.join(", ")
来源：http://rg.colortex.cn

C#:   string.Join(", ", list)
来源：http://wo.newstarts.cn

================================================================================
来源：http://bt.panjiajie.cn

E. 字符串处理
来源：http://zq.panjiajie.cn

================================================================================
来源：http://wq.muxihuayi.cn

[E01] 拼接字符串
来源：http://yt.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://or.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yw.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yz.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ou.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sh.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oz.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vm.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nm.chemitech.net.cn

[E02] 重复字符串
来源：http://nh.huanxung.cn

Py:   "ab" * 3
来源：http://kr.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://zt.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://lf.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://nu.huanxung.cn

Java: "ab".repeat(3)
来源：http://xg.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://hg.lnxyls.cn

Ruby: "ab" * 3
来源：http://jp.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qh.hnjuh.cn

[E03] 截取子串
来源：http://kj.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ko.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bp.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ts.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://sl.szsharing.cn

Java: s.substring(1, 4)
来源：http://qo.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gv.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sc.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://im.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://pt.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://cr.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://ym.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pb.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ff.shxzskj.cn

Java: s.indexOf("x")
来源：http://dr.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://in.haigaiapp.cn

Ruby: s.index("x")
来源：http://dk.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://zq.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ik.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oz.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ah.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ho.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kt.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ec.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://at.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bt.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://di.chemitech.net.cn

[E06] 替换子串
来源：http://zb.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gh.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://hl.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xe.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://il.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ko.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wd.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://an.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://wq.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://ta.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://la.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dj.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fa.panjiajie.cn

TS:   s.split(",")
来源：http://ao.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yy.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ou.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://yo.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nk.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://kt.haigaiapp.cn

Py:   ",".join(items)
来源：http://ki.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://cj.huixiangedu.cn

JS:   items.join(",")
来源：http://ha.huanxung.cn

TS:   items.join(",")
来源：http://nj.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://ti.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://wu.nicolike.cn

Ruby: items.join(",")
来源：http://zf.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://as.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://zv.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kx.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yb.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://gl.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://rw.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://gp.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qi.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ou.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rv.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://ez.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ya.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sh.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://hp.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://cn.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://nx.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pu.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ac.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sy.szxytkj.cn

[E11] 反转字符串
来源：http://tz.bookmarksfly.cn

Py:   s[::-1]
来源：http://fv.hahajie.cn

PHP:  strrev($s);
来源：http://zc.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://mi.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://wj.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lp.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dy.huixiangedu.cn


<!-- 参考信息 -->