代发 wailian999

Java: list.add(4);
来源：http://xp.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://ps.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://fx.chemitech.net.cn

C#:   list.Add(4);
来源：http://ol.huanxung.cn

[D03] 在指定位置插入元素
来源：http://zn.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://zz.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ja.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ra.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://rs.shxzskj.cn

Java: list.add(0, 0);
来源：http://ck.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xj.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rz.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://jl.lnxyls.cn

[D04] 删除元素
来源：http://en.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ub.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sk.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lr.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://pd.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bz.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gd.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://es.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mu.shxzukj.cn

[D05] 访问与修改元素
来源：http://sn.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ol.jctech888.com.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://go.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ng.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://jx.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://rs.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ae.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oo.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nz.szsharing.cn

[D06] 数组长度
来源：http://bg.nszjky.cn

Py:   len(arr)
来源：http://hz.hahajie.cn

PHP:  count($arr);
来源：http://bd.hnjuh.cn

JS:   arr.length
来源：http://ji.9csxet.cn

TS:   arr.length
来源：http://cy.shtwfgs.cn

Java: list.size();
来源：http://qc.lnxyls.cn

Go:   len(arr)
来源：http://ul.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://hl.shxzskj.cn

C#:   list.Count;
来源：http://lb.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://bv.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ms.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://db.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://cy.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://og.hahajie.cn

Java: list.subList(1, 4);
来源：http://wx.lnxyls.cn

Go:   arr[1:4]
来源：http://xo.szxytkj.cn

Ruby: arr[1, 3]
来源：http://bm.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://ss.shxzskj.cn

[D08] 合并两个数组
来源：http://wi.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://je.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://kg.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sy.9csxet.cn

TS:   [...a, ...b];
来源：http://yt.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ib.huixiangedu.cn

Go:   append(a, b...)
来源：http://is.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://ka.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://ar.asd995.cn

[D09] 排序（升序）
来源：http://vg.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ed.nszjky.cn

PHP:  sort($arr);
来源：http://sl.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rj.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fg.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lw.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ku.lnxyls.cn

Ruby: arr.sort
来源：http://ud.newstarts.cn

C#:   list.Sort();
来源：http://fd.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tr.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fy.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kn.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eb.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wy.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dm.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hs.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bw.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://on.521024.cn

[D11] 反转数组
来源：http://iv.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jq.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://yh.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qy.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://hh.huanxung.cn

Java: Collections.reverse(list);
来源：http://io.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://zf.haigaiapp.cn

Ruby: arr.reverse
来源：http://zw.huixiangedu.cn

C#:   list.Reverse();
来源：http://hu.521024.cn

[D12] 查找元素下标
来源：http://rg.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://ak.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xj.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oa.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cz.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cb.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://po.huanxung.cn

Ruby: arr.index(x)
来源：http://xm.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://zy.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://oh.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hi.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yb.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://zm.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://cw.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oe.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qn.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fs.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bc.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://bd.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dz.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lo.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://eq.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://mx.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gt.nicolike.cn

Go:   // 手写循环
来源：http://nb.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xp.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://os.chemitech.net.cn

[D15] 去重
来源：http://kh.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lm.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://yt.nszjky.cn

JS:   [...new Set(arr)]
来源：http://ol.521024.cn

TS:   [...new Set(arr)]
来源：http://iv.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ym.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xt.haigaiapp.cn

Ruby: arr.uniq
来源：http://yp.asd995.cn

C#:   list.Distinct().ToList()
来源：http://ty.shxzukj.cn

[D16] 求和与平均值
来源：http://xm.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ky.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ow.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gv.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://su.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qa.gzmigu.cn

Go:   // 手写循环累加
来源：http://ge.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yk.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://fd.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://wt.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://fg.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://pz.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dq.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://er.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vc.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ck.asd995.cn

Ruby: arr.max;  arr.min
来源：http://iq.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://au.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://pr.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ia.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://zz.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ng.asd995.cn

TS:   nested.flat();
来源：http://rn.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dm.colortex.cn

Go:   // 手写双层循环
来源：http://sz.nszjky.cn

Ruby: nested.flatten
来源：http://cl.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tn.shxzskj.cn

[D19] 按字段分组
来源：http://fa.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yj.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mp.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eq.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nq.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nw.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://kb.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wa.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ji.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://xw.shtwfgs.cn

Py:   Counter(arr)
来源：http://wi.nszjky.cn

PHP:  array_count_values($arr);
来源：http://gk.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qg.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jg.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hj.hahajie.cn

Go:   // 手写 map[T]int
来源：http://bs.wgjwhj.cn

Ruby: arr.tally
来源：http://df.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xe.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://fc.szsharing.cn

Py:   x in arr
来源：http://ko.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://kt.521024.cn

JS:   arr.includes(x)
来源：http://bz.nicolike.cn

TS:   arr.includes(x)
来源：http://va.muxihuayi.cn

Java: list.contains(x)
来源：http://nd.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://ob.szxytkj.cn

Ruby: arr.include?(x)
来源：http://pv.bjjhwx.cn

C#:   list.Contains(x)
来源：http://pg.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://pr.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bu.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hu.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ci.yuexingan06.cn

TS:   [...arr];
来源：http://cv.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://hw.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dr.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://uc.jctech888.com.cn

C#:   new List<int>(list);
来源：http://oc.asd995.cn

[D23] reduce 累积计算
来源：http://yu.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gn.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cb.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zi.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kp.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yb.hnjuh.cn

Go:   // 手写循环
来源：http://so.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vh.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gx.521024.cn

[D24] 字典 / Map 基本操作
来源：http://dd.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://li.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vd.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nu.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ih.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jg.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sw.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xs.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mj.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://gw.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jc.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vr.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ij.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ud.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dt.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kd.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dy.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mm.huixiangedu.cn

[D26] 数组转字符串
来源：http://oo.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://ia.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://yu.shxzskj.cn

JS:   arr.join(", ")
来源：http://jg.colortex.cn

TS:   arr.join(", ")
来源：http://nj.szsharing.cn

Java: String.join(", ", list)
来源：http://wl.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://jq.szsharing.cn

Ruby: arr.join(", ")
来源：http://uu.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://nx.panjiajie.cn

================================================================================
来源：http://tk.szsharing.cn

E. 字符串处理
来源：http://hx.shtwfgs.cn

================================================================================
来源：http://jr.szsharing.cn

[E01] 拼接字符串
来源：http://mi.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://na.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bb.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wp.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://en.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oe.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pv.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lx.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bg.nicolike.cn

[E02] 重复字符串
来源：http://rx.huanxung.cn

Py:   "ab" * 3
来源：http://hm.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://zi.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://kp.newstarts.cn

TS:   "ab".repeat(3)
来源：http://rf.shxzukj.cn

Java: "ab".repeat(3)
来源：http://vo.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://gi.shxzskj.cn

Ruby: "ab" * 3
来源：http://yw.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gg.newstarts.cn

[E03] 截取子串
来源：http://mo.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gc.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ll.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wk.521024.cn

TS:   s.slice(1, 4)
来源：http://cq.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://xb.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dg.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zp.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://bw.chemitech.net.cn

[E04] 查找子串位置
来源：http://rn.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://de.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://hq.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sj.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://ru.szxytkj.cn

Java: s.indexOf("x")
来源：http://hg.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://cz.nicolike.cn

Ruby: s.index("x")
来源：http://wj.newstarts.cn

C#:   s.IndexOf("x")
来源：http://vx.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gx.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zt.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ll.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xh.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bm.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sh.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jw.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xu.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wx.huixiangedu.cn

[E06] 替换子串
来源：http://dt.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://de.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://be.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pl.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://lt.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gt.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qk.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vb.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://wo.szxytkj.cn

[E07] 按分隔符拆分
来源：http://zr.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://da.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mf.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://it.chemitech.net.cn

TS:   s.split(",")
来源：http://pp.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uv.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lv.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://fb.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mk.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://ue.hnjuh.cn

Py:   ",".join(items)
来源：http://go.nszjky.cn

PHP:  implode(",", $items);
来源：http://eq.hahajie.cn

JS:   items.join(",")
来源：http://ur.gzmigu.cn

TS:   items.join(",")
来源：http://vn.bookmarksfly.cn

Java: String.join(",", items)
来源：http://me.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://ah.shxzukj.cn

Ruby: items.join(",")
来源：http://fz.szxytkj.cn

C#:   string.Join(",", items)
来源：http://ly.521024.cn

[E09] 去除所有空白字符
来源：http://co.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oz.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kv.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://gl.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://lr.hahajie.cn


<!-- 参考信息 -->