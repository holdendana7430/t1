代发 wailian999

D. 数组 / 列表 / 集合
来源：http://uc.asd995.cn

================================================================================
来源：http://sl.hahajie.cn

[D01] 创建数组 / 列表
来源：http://df.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dx.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xb.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dw.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kc.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sc.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://mo.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://on.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uc.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://yh.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zb.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zd.huanxung.cn

JS:   arr.push(4);
来源：http://tm.huixiangedu.cn

TS:   arr.push(4);
来源：http://eo.lnxyls.cn

Java: list.add(4);
来源：http://yk.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://ar.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://rb.yuexingan06.cn

C#:   list.Add(4);
来源：http://nd.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://ul.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://yd.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gj.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gw.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://yu.shxzukj.cn

Java: list.add(0, 0);
来源：http://lm.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kg.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jp.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://rr.wgjwhj.cn

[D04] 删除元素
来源：http://om.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zr.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lg.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fy.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://wi.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://np.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xw.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vr.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ml.bjjhwx.cn

[D05] 访问与修改元素
来源：http://ch.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iw.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mq.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ui.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://hd.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://zg.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://pn.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qq.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zb.huixiangedu.cn

[D06] 数组长度
来源：http://wb.newstarts.cn

Py:   len(arr)
来源：http://vx.bookmarksfly.cn

PHP:  count($arr);
来源：http://ij.shxzukj.cn

JS:   arr.length
来源：http://vx.huixiangedu.cn

TS:   arr.length
来源：http://ai.bookmarksfly.cn

Java: list.size();
来源：http://yb.jctech888.com.cn

Go:   len(arr)
来源：http://cx.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://hy.nszjky.cn

C#:   list.Count;
来源：http://en.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://wc.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rr.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cg.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://fa.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://af.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://ju.shxzskj.cn

Go:   arr[1:4]
来源：http://gh.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://ef.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://rw.newstarts.cn

[D08] 合并两个数组
来源：http://fm.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://sr.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://yl.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://by.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://kg.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hu.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://yt.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://gp.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://eu.shxzskj.cn

[D09] 排序（升序）
来源：http://jt.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://xq.huixiangedu.cn

PHP:  sort($arr);
来源：http://el.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qq.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gu.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://je.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wo.bookmarksfly.cn

Ruby: arr.sort
来源：http://bp.panjiajie.cn

C#:   list.Sort();
来源：http://te.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qy.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://my.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://po.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jw.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qx.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pf.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://em.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dx.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bd.nszjky.cn

[D11] 反转数组
来源：http://fa.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bn.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://pm.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gf.colortex.cn

TS:   [...arr].reverse();
来源：http://io.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://po.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://xd.9csxet.cn

Ruby: arr.reverse
来源：http://ds.9csxet.cn

C#:   list.Reverse();
来源：http://yo.colortex.cn

[D12] 查找元素下标
来源：http://qt.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://wd.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yo.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ln.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://et.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cm.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://pu.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ee.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://bu.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://qj.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ec.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rb.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://yj.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://mz.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ni.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://do.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://us.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cz.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://tu.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gj.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ks.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://en.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://uj.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ub.panjiajie.cn

Go:   // 手写循环
来源：http://ow.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qr.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rv.newstarts.cn

[D15] 去重
来源：http://yy.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://be.lnxyls.cn

PHP:  array_unique($arr);
来源：http://as.newstarts.cn

JS:   [...new Set(arr)]
来源：http://zx.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://nl.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bw.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ih.bjjhwx.cn

Ruby: arr.uniq
来源：http://xy.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://wc.asd995.cn

[D16] 求和与平均值
来源：http://ta.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wj.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mv.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mb.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bd.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qz.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://pt.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fr.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ia.yuexingan06.cn

[D17] 最大值与最小值
来源：http://cf.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://kx.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://jk.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nc.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://eb.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lu.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yr.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://gi.colortex.cn

C#:   list.Max();  list.Min()
来源：http://lr.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://pb.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ud.521024.cn

PHP:  array_merge(...$nested);
来源：http://ym.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ru.yuexingan06.cn

TS:   nested.flat();
来源：http://on.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mx.hahajie.cn

Go:   // 手写双层循环
来源：http://fo.gzmigu.cn

Ruby: nested.flatten
来源：http://kn.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aq.bookmarksfly.cn

[D19] 按字段分组
来源：http://qf.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xc.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fq.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://er.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yl.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oj.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://qq.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://le.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lw.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://zq.szsharing.cn

Py:   Counter(arr)
来源：http://qh.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://bi.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://po.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xl.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ki.hahajie.cn

Go:   // 手写 map[T]int
来源：http://gs.shxzukj.cn

Ruby: arr.tally
来源：http://iu.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zz.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://mj.wgjwhj.cn

Py:   x in arr
来源：http://nt.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://ey.newstarts.cn

JS:   arr.includes(x)
来源：http://is.szxytkj.cn

TS:   arr.includes(x)
来源：http://mr.wgjwhj.cn

Java: list.contains(x)
来源：http://om.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://yq.521024.cn

Ruby: arr.include?(x)
来源：http://vk.colortex.cn

C#:   list.Contains(x)
来源：http://zu.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://wz.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kb.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ap.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cc.hahajie.cn

TS:   [...arr];
来源：http://ai.hahajie.cn

Java: new ArrayList<>(list);
来源：http://xr.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oy.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://pn.521024.cn

C#:   new List<int>(list);
来源：http://dp.nicolike.cn

[D23] reduce 累积计算
来源：http://ez.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yt.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sb.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cl.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qw.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qd.chemitech.net.cn

Go:   // 手写循环
来源：http://hb.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gx.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://he.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://zv.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uu.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kh.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ot.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://th.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uu.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vb.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ly.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ch.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://vu.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jd.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kx.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://er.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ca.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qc.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aw.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fi.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yv.wgjwhj.cn

[D26] 数组转字符串
来源：http://ry.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://wa.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://tt.hnjuh.cn

JS:   arr.join(", ")
来源：http://rf.9csxet.cn

TS:   arr.join(", ")
来源：http://ok.haigaiapp.cn

Java: String.join(", ", list)
来源：http://xr.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ma.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://jh.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://ec.521024.cn

================================================================================
来源：http://lb.huixinmuqiang.cn

E. 字符串处理
来源：http://wu.yuntaijiaju.cn

================================================================================
来源：http://sq.nicolike.cn

[E01] 拼接字符串
来源：http://ec.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iu.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zf.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kg.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kj.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vr.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nf.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sp.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://do.shtwfgs.cn

[E02] 重复字符串
来源：http://by.lnxyls.cn

Py:   "ab" * 3
来源：http://ls.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://mb.colortex.cn

JS:   "ab".repeat(3)
来源：http://bs.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://cu.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://rv.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ow.lnxyls.cn

Ruby: "ab" * 3
来源：http://bd.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rk.newstarts.cn

[E03] 截取子串
来源：http://kh.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pt.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rp.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kc.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://sl.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://ti.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lf.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ex.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://dl.shxzskj.cn

[E04] 查找子串位置
来源：http://xx.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://va.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://iu.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vr.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://uw.chemitech.net.cn

Java: s.indexOf("x")
来源：http://ht.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://ti.bookmarksfly.cn

Ruby: s.index("x")
来源：http://rn.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://jm.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wo.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xn.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qi.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nw.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ry.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://km.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dp.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hm.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wq.chemitech.net.cn

[E06] 替换子串
来源：http://gx.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ia.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://sk.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gc.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://ly.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://us.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vv.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ii.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://ov.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://fb.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ly.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ba.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://by.shxzskj.cn

TS:   s.split(",")
来源：http://hi.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tt.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lh.huixinmuqiang.cn


<!-- 参考信息 -->