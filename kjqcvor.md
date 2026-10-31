代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ix.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://za.lnxyls.cn

JS:   arr.push(4);
来源：http://wq.nszjky.cn

TS:   arr.push(4);
来源：http://rp.yuexingan06.cn

Java: list.add(4);
来源：http://sg.colortex.cn

Go:   arr = append(arr, 4)
来源：http://sj.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://uj.bookmarksfly.cn

C#:   list.Add(4);
来源：http://uf.huanxung.cn

[D03] 在指定位置插入元素
来源：http://zx.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://kg.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qs.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ik.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://yp.521024.cn

Java: list.add(0, 0);
来源：http://ob.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zz.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ow.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://cy.huanxung.cn

[D04] 删除元素
来源：http://rb.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ft.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qt.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kh.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://uo.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cq.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ez.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yt.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bo.newstarts.cn

[D05] 访问与修改元素
来源：http://uc.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pk.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rf.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nv.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://fb.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://mr.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://vd.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wt.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lh.hnjuh.cn

[D06] 数组长度
来源：http://fo.gzmigu.cn

Py:   len(arr)
来源：http://ge.gzmigu.cn

PHP:  count($arr);
来源：http://qc.bookmarksfly.cn

JS:   arr.length
来源：http://md.chemitech.net.cn

TS:   arr.length
来源：http://vk.colortex.cn

Java: list.size();
来源：http://dt.colortex.cn

Go:   len(arr)
来源：http://zg.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://bm.yuexingan06.cn

C#:   list.Count;
来源：http://hz.huanxung.cn

[D07] 切片 / 取子数组
来源：http://hc.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kt.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://be.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://ij.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://ae.panjiajie.cn

Java: list.subList(1, 4);
来源：http://xs.haigaiapp.cn

Go:   arr[1:4]
来源：http://yl.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://zy.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://kv.lnxyls.cn

[D08] 合并两个数组
来源：http://rh.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://rx.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://lk.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gj.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://ct.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dh.gzmigu.cn

Go:   append(a, b...)
来源：http://nf.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://ev.521024.cn

C#:   a.Concat(b).ToList()
来源：http://al.haigaiapp.cn

[D09] 排序（升序）
来源：http://af.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ad.jctech888.com.cn

PHP:  sort($arr);
来源：http://yq.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://be.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lj.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pk.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://in.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ac.nicolike.cn

C#:   list.Sort();
来源：http://hg.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ez.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yg.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ob.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zz.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xi.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kc.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zu.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hc.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://at.chemitech.net.cn

[D11] 反转数组
来源：http://qw.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vk.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://km.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ic.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://ox.szsharing.cn

Java: Collections.reverse(list);
来源：http://ew.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://zo.nszjky.cn

Ruby: arr.reverse
来源：http://yy.yuexingan06.cn

C#:   list.Reverse();
来源：http://yg.muxihuayi.cn

[D12] 查找元素下标
来源：http://sk.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://nx.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ed.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lj.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wx.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sp.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://ql.9csxet.cn

Ruby: arr.index(x)
来源：http://bb.szsharing.cn

C#:   list.IndexOf(x);
来源：http://yj.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://zm.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wv.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sr.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ch.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://wo.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iu.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tx.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ts.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://od.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://ce.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gz.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mc.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://uq.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://hl.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sd.haigaiapp.cn

Go:   // 手写循环
来源：http://lp.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cw.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://te.szxytkj.cn

[D15] 去重
来源：http://pp.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dc.521024.cn

PHP:  array_unique($arr);
来源：http://nd.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://rr.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://rd.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mj.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dr.szsharing.cn

Ruby: arr.uniq
来源：http://mr.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://qx.9csxet.cn

[D16] 求和与平均值
来源：http://es.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wz.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dn.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://no.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gw.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dq.9csxet.cn

Go:   // 手写循环累加
来源：http://nt.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jt.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://he.521024.cn

[D17] 最大值与最小值
来源：http://tc.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://pj.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://iw.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gm.shxzskj.cn

TS:   Math.max(...arr);
来源：http://vi.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qv.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bd.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://bt.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://gt.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://oo.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gn.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://bo.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dn.9csxet.cn

TS:   nested.flat();
来源：http://sa.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hr.haigaiapp.cn

Go:   // 手写双层循环
来源：http://vw.muxihuayi.cn

Ruby: nested.flatten
来源：http://wh.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ik.huixinmuqiang.cn

[D19] 按字段分组
来源：http://vb.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zj.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mp.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rc.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zs.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://he.521024.cn

Go:   // 手写 map[string][]T
来源：http://lm.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eo.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bz.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://cy.bookmarksfly.cn

Py:   Counter(arr)
来源：http://qb.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://jm.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pl.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ij.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pg.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://fo.shxzukj.cn

Ruby: arr.tally
来源：http://rf.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sa.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://hw.haigaiapp.cn

Py:   x in arr
来源：http://rp.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://ja.gzmigu.cn

JS:   arr.includes(x)
来源：http://he.gzmigu.cn

TS:   arr.includes(x)
来源：http://cy.colortex.cn

Java: list.contains(x)
来源：http://kh.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://wn.huanxung.cn

Ruby: arr.include?(x)
来源：http://ag.haigaiapp.cn

C#:   list.Contains(x)
来源：http://yh.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://kt.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yc.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lw.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qh.chemitech.net.cn

TS:   [...arr];
来源：http://qg.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://jr.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ml.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://gm.shxzskj.cn

C#:   new List<int>(list);
来源：http://qi.asd995.cn

[D23] reduce 累积计算
来源：http://bz.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ex.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rw.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wo.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gh.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ed.colortex.cn

Go:   // 手写循环
来源：http://sy.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hk.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ah.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://wn.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ez.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rt.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zi.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nu.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gh.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://do.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vp.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nq.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://bf.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zc.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gj.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nx.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://am.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jc.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zi.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cc.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uo.521024.cn

[D26] 数组转字符串
来源：http://mk.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://bv.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://sk.lnxyls.cn

JS:   arr.join(", ")
来源：http://fr.521024.cn

TS:   arr.join(", ")
来源：http://ph.huixiangedu.cn

Java: String.join(", ", list)
来源：http://nz.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://vm.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://gl.colortex.cn

C#:   string.Join(", ", list)
来源：http://ob.newstarts.cn

================================================================================
来源：http://vw.9csxet.cn

E. 字符串处理
来源：http://ts.colortex.cn

================================================================================
来源：http://ja.szxytkj.cn

[E01] 拼接字符串
来源：http://ng.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wx.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oc.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vy.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ow.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://go.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ld.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ws.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lg.newstarts.cn

[E02] 重复字符串
来源：http://kj.newstarts.cn

Py:   "ab" * 3
来源：http://iq.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://kw.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://my.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://wl.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://mh.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://sh.nszjky.cn

Ruby: "ab" * 3
来源：http://xz.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dv.colortex.cn

[E03] 截取子串
来源：http://dy.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tp.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ai.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rd.huanxung.cn

TS:   s.slice(1, 4)
来源：http://xk.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://rv.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://be.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ik.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://zx.bookmarksfly.cn

[E04] 查找子串位置
来源：http://ba.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://cp.huanxung.cn

PHP:  strpos($s, "x");
来源：http://bu.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gt.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://yo.shxzskj.cn

Java: s.indexOf("x")
来源：http://wk.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://fi.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://it.szsharing.cn

C#:   s.IndexOf("x")
来源：http://bd.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://th.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xn.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bc.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eo.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lc.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gg.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pr.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cu.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://na.huanxung.cn

[E06] 替换子串
来源：http://nv.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ba.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://yb.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ot.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://vm.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://au.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dt.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ao.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://sd.gzmigu.cn

[E07] 按分隔符拆分
来源：http://fq.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rg.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dn.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sa.hnjuh.cn

TS:   s.split(",")
来源：http://xq.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pv.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://el.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://ye.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ml.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://eq.huanxung.cn

Py:   ",".join(items)
来源：http://lk.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://ky.colortex.cn

JS:   items.join(",")
来源：http://do.521024.cn

TS:   items.join(",")
来源：http://xs.szsharing.cn

Java: String.join(",", items)
来源：http://yz.asd995.cn

Go:   strings.Join(items, ",")
来源：http://tp.lnxyls.cn

Ruby: items.join(",")
来源：http://se.shxzskj.cn

C#:   string.Join(",", items)
来源：http://tl.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://sl.shtwfgs.cn


<!-- 参考信息 -->