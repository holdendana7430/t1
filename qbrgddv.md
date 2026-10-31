代发 wailian999

D. 数组 / 列表 / 集合
来源：http://hd.yuexingan06.cn

================================================================================
来源：http://td.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://dg.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ti.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jf.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xa.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nb.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bm.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://tr.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://ba.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eg.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://hd.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zu.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kp.szsharing.cn

JS:   arr.push(4);
来源：http://ay.shtwfgs.cn

TS:   arr.push(4);
来源：http://ig.nicolike.cn

Java: list.add(4);
来源：http://wg.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://tb.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://wm.shxzskj.cn

C#:   list.Add(4);
来源：http://vn.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://ib.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://bp.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jw.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mp.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://nv.muxihuayi.cn

Java: list.add(0, 0);
来源：http://ix.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cy.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gc.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://hl.szxytkj.cn

[D04] 删除元素
来源：http://mk.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jo.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qs.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://du.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://km.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://da.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aw.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fk.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jt.hahajie.cn

[D05] 访问与修改元素
来源：http://bq.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ns.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jb.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ne.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://vp.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://ga.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://tu.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jj.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ez.yuexingan06.cn

[D06] 数组长度
来源：http://cl.lnxyls.cn

Py:   len(arr)
来源：http://uh.wgjwhj.cn

PHP:  count($arr);
来源：http://qk.colortex.cn

JS:   arr.length
来源：http://pr.gzmigu.cn

TS:   arr.length
来源：http://mx.huanxung.cn

Java: list.size();
来源：http://ad.shxzskj.cn

Go:   len(arr)
来源：http://cc.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://pi.szxytkj.cn

C#:   list.Count;
来源：http://ad.nicolike.cn

[D07] 切片 / 取子数组
来源：http://ox.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bd.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ec.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://fu.asd995.cn

TS:   arr.slice(1, 4);
来源：http://rz.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://mt.lnxyls.cn

Go:   arr[1:4]
来源：http://gf.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://qs.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://hf.gzmigu.cn

[D08] 合并两个数组
来源：http://mb.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://ca.colortex.cn

PHP:  array_merge($a, $b);
来源：http://ro.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wd.asd995.cn

TS:   [...a, ...b];
来源：http://vt.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dw.hnjuh.cn

Go:   append(a, b...)
来源：http://tz.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://dq.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://yy.shtwfgs.cn

[D09] 排序（升序）
来源：http://zl.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://gn.huanxung.cn

PHP:  sort($arr);
来源：http://nm.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ei.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kc.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wu.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yh.nszjky.cn

Ruby: arr.sort
来源：http://sg.yuntaijiaju.cn

C#:   list.Sort();
来源：http://mj.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nt.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sx.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://km.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ic.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mi.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gj.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xk.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ek.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jk.huixiangedu.cn

[D11] 反转数组
来源：http://lz.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wz.nszjky.cn

PHP:  array_reverse($arr);
来源：http://zt.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cl.szsharing.cn

TS:   [...arr].reverse();
来源：http://fm.szxytkj.cn

Java: Collections.reverse(list);
来源：http://yf.colortex.cn

Go:   slices.Reverse(arr)
来源：http://xs.nicolike.cn

Ruby: arr.reverse
来源：http://po.colortex.cn

C#:   list.Reverse();
来源：http://rx.colortex.cn

[D12] 查找元素下标
来源：http://ak.521024.cn

Py:   arr.index(x);  x in arr
来源：http://ny.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dn.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aj.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ex.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ux.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://kb.panjiajie.cn

Ruby: arr.index(x)
来源：http://eo.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://xh.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://wb.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://si.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zk.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://ma.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://vv.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rx.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://un.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hr.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://id.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://ob.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dn.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ex.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://ui.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://xr.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nf.szsharing.cn

Go:   // 手写循环
来源：http://jf.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sc.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lo.asd995.cn

[D15] 去重
来源：http://ni.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://md.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://wr.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://we.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://hv.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mw.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ou.9csxet.cn

Ruby: arr.uniq
来源：http://dg.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://ad.hnjuh.cn

[D16] 求和与平均值
来源：http://jr.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tu.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iz.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ki.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ut.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://en.hnjuh.cn

Go:   // 手写循环累加
来源：http://pa.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://su.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://tl.hahajie.cn

[D17] 最大值与最小值
来源：http://nv.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://iw.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://wo.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qx.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://iq.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qm.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rx.521024.cn

Ruby: arr.max;  arr.min
来源：http://kd.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://jq.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://nz.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kp.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://zk.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://db.szsharing.cn

TS:   nested.flat();
来源：http://th.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ei.asd995.cn

Go:   // 手写双层循环
来源：http://wi.bookmarksfly.cn

Ruby: nested.flatten
来源：http://oh.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ct.lnxyls.cn

[D19] 按字段分组
来源：http://la.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yj.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://as.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jy.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wh.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ul.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://in.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ta.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bl.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://xe.szxytkj.cn

Py:   Counter(arr)
来源：http://ds.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://zd.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lb.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ob.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://av.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://uz.521024.cn

Ruby: arr.tally
来源：http://gp.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qg.asd995.cn

[D21] 判断是否包含某元素
来源：http://jy.newstarts.cn

Py:   x in arr
来源：http://ny.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://fl.szxytkj.cn

JS:   arr.includes(x)
来源：http://sh.haigaiapp.cn

TS:   arr.includes(x)
来源：http://yb.jctech888.com.cn

Java: list.contains(x)
来源：http://jf.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://xh.9csxet.cn

Ruby: arr.include?(x)
来源：http://sr.shtwfgs.cn

C#:   list.Contains(x)
来源：http://yl.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://lm.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ob.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://el.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fh.muxihuayi.cn

TS:   [...arr];
来源：http://xn.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://fd.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cr.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://yu.shtwfgs.cn

C#:   new List<int>(list);
来源：http://gb.9csxet.cn

[D23] reduce 累积计算
来源：http://vw.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tj.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nu.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bc.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yu.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fp.haigaiapp.cn

Go:   // 手写循环
来源：http://lt.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mw.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ja.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ml.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yt.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tc.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wt.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qk.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mk.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ja.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yh.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qs.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://eq.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ha.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gi.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tx.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dh.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cp.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bs.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vz.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ck.bjjhwx.cn

[D26] 数组转字符串
来源：http://ay.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://xr.colortex.cn

PHP:  implode(", ", $arr);
来源：http://zu.gzmigu.cn

JS:   arr.join(", ")
来源：http://ze.nszjky.cn

TS:   arr.join(", ")
来源：http://pf.szxytkj.cn

Java: String.join(", ", list)
来源：http://lq.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://qw.nicolike.cn

Ruby: arr.join(", ")
来源：http://gd.newstarts.cn

C#:   string.Join(", ", list)
来源：http://li.nicolike.cn

================================================================================
来源：http://gv.hahajie.cn

E. 字符串处理
来源：http://we.newstarts.cn

================================================================================
来源：http://jh.shtwfgs.cn

[E01] 拼接字符串
来源：http://ib.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rc.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xp.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hp.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pb.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yn.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zn.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zc.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zx.asd995.cn

[E02] 重复字符串
来源：http://im.gzmigu.cn

Py:   "ab" * 3
来源：http://jo.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://tg.newstarts.cn

JS:   "ab".repeat(3)
来源：http://lx.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://iq.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://ft.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://oc.shxzukj.cn

Ruby: "ab" * 3
来源：http://mh.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rz.chemitech.net.cn

[E03] 截取子串
来源：http://sf.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ce.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iz.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cf.521024.cn

TS:   s.slice(1, 4)
来源：http://pq.huanxung.cn

Java: s.substring(1, 4)
来源：http://sv.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ew.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vl.asd995.cn

C#:   s.Substring(1, 3)
来源：http://qs.panjiajie.cn

[E04] 查找子串位置
来源：http://me.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://qr.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://er.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dq.nszjky.cn

TS:   s.indexOf("x")
来源：http://pr.9csxet.cn

Java: s.indexOf("x")
来源：http://ga.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://jx.colortex.cn

Ruby: s.index("x")
来源：http://fj.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://bv.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nj.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uk.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nu.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xz.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bn.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dl.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rd.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lr.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mb.chemitech.net.cn

[E06] 替换子串
来源：http://zc.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vr.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://qy.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vv.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://nr.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nt.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qc.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jd.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://pt.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://cs.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mx.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kv.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tx.hahajie.cn

TS:   s.split(",")
来源：http://vn.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vh.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gg.nicolike.cn


<!-- 参考信息 -->