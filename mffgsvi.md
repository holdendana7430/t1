代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wi.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jq.panjiajie.cn

JS:   arr.push(4);
来源：http://pa.nicolike.cn

TS:   arr.push(4);
来源：http://yp.muxihuayi.cn

Java: list.add(4);
来源：http://yi.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://jx.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://jt.hnjuh.cn

C#:   list.Add(4);
来源：http://fp.asd995.cn

[D03] 在指定位置插入元素
来源：http://co.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://hr.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dr.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://et.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://pr.nicolike.cn

Java: list.add(0, 0);
来源：http://cq.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uo.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hr.asd995.cn

C#:   list.Insert(0, 0);
来源：http://md.newstarts.cn

[D04] 删除元素
来源：http://zy.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jx.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ji.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uu.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://fj.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aq.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tq.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zr.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nl.asd995.cn

[D05] 访问与修改元素
来源：http://dk.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://he.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dz.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ub.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://sg.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://uq.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ku.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zx.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://do.chemitech.net.cn

[D06] 数组长度
来源：http://gl.yuntaijiaju.cn

Py:   len(arr)
来源：http://ru.huixinmuqiang.cn

PHP:  count($arr);
来源：http://ci.colortex.cn

JS:   arr.length
来源：http://gs.huixiangedu.cn

TS:   arr.length
来源：http://gl.gzmigu.cn

Java: list.size();
来源：http://nr.chemitech.net.cn

Go:   len(arr)
来源：http://zy.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://ui.yuntaijiaju.cn

C#:   list.Count;
来源：http://rn.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://da.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sj.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vl.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://lm.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://mn.gzmigu.cn

Java: list.subList(1, 4);
来源：http://fe.nicolike.cn

Go:   arr[1:4]
来源：http://tv.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://bb.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://hs.hnjuh.cn

[D08] 合并两个数组
来源：http://tw.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://rf.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://oy.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://em.nszjky.cn

TS:   [...a, ...b];
来源：http://of.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vr.jctech888.com.cn

Go:   append(a, b...)
来源：http://tp.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://hu.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://zt.521024.cn

[D09] 排序（升序）
来源：http://zq.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ec.gzmigu.cn

PHP:  sort($arr);
来源：http://rp.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zf.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xu.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sn.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uv.9csxet.cn

Ruby: arr.sort
来源：http://ec.panjiajie.cn

C#:   list.Sort();
来源：http://dt.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bi.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fs.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fs.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ay.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lw.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://in.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yv.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qj.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bu.panjiajie.cn

[D11] 反转数组
来源：http://dt.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ki.521024.cn

PHP:  array_reverse($arr);
来源：http://uj.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zq.huanxung.cn

TS:   [...arr].reverse();
来源：http://hw.colortex.cn

Java: Collections.reverse(list);
来源：http://zz.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://mz.521024.cn

Ruby: arr.reverse
来源：http://iv.9csxet.cn

C#:   list.Reverse();
来源：http://ag.chemitech.net.cn

[D12] 查找元素下标
来源：http://ch.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://yx.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zv.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eu.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uk.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tr.colortex.cn

Go:   slices.Index(arr, x)
来源：http://cl.shtwfgs.cn

Ruby: arr.index(x)
来源：http://sz.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://ch.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://nn.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hp.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://px.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://wt.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://oj.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mn.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gn.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ww.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zk.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://fl.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oz.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ho.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://ye.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://xk.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nm.hahajie.cn

Go:   // 手写循环
来源：http://uj.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pi.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eu.shxzskj.cn

[D15] 去重
来源：http://do.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hq.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ce.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://wc.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://rx.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ch.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ep.bookmarksfly.cn

Ruby: arr.uniq
来源：http://hs.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://go.huanxung.cn

[D16] 求和与平均值
来源：http://af.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zi.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bn.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ac.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hi.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jb.chemitech.net.cn

Go:   // 手写循环累加
来源：http://qb.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rr.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://oc.huanxung.cn

[D17] 最大值与最小值
来源：http://yl.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://jk.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://wu.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kg.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://df.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://js.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ml.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://dd.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://py.asd995.cn

[D18] 扁平化嵌套数组
来源：http://ea.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ld.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://ie.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mb.muxihuayi.cn

TS:   nested.flat();
来源：http://xb.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qt.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://nn.szsharing.cn

Ruby: nested.flatten
来源：http://on.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oc.bjjhwx.cn

[D19] 按字段分组
来源：http://uz.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rk.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nw.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fl.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rl.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pn.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://om.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rv.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xv.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://ex.panjiajie.cn

Py:   Counter(arr)
来源：http://ug.szsharing.cn

PHP:  array_count_values($arr);
来源：http://oe.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zg.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kv.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yg.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://ln.shxzskj.cn

Ruby: arr.tally
来源：http://dg.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vg.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://fd.gzmigu.cn

Py:   x in arr
来源：http://kf.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://mj.haigaiapp.cn

JS:   arr.includes(x)
来源：http://wt.asd995.cn

TS:   arr.includes(x)
来源：http://ew.yuntaijiaju.cn

Java: list.contains(x)
来源：http://as.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://lm.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://ua.shxzskj.cn

C#:   list.Contains(x)
来源：http://rv.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://dn.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hf.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://up.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://at.chemitech.net.cn

TS:   [...arr];
来源：http://jx.nicolike.cn

Java: new ArrayList<>(list);
来源：http://po.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tu.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://jb.szsharing.cn

C#:   new List<int>(list);
来源：http://af.shxzskj.cn

[D23] reduce 累积计算
来源：http://jx.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ue.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eu.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dl.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ap.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lx.gzmigu.cn

Go:   // 手写循环
来源：http://ol.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hv.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wh.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://gq.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ep.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gp.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dt.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cz.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gg.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mc.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jz.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mk.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://hh.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://th.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wh.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ar.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yw.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://si.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lp.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pe.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qc.jctech888.com.cn

[D26] 数组转字符串
来源：http://sv.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://cu.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://oa.wgjwhj.cn

JS:   arr.join(", ")
来源：http://cf.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://xb.jctech888.com.cn

Java: String.join(", ", list)
来源：http://vw.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://av.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://vj.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://ik.yuntaijiaju.cn

================================================================================
来源：http://oc.asd995.cn

E. 字符串处理
来源：http://tp.huixinmuqiang.cn

================================================================================
来源：http://qg.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://po.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mk.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ai.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dn.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ee.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cm.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kb.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cn.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gd.jctech888.com.cn

[E02] 重复字符串
来源：http://cj.shxzskj.cn

Py:   "ab" * 3
来源：http://rg.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://rt.9csxet.cn

JS:   "ab".repeat(3)
来源：http://cd.asd995.cn

TS:   "ab".repeat(3)
来源：http://fg.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://fa.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://dc.9csxet.cn

Ruby: "ab" * 3
来源：http://zx.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wj.jctech888.com.cn

[E03] 截取子串
来源：http://wp.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iv.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://os.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oe.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://lj.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://hg.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sj.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ac.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://al.szsharing.cn

[E04] 查找子串位置
来源：http://aw.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://ui.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://is.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gl.nszjky.cn

TS:   s.indexOf("x")
来源：http://gq.nicolike.cn

Java: s.indexOf("x")
来源：http://ge.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://fj.haigaiapp.cn

Ruby: s.index("x")
来源：http://si.hahajie.cn

C#:   s.IndexOf("x")
来源：http://st.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tj.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fd.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ej.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lv.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xz.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ox.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ix.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ug.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qc.jctech888.com.cn

[E06] 替换子串
来源：http://go.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dl.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://bn.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zh.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://rr.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lp.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ot.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ey.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://yq.colortex.cn

[E07] 按分隔符拆分
来源：http://xc.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nw.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cj.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ra.jctech888.com.cn

TS:   s.split(",")
来源：http://yc.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kp.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sp.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://gx.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zi.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://ul.nicolike.cn

Py:   ",".join(items)
来源：http://ir.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://cb.asd995.cn

JS:   items.join(",")
来源：http://uu.jctech888.com.cn

TS:   items.join(",")
来源：http://sl.wgjwhj.cn

Java: String.join(",", items)
来源：http://uu.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://gz.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://fa.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://au.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://ig.huixinmuqiang.cn


<!-- 参考信息 -->