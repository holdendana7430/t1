代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pb.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ba.panjiajie.cn

Java: // 无解构
来源：http://yr.yuntaijiaju.cn

Go:   // 无解构
来源：http://mt.9csxet.cn

Ruby: a, b = pair
来源：http://bj.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://pe.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://gt.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vr.shxzskj.cn

PHP:  // 无重载
来源：http://ry.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yk.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://sw.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wv.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://pm.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://ko.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fd.jianghongdianzi.cn

================================================================================
来源：http://mu.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://xk.shtwfgs.cn

================================================================================
来源：http://vp.szsharing.cn

[D01] 创建数组 / 列表
来源：http://pm.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bz.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ve.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rw.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xg.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://io.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://oz.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://ee.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ai.szxytkj.cn

[D02] 追加元素到末尾
来源：http://hs.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wy.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zr.muxihuayi.cn

JS:   arr.push(4);
来源：http://nx.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://fk.hnjuh.cn

Java: list.add(4);
来源：http://td.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://bp.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://qp.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://pv.colortex.cn

[D03] 在指定位置插入元素
来源：http://al.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://hy.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aj.521024.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eh.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://jj.wgjwhj.cn

Java: list.add(0, 0);
来源：http://fn.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ic.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iv.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://im.jctech888.com.cn

[D04] 删除元素
来源：http://uc.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ng.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dw.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ws.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://jf.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pm.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yc.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jc.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dg.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://tf.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://at.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lt.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pt.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://jb.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://hb.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://au.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oj.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ae.muxihuayi.cn

[D06] 数组长度
来源：http://yz.shxzskj.cn

Py:   len(arr)
来源：http://yp.lnxyls.cn

PHP:  count($arr);
来源：http://ke.lnxyls.cn

JS:   arr.length
来源：http://lr.lnxyls.cn

TS:   arr.length
来源：http://bw.gzmigu.cn

Java: list.size();
来源：http://zm.gzmigu.cn

Go:   len(arr)
来源：http://ud.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://vd.haigaiapp.cn

C#:   list.Count;
来源：http://lk.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://ve.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://on.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vj.521024.cn

JS:   arr.slice(1, 4);
来源：http://ss.521024.cn

TS:   arr.slice(1, 4);
来源：http://cf.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://hz.nszjky.cn

Go:   arr[1:4]
来源：http://fk.hahajie.cn

Ruby: arr[1, 3]
来源：http://zg.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://ff.huixiangedu.cn

[D08] 合并两个数组
来源：http://tx.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://gu.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://ev.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tx.9csxet.cn

TS:   [...a, ...b];
来源：http://cq.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jv.gzmigu.cn

Go:   append(a, b...)
来源：http://bg.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://br.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://pp.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://ju.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://iq.colortex.cn

PHP:  sort($arr);
来源：http://na.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kb.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rn.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tf.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mp.jianghongdianzi.cn

Ruby: arr.sort
来源：http://dg.bjjhwx.cn

C#:   list.Sort();
来源：http://hq.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yb.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oh.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dz.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wj.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aa.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://no.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ds.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qr.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zw.bjjhwx.cn

[D11] 反转数组
来源：http://uf.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lc.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://ah.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pl.521024.cn

TS:   [...arr].reverse();
来源：http://oh.nicolike.cn

Java: Collections.reverse(list);
来源：http://mq.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://qu.hahajie.cn

Ruby: arr.reverse
来源：http://av.szsharing.cn

C#:   list.Reverse();
来源：http://hx.haigaiapp.cn

[D12] 查找元素下标
来源：http://hj.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://jk.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lf.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ya.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xn.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cw.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://xf.521024.cn

Ruby: arr.index(x)
来源：http://cf.9csxet.cn

C#:   list.IndexOf(x);
来源：http://gu.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://uy.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ir.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mo.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://xf.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://cn.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vl.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rn.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fc.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sx.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://wz.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zz.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gd.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://pc.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://we.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://we.szsharing.cn

Go:   // 手写循环
来源：http://sc.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mm.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gh.bookmarksfly.cn

[D15] 去重
来源：http://bz.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tn.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://mp.newstarts.cn

JS:   [...new Set(arr)]
来源：http://qg.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://zt.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pt.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pu.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://vj.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://dd.hahajie.cn

[D16] 求和与平均值
来源：http://vk.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xv.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hg.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pz.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jq.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vh.nicolike.cn

Go:   // 手写循环累加
来源：http://ib.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rr.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://nx.huixiangedu.cn

[D17] 最大值与最小值
来源：http://om.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://tj.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://ug.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kt.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://kh.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rq.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://js.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://ci.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://pc.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://ra.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lh.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://md.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hv.asd995.cn

TS:   nested.flat();
来源：http://ec.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vu.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://mz.muxihuayi.cn

Ruby: nested.flatten
来源：http://ts.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.huanxung.cn

[D19] 按字段分组
来源：http://wn.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jy.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ii.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fa.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kv.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eu.521024.cn

Go:   // 手写 map[string][]T
来源：http://ve.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ey.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sw.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://uf.huanxung.cn

Py:   Counter(arr)
来源：http://dy.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://jq.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://no.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zh.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://su.9csxet.cn

Go:   // 手写 map[T]int
来源：http://se.muxihuayi.cn

Ruby: arr.tally
来源：http://fo.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://su.hahajie.cn

[D21] 判断是否包含某元素
来源：http://ou.521024.cn

Py:   x in arr
来源：http://eu.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://gh.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://qe.szxytkj.cn

TS:   arr.includes(x)
来源：http://jf.bookmarksfly.cn

Java: list.contains(x)
来源：http://mz.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://cj.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://kw.lnxyls.cn

C#:   list.Contains(x)
来源：http://eo.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://mj.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wv.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ir.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cx.szxytkj.cn

TS:   [...arr];
来源：http://ic.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://pl.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://is.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://eu.hahajie.cn

C#:   new List<int>(list);
来源：http://nu.shxzukj.cn

[D23] reduce 累积计算
来源：http://ku.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://la.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bk.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yt.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tf.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dn.jianghongdianzi.cn

Go:   // 手写循环
来源：http://hm.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://it.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fm.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://mo.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nv.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ih.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zb.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ah.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cl.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://la.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hv.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wf.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://nt.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zc.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dr.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mh.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fn.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ap.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vq.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pv.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cn.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://kp.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://dn.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://qi.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://qr.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://mu.jctech888.com.cn

Java: String.join(", ", list)
来源：http://br.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://sa.shxzukj.cn

Ruby: arr.join(", ")
来源：http://hw.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://qr.shtwfgs.cn

================================================================================
来源：http://ww.yuexingan06.cn

E. 字符串处理
来源：http://kc.jctech888.com.cn

================================================================================
来源：http://on.hnjuh.cn

[E01] 拼接字符串
来源：http://ws.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xy.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cq.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sb.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ma.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iz.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qw.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xz.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ch.haigaiapp.cn

[E02] 重复字符串
来源：http://kq.nicolike.cn

Py:   "ab" * 3
来源：http://pc.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://in.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://zf.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://sr.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://si.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://oa.nicolike.cn

Ruby: "ab" * 3
来源：http://sb.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ux.hnjuh.cn

[E03] 截取子串
来源：http://up.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ix.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mk.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oz.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://kf.gzmigu.cn

Java: s.substring(1, 4)
来源：http://za.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rv.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ed.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://yl.bookmarksfly.cn

[E04] 查找子串位置
来源：http://dk.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://ri.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://cg.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://un.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://yz.nicolike.cn

Java: s.indexOf("x")
来源：http://zv.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://jw.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://bo.nicolike.cn

C#:   s.IndexOf("x")
来源：http://ud.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vi.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mc.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cs.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kl.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://be.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pg.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cx.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qt.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wb.panjiajie.cn


<!-- 参考信息 -->