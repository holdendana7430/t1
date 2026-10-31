代发 wailian999

PHP:  // 无重载
来源：http://uh.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xi.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://pl.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xh.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://am.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://ye.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vd.haigaiapp.cn

================================================================================
来源：http://zh.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://rj.jianghongdianzi.cn

================================================================================
来源：http://mv.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://zt.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qd.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rp.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kp.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xf.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rr.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://gh.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://hf.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dt.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ef.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sx.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jf.chemitech.net.cn

JS:   arr.push(4);
来源：http://yr.shxzukj.cn

TS:   arr.push(4);
来源：http://iz.panjiajie.cn

Java: list.add(4);
来源：http://tr.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://wj.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://nz.jctech888.com.cn

C#:   list.Add(4);
来源：http://tr.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://pk.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://vo.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dp.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uj.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://xj.hahajie.cn

Java: list.add(0, 0);
来源：http://fp.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dh.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pl.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://hv.szsharing.cn

[D04] 删除元素
来源：http://ed.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qs.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ps.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mr.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://lm.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ur.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gc.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://at.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qc.haigaiapp.cn

[D05] 访问与修改元素
来源：http://bw.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ez.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jj.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kz.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://mo.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://po.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://hc.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bb.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mi.521024.cn

[D06] 数组长度
来源：http://qy.huanxung.cn

Py:   len(arr)
来源：http://uo.newstarts.cn

PHP:  count($arr);
来源：http://uj.jctech888.com.cn

JS:   arr.length
来源：http://cw.muxihuayi.cn

TS:   arr.length
来源：http://rw.haigaiapp.cn

Java: list.size();
来源：http://lb.shxzukj.cn

Go:   len(arr)
来源：http://aq.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://lw.bookmarksfly.cn

C#:   list.Count;
来源：http://cj.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://tc.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qi.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wa.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://cb.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://pd.shxzukj.cn

Java: list.subList(1, 4);
来源：http://aw.9csxet.cn

Go:   arr[1:4]
来源：http://gb.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://qt.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://wd.bjjhwx.cn

[D08] 合并两个数组
来源：http://bl.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://te.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://id.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cu.9csxet.cn

TS:   [...a, ...b];
来源：http://ua.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sv.9csxet.cn

Go:   append(a, b...)
来源：http://gq.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://fl.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://rv.lnxyls.cn

[D09] 排序（升序）
来源：http://ja.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://sn.yuexingan06.cn

PHP:  sort($arr);
来源：http://zn.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pa.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gn.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dw.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tu.shxzukj.cn

Ruby: arr.sort
来源：http://zm.shtwfgs.cn

C#:   list.Sort();
来源：http://mi.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ub.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pv.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wr.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ov.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lg.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vw.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rz.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://he.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mi.huixiangedu.cn

[D11] 反转数组
来源：http://fo.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vr.colortex.cn

PHP:  array_reverse($arr);
来源：http://ib.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qb.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://me.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://th.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://lp.chemitech.net.cn

Ruby: arr.reverse
来源：http://qh.haigaiapp.cn

C#:   list.Reverse();
来源：http://ux.gzmigu.cn

[D12] 查找元素下标
来源：http://vo.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://od.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nk.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rs.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nt.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sc.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://kk.gzmigu.cn

Ruby: arr.index(x)
来源：http://ym.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://rt.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://bi.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lc.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nu.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://ci.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://wo.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ql.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fx.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fz.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ae.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://wn.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hj.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qm.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://zb.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://il.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mz.shxzukj.cn

Go:   // 手写循环
来源：http://ui.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ls.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xw.haigaiapp.cn

[D15] 去重
来源：http://do.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ns.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://xf.521024.cn

JS:   [...new Set(arr)]
来源：http://tk.colortex.cn

TS:   [...new Set(arr)]
来源：http://nk.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pp.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ty.jctech888.com.cn

Ruby: arr.uniq
来源：http://pg.asd995.cn

C#:   list.Distinct().ToList()
来源：http://cp.szsharing.cn

[D16] 求和与平均值
来源：http://oq.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://be.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ol.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ac.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cr.9csxet.cn

Go:   // 手写循环累加
来源：http://xr.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mm.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://jd.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://vv.asd995.cn

Py:   max(arr);  min(arr)
来源：http://lr.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://gd.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iz.lnxyls.cn

TS:   Math.max(...arr);
来源：http://yq.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xi.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ss.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://xy.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://yk.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://xw.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xs.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://mv.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gk.shxzukj.cn

TS:   nested.flat();
来源：http://qx.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xw.asd995.cn

Go:   // 手写双层循环
来源：http://kp.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://dy.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yc.nszjky.cn

[D19] 按字段分组
来源：http://ic.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bu.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zz.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gx.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vp.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dd.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://qi.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://py.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tf.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://bi.bookmarksfly.cn

Py:   Counter(arr)
来源：http://uq.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://kr.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mf.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tm.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wp.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://nu.huixinmuqiang.cn

Ruby: arr.tally
来源：http://kl.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qu.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://oe.colortex.cn

Py:   x in arr
来源：http://me.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://lq.521024.cn

JS:   arr.includes(x)
来源：http://jg.shxzukj.cn

TS:   arr.includes(x)
来源：http://wy.bookmarksfly.cn

Java: list.contains(x)
来源：http://yn.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://fo.nicolike.cn

Ruby: arr.include?(x)
来源：http://tn.nszjky.cn

C#:   list.Contains(x)
来源：http://lw.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://nz.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pe.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nn.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xj.bjjhwx.cn

TS:   [...arr];
来源：http://pj.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://iq.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cm.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://it.chemitech.net.cn

C#:   new List<int>(list);
来源：http://ei.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://cl.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gu.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ft.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rt.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sl.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://te.9csxet.cn

Go:   // 手写循环
来源：http://mp.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xm.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://le.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://yc.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://er.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://up.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ze.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hm.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ad.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zd.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tt.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pg.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://dv.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ye.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mb.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qz.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qu.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xf.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zr.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hc.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qf.huanxung.cn

[D26] 数组转字符串
来源：http://tx.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://ei.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://uk.shxzskj.cn

JS:   arr.join(", ")
来源：http://sh.shxzukj.cn

TS:   arr.join(", ")
来源：http://hy.521024.cn

Java: String.join(", ", list)
来源：http://ft.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://ua.nszjky.cn

Ruby: arr.join(", ")
来源：http://ud.521024.cn

C#:   string.Join(", ", list)
来源：http://qh.bjjhwx.cn

================================================================================
来源：http://zl.lnxyls.cn

E. 字符串处理
来源：http://ba.asd995.cn

================================================================================
来源：http://ey.asd995.cn

[E01] 拼接字符串
来源：http://jf.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xk.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zg.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gl.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vo.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cd.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mr.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bf.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tj.shxzukj.cn

[E02] 重复字符串
来源：http://pb.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://so.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://gi.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://kp.asd995.cn

TS:   "ab".repeat(3)
来源：http://ut.shxzskj.cn

Java: "ab".repeat(3)
来源：http://hh.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://zg.huanxung.cn

Ruby: "ab" * 3
来源：http://cu.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dc.hahajie.cn

[E03] 截取子串
来源：http://ra.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xo.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xc.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pm.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://kh.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://gu.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qw.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zo.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://rc.nicolike.cn

[E04] 查找子串位置
来源：http://ax.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://bf.nicolike.cn

PHP:  strpos($s, "x");
来源：http://xy.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ok.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://oc.colortex.cn

Java: s.indexOf("x")
来源：http://er.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://pm.jctech888.com.cn

Ruby: s.index("x")
来源：http://fv.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://kw.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ku.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gr.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pz.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cq.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kg.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sm.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bq.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sy.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nm.newstarts.cn

[E06] 替换子串
来源：http://dx.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://od.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://gp.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jp.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://co.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kl.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zh.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yr.hahajie.cn


<!-- 参考信息 -->