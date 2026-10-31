代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cb.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hn.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gj.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mv.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://jc.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://tg.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mv.szsharing.cn

[D02] 追加元素到末尾
来源：http://qg.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tt.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oc.huixiangedu.cn

JS:   arr.push(4);
来源：http://db.chemitech.net.cn

TS:   arr.push(4);
来源：http://xb.jctech888.com.cn

Java: list.add(4);
来源：http://zh.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://re.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://cc.huixiangedu.cn

C#:   list.Add(4);
来源：http://hm.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://db.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ts.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://in.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jb.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://ff.newstarts.cn

Java: list.add(0, 0);
来源：http://ej.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rs.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ri.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://ba.colortex.cn

[D04] 删除元素
来源：http://lk.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wl.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ke.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vs.colortex.cn

TS:   arr.splice(0, 1);
来源：http://ae.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://de.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sj.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ud.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nu.shtwfgs.cn

[D05] 访问与修改元素
来源：http://eq.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rj.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vt.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ib.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://co.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://ao.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://su.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://is.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vr.panjiajie.cn

[D06] 数组长度
来源：http://cy.hahajie.cn

Py:   len(arr)
来源：http://dw.wgjwhj.cn

PHP:  count($arr);
来源：http://gb.9csxet.cn

JS:   arr.length
来源：http://ul.yuexingan06.cn

TS:   arr.length
来源：http://hy.hnjuh.cn

Java: list.size();
来源：http://dc.chemitech.net.cn

Go:   len(arr)
来源：http://cp.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://qu.nszjky.cn

C#:   list.Count;
来源：http://tp.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://tv.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tk.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qu.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://lr.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://kh.shxzukj.cn

Java: list.subList(1, 4);
来源：http://au.nicolike.cn

Go:   arr[1:4]
来源：http://hm.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://qc.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://qs.szsharing.cn

[D08] 合并两个数组
来源：http://lt.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://gu.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://dp.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://op.panjiajie.cn

TS:   [...a, ...b];
来源：http://gw.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kq.521024.cn

Go:   append(a, b...)
来源：http://og.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://go.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://sh.panjiajie.cn

[D09] 排序（升序）
来源：http://te.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://uu.bookmarksfly.cn

PHP:  sort($arr);
来源：http://at.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fx.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://af.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bs.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oq.muxihuayi.cn

Ruby: arr.sort
来源：http://ea.nszjky.cn

C#:   list.Sort();
来源：http://fe.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xr.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xb.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fs.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ou.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ft.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yq.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vf.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dh.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ez.yuntaijiaju.cn

[D11] 反转数组
来源：http://el.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ec.hahajie.cn

PHP:  array_reverse($arr);
来源：http://ru.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://md.nicolike.cn

TS:   [...arr].reverse();
来源：http://ui.shxzukj.cn

Java: Collections.reverse(list);
来源：http://yd.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://ir.nszjky.cn

Ruby: arr.reverse
来源：http://mv.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://zs.bjjhwx.cn

[D12] 查找元素下标
来源：http://rt.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://pw.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rt.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://af.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vk.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://om.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://de.521024.cn

Ruby: arr.index(x)
来源：http://wq.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://bc.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://rt.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://py.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://md.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://jd.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://ng.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bj.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wm.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://su.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ud.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://tr.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mp.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ai.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://pz.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://mj.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xe.hnjuh.cn

Go:   // 手写循环
来源：http://px.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vl.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mc.nicolike.cn

[D15] 去重
来源：http://pw.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uo.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://ni.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://vj.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://vu.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hj.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ga.jctech888.com.cn

Ruby: arr.uniq
来源：http://rr.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://rx.jctech888.com.cn

[D16] 求和与平均值
来源：http://hg.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qv.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vz.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ji.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cr.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uj.szxytkj.cn

Go:   // 手写循环累加
来源：http://pf.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kn.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://av.hnjuh.cn

[D17] 最大值与最小值
来源：http://ed.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://cm.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://aj.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lj.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://oa.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mb.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qi.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://zc.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://sk.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://dy.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rz.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://fd.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cs.hahajie.cn

TS:   nested.flat();
来源：http://su.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jw.nicolike.cn

Go:   // 手写双层循环
来源：http://vh.521024.cn

Ruby: nested.flatten
来源：http://el.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zc.shxzskj.cn

[D19] 按字段分组
来源：http://ur.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vz.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ns.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gc.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jc.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oy.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://vx.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ub.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tz.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://pq.chemitech.net.cn

Py:   Counter(arr)
来源：http://bk.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://hd.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ci.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fm.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uw.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://hc.shxzskj.cn

Ruby: arr.tally
来源：http://yt.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fv.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://at.newstarts.cn

Py:   x in arr
来源：http://zr.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://kf.hnjuh.cn

JS:   arr.includes(x)
来源：http://cv.hnjuh.cn

TS:   arr.includes(x)
来源：http://ja.hahajie.cn

Java: list.contains(x)
来源：http://rj.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://ky.newstarts.cn

Ruby: arr.include?(x)
来源：http://wb.huixiangedu.cn

C#:   list.Contains(x)
来源：http://ta.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://jy.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qt.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gr.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wt.shxzskj.cn

TS:   [...arr];
来源：http://ku.asd995.cn

Java: new ArrayList<>(list);
来源：http://eo.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ob.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://mo.wgjwhj.cn

C#:   new List<int>(list);
来源：http://fq.shtwfgs.cn

[D23] reduce 累积计算
来源：http://nf.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ep.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iv.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ke.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uv.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yv.haigaiapp.cn

Go:   // 手写循环
来源：http://fx.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gu.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bb.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://bc.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qg.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ru.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ip.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cd.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nt.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rc.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eg.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://br.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://xa.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ly.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rp.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ib.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ta.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kn.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wm.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rd.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nb.shxzukj.cn

[D26] 数组转字符串
来源：http://kg.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://bo.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://yp.colortex.cn

JS:   arr.join(", ")
来源：http://ic.newstarts.cn

TS:   arr.join(", ")
来源：http://lo.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://hg.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://ry.521024.cn

Ruby: arr.join(", ")
来源：http://hp.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://je.panjiajie.cn

================================================================================
来源：http://ut.lnxyls.cn

E. 字符串处理
来源：http://kz.huixiangedu.cn

================================================================================
来源：http://el.lnxyls.cn

[E01] 拼接字符串
来源：http://uy.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qw.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fn.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nq.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ws.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cx.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kz.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lr.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bl.shtwfgs.cn

[E02] 重复字符串
来源：http://zf.muxihuayi.cn

Py:   "ab" * 3
来源：http://fh.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://em.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://ui.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://wu.shxzukj.cn

Java: "ab".repeat(3)
来源：http://ky.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://on.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://ud.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://az.jianghongdianzi.cn

[E03] 截取子串
来源：http://bt.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lh.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iu.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rt.nicolike.cn

TS:   s.slice(1, 4)
来源：http://ed.szsharing.cn

Java: s.substring(1, 4)
来源：http://zl.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fx.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jx.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://pk.colortex.cn

[E04] 查找子串位置
来源：http://gp.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://sr.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://gf.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ts.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://lc.521024.cn

Java: s.indexOf("x")
来源：http://jr.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://tz.szxytkj.cn

Ruby: s.index("x")
来源：http://an.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://mv.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://of.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yo.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://in.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fg.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xs.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uc.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ey.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://go.jianghongdianzi.cn

[E06] 替换子串
来源：http://fw.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dg.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://nq.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uf.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://mb.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ev.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xy.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nr.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://jg.shxzskj.cn

[E07] 按分隔符拆分
来源：http://gw.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bq.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aj.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zv.hnjuh.cn

TS:   s.split(",")
来源：http://ig.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://id.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ah.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://uv.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kd.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://ad.huixiangedu.cn

Py:   ",".join(items)
来源：http://de.panjiajie.cn


<!-- 参考信息 -->