代发 wailian999

Ruby: a, b = pair
来源：http://nq.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://cv.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://nm.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xa.9csxet.cn

PHP:  // 无重载
来源：http://tp.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eu.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://pq.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ug.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://kq.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://pk.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lv.bookmarksfly.cn

================================================================================
来源：http://ot.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://ge.9csxet.cn

================================================================================
来源：http://uu.nszjky.cn

[D01] 创建数组 / 列表
来源：http://fw.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fr.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ze.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nc.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wk.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fq.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://yl.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://yu.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ru.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://ab.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zw.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bf.wgjwhj.cn

JS:   arr.push(4);
来源：http://bl.nszjky.cn

TS:   arr.push(4);
来源：http://wo.shxzukj.cn

Java: list.add(4);
来源：http://df.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://ww.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://mh.9csxet.cn

C#:   list.Add(4);
来源：http://tz.9csxet.cn

[D03] 在指定位置插入元素
来源：http://to.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://qb.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://am.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xk.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://ux.asd995.cn

Java: list.add(0, 0);
来源：http://vp.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://li.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mx.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://li.szxytkj.cn

[D04] 删除元素
来源：http://xm.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tj.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kk.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wk.521024.cn

TS:   arr.splice(0, 1);
来源：http://qp.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zc.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uj.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ig.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uu.muxihuayi.cn

[D05] 访问与修改元素
来源：http://sk.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ci.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uj.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fj.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://hy.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://qs.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ph.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nr.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vv.panjiajie.cn

[D06] 数组长度
来源：http://oa.hahajie.cn

Py:   len(arr)
来源：http://nf.haigaiapp.cn

PHP:  count($arr);
来源：http://uu.jianghongdianzi.cn

JS:   arr.length
来源：http://xy.szsharing.cn

TS:   arr.length
来源：http://xh.newstarts.cn

Java: list.size();
来源：http://yf.hahajie.cn

Go:   len(arr)
来源：http://hd.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://eo.jctech888.com.cn

C#:   list.Count;
来源：http://pa.szsharing.cn

[D07] 切片 / 取子数组
来源：http://ep.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fz.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cq.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://id.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://to.521024.cn

Java: list.subList(1, 4);
来源：http://ra.bookmarksfly.cn

Go:   arr[1:4]
来源：http://lo.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://ua.521024.cn

C#:   list.GetRange(1, 3);
来源：http://jl.nszjky.cn

[D08] 合并两个数组
来源：http://fj.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://ew.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://hj.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mc.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://lh.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eu.colortex.cn

Go:   append(a, b...)
来源：http://jo.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://qt.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://on.shxzskj.cn

[D09] 排序（升序）
来源：http://uu.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://hx.nszjky.cn

PHP:  sort($arr);
来源：http://rc.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://de.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vg.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oj.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hv.bookmarksfly.cn

Ruby: arr.sort
来源：http://cn.bjjhwx.cn

C#:   list.Sort();
来源：http://ia.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ms.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dy.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ov.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bs.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cq.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nn.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dv.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cw.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sz.jctech888.com.cn

[D11] 反转数组
来源：http://cy.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oj.nszjky.cn

PHP:  array_reverse($arr);
来源：http://tf.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ph.lnxyls.cn

TS:   [...arr].reverse();
来源：http://ix.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ya.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://gm.hahajie.cn

Ruby: arr.reverse
来源：http://bq.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://xz.huanxung.cn

[D12] 查找元素下标
来源：http://lu.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://du.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pl.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gq.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ep.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tu.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://yi.panjiajie.cn

Ruby: arr.index(x)
来源：http://rx.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://av.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://uu.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jb.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pe.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://gk.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://hr.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hn.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jl.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qj.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sv.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://qe.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tf.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://du.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://bn.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://mk.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mz.bookmarksfly.cn

Go:   // 手写循环
来源：http://al.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uc.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zc.muxihuayi.cn

[D15] 去重
来源：http://ia.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oy.9csxet.cn

PHP:  array_unique($arr);
来源：http://ff.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://mp.nszjky.cn

TS:   [...new Set(arr)]
来源：http://nn.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://up.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dg.shtwfgs.cn

Ruby: arr.uniq
来源：http://pm.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://kk.shxzukj.cn

[D16] 求和与平均值
来源：http://at.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ma.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sl.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://un.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aw.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zn.hnjuh.cn

Go:   // 手写循环累加
来源：http://mm.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ji.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://uf.hahajie.cn

[D17] 最大值与最小值
来源：http://gi.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://iw.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://um.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qg.asd995.cn

TS:   Math.max(...arr);
来源：http://su.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wk.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wz.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://hw.asd995.cn

C#:   list.Max();  list.Min()
来源：http://nd.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://xl.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wn.colortex.cn

PHP:  array_merge(...$nested);
来源：http://oi.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ch.bookmarksfly.cn

TS:   nested.flat();
来源：http://mb.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://no.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://ut.haigaiapp.cn

Ruby: nested.flatten
来源：http://ra.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wq.bjjhwx.cn

[D19] 按字段分组
来源：http://yb.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zp.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zq.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ye.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bq.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ak.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://nr.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ar.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bs.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://mg.9csxet.cn

Py:   Counter(arr)
来源：http://wt.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://rp.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iv.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ln.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vo.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://lf.muxihuayi.cn

Ruby: arr.tally
来源：http://ss.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dk.huanxung.cn

[D21] 判断是否包含某元素
来源：http://gz.hahajie.cn

Py:   x in arr
来源：http://zh.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://qj.nszjky.cn

JS:   arr.includes(x)
来源：http://hv.yuexingan06.cn

TS:   arr.includes(x)
来源：http://le.colortex.cn

Java: list.contains(x)
来源：http://qh.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://il.newstarts.cn

Ruby: arr.include?(x)
来源：http://gb.panjiajie.cn

C#:   list.Contains(x)
来源：http://uf.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://vo.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fa.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dv.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jc.jctech888.com.cn

TS:   [...arr];
来源：http://tn.hahajie.cn

Java: new ArrayList<>(list);
来源：http://ig.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jk.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://rr.hahajie.cn

C#:   new List<int>(list);
来源：http://el.yuexingan06.cn

[D23] reduce 累积计算
来源：http://se.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qk.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zj.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ig.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mp.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dn.521024.cn

Go:   // 手写循环
来源：http://mn.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pu.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ke.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://jr.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zw.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ws.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ft.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zu.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jl.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rc.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nn.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hv.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://rn.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://as.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tz.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qr.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://co.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zd.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fq.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kv.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dp.asd995.cn

[D26] 数组转字符串
来源：http://lz.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://vn.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://kp.gzmigu.cn

JS:   arr.join(", ")
来源：http://ly.nicolike.cn

TS:   arr.join(", ")
来源：http://lf.newstarts.cn

Java: String.join(", ", list)
来源：http://wa.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://kx.hahajie.cn

Ruby: arr.join(", ")
来源：http://ct.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://mg.huanxung.cn

================================================================================
来源：http://kq.bookmarksfly.cn

E. 字符串处理
来源：http://qy.panjiajie.cn

================================================================================
来源：http://xy.panjiajie.cn

[E01] 拼接字符串
来源：http://ni.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://am.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sw.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qb.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vi.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wu.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tg.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ts.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://js.yuexingan06.cn

[E02] 重复字符串
来源：http://ch.9csxet.cn

Py:   "ab" * 3
来源：http://sy.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://nf.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://vf.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://xu.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://xb.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ti.asd995.cn

Ruby: "ab" * 3
来源：http://ki.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ca.panjiajie.cn

[E03] 截取子串
来源：http://jp.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hc.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zh.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ad.szsharing.cn

TS:   s.slice(1, 4)
来源：http://ec.szxytkj.cn

Java: s.substring(1, 4)
来源：http://sz.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xi.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://od.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://hx.bookmarksfly.cn

[E04] 查找子串位置
来源：http://ef.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://wc.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://hq.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tc.gzmigu.cn

TS:   s.indexOf("x")
来源：http://ji.nszjky.cn

Java: s.indexOf("x")
来源：http://qu.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://rw.yuexingan06.cn

Ruby: s.index("x")
来源：http://yt.szsharing.cn

C#:   s.IndexOf("x")
来源：http://rc.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ei.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zq.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jy.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ur.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fr.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cn.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xb.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bt.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ht.newstarts.cn

[E06] 替换子串
来源：http://tx.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xe.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://jd.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://im.shxzskj.cn


<!-- 参考信息 -->