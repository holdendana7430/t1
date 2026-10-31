代发 wailian999

PHP:  // 无重载
来源：http://zu.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yt.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://yu.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jd.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://nc.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://ou.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sp.huixiangedu.cn

================================================================================
来源：http://ik.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://kr.asd995.cn

================================================================================
来源：http://mg.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://wj.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://do.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bn.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jp.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qk.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ta.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://lz.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://zi.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oh.szsharing.cn

[D02] 追加元素到末尾
来源：http://fu.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xr.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cm.szxytkj.cn

JS:   arr.push(4);
来源：http://pc.shtwfgs.cn

TS:   arr.push(4);
来源：http://rh.huixiangedu.cn

Java: list.add(4);
来源：http://ga.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://ht.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://ok.szxytkj.cn

C#:   list.Add(4);
来源：http://mp.nicolike.cn

[D03] 在指定位置插入元素
来源：http://lp.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://yn.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xy.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xd.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://fn.wgjwhj.cn

Java: list.add(0, 0);
来源：http://fo.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gq.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://md.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://lv.hnjuh.cn

[D04] 删除元素
来源：http://nd.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zp.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://om.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jg.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://vh.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mw.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gh.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://df.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sa.haigaiapp.cn

[D05] 访问与修改元素
来源：http://bx.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fa.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lb.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rm.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://lz.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://nd.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://tt.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wb.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hf.haigaiapp.cn

[D06] 数组长度
来源：http://ux.huixiangedu.cn

Py:   len(arr)
来源：http://cn.huanxung.cn

PHP:  count($arr);
来源：http://jh.nicolike.cn

JS:   arr.length
来源：http://sl.huanxung.cn

TS:   arr.length
来源：http://ii.newstarts.cn

Java: list.size();
来源：http://ip.shxzukj.cn

Go:   len(arr)
来源：http://pm.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://jc.colortex.cn

C#:   list.Count;
来源：http://in.521024.cn

[D07] 切片 / 取子数组
来源：http://gh.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qm.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zd.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://et.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://af.szxytkj.cn

Java: list.subList(1, 4);
来源：http://dp.chemitech.net.cn

Go:   arr[1:4]
来源：http://kx.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://pq.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://hc.shxzskj.cn

[D08] 合并两个数组
来源：http://ha.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://jt.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://iz.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bb.muxihuayi.cn

TS:   [...a, ...b];
来源：http://cm.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cs.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://nz.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://jr.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://up.521024.cn

[D09] 排序（升序）
来源：http://dr.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ye.9csxet.cn

PHP:  sort($arr);
来源：http://jb.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://js.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mw.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dq.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://th.yuexingan06.cn

Ruby: arr.sort
来源：http://zm.bjjhwx.cn

C#:   list.Sort();
来源：http://cn.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ht.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wp.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ox.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tw.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pn.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gm.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oj.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ss.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ny.nicolike.cn

[D11] 反转数组
来源：http://ye.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ax.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://hr.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xx.9csxet.cn

TS:   [...arr].reverse();
来源：http://wi.hahajie.cn

Java: Collections.reverse(list);
来源：http://zp.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://pb.asd995.cn

Ruby: arr.reverse
来源：http://fu.shxzukj.cn

C#:   list.Reverse();
来源：http://ht.panjiajie.cn

[D12] 查找元素下标
来源：http://ch.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://of.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sf.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hk.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ed.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qf.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://ip.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://pr.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://zk.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://vg.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wu.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ie.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://uz.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://pg.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ev.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tf.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qt.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wq.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://hh.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qu.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ps.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://nd.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://uh.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uy.huixiangedu.cn

Go:   // 手写循环
来源：http://px.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dt.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dq.shxzukj.cn

[D15] 去重
来源：http://kn.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yp.shxzukj.cn

PHP:  array_unique($arr);
来源：http://uu.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://rj.szsharing.cn

TS:   [...new Set(arr)]
来源：http://or.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rb.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sl.muxihuayi.cn

Ruby: arr.uniq
来源：http://sg.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://wy.hnjuh.cn

[D16] 求和与平均值
来源：http://it.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ih.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cb.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ck.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://og.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bp.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://dg.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kp.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://mu.9csxet.cn

[D17] 最大值与最小值
来源：http://zk.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://wf.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://yj.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kh.lnxyls.cn

TS:   Math.max(...arr);
来源：http://ic.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aq.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jz.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://qy.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ul.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://nr.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sw.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://zl.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hm.hnjuh.cn

TS:   nested.flat();
来源：http://ud.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://np.nszjky.cn

Go:   // 手写双层循环
来源：http://us.muxihuayi.cn

Ruby: nested.flatten
来源：http://pe.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oe.yuntaijiaju.cn

[D19] 按字段分组
来源：http://lo.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wn.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://du.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bs.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vs.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cf.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://xi.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vz.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fw.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://wy.colortex.cn

Py:   Counter(arr)
来源：http://et.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://yi.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://os.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ez.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yz.hahajie.cn

Go:   // 手写 map[T]int
来源：http://wk.jctech888.com.cn

Ruby: arr.tally
来源：http://tw.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nd.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://qe.hnjuh.cn

Py:   x in arr
来源：http://pb.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://nr.newstarts.cn

JS:   arr.includes(x)
来源：http://xe.jctech888.com.cn

TS:   arr.includes(x)
来源：http://bv.jctech888.com.cn

Java: list.contains(x)
来源：http://tn.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://ha.hnjuh.cn

Ruby: arr.include?(x)
来源：http://ul.haigaiapp.cn

C#:   list.Contains(x)
来源：http://fp.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://rk.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ld.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ro.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vs.nicolike.cn

TS:   [...arr];
来源：http://jz.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://hg.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://na.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://qu.newstarts.cn

C#:   new List<int>(list);
来源：http://tb.9csxet.cn

[D23] reduce 累积计算
来源：http://vh.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gn.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tf.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bf.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xg.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ol.yuntaijiaju.cn

Go:   // 手写循环
来源：http://pn.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vd.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ax.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://np.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jd.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zi.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fe.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://of.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xs.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jr.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dd.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uc.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://hs.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hm.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gd.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jd.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://in.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ed.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sg.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gj.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xm.shtwfgs.cn

[D26] 数组转字符串
来源：http://gc.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://kp.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://gu.bjjhwx.cn

JS:   arr.join(", ")
来源：http://md.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://yj.chemitech.net.cn

Java: String.join(", ", list)
来源：http://eb.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://vl.nszjky.cn

Ruby: arr.join(", ")
来源：http://zz.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://qj.shtwfgs.cn

================================================================================
来源：http://tr.lnxyls.cn

E. 字符串处理
来源：http://zc.521024.cn

================================================================================
来源：http://vf.colortex.cn

[E01] 拼接字符串
来源：http://af.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ed.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tk.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rt.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iv.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ch.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kt.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ub.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mv.chemitech.net.cn

[E02] 重复字符串
来源：http://bm.newstarts.cn

Py:   "ab" * 3
来源：http://xn.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://so.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://qp.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://ha.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://ld.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://ri.shxzskj.cn

Ruby: "ab" * 3
来源：http://da.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zp.shxzskj.cn

[E03] 截取子串
来源：http://tb.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://em.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zb.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://va.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://nv.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://sq.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ug.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qg.asd995.cn

C#:   s.Substring(1, 3)
来源：http://xc.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://ap.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://bn.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://fw.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zv.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://qx.huixiangedu.cn

Java: s.indexOf("x")
来源：http://og.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://wy.shxzukj.cn

Ruby: s.index("x")
来源：http://zr.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://oc.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jq.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wj.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ag.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mq.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ow.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bu.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://td.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qw.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zd.szsharing.cn

[E06] 替换子串
来源：http://lg.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://os.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://tc.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gy.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://qb.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ai.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tp.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uy.yuexingan06.cn


<!-- 参考信息 -->