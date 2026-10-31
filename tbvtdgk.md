代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hy.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://or.szxytkj.cn

[D05] 访问与修改元素
来源：http://ns.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nw.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://li.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qv.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://gt.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ed.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ht.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zy.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vu.szxytkj.cn

[D06] 数组长度
来源：http://ei.panjiajie.cn

Py:   len(arr)
来源：http://cg.9csxet.cn

PHP:  count($arr);
来源：http://jj.shxzukj.cn

JS:   arr.length
来源：http://yt.bjjhwx.cn

TS:   arr.length
来源：http://od.9csxet.cn

Java: list.size();
来源：http://ja.szxytkj.cn

Go:   len(arr)
来源：http://ma.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://py.shxzskj.cn

C#:   list.Count;
来源：http://tk.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://bd.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ky.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zy.asd995.cn

JS:   arr.slice(1, 4);
来源：http://ul.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://nw.lnxyls.cn

Java: list.subList(1, 4);
来源：http://tk.muxihuayi.cn

Go:   arr[1:4]
来源：http://du.hnjuh.cn

Ruby: arr[1, 3]
来源：http://yb.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://wn.nicolike.cn

[D08] 合并两个数组
来源：http://zq.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://wb.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://wq.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ub.hahajie.cn

TS:   [...a, ...b];
来源：http://jt.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tb.panjiajie.cn

Go:   append(a, b...)
来源：http://gc.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://xv.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://bv.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://fx.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://bp.asd995.cn

PHP:  sort($arr);
来源：http://ov.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mf.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pq.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zj.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://no.colortex.cn

Ruby: arr.sort
来源：http://oj.yuntaijiaju.cn

C#:   list.Sort();
来源：http://ql.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vb.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qe.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://as.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ph.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gk.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dj.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pm.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lc.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tk.asd995.cn

[D11] 反转数组
来源：http://ym.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ax.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://sn.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kh.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://uy.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://vb.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://pk.gzmigu.cn

Ruby: arr.reverse
来源：http://ib.jctech888.com.cn

C#:   list.Reverse();
来源：http://ge.haigaiapp.cn

[D12] 查找元素下标
来源：http://ww.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://ic.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rb.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jp.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bf.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xt.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://nw.szsharing.cn

Ruby: arr.index(x)
来源：http://px.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://ep.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ka.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ro.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fk.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://kh.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://sd.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oj.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://df.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yf.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gm.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://ue.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pu.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fx.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://ik.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://xy.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wt.szsharing.cn

Go:   // 手写循环
来源：http://yz.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ez.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iq.szsharing.cn

[D15] 去重
来源：http://ph.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tj.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://wz.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://bm.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ma.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zi.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mq.newstarts.cn

Ruby: arr.uniq
来源：http://lk.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://em.jctech888.com.cn

[D16] 求和与平均值
来源：http://fw.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lu.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jf.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gz.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://op.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gi.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://xu.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hd.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://bb.newstarts.cn

[D17] 最大值与最小值
来源：http://vf.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://hk.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://gn.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nc.521024.cn

TS:   Math.max(...arr);
来源：http://wh.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zb.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://do.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://oo.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://ny.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://hg.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ve.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://kg.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nn.colortex.cn

TS:   nested.flat();
来源：http://rp.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ny.huanxung.cn

Go:   // 手写双层循环
来源：http://ou.huanxung.cn

Ruby: nested.flatten
来源：http://lv.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://or.huanxung.cn

[D19] 按字段分组
来源：http://dm.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pj.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bl.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://av.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oa.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kd.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://bw.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://la.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gr.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://dd.jctech888.com.cn

Py:   Counter(arr)
来源：http://wx.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://xu.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ts.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tx.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tj.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://ya.huanxung.cn

Ruby: arr.tally
来源：http://oy.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mo.hahajie.cn

[D21] 判断是否包含某元素
来源：http://vh.shtwfgs.cn

Py:   x in arr
来源：http://dw.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://tj.bjjhwx.cn

JS:   arr.includes(x)
来源：http://nd.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://ui.nicolike.cn

Java: list.contains(x)
来源：http://dp.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://jd.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://cj.yuexingan06.cn

C#:   list.Contains(x)
来源：http://tb.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://ux.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aw.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tc.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uy.bjjhwx.cn

TS:   [...arr];
来源：http://zy.hahajie.cn

Java: new ArrayList<>(list);
来源：http://hm.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://py.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://en.huanxung.cn

C#:   new List<int>(list);
来源：http://qw.panjiajie.cn

[D23] reduce 累积计算
来源：http://jy.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ti.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://me.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tk.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zw.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bp.nicolike.cn

Go:   // 手写循环
来源：http://xl.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ns.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ax.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://ee.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eu.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aw.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mc.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dw.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cy.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ut.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ad.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lu.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://rv.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nt.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gd.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ab.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fj.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xn.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ma.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mi.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://za.gzmigu.cn

[D26] 数组转字符串
来源：http://xa.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://lr.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://lm.bjjhwx.cn

JS:   arr.join(", ")
来源：http://ue.wgjwhj.cn

TS:   arr.join(", ")
来源：http://hc.shxzukj.cn

Java: String.join(", ", list)
来源：http://td.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://qe.asd995.cn

Ruby: arr.join(", ")
来源：http://jj.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://rc.szsharing.cn

================================================================================
来源：http://me.lnxyls.cn

E. 字符串处理
来源：http://ij.shxzukj.cn

================================================================================
来源：http://mo.lnxyls.cn

[E01] 拼接字符串
来源：http://hg.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ik.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rc.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hr.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jj.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uh.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ap.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jv.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ei.yuexingan06.cn

[E02] 重复字符串
来源：http://ry.newstarts.cn

Py:   "ab" * 3
来源：http://jc.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://in.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://dj.nszjky.cn

TS:   "ab".repeat(3)
来源：http://fp.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://cb.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ou.wgjwhj.cn

Ruby: "ab" * 3
来源：http://ep.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ut.yuexingan06.cn

[E03] 截取子串
来源：http://fj.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iw.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ai.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hm.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://rk.nicolike.cn

Java: s.substring(1, 4)
来源：http://fr.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yj.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tv.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://si.huanxung.cn

[E04] 查找子串位置
来源：http://tc.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://lq.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://le.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fg.nicolike.cn

TS:   s.indexOf("x")
来源：http://jc.szsharing.cn

Java: s.indexOf("x")
来源：http://jq.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://iv.jctech888.com.cn

Ruby: s.index("x")
来源：http://wo.nicolike.cn

C#:   s.IndexOf("x")
来源：http://ne.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tn.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ho.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ya.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dx.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ag.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cw.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qg.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wt.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uh.bookmarksfly.cn

[E06] 替换子串
来源：http://mo.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wj.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://zm.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ze.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://wz.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://go.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ek.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://at.521024.cn

C#:   s.Replace("a", "b")
来源：http://bi.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://qq.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://us.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zq.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wl.bjjhwx.cn

TS:   s.split(",")
来源：http://xv.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nt.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rg.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://wr.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vu.521024.cn

[E08] 数组按分隔符合并
来源：http://di.colortex.cn

Py:   ",".join(items)
来源：http://ju.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://tz.jianghongdianzi.cn

JS:   items.join(",")
来源：http://rb.panjiajie.cn

TS:   items.join(",")
来源：http://oo.yuexingan06.cn

Java: String.join(",", items)
来源：http://ev.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://cs.wgjwhj.cn

Ruby: items.join(",")
来源：http://tj.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://az.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://xi.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eo.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tt.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://pi.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://mn.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://ki.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://al.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tg.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xo.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://fy.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gv.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sm.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://ox.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://zy.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://hf.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ld.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rx.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zq.yuexingan06.cn

[E11] 反转字符串
来源：http://nc.yuntaijiaju.cn

Py:   s[::-1]
来源：http://yv.panjiajie.cn

PHP:  strrev($s);
来源：http://dk.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://jq.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://wn.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oq.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sj.chemitech.net.cn


<!-- 参考信息 -->