代发 wailian999

PHP:  // 无重载
来源：http://yq.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mf.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://ik.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bw.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://gu.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://ny.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://de.bjjhwx.cn

================================================================================
来源：http://tb.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://we.hnjuh.cn

================================================================================
来源：http://wh.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://re.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nv.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qo.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cg.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bx.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ex.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://lu.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://xa.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iq.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://ym.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://do.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cv.shtwfgs.cn

JS:   arr.push(4);
来源：http://uy.colortex.cn

TS:   arr.push(4);
来源：http://yb.jctech888.com.cn

Java: list.add(4);
来源：http://mv.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://it.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://sp.chemitech.net.cn

C#:   list.Add(4);
来源：http://xm.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://fo.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://rq.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kj.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hj.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://wb.huixiangedu.cn

Java: list.add(0, 0);
来源：http://wi.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wa.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lw.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://qj.panjiajie.cn

[D04] 删除元素
来源：http://mg.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ka.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zn.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mz.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://jp.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://br.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wk.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ao.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fj.shxzskj.cn

[D05] 访问与修改元素
来源：http://ea.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ow.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iy.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yj.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://tu.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://bg.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://vl.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vo.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kn.nszjky.cn

[D06] 数组长度
来源：http://vd.shxzskj.cn

Py:   len(arr)
来源：http://gq.yuexingan06.cn

PHP:  count($arr);
来源：http://jd.gzmigu.cn

JS:   arr.length
来源：http://vh.szsharing.cn

TS:   arr.length
来源：http://dz.9csxet.cn

Java: list.size();
来源：http://gt.chemitech.net.cn

Go:   len(arr)
来源：http://jg.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://xz.521024.cn

C#:   list.Count;
来源：http://nr.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://ph.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gc.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kr.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://kd.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://nx.nicolike.cn

Java: list.subList(1, 4);
来源：http://qn.szsharing.cn

Go:   arr[1:4]
来源：http://vk.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://mv.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://wt.colortex.cn

[D08] 合并两个数组
来源：http://ce.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://bi.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://do.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zr.szsharing.cn

TS:   [...a, ...b];
来源：http://nh.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tt.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://cw.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://ox.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://ni.panjiajie.cn

[D09] 排序（升序）
来源：http://gy.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://nf.panjiajie.cn

PHP:  sort($arr);
来源：http://hu.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qo.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qp.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://al.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nl.bjjhwx.cn

Ruby: arr.sort
来源：http://lf.nszjky.cn

C#:   list.Sort();
来源：http://uu.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qx.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://en.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vk.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://is.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://od.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cu.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ma.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ug.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://md.lnxyls.cn

[D11] 反转数组
来源：http://bl.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ng.szsharing.cn

PHP:  array_reverse($arr);
来源：http://cc.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cj.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://eh.shxzskj.cn

Java: Collections.reverse(list);
来源：http://hy.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://ct.521024.cn

Ruby: arr.reverse
来源：http://jb.nicolike.cn

C#:   list.Reverse();
来源：http://yv.shxzskj.cn

[D12] 查找元素下标
来源：http://pa.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://pt.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pb.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lf.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hb.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hw.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://gk.asd995.cn

Ruby: arr.index(x)
来源：http://ex.521024.cn

C#:   list.IndexOf(x);
来源：http://cz.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://pm.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ys.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vd.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://gh.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://ey.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dg.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nt.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ks.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nx.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://aj.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hk.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jz.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://tr.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://eo.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ve.huixinmuqiang.cn

Go:   // 手写循环
来源：http://bq.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tu.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ku.9csxet.cn

[D15] 去重
来源：http://yp.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pn.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://qz.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://aq.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://rf.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://of.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jp.gzmigu.cn

Ruby: arr.uniq
来源：http://uv.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://vj.szsharing.cn

[D16] 求和与平均值
来源：http://ei.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sl.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xm.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pe.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sw.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bc.521024.cn

Go:   // 手写循环累加
来源：http://tj.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://is.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://hd.bjjhwx.cn

[D17] 最大值与最小值
来源：http://vu.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://vv.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://jv.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ap.9csxet.cn

TS:   Math.max(...arr);
来源：http://qh.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mc.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ym.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://jt.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://rx.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://ng.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fo.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://xz.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ky.lnxyls.cn

TS:   nested.flat();
来源：http://pe.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jw.yuexingan06.cn

Go:   // 手写双层循环
来源：http://rx.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://dv.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qm.bjjhwx.cn

[D19] 按字段分组
来源：http://jj.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jp.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ee.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zn.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jf.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://il.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://up.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rb.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zy.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://cw.bjjhwx.cn

Py:   Counter(arr)
来源：http://uv.huanxung.cn

PHP:  array_count_values($arr);
来源：http://nr.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ae.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kf.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dn.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://ee.shxzskj.cn

Ruby: arr.tally
来源：http://dc.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cl.szsharing.cn

[D21] 判断是否包含某元素
来源：http://lt.yuexingan06.cn

Py:   x in arr
来源：http://oh.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://eq.nszjky.cn

JS:   arr.includes(x)
来源：http://ig.hahajie.cn

TS:   arr.includes(x)
来源：http://cl.jianghongdianzi.cn

Java: list.contains(x)
来源：http://gm.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://fi.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://pv.lnxyls.cn

C#:   list.Contains(x)
来源：http://fu.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://vz.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xi.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jl.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sq.bookmarksfly.cn

TS:   [...arr];
来源：http://wn.newstarts.cn

Java: new ArrayList<>(list);
来源：http://uk.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ib.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ut.lnxyls.cn

C#:   new List<int>(list);
来源：http://aw.shtwfgs.cn

[D23] reduce 累积计算
来源：http://dz.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oo.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jv.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://es.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gf.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xq.jianghongdianzi.cn

Go:   // 手写循环
来源：http://ix.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sf.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fc.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://dj.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ll.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pn.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://td.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wd.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gl.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vo.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fc.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://js.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://wn.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hc.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ul.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fi.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oq.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vg.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oo.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pj.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ov.9csxet.cn

[D26] 数组转字符串
来源：http://ns.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://jm.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://hi.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://vf.lnxyls.cn

TS:   arr.join(", ")
来源：http://zu.hahajie.cn

Java: String.join(", ", list)
来源：http://yu.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://pm.gzmigu.cn

Ruby: arr.join(", ")
来源：http://tc.nszjky.cn

C#:   string.Join(", ", list)
来源：http://vr.colortex.cn

================================================================================
来源：http://ts.szsharing.cn

E. 字符串处理
来源：http://iv.panjiajie.cn

================================================================================
来源：http://yu.jctech888.com.cn

[E01] 拼接字符串
来源：http://zt.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://db.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mb.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wh.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dz.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fl.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bs.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nm.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tr.muxihuayi.cn

[E02] 重复字符串
来源：http://qk.gzmigu.cn

Py:   "ab" * 3
来源：http://pf.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://zs.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://kj.szsharing.cn

TS:   "ab".repeat(3)
来源：http://xe.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://hq.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://vz.panjiajie.cn

Ruby: "ab" * 3
来源：http://no.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zo.lnxyls.cn

[E03] 截取子串
来源：http://lr.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uy.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ta.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sq.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://on.521024.cn

Java: s.substring(1, 4)
来源：http://tv.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kw.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mx.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://ds.bjjhwx.cn

[E04] 查找子串位置
来源：http://dj.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://ki.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://fq.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xv.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://ev.hnjuh.cn

Java: s.indexOf("x")
来源：http://rm.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://gq.shxzskj.cn

Ruby: s.index("x")
来源：http://ki.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://wa.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jt.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xe.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jg.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yg.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oi.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oe.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jh.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gx.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zg.haigaiapp.cn

[E06] 替换子串
来源：http://kq.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nh.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://wa.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wq.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://it.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qe.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://by.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lq.bjjhwx.cn


<!-- 参考信息 -->