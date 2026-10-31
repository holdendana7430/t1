代发 wailian999

C#:   list.Insert(0, 0);
来源：http://ev.huanxung.cn

[D04] 删除元素
来源：http://kt.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ec.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ak.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tx.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://td.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zt.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gv.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oy.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ay.shxzskj.cn

[D05] 访问与修改元素
来源：http://yv.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oh.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tr.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uh.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://uw.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://dr.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://bu.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rh.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qm.chemitech.net.cn

[D06] 数组长度
来源：http://bf.muxihuayi.cn

Py:   len(arr)
来源：http://op.9csxet.cn

PHP:  count($arr);
来源：http://ws.shxzskj.cn

JS:   arr.length
来源：http://sf.nszjky.cn

TS:   arr.length
来源：http://ss.colortex.cn

Java: list.size();
来源：http://dk.lnxyls.cn

Go:   len(arr)
来源：http://sk.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://ht.521024.cn

C#:   list.Count;
来源：http://pt.nszjky.cn

[D07] 切片 / 取子数组
来源：http://ge.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://co.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://po.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://ep.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://xg.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://uu.jctech888.com.cn

Go:   arr[1:4]
来源：http://vb.521024.cn

Ruby: arr[1, 3]
来源：http://yj.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://fn.haigaiapp.cn

[D08] 合并两个数组
来源：http://oq.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://fa.asd995.cn

PHP:  array_merge($a, $b);
来源：http://wy.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dp.jctech888.com.cn

TS:   [...a, ...b];
来源：http://xy.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kv.gzmigu.cn

Go:   append(a, b...)
来源：http://hf.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://ls.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://ye.wgjwhj.cn

[D09] 排序（升序）
来源：http://og.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://mv.shtwfgs.cn

PHP:  sort($arr);
来源：http://dp.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wj.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xv.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ov.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hu.shxzskj.cn

Ruby: arr.sort
来源：http://hx.huixinmuqiang.cn

C#:   list.Sort();
来源：http://of.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nq.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://di.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tb.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bl.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nv.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nw.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yj.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ca.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pf.colortex.cn

[D11] 反转数组
来源：http://ht.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bl.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://me.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kt.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://vi.shxzukj.cn

Java: Collections.reverse(list);
来源：http://ln.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://oe.wgjwhj.cn

Ruby: arr.reverse
来源：http://uw.bookmarksfly.cn

C#:   list.Reverse();
来源：http://cy.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://rb.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://hu.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ge.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lv.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bl.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bt.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://dv.nszjky.cn

Ruby: arr.index(x)
来源：http://ti.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://nj.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://dq.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://we.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sq.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://dh.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://ep.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ih.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://im.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eh.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gi.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://kb.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ug.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://de.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://es.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://qt.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pi.colortex.cn

Go:   // 手写循环
来源：http://bh.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://he.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ou.bjjhwx.cn

[D15] 去重
来源：http://zb.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gi.newstarts.cn

PHP:  array_unique($arr);
来源：http://ni.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://wh.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://eq.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yp.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://on.shxzskj.cn

Ruby: arr.uniq
来源：http://ay.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://tn.nszjky.cn

[D16] 求和与平均值
来源：http://td.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fd.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ml.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lj.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bz.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://py.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://wp.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qr.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://yp.bjjhwx.cn

[D17] 最大值与最小值
来源：http://fs.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://lm.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://nj.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pd.nszjky.cn

TS:   Math.max(...arr);
来源：http://ep.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bd.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sz.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://cb.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://wu.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://fh.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eb.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://rx.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://je.muxihuayi.cn

TS:   nested.flat();
来源：http://rc.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://af.bjjhwx.cn

Go:   // 手写双层循环
来源：http://lm.bjjhwx.cn

Ruby: nested.flatten
来源：http://ac.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ch.521024.cn

[D19] 按字段分组
来源：http://xw.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://av.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pd.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vk.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ri.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aw.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://am.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ct.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ag.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://hb.huanxung.cn

Py:   Counter(arr)
来源：http://zk.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://ni.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://te.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://le.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qf.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://ws.nszjky.cn

Ruby: arr.tally
来源：http://cc.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lz.colortex.cn

[D21] 判断是否包含某元素
来源：http://pr.shtwfgs.cn

Py:   x in arr
来源：http://vm.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://hr.newstarts.cn

JS:   arr.includes(x)
来源：http://vf.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://nj.lnxyls.cn

Java: list.contains(x)
来源：http://vm.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://pm.huanxung.cn

Ruby: arr.include?(x)
来源：http://yc.bjjhwx.cn

C#:   list.Contains(x)
来源：http://ix.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://it.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eb.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ki.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nh.jianghongdianzi.cn

TS:   [...arr];
来源：http://tx.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://mt.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rf.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://zw.jctech888.com.cn

C#:   new List<int>(list);
来源：http://zy.szxytkj.cn

[D23] reduce 累积计算
来源：http://pf.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yh.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://im.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zo.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fo.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lt.newstarts.cn

Go:   // 手写循环
来源：http://jc.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dm.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jt.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://yg.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://co.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://el.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zx.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sj.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://js.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wf.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pz.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lv.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://id.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vs.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dm.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ne.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ql.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tb.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dj.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qq.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://je.521024.cn

[D26] 数组转字符串
来源：http://tp.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://lc.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://yc.panjiajie.cn

JS:   arr.join(", ")
来源：http://iu.colortex.cn

TS:   arr.join(", ")
来源：http://ub.muxihuayi.cn

Java: String.join(", ", list)
来源：http://bq.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://fz.shxzukj.cn

Ruby: arr.join(", ")
来源：http://xd.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://no.huixiangedu.cn

================================================================================
来源：http://ij.bjjhwx.cn

E. 字符串处理
来源：http://yp.szsharing.cn

================================================================================
来源：http://wq.521024.cn

[E01] 拼接字符串
来源：http://yk.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ey.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zi.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oi.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gy.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tp.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ot.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hy.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nc.jianghongdianzi.cn

[E02] 重复字符串
来源：http://ho.hahajie.cn

Py:   "ab" * 3
来源：http://eb.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://fc.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://iy.nszjky.cn

TS:   "ab".repeat(3)
来源：http://ad.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://iz.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://xi.nicolike.cn

Ruby: "ab" * 3
来源：http://gl.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ms.jctech888.com.cn

[E03] 截取子串
来源：http://pv.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cj.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ju.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://np.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://sc.lnxyls.cn

Java: s.substring(1, 4)
来源：http://sd.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nj.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hf.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://sn.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://zo.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://kj.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://ng.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nk.521024.cn

TS:   s.indexOf("x")
来源：http://se.9csxet.cn

Java: s.indexOf("x")
来源：http://cx.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://mt.asd995.cn

Ruby: s.index("x")
来源：http://pj.nicolike.cn

C#:   s.IndexOf("x")
来源：http://nu.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qt.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sl.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yy.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ha.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rq.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://on.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fg.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kv.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dq.shxzukj.cn

[E06] 替换子串
来源：http://mm.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fm.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://nu.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hs.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://um.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dx.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://il.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wf.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://ci.hahajie.cn

[E07] 按分隔符拆分
来源：http://wn.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wj.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yt.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ls.9csxet.cn

TS:   s.split(",")
来源：http://fb.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pv.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mc.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://it.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ud.colortex.cn

[E08] 数组按分隔符合并
来源：http://il.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://me.hahajie.cn

PHP:  implode(",", $items);
来源：http://ym.shxzukj.cn

JS:   items.join(",")
来源：http://ea.newstarts.cn

TS:   items.join(",")
来源：http://qf.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://lf.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://ci.panjiajie.cn

Ruby: items.join(",")
来源：http://ay.panjiajie.cn

C#:   string.Join(",", items)
来源：http://bi.9csxet.cn

[E09] 去除所有空白字符
来源：http://za.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lr.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vu.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://iu.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://oi.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ra.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sw.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vd.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wx.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://qo.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://if.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fc.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://rh.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://do.huanxung.cn

Java: String.format("%03d", 7)
来源：http://tt.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://to.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ti.panjiajie.cn


<!-- 参考信息 -->