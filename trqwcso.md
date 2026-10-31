代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://ca.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://pc.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hm.shxzukj.cn

================================================================================
来源：http://hy.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://sr.lnxyls.cn

================================================================================
来源：http://or.hahajie.cn

[D01] 创建数组 / 列表
来源：http://es.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lr.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ei.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gi.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sf.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hw.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://kf.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://ap.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://at.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://ph.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fm.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ry.nszjky.cn

JS:   arr.push(4);
来源：http://ma.bookmarksfly.cn

TS:   arr.push(4);
来源：http://yn.lnxyls.cn

Java: list.add(4);
来源：http://dc.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://xu.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://lp.chemitech.net.cn

C#:   list.Add(4);
来源：http://da.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://vv.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://ks.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vx.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ew.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://vv.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://ul.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tm.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rx.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://oe.muxihuayi.cn

[D04] 删除元素
来源：http://fw.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ml.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yi.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tv.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://be.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ly.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rc.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gc.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fl.szxytkj.cn

[D05] 访问与修改元素
来源：http://od.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://po.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wy.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yn.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://zq.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ad.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ku.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yq.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bh.wgjwhj.cn

[D06] 数组长度
来源：http://zo.nszjky.cn

Py:   len(arr)
来源：http://id.jctech888.com.cn

PHP:  count($arr);
来源：http://wo.huanxung.cn

JS:   arr.length
来源：http://mw.bookmarksfly.cn

TS:   arr.length
来源：http://si.nicolike.cn

Java: list.size();
来源：http://mg.nszjky.cn

Go:   len(arr)
来源：http://nt.nicolike.cn

Ruby: arr.length; arr.size
来源：http://dv.gzmigu.cn

C#:   list.Count;
来源：http://fa.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://py.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jy.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ux.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://er.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://wb.521024.cn

Java: list.subList(1, 4);
来源：http://yd.hnjuh.cn

Go:   arr[1:4]
来源：http://rg.521024.cn

Ruby: arr[1, 3]
来源：http://rp.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://qq.shxzskj.cn

[D08] 合并两个数组
来源：http://zi.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://xi.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://vm.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oz.jctech888.com.cn

TS:   [...a, ...b];
来源：http://ov.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dc.newstarts.cn

Go:   append(a, b...)
来源：http://lp.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://ah.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://fi.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://lq.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://qo.gzmigu.cn

PHP:  sort($arr);
来源：http://cd.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://er.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ac.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xv.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gg.nszjky.cn

Ruby: arr.sort
来源：http://zq.yuntaijiaju.cn

C#:   list.Sort();
来源：http://qm.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ql.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ch.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ru.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lb.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sp.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rz.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://as.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yb.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wb.asd995.cn

[D11] 反转数组
来源：http://vd.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zf.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://bb.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hq.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://vx.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://pb.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://xo.bookmarksfly.cn

Ruby: arr.reverse
来源：http://py.haigaiapp.cn

C#:   list.Reverse();
来源：http://al.bookmarksfly.cn

[D12] 查找元素下标
来源：http://os.521024.cn

Py:   arr.index(x);  x in arr
来源：http://eg.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jb.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uy.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ax.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://co.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://ps.9csxet.cn

Ruby: arr.index(x)
来源：http://ug.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://bq.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://yk.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ki.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ky.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://sd.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://yq.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rj.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gc.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gm.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sz.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://nb.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fu.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gw.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://xm.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://xl.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eu.shxzskj.cn

Go:   // 手写循环
来源：http://nb.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lh.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ng.jctech888.com.cn

[D15] 去重
来源：http://ck.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ni.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://zw.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://yv.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ss.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fx.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zq.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://uo.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://dc.hnjuh.cn

[D16] 求和与平均值
来源：http://rs.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tm.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bj.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yb.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ke.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pa.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://cs.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bb.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://gs.panjiajie.cn

[D17] 最大值与最小值
来源：http://qe.asd995.cn

Py:   max(arr);  min(arr)
来源：http://ve.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://ou.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bj.hahajie.cn

TS:   Math.max(...arr);
来源：http://ih.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uf.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tc.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://dg.colortex.cn

C#:   list.Max();  list.Min()
来源：http://lj.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://eq.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uy.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://af.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ss.muxihuayi.cn

TS:   nested.flat();
来源：http://ai.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lb.shtwfgs.cn

Go:   // 手写双层循环
来源：http://uz.muxihuayi.cn

Ruby: nested.flatten
来源：http://ci.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vb.panjiajie.cn

[D19] 按字段分组
来源：http://qc.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bu.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mw.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://td.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ec.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sj.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://vd.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vg.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lj.521024.cn

[D20] 统计每个元素出现次数
来源：http://po.newstarts.cn

Py:   Counter(arr)
来源：http://vz.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://sl.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://on.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iu.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tv.521024.cn

Go:   // 手写 map[T]int
来源：http://qw.chemitech.net.cn

Ruby: arr.tally
来源：http://bd.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://au.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://mw.nicolike.cn

Py:   x in arr
来源：http://wq.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://ox.bjjhwx.cn

JS:   arr.includes(x)
来源：http://oy.gzmigu.cn

TS:   arr.includes(x)
来源：http://kv.muxihuayi.cn

Java: list.contains(x)
来源：http://hb.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://qi.szsharing.cn

Ruby: arr.include?(x)
来源：http://jq.colortex.cn

C#:   list.Contains(x)
来源：http://up.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://ec.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://op.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uh.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://en.huanxung.cn

TS:   [...arr];
来源：http://je.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://yj.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ag.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://qo.colortex.cn

C#:   new List<int>(list);
来源：http://fn.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://qo.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zq.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qh.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bt.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ic.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sz.bookmarksfly.cn

Go:   // 手写循环
来源：http://yi.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vm.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tz.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://tx.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wo.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fi.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bf.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cd.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uh.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pn.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nh.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dt.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://gn.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rc.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wn.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cr.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ai.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hx.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cx.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://op.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lz.wgjwhj.cn

[D26] 数组转字符串
来源：http://lh.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://vt.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://ji.hnjuh.cn

JS:   arr.join(", ")
来源：http://ij.bjjhwx.cn

TS:   arr.join(", ")
来源：http://yd.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://wa.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://cp.yuexingan06.cn

Ruby: arr.join(", ")
来源：http://pi.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://qa.shxzskj.cn

================================================================================
来源：http://nt.muxihuayi.cn

E. 字符串处理
来源：http://hl.bjjhwx.cn

================================================================================
来源：http://qx.panjiajie.cn

[E01] 拼接字符串
来源：http://ye.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tb.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xk.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lz.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://st.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cq.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xu.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ch.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://km.nszjky.cn

[E02] 重复字符串
来源：http://uc.nicolike.cn

Py:   "ab" * 3
来源：http://vi.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://lt.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://cn.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://my.szxytkj.cn

Java: "ab".repeat(3)
来源：http://vc.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://wd.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://ct.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oo.huanxung.cn

[E03] 截取子串
来源：http://nz.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qo.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mi.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ww.huanxung.cn

TS:   s.slice(1, 4)
来源：http://yr.nszjky.cn

Java: s.substring(1, 4)
来源：http://ux.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ne.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wo.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://wv.szxytkj.cn

[E04] 查找子串位置
来源：http://qo.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://yn.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ub.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://su.huanxung.cn

TS:   s.indexOf("x")
来源：http://kx.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://nq.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://la.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://vg.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://wm.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ke.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gd.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bb.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rg.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rv.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gc.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lk.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://en.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oo.521024.cn

[E06] 替换子串
来源：http://xs.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sr.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://lk.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ek.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://pj.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jh.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qx.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tr.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://bs.nszjky.cn

[E07] 按分隔符拆分
来源：http://vk.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bj.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yo.yuexingan06.cn


<!-- 参考信息 -->