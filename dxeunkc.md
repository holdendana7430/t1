代发 wailian999

PHP:  // 无重载
来源：http://jr.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ao.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://rp.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yy.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://to.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://qv.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://iz.wgjwhj.cn

================================================================================
来源：http://fn.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://nl.bjjhwx.cn

================================================================================
来源：http://vg.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://vf.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cp.huixiangedu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yg.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sc.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ck.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bb.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://zn.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://pa.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mt.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://dp.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://an.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://go.hnjuh.cn

JS:   arr.push(4);
来源：http://kq.shtwfgs.cn

TS:   arr.push(4);
来源：http://ms.jianghongdianzi.cn

Java: list.add(4);
来源：http://va.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://pa.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://hy.nicolike.cn

C#:   list.Add(4);
来源：http://rl.huanxung.cn

[D03] 在指定位置插入元素
来源：http://jl.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://bs.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ff.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ag.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://jb.haigaiapp.cn

Java: list.add(0, 0);
来源：http://bh.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pc.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qy.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://hl.nicolike.cn

[D04] 删除元素
来源：http://qd.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dm.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://al.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jo.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://cm.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lq.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ic.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iu.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uh.shxzukj.cn

[D05] 访问与修改元素
来源：http://ts.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lt.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tw.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yn.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://jk.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://ni.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://rk.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xm.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tj.hahajie.cn

[D06] 数组长度
来源：http://fp.colortex.cn

Py:   len(arr)
来源：http://jf.yuexingan06.cn

PHP:  count($arr);
来源：http://cm.asd995.cn

JS:   arr.length
来源：http://tb.hahajie.cn

TS:   arr.length
来源：http://ga.chemitech.net.cn

Java: list.size();
来源：http://ww.gzmigu.cn

Go:   len(arr)
来源：http://xt.hahajie.cn

Ruby: arr.length; arr.size
来源：http://dz.gzmigu.cn

C#:   list.Count;
来源：http://rf.asd995.cn

[D07] 切片 / 取子数组
来源：http://ir.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xj.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fa.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://xn.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://cm.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://rc.szxytkj.cn

Go:   arr[1:4]
来源：http://kn.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://ng.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://ly.szxytkj.cn

[D08] 合并两个数组
来源：http://lg.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://el.521024.cn

PHP:  array_merge($a, $b);
来源：http://xy.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pq.huanxung.cn

TS:   [...a, ...b];
来源：http://vl.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wk.panjiajie.cn

Go:   append(a, b...)
来源：http://wr.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://ar.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://hm.shtwfgs.cn

[D09] 排序（升序）
来源：http://gt.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://hj.szsharing.cn

PHP:  sort($arr);
来源：http://zm.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xc.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sw.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yd.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ir.yuexingan06.cn

Ruby: arr.sort
来源：http://gq.nicolike.cn

C#:   list.Sort();
来源：http://yr.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sv.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://er.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cr.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gk.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xw.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://li.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wd.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oe.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fm.szxytkj.cn

[D11] 反转数组
来源：http://zg.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mg.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://ix.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jr.colortex.cn

TS:   [...arr].reverse();
来源：http://bi.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://bw.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://up.chemitech.net.cn

Ruby: arr.reverse
来源：http://wd.yuexingan06.cn

C#:   list.Reverse();
来源：http://oe.colortex.cn

[D12] 查找元素下标
来源：http://cp.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://li.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wy.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mg.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wv.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jj.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://po.muxihuayi.cn

Ruby: arr.index(x)
来源：http://eg.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://yq.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://ej.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qk.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ps.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://ty.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://vd.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uh.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wq.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vf.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rc.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://jd.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lr.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hj.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://fc.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://ey.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xr.huanxung.cn

Go:   // 手写循环
来源：http://rt.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ta.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://po.huixinmuqiang.cn

[D15] 去重
来源：http://zn.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ky.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://pf.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://gw.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://mx.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rg.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jm.haigaiapp.cn

Ruby: arr.uniq
来源：http://rk.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://gg.panjiajie.cn

[D16] 求和与平均值
来源：http://vt.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xs.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uu.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://te.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qp.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cu.muxihuayi.cn

Go:   // 手写循环累加
来源：http://jd.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ih.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://dz.shxzskj.cn

[D17] 最大值与最小值
来源：http://om.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://uw.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://jp.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tl.huanxung.cn

TS:   Math.max(...arr);
来源：http://vv.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mt.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fa.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://cy.521024.cn

C#:   list.Max();  list.Min()
来源：http://od.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://qu.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hd.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://xn.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jk.hahajie.cn

TS:   nested.flat();
来源：http://bv.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ow.haigaiapp.cn

Go:   // 手写双层循环
来源：http://aw.shxzskj.cn

Ruby: nested.flatten
来源：http://vg.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://na.bjjhwx.cn

[D19] 按字段分组
来源：http://hl.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xy.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eh.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hh.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://im.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eo.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://at.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nq.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nj.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://fi.szxytkj.cn

Py:   Counter(arr)
来源：http://jt.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://vg.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ay.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yq.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mt.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://vz.nszjky.cn

Ruby: arr.tally
来源：http://ud.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xs.521024.cn

[D21] 判断是否包含某元素
来源：http://dn.colortex.cn

Py:   x in arr
来源：http://nd.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://xv.yuexingan06.cn

JS:   arr.includes(x)
来源：http://rb.asd995.cn

TS:   arr.includes(x)
来源：http://kq.hnjuh.cn

Java: list.contains(x)
来源：http://go.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://fn.nszjky.cn

Ruby: arr.include?(x)
来源：http://oo.hahajie.cn

C#:   list.Contains(x)
来源：http://qw.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://wj.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nu.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ju.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://el.hahajie.cn

TS:   [...arr];
来源：http://ag.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://uq.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ei.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://kk.huixiangedu.cn

C#:   new List<int>(list);
来源：http://ty.nicolike.cn

[D23] reduce 累积计算
来源：http://kb.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qs.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zy.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cf.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ja.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cc.lnxyls.cn

Go:   // 手写循环
来源：http://kc.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cs.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qr.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://kc.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://su.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xj.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ga.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nq.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pb.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sv.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eo.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cm.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://ly.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jl.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zw.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ri.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bx.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uf.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wh.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zt.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ga.szxytkj.cn

[D26] 数组转字符串
来源：http://nj.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://bf.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://lb.521024.cn

JS:   arr.join(", ")
来源：http://ft.yuexingan06.cn

TS:   arr.join(", ")
来源：http://xw.colortex.cn

Java: String.join(", ", list)
来源：http://fa.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://bk.lnxyls.cn

Ruby: arr.join(", ")
来源：http://vx.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://qy.hahajie.cn

================================================================================
来源：http://fq.huixinmuqiang.cn

E. 字符串处理
来源：http://kk.lnxyls.cn

================================================================================
来源：http://fd.hahajie.cn

[E01] 拼接字符串
来源：http://xj.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dw.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lf.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hv.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kf.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gj.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ty.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vg.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uu.haigaiapp.cn

[E02] 重复字符串
来源：http://wi.shxzskj.cn

Py:   "ab" * 3
来源：http://qn.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://ny.huanxung.cn

JS:   "ab".repeat(3)
来源：http://jt.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://hg.521024.cn

Java: "ab".repeat(3)
来源：http://fy.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://rl.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://ha.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rw.shxzskj.cn

[E03] 截取子串
来源：http://ww.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vi.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yb.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gl.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ej.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ou.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vh.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gl.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://xc.shxzskj.cn

[E04] 查找子串位置
来源：http://zq.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://cj.newstarts.cn

PHP:  strpos($s, "x");
来源：http://bc.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ab.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://pl.shxzukj.cn

Java: s.indexOf("x")
来源：http://mo.colortex.cn

Go:   strings.Index(s, "x")
来源：http://uy.shtwfgs.cn

Ruby: s.index("x")
来源：http://bc.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://wr.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ok.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wp.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ng.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qy.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://np.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zj.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vi.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sh.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bb.nicolike.cn

[E06] 替换子串
来源：http://qu.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ha.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://fy.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jx.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://fh.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://au.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ot.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lx.haigaiapp.cn


<!-- 参考信息 -->