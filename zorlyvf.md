代发 wailian999

PHP:  // 无重载
来源：http://nt.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fh.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://rk.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zs.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://ez.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://zf.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sd.szsharing.cn

================================================================================
来源：http://ld.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://bo.chemitech.net.cn

================================================================================
来源：http://yz.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://ku.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ps.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qw.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pi.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oe.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tr.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://vd.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://ha.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://um.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://fb.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hq.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lr.szsharing.cn

JS:   arr.push(4);
来源：http://kp.colortex.cn

TS:   arr.push(4);
来源：http://qe.panjiajie.cn

Java: list.add(4);
来源：http://au.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://mx.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://gv.521024.cn

C#:   list.Add(4);
来源：http://jm.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://tf.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ld.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cw.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uy.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://bg.hahajie.cn

Java: list.add(0, 0);
来源：http://cg.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rj.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tr.521024.cn

C#:   list.Insert(0, 0);
来源：http://zz.yuexingan06.cn

[D04] 删除元素
来源：http://kf.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pp.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xx.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jx.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://tf.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jd.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vf.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://um.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://it.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://yx.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vm.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ln.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jq.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://jg.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://dx.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://aa.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dp.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hx.lnxyls.cn

[D06] 数组长度
来源：http://am.szxytkj.cn

Py:   len(arr)
来源：http://md.huanxung.cn

PHP:  count($arr);
来源：http://pn.hahajie.cn

JS:   arr.length
来源：http://wd.shtwfgs.cn

TS:   arr.length
来源：http://ej.wgjwhj.cn

Java: list.size();
来源：http://gf.gzmigu.cn

Go:   len(arr)
来源：http://aj.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://zp.bookmarksfly.cn

C#:   list.Count;
来源：http://xn.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://wq.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kk.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gv.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://vs.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://lw.colortex.cn

Java: list.subList(1, 4);
来源：http://yx.chemitech.net.cn

Go:   arr[1:4]
来源：http://te.521024.cn

Ruby: arr[1, 3]
来源：http://qw.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://jy.szsharing.cn

[D08] 合并两个数组
来源：http://je.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://cl.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://ql.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wb.bjjhwx.cn

TS:   [...a, ...b];
来源：http://sy.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uq.shtwfgs.cn

Go:   append(a, b...)
来源：http://rk.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://cx.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://dk.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://kb.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://wy.chemitech.net.cn

PHP:  sort($arr);
来源：http://sb.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tp.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://is.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fk.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ll.panjiajie.cn

Ruby: arr.sort
来源：http://la.jianghongdianzi.cn

C#:   list.Sort();
来源：http://fe.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vv.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dz.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ot.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yb.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nt.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://js.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ar.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vv.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zz.szsharing.cn

[D11] 反转数组
来源：http://ys.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bs.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://xs.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ml.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://fc.hnjuh.cn

Java: Collections.reverse(list);
来源：http://bl.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://qx.gzmigu.cn

Ruby: arr.reverse
来源：http://ae.gzmigu.cn

C#:   list.Reverse();
来源：http://ee.huixiangedu.cn

[D12] 查找元素下标
来源：http://if.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://bl.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kg.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rh.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cr.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ux.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://hk.panjiajie.cn

Ruby: arr.index(x)
来源：http://ep.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://fx.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://fq.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fg.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ky.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://qf.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://rg.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rh.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qz.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fy.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ro.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://ef.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dv.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xi.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://yc.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://bs.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sn.szsharing.cn

Go:   // 手写循环
来源：http://is.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pa.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cg.jianghongdianzi.cn

[D15] 去重
来源：http://td.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lo.szsharing.cn

PHP:  array_unique($arr);
来源：http://qn.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://xd.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://ih.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sn.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ha.gzmigu.cn

Ruby: arr.uniq
来源：http://qx.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://zp.muxihuayi.cn

[D16] 求和与平均值
来源：http://ci.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hh.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ch.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ki.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fa.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ly.shxzukj.cn

Go:   // 手写循环累加
来源：http://pd.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ay.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://fe.jctech888.com.cn

[D17] 最大值与最小值
来源：http://jf.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://sa.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://aj.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pj.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://mi.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mp.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vd.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://zt.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://pj.asd995.cn

[D18] 扁平化嵌套数组
来源：http://xd.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tw.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://za.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ac.huixiangedu.cn

TS:   nested.flat();
来源：http://su.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kg.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://hy.chemitech.net.cn

Ruby: nested.flatten
来源：http://da.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ly.hnjuh.cn

[D19] 按字段分组
来源：http://pd.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://db.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mw.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fl.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yi.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://su.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://yi.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ap.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cy.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://nr.9csxet.cn

Py:   Counter(arr)
来源：http://xx.hahajie.cn

PHP:  array_count_values($arr);
来源：http://rj.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wy.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jj.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hj.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://fj.9csxet.cn

Ruby: arr.tally
来源：http://xm.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hh.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://ni.hahajie.cn

Py:   x in arr
来源：http://oq.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://cn.haigaiapp.cn

JS:   arr.includes(x)
来源：http://jj.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://mu.bookmarksfly.cn

Java: list.contains(x)
来源：http://ek.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://oj.panjiajie.cn

Ruby: arr.include?(x)
来源：http://mi.chemitech.net.cn

C#:   list.Contains(x)
来源：http://an.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://sl.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qo.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ud.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lg.huixinmuqiang.cn

TS:   [...arr];
来源：http://da.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://fc.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://my.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://mt.muxihuayi.cn

C#:   new List<int>(list);
来源：http://ai.haigaiapp.cn

[D23] reduce 累积计算
来源：http://bx.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ds.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pl.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ic.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rh.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dg.jctech888.com.cn

Go:   // 手写循环
来源：http://aw.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uy.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oc.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://fb.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yc.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kn.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qv.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fv.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://he.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nq.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://la.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zd.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://rp.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kt.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ov.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://du.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ya.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hq.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iv.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kl.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zq.huanxung.cn

[D26] 数组转字符串
来源：http://fo.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://rd.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://ce.wgjwhj.cn

JS:   arr.join(", ")
来源：http://ak.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://rx.haigaiapp.cn

Java: String.join(", ", list)
来源：http://pt.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://xe.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://oo.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://yr.521024.cn

================================================================================
来源：http://ui.colortex.cn

E. 字符串处理
来源：http://hh.bookmarksfly.cn

================================================================================
来源：http://xd.9csxet.cn

[E01] 拼接字符串
来源：http://go.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ho.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ng.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bn.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://us.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://td.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kf.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ig.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uk.gzmigu.cn

[E02] 重复字符串
来源：http://zj.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://id.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://ju.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://as.asd995.cn

TS:   "ab".repeat(3)
来源：http://zv.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://wl.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://mj.lnxyls.cn

Ruby: "ab" * 3
来源：http://it.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ud.haigaiapp.cn

[E03] 截取子串
来源：http://hf.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qy.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pw.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ey.asd995.cn

TS:   s.slice(1, 4)
来源：http://zp.shxzskj.cn

Java: s.substring(1, 4)
来源：http://wc.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fc.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jw.asd995.cn

C#:   s.Substring(1, 3)
来源：http://ko.gzmigu.cn

[E04] 查找子串位置
来源：http://zj.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://at.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://lq.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yw.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://sg.szsharing.cn

Java: s.indexOf("x")
来源：http://pv.colortex.cn

Go:   strings.Index(s, "x")
来源：http://mn.shxzukj.cn

Ruby: s.index("x")
来源：http://im.szsharing.cn

C#:   s.IndexOf("x")
来源：http://ep.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://co.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jx.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://me.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ql.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://im.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qb.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jw.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fs.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gi.521024.cn

[E06] 替换子串
来源：http://vd.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gw.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ia.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jp.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://eu.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ry.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mc.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xl.panjiajie.cn


<!-- 参考信息 -->