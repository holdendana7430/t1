代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nw.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gp.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ho.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qo.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://mf.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://hn.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bp.colortex.cn

[D02] 追加元素到末尾
来源：http://wn.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aw.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://kq.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://hg.lnxyls.cn

Java: list.add(4);
来源：http://hr.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://bc.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://kt.colortex.cn

C#:   list.Add(4);
来源：http://it.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://ok.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://as.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jg.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ww.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://hx.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://mp.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://og.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yr.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://dd.shxzskj.cn

[D04] 删除元素
来源：http://ab.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://we.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gp.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://st.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://me.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xd.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vu.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fe.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vr.gzmigu.cn

[D05] 访问与修改元素
来源：http://zp.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cu.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zh.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gf.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://dw.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://mb.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://eh.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hg.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://us.shxzukj.cn

[D06] 数组长度
来源：http://qc.szsharing.cn

Py:   len(arr)
来源：http://fg.hahajie.cn

PHP:  count($arr);
来源：http://yu.521024.cn

JS:   arr.length
来源：http://cz.chemitech.net.cn

TS:   arr.length
来源：http://zm.nicolike.cn

Java: list.size();
来源：http://py.bookmarksfly.cn

Go:   len(arr)
来源：http://ni.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://wd.nszjky.cn

C#:   list.Count;
来源：http://pr.9csxet.cn

[D07] 切片 / 取子数组
来源：http://wh.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oh.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kc.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://ca.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://ak.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://wz.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ll.newstarts.cn

Ruby: arr[1, 3]
来源：http://kc.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://gg.wgjwhj.cn

[D08] 合并两个数组
来源：http://zp.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://nv.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://xd.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cq.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://sp.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jz.lnxyls.cn

Go:   append(a, b...)
来源：http://xn.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://ho.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://od.chemitech.net.cn

[D09] 排序（升序）
来源：http://rw.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://wu.asd995.cn

PHP:  sort($arr);
来源：http://rn.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://px.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xr.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wi.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zp.hahajie.cn

Ruby: arr.sort
来源：http://gh.newstarts.cn

C#:   list.Sort();
来源：http://zz.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zm.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jx.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://id.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zq.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bz.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gt.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lp.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bo.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://is.yuntaijiaju.cn

[D11] 反转数组
来源：http://vi.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://le.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://xs.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ij.szsharing.cn

TS:   [...arr].reverse();
来源：http://aq.hahajie.cn

Java: Collections.reverse(list);
来源：http://zk.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://li.wgjwhj.cn

Ruby: arr.reverse
来源：http://mv.newstarts.cn

C#:   list.Reverse();
来源：http://pc.yuexingan06.cn

[D12] 查找元素下标
来源：http://jc.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://fc.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tq.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bz.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://va.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://my.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://wc.jctech888.com.cn

Ruby: arr.index(x)
来源：http://xo.colortex.cn

C#:   list.IndexOf(x);
来源：http://wx.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ug.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wc.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ob.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://cx.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://bn.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tb.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ud.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ul.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://my.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://pk.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jy.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ma.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://eo.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://vk.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ob.jctech888.com.cn

Go:   // 手写循环
来源：http://bf.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vo.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ym.shtwfgs.cn

[D15] 去重
来源：http://bw.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lg.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://ku.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://vb.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://zs.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gv.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cg.gzmigu.cn

Ruby: arr.uniq
来源：http://sz.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://cq.chemitech.net.cn

[D16] 求和与平均值
来源：http://ml.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kh.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sy.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sm.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cc.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vd.asd995.cn

Go:   // 手写循环累加
来源：http://dp.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cl.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://qv.huixiangedu.cn

[D17] 最大值与最小值
来源：http://mm.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://mi.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://cg.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rw.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://sz.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jv.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rt.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ow.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://qs.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://lq.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xc.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://px.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wb.shtwfgs.cn

TS:   nested.flat();
来源：http://id.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iz.asd995.cn

Go:   // 手写双层循环
来源：http://wd.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://gu.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jv.9csxet.cn

[D19] 按字段分组
来源：http://ui.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tk.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yx.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vc.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pn.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ag.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://zw.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dn.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gk.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://ny.shtwfgs.cn

Py:   Counter(arr)
来源：http://lt.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://jt.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hk.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xa.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yh.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://da.521024.cn

Ruby: arr.tally
来源：http://kt.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oj.huanxung.cn

[D21] 判断是否包含某元素
来源：http://uo.szxytkj.cn

Py:   x in arr
来源：http://cr.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://vr.lnxyls.cn

JS:   arr.includes(x)
来源：http://cr.shxzskj.cn

TS:   arr.includes(x)
来源：http://hx.jctech888.com.cn

Java: list.contains(x)
来源：http://df.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://dg.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://ck.shxzukj.cn

C#:   list.Contains(x)
来源：http://fw.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://pp.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oc.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ds.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ug.chemitech.net.cn

TS:   [...arr];
来源：http://sk.nszjky.cn

Java: new ArrayList<>(list);
来源：http://ju.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sj.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://yk.szxytkj.cn

C#:   new List<int>(list);
来源：http://qy.bjjhwx.cn

[D23] reduce 累积计算
来源：http://mu.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uk.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ra.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cw.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vs.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ig.szxytkj.cn

Go:   // 手写循环
来源：http://du.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hl.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ey.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://qz.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bh.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kc.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ci.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aj.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ho.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yx.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xa.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oe.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://yq.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ws.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://at.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kk.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nu.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lv.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gn.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bq.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yy.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://ca.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://ix.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://ks.huanxung.cn

JS:   arr.join(", ")
来源：http://kc.521024.cn

TS:   arr.join(", ")
来源：http://ew.panjiajie.cn

Java: String.join(", ", list)
来源：http://fc.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://xr.huanxung.cn

Ruby: arr.join(", ")
来源：http://hc.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://kf.521024.cn

================================================================================
来源：http://ws.huanxung.cn

E. 字符串处理
来源：http://me.huixiangedu.cn

================================================================================
来源：http://dl.9csxet.cn

[E01] 拼接字符串
来源：http://uh.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ox.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yz.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dr.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://py.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ok.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oa.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ob.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ey.yuexingan06.cn

[E02] 重复字符串
来源：http://wv.asd995.cn

Py:   "ab" * 3
来源：http://ip.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://he.nicolike.cn

JS:   "ab".repeat(3)
来源：http://fd.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://zx.521024.cn

Java: "ab".repeat(3)
来源：http://ez.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://ip.bjjhwx.cn

Ruby: "ab" * 3
来源：http://bn.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ce.jctech888.com.cn

[E03] 截取子串
来源：http://ox.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://id.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://le.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://au.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://co.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://ti.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jl.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ms.521024.cn

C#:   s.Substring(1, 3)
来源：http://dc.521024.cn

[E04] 查找子串位置
来源：http://pi.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://zr.nszjky.cn

PHP:  strpos($s, "x");
来源：http://vz.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lt.nicolike.cn

TS:   s.indexOf("x")
来源：http://li.yuexingan06.cn

Java: s.indexOf("x")
来源：http://qj.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://em.gzmigu.cn

Ruby: s.index("x")
来源：http://gi.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://cm.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tb.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oj.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gd.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ad.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jn.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qh.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sj.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mw.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kx.yuexingan06.cn

[E06] 替换子串
来源：http://si.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oj.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://pl.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://af.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://ji.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sz.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iv.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hu.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://zf.nicolike.cn

[E07] 按分隔符拆分
来源：http://lj.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fq.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uo.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ik.nszjky.cn

TS:   s.split(",")
来源：http://ho.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qa.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ay.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://nk.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ay.huanxung.cn

[E08] 数组按分隔符合并
来源：http://rs.shtwfgs.cn

Py:   ",".join(items)
来源：http://uo.asd995.cn


<!-- 参考信息 -->