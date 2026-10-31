代发 wailian999

D. 数组 / 列表 / 集合
来源：http://rh.hnjuh.cn

================================================================================
来源：http://eg.nszjky.cn

[D01] 创建数组 / 列表
来源：http://hg.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ug.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wd.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zj.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rz.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hu.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://au.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://ur.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mw.shxzukj.cn

[D02] 追加元素到末尾
来源：http://ky.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ot.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mu.newstarts.cn

JS:   arr.push(4);
来源：http://di.asd995.cn

TS:   arr.push(4);
来源：http://yd.jctech888.com.cn

Java: list.add(4);
来源：http://dw.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ve.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://rm.jctech888.com.cn

C#:   list.Add(4);
来源：http://ft.nszjky.cn

[D03] 在指定位置插入元素
来源：http://vq.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://em.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wp.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zf.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://ct.521024.cn

Java: list.add(0, 0);
来源：http://it.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uu.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tx.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ks.hnjuh.cn

[D04] 删除元素
来源：http://ys.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iw.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ti.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vm.yuexingan06.cn

TS:   arr.splice(0, 1);
来源：http://vo.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sl.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://or.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tu.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xa.colortex.cn

[D05] 访问与修改元素
来源：http://dv.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ed.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ee.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pj.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://gk.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://yh.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://tt.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ti.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lp.nszjky.cn

[D06] 数组长度
来源：http://gy.panjiajie.cn

Py:   len(arr)
来源：http://eq.huixiangedu.cn

PHP:  count($arr);
来源：http://bp.panjiajie.cn

JS:   arr.length
来源：http://su.haigaiapp.cn

TS:   arr.length
来源：http://wy.shxzukj.cn

Java: list.size();
来源：http://ct.9csxet.cn

Go:   len(arr)
来源：http://wh.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://aj.jianghongdianzi.cn

C#:   list.Count;
来源：http://gz.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://jz.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uw.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lo.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://po.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://th.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://ej.huanxung.cn

Go:   arr[1:4]
来源：http://ku.hahajie.cn

Ruby: arr[1, 3]
来源：http://va.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://mv.huixiangedu.cn

[D08] 合并两个数组
来源：http://gr.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://gx.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://la.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://da.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://ts.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hf.huixiangedu.cn

Go:   append(a, b...)
来源：http://ni.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://sb.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://gs.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://ym.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.bookmarksfly.cn

PHP:  sort($arr);
来源：http://mg.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fu.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wm.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gk.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://er.hahajie.cn

Ruby: arr.sort
来源：http://cb.hahajie.cn

C#:   list.Sort();
来源：http://ar.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bp.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pq.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xp.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ot.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bm.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aw.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ef.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ps.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dq.huixinmuqiang.cn

[D11] 反转数组
来源：http://ef.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rh.asd995.cn

PHP:  array_reverse($arr);
来源：http://ki.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://av.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://vu.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://ya.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://dh.huixiangedu.cn

Ruby: arr.reverse
来源：http://om.9csxet.cn

C#:   list.Reverse();
来源：http://eu.9csxet.cn

[D12] 查找元素下标
来源：http://kq.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://at.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ky.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kf.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ks.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ge.asd995.cn

Go:   slices.Index(arr, x)
来源：http://su.huanxung.cn

Ruby: arr.index(x)
来源：http://gc.521024.cn

C#:   list.IndexOf(x);
来源：http://ge.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://pd.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ml.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ho.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://sz.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://vs.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nt.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://if.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ze.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aa.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://lh.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fs.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uy.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://fq.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://rk.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sd.hahajie.cn

Go:   // 手写循环
来源：http://wv.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mx.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xa.huanxung.cn

[D15] 去重
来源：http://qf.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tv.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://gi.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://lv.hahajie.cn

TS:   [...new Set(arr)]
来源：http://jm.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ub.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ov.nicolike.cn

Ruby: arr.uniq
来源：http://cu.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://yp.521024.cn

[D16] 求和与平均值
来源：http://cx.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://px.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cv.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hi.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dn.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://op.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://mq.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xh.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://dy.chemitech.net.cn

[D17] 最大值与最小值
来源：http://bb.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://am.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://gf.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xb.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://wb.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dw.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ol.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://gv.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://jh.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://lw.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oz.colortex.cn

PHP:  array_merge(...$nested);
来源：http://vj.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mo.521024.cn

TS:   nested.flat();
来源：http://hb.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gp.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://zv.shtwfgs.cn

Ruby: nested.flatten
来源：http://xj.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jf.9csxet.cn

[D19] 按字段分组
来源：http://lj.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bj.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cx.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eb.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hx.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qr.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://mm.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ts.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ru.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://bt.huixiangedu.cn

Py:   Counter(arr)
来源：http://ef.newstarts.cn

PHP:  array_count_values($arr);
来源：http://qo.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iy.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hd.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dp.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://pw.nszjky.cn

Ruby: arr.tally
来源：http://et.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jv.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://hz.521024.cn

Py:   x in arr
来源：http://bn.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://ya.haigaiapp.cn

JS:   arr.includes(x)
来源：http://yg.haigaiapp.cn

TS:   arr.includes(x)
来源：http://ev.huixinmuqiang.cn

Java: list.contains(x)
来源：http://px.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://dw.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://yu.hnjuh.cn

C#:   list.Contains(x)
来源：http://zh.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://mb.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zy.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ul.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jn.521024.cn

TS:   [...arr];
来源：http://lw.huanxung.cn

Java: new ArrayList<>(list);
来源：http://tj.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hs.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://xb.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://ah.yuexingan06.cn

[D23] reduce 累积计算
来源：http://pj.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rh.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yk.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://an.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://id.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oh.nszjky.cn

Go:   // 手写循环
来源：http://ec.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fw.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pl.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://gi.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zr.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rm.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ea.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kp.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://he.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tw.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ib.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ma.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://xt.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ub.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zc.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://my.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xo.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://en.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hr.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uj.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lf.gzmigu.cn

[D26] 数组转字符串
来源：http://mw.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://xi.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://yf.lnxyls.cn

JS:   arr.join(", ")
来源：http://ch.lnxyls.cn

TS:   arr.join(", ")
来源：http://gv.jctech888.com.cn

Java: String.join(", ", list)
来源：http://vz.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://lc.9csxet.cn

Ruby: arr.join(", ")
来源：http://af.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://wb.9csxet.cn

================================================================================
来源：http://eo.shxzukj.cn

E. 字符串处理
来源：http://ws.chemitech.net.cn

================================================================================
来源：http://hl.newstarts.cn

[E01] 拼接字符串
来源：http://ll.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zk.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nw.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mi.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ll.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fy.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wt.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rk.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mu.panjiajie.cn

[E02] 重复字符串
来源：http://qq.panjiajie.cn

Py:   "ab" * 3
来源：http://ie.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://my.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://xa.asd995.cn

TS:   "ab".repeat(3)
来源：http://jw.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://ro.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ea.bjjhwx.cn

Ruby: "ab" * 3
来源：http://ze.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vn.hnjuh.cn

[E03] 截取子串
来源：http://fl.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ld.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tj.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bq.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://qd.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ek.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wz.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bl.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://bz.521024.cn

[E04] 查找子串位置
来源：http://sd.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://jt.colortex.cn

PHP:  strpos($s, "x");
来源：http://wf.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sw.huanxung.cn

TS:   s.indexOf("x")
来源：http://qw.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ko.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://nu.haigaiapp.cn

Ruby: s.index("x")
来源：http://zf.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://yr.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tf.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ju.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://se.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gb.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rb.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uc.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://af.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mn.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oo.hahajie.cn

[E06] 替换子串
来源：http://jf.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ex.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://ph.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xx.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://mk.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://da.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bc.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sy.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://jk.hahajie.cn

[E07] 按分隔符拆分
来源：http://up.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dd.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mm.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ei.hnjuh.cn

TS:   s.split(",")
来源：http://sp.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hf.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://om.panjiajie.cn


<!-- 参考信息 -->