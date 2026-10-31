代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://er.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zl.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xn.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cp.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://dv.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://bh.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jy.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://ge.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yg.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nb.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://em.newstarts.cn

TS:   arr.push(4);
来源：http://ec.yuntaijiaju.cn

Java: list.add(4);
来源：http://it.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://ti.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://af.521024.cn

C#:   list.Add(4);
来源：http://qy.9csxet.cn

[D03] 在指定位置插入元素
来源：http://zi.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://tu.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xg.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aj.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ti.wgjwhj.cn

Java: list.add(0, 0);
来源：http://py.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jq.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ti.521024.cn

C#:   list.Insert(0, 0);
来源：http://xn.haigaiapp.cn

[D04] 删除元素
来源：http://qm.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hh.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bf.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://py.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://sq.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jo.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fp.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zu.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rl.nicolike.cn

[D05] 访问与修改元素
来源：http://iu.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ej.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rw.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ey.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://le.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://pz.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://xz.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lk.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eh.shtwfgs.cn

[D06] 数组长度
来源：http://vo.panjiajie.cn

Py:   len(arr)
来源：http://vx.yuexingan06.cn

PHP:  count($arr);
来源：http://mp.9csxet.cn

JS:   arr.length
来源：http://ol.nszjky.cn

TS:   arr.length
来源：http://np.huixiangedu.cn

Java: list.size();
来源：http://zl.521024.cn

Go:   len(arr)
来源：http://vj.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://mp.colortex.cn

C#:   list.Count;
来源：http://jm.9csxet.cn

[D07] 切片 / 取子数组
来源：http://zg.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ut.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tm.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://hl.asd995.cn

TS:   arr.slice(1, 4);
来源：http://fd.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://vj.gzmigu.cn

Go:   arr[1:4]
来源：http://my.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://cn.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://ql.lnxyls.cn

[D08] 合并两个数组
来源：http://ty.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://gd.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://ly.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zd.newstarts.cn

TS:   [...a, ...b];
来源：http://yp.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gq.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://ti.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://bz.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://di.szxytkj.cn

[D09] 排序（升序）
来源：http://qa.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://my.newstarts.cn

PHP:  sort($arr);
来源：http://uw.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cz.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bs.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ah.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yh.huixiangedu.cn

Ruby: arr.sort
来源：http://nr.nszjky.cn

C#:   list.Sort();
来源：http://oe.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mg.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rr.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rg.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://id.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wb.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kw.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ou.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mw.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ix.huanxung.cn

[D11] 反转数组
来源：http://dn.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ct.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://oq.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xh.shxzskj.cn

TS:   [...arr].reverse();
来源：http://hj.gzmigu.cn

Java: Collections.reverse(list);
来源：http://ug.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://nq.jctech888.com.cn

Ruby: arr.reverse
来源：http://pu.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://kz.yuexingan06.cn

[D12] 查找元素下标
来源：http://qx.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://ks.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://on.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bu.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://at.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://az.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://rg.hahajie.cn

Ruby: arr.index(x)
来源：http://pb.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://oc.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://uz.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hp.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sq.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://yu.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://ox.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zl.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pv.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sb.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rr.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ph.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qb.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ra.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://jk.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://rv.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rb.newstarts.cn

Go:   // 手写循环
来源：http://tu.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lg.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cl.yuexingan06.cn

[D15] 去重
来源：http://yx.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hf.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://cu.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://za.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://ud.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hy.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ip.nicolike.cn

Ruby: arr.uniq
来源：http://op.asd995.cn

C#:   list.Distinct().ToList()
来源：http://cy.lnxyls.cn

[D16] 求和与平均值
来源：http://zj.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fc.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xt.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gg.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bs.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dd.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://ct.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rc.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://yx.hahajie.cn

[D17] 最大值与最小值
来源：http://gu.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://tb.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://kf.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lc.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://dh.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ms.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://no.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://nz.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://ds.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://fm.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xg.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://jt.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xj.huixinmuqiang.cn

TS:   nested.flat();
来源：http://ae.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ts.shtwfgs.cn

Go:   // 手写双层循环
来源：http://sc.bookmarksfly.cn

Ruby: nested.flatten
来源：http://cc.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xx.shtwfgs.cn

[D19] 按字段分组
来源：http://li.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mg.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dr.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rb.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vi.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ts.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://dw.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vm.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gq.colortex.cn

[D20] 统计每个元素出现次数
来源：http://bl.wgjwhj.cn

Py:   Counter(arr)
来源：http://le.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://cf.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://st.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://po.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dk.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://cq.nszjky.cn

Ruby: arr.tally
来源：http://ec.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qs.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://jy.lnxyls.cn

Py:   x in arr
来源：http://dz.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://kt.521024.cn

JS:   arr.includes(x)
来源：http://gs.szxytkj.cn

TS:   arr.includes(x)
来源：http://tp.nicolike.cn

Java: list.contains(x)
来源：http://yq.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://gk.colortex.cn

Ruby: arr.include?(x)
来源：http://ja.bjjhwx.cn

C#:   list.Contains(x)
来源：http://na.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://rc.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uq.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hq.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sz.bookmarksfly.cn

TS:   [...arr];
来源：http://mj.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://lg.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ta.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://vk.9csxet.cn

C#:   new List<int>(list);
来源：http://bn.panjiajie.cn

[D23] reduce 累积计算
来源：http://xg.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://by.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yl.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ba.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fl.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ai.shxzukj.cn

Go:   // 手写循环
来源：http://vc.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ik.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oo.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://tz.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kb.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nb.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xf.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bo.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fp.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qw.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://he.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ji.521024.cn

[D25] Set 集合去重与交并差
来源：http://bz.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ew.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://um.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kl.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xb.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wm.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oa.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zu.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kq.jctech888.com.cn

[D26] 数组转字符串
来源：http://lb.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://lh.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://zp.shtwfgs.cn

JS:   arr.join(", ")
来源：http://pu.panjiajie.cn

TS:   arr.join(", ")
来源：http://dn.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://ej.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://qa.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://yq.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ca.szsharing.cn

================================================================================
来源：http://xb.shxzskj.cn

E. 字符串处理
来源：http://wr.huixiangedu.cn

================================================================================
来源：http://vs.9csxet.cn

[E01] 拼接字符串
来源：http://ur.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uo.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ns.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lo.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mz.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zc.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sv.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dq.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eh.colortex.cn

[E02] 重复字符串
来源：http://ne.hnjuh.cn

Py:   "ab" * 3
来源：http://ai.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://fi.hahajie.cn

JS:   "ab".repeat(3)
来源：http://fm.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://zt.nszjky.cn

Java: "ab".repeat(3)
来源：http://dn.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://bv.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://np.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ds.521024.cn

[E03] 截取子串
来源：http://fn.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ij.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xt.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fb.9csxet.cn

TS:   s.slice(1, 4)
来源：http://qn.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://hf.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dv.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sl.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://gy.wgjwhj.cn

[E04] 查找子串位置
来源：http://ve.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://nf.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://ao.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xl.shxzukj.cn

TS:   s.indexOf("x")
来源：http://ld.newstarts.cn

Java: s.indexOf("x")
来源：http://mw.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://hg.muxihuayi.cn

Ruby: s.index("x")
来源：http://el.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://gr.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pi.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oa.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wy.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mq.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ra.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vr.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rm.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ll.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oj.chemitech.net.cn

[E06] 替换子串
来源：http://hc.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ok.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ho.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uc.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://qp.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zp.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gr.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://au.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://ua.newstarts.cn

[E07] 按分隔符拆分
来源：http://zp.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lw.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lm.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rl.jianghongdianzi.cn

TS:   s.split(",")
来源：http://fp.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jm.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ib.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://zl.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qh.huanxung.cn

[E08] 数组按分隔符合并
来源：http://zh.gzmigu.cn

Py:   ",".join(items)
来源：http://ds.jianghongdianzi.cn


<!-- 参考信息 -->