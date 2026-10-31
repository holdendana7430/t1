代发 wailian999

D. 数组 / 列表 / 集合
来源：http://ky.newstarts.cn

================================================================================
来源：http://iu.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://eh.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cq.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sm.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tt.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wl.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ih.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://sr.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://wj.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gi.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://hv.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://md.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pf.shxzukj.cn

JS:   arr.push(4);
来源：http://ue.521024.cn

TS:   arr.push(4);
来源：http://ol.hahajie.cn

Java: list.add(4);
来源：http://lv.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://an.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://wl.huixiangedu.cn

C#:   list.Add(4);
来源：http://kq.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://oc.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://vq.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://as.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lz.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://rr.muxihuayi.cn

Java: list.add(0, 0);
来源：http://il.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zp.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nz.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://vc.muxihuayi.cn

[D04] 删除元素
来源：http://oa.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mk.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://de.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://em.colortex.cn

TS:   arr.splice(0, 1);
来源：http://tv.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xb.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nk.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qf.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bs.yuexingan06.cn

[D05] 访问与修改元素
来源：http://ly.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bc.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://of.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bc.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://ur.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://lb.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ep.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xb.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dm.yuntaijiaju.cn

[D06] 数组长度
来源：http://px.521024.cn

Py:   len(arr)
来源：http://vu.9csxet.cn

PHP:  count($arr);
来源：http://zi.521024.cn

JS:   arr.length
来源：http://wb.bjjhwx.cn

TS:   arr.length
来源：http://jr.bookmarksfly.cn

Java: list.size();
来源：http://xn.colortex.cn

Go:   len(arr)
来源：http://we.newstarts.cn

Ruby: arr.length; arr.size
来源：http://rc.newstarts.cn

C#:   list.Count;
来源：http://lp.9csxet.cn

[D07] 切片 / 取子数组
来源：http://eg.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://in.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dv.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://ji.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://zy.szsharing.cn

Java: list.subList(1, 4);
来源：http://ir.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://sx.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://io.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://gc.shxzskj.cn

[D08] 合并两个数组
来源：http://cs.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://wu.521024.cn

PHP:  array_merge($a, $b);
来源：http://py.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mu.huixiangedu.cn

TS:   [...a, ...b];
来源：http://xk.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ef.jctech888.com.cn

Go:   append(a, b...)
来源：http://ak.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://dp.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://vs.newstarts.cn

[D09] 排序（升序）
来源：http://jh.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://kr.shxzukj.cn

PHP:  sort($arr);
来源：http://eg.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nl.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lm.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://de.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dr.hnjuh.cn

Ruby: arr.sort
来源：http://eu.nicolike.cn

C#:   list.Sort();
来源：http://fb.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sj.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jx.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bt.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gr.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yy.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bc.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cn.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pr.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rp.shxzskj.cn

[D11] 反转数组
来源：http://ks.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://eh.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://pe.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vo.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://ov.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://gl.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://qq.bjjhwx.cn

Ruby: arr.reverse
来源：http://rf.9csxet.cn

C#:   list.Reverse();
来源：http://jw.panjiajie.cn

[D12] 查找元素下标
来源：http://ca.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://zv.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://um.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pt.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gt.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cy.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://yc.gzmigu.cn

Ruby: arr.index(x)
来源：http://lw.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://tw.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://fs.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://na.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oh.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://un.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://bn.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ev.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cd.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yh.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oz.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://fj.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ri.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ut.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://rh.521024.cn

TS:   arr.map(x => x * 2)
来源：http://dv.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fe.hnjuh.cn

Go:   // 手写循环
来源：http://tk.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gy.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ma.chemitech.net.cn

[D15] 去重
来源：http://ow.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://we.huanxung.cn

PHP:  array_unique($arr);
来源：http://ic.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://mv.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://ao.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eo.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vq.hahajie.cn

Ruby: arr.uniq
来源：http://ix.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://lu.shxzukj.cn

[D16] 求和与平均值
来源：http://ku.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oq.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://am.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vg.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ku.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rp.asd995.cn

Go:   // 手写循环累加
来源：http://ak.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rh.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://or.asd995.cn

[D17] 最大值与最小值
来源：http://tu.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://ze.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ed.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tc.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://hd.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gg.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gb.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://mw.521024.cn

C#:   list.Max();  list.Min()
来源：http://iy.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://aj.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wj.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://zs.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tm.muxihuayi.cn

TS:   nested.flat();
来源：http://iw.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kb.yuexingan06.cn

Go:   // 手写双层循环
来源：http://dd.nicolike.cn

Ruby: nested.flatten
来源：http://zg.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xr.9csxet.cn

[D19] 按字段分组
来源：http://lp.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cl.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jf.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wg.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jh.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jj.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://qe.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ip.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oc.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://ym.newstarts.cn

Py:   Counter(arr)
来源：http://ke.colortex.cn

PHP:  array_count_values($arr);
来源：http://kx.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fq.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uo.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qr.521024.cn

Go:   // 手写 map[T]int
来源：http://xi.szsharing.cn

Ruby: arr.tally
来源：http://xd.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ei.szsharing.cn

[D21] 判断是否包含某元素
来源：http://fr.hahajie.cn

Py:   x in arr
来源：http://wm.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://vi.gzmigu.cn

JS:   arr.includes(x)
来源：http://hk.shtwfgs.cn

TS:   arr.includes(x)
来源：http://tm.9csxet.cn

Java: list.contains(x)
来源：http://yb.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://jj.9csxet.cn

Ruby: arr.include?(x)
来源：http://gb.panjiajie.cn

C#:   list.Contains(x)
来源：http://cn.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://eg.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tb.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kw.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mx.9csxet.cn

TS:   [...arr];
来源：http://pt.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://gk.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ud.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://qm.haigaiapp.cn

C#:   new List<int>(list);
来源：http://cd.bjjhwx.cn

[D23] reduce 累积计算
来源：http://by.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ag.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eo.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ag.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fd.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qr.muxihuayi.cn

Go:   // 手写循环
来源：http://yb.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tg.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ng.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://xj.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kv.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dc.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://de.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qx.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kj.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hs.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ly.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hw.asd995.cn

[D25] Set 集合去重与交并差
来源：http://hi.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sh.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gc.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://de.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gq.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sb.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lu.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mc.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zt.huanxung.cn

[D26] 数组转字符串
来源：http://gr.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://me.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://my.9csxet.cn

JS:   arr.join(", ")
来源：http://ef.521024.cn

TS:   arr.join(", ")
来源：http://zm.nszjky.cn

Java: String.join(", ", list)
来源：http://da.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://yg.nszjky.cn

Ruby: arr.join(", ")
来源：http://ak.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://fv.newstarts.cn

================================================================================
来源：http://de.521024.cn

E. 字符串处理
来源：http://px.muxihuayi.cn

================================================================================
来源：http://ts.lnxyls.cn

[E01] 拼接字符串
来源：http://kz.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jt.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kw.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ct.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sj.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cx.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vh.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sj.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qh.bookmarksfly.cn

[E02] 重复字符串
来源：http://el.hahajie.cn

Py:   "ab" * 3
来源：http://ed.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://oy.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://uc.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://sz.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://py.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://kc.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://og.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://em.panjiajie.cn

[E03] 截取子串
来源：http://bt.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hw.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ka.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qi.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://jk.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://hs.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jp.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cz.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://bf.gzmigu.cn

[E04] 查找子串位置
来源：http://ui.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://zo.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://hb.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ll.asd995.cn

TS:   s.indexOf("x")
来源：http://lu.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://nm.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://cb.shxzukj.cn

Ruby: s.index("x")
来源：http://dk.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://jw.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jk.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vf.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kv.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rw.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zf.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xt.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cj.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uy.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lp.shxzskj.cn

[E06] 替换子串
来源：http://de.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zq.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://xp.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tw.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://sw.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ee.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kp.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sg.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://ig.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://lb.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ml.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zz.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sv.gzmigu.cn

TS:   s.split(",")
来源：http://ks.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mn.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uh.gzmigu.cn


<!-- 参考信息 -->