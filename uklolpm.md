代发 wailian999

Ruby: a, b = pair
来源：http://ax.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://kk.hahajie.cn

[C16] 函数 / 方法重载
来源：http://yc.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yd.hnjuh.cn

PHP:  // 无重载
来源：http://ht.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xy.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://vn.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wy.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://pr.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://qj.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://po.nszjky.cn

================================================================================
来源：http://sc.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://oh.shxzskj.cn

================================================================================
来源：http://bb.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://jl.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mx.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ar.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rg.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pt.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jf.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://vc.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://rm.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nr.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://cd.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://di.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://at.haigaiapp.cn

JS:   arr.push(4);
来源：http://iu.nszjky.cn

TS:   arr.push(4);
来源：http://rj.muxihuayi.cn

Java: list.add(4);
来源：http://px.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://oy.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://aq.bjjhwx.cn

C#:   list.Add(4);
来源：http://ls.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://sp.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://je.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zr.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zw.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://na.gzmigu.cn

Java: list.add(0, 0);
来源：http://ra.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rl.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kv.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://va.szsharing.cn

[D04] 删除元素
来源：http://dq.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pr.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ux.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fl.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://nq.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vu.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qj.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ti.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ph.shxzskj.cn

[D05] 访问与修改元素
来源：http://rj.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aj.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uq.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xn.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://go.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://pb.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://ev.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vy.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bh.wgjwhj.cn

[D06] 数组长度
来源：http://km.bookmarksfly.cn

Py:   len(arr)
来源：http://tc.nicolike.cn

PHP:  count($arr);
来源：http://fx.yuexingan06.cn

JS:   arr.length
来源：http://ih.huixinmuqiang.cn

TS:   arr.length
来源：http://ld.colortex.cn

Java: list.size();
来源：http://nf.panjiajie.cn

Go:   len(arr)
来源：http://lk.9csxet.cn

Ruby: arr.length; arr.size
来源：http://pr.chemitech.net.cn

C#:   list.Count;
来源：http://gb.521024.cn

[D07] 切片 / 取子数组
来源：http://oi.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ui.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gd.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ff.521024.cn

TS:   arr.slice(1, 4);
来源：http://si.hnjuh.cn

Java: list.subList(1, 4);
来源：http://rm.jctech888.com.cn

Go:   arr[1:4]
来源：http://dt.huanxung.cn

Ruby: arr[1, 3]
来源：http://cj.521024.cn

C#:   list.GetRange(1, 3);
来源：http://qg.newstarts.cn

[D08] 合并两个数组
来源：http://cc.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://wd.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://sr.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qs.nszjky.cn

TS:   [...a, ...b];
来源：http://yg.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://of.newstarts.cn

Go:   append(a, b...)
来源：http://ys.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://oc.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://tc.muxihuayi.cn

[D09] 排序（升序）
来源：http://qp.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://to.nszjky.cn

PHP:  sort($arr);
来源：http://yf.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ra.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://as.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qi.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ie.huixinmuqiang.cn

Ruby: arr.sort
来源：http://lu.nszjky.cn

C#:   list.Sort();
来源：http://yh.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rc.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ca.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://im.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kg.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hm.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cn.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ly.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bc.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pw.wgjwhj.cn

[D11] 反转数组
来源：http://tk.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yk.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://pd.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bw.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://yc.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://yn.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://zy.521024.cn

Ruby: arr.reverse
来源：http://lj.nicolike.cn

C#:   list.Reverse();
来源：http://ur.huixiangedu.cn

[D12] 查找元素下标
来源：http://ed.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://xw.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qy.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xf.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xz.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rs.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://nh.huanxung.cn

Ruby: arr.index(x)
来源：http://da.huanxung.cn

C#:   list.IndexOf(x);
来源：http://zr.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://gx.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ok.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rm.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://kw.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://xf.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://et.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nh.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oc.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://td.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://ko.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xr.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iv.521024.cn

JS:   arr.map(x => x * 2)
来源：http://mg.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://jd.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kb.hnjuh.cn

Go:   // 手写循环
来源：http://nt.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://km.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cm.chemitech.net.cn

[D15] 去重
来源：http://hh.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lt.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://fj.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://eu.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://uh.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hj.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bp.szsharing.cn

Ruby: arr.uniq
来源：http://nh.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://gy.shxzukj.cn

[D16] 求和与平均值
来源：http://ek.muxihuayi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jz.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ys.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://at.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pc.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wb.yuexingan06.cn

Go:   // 手写循环累加
来源：http://sc.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yq.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://ip.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://fa.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://zp.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://pz.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tn.colortex.cn

TS:   Math.max(...arr);
来源：http://vb.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://au.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mu.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://wz.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://nu.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://hi.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kl.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://lx.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vn.colortex.cn

TS:   nested.flat();
来源：http://ju.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hv.chemitech.net.cn

Go:   // 手写双层循环
来源：http://jj.gzmigu.cn

Ruby: nested.flatten
来源：http://fg.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ec.bjjhwx.cn

[D19] 按字段分组
来源：http://by.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gh.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uz.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xu.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yq.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zc.colortex.cn

Go:   // 手写 map[string][]T
来源：http://oh.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://de.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lw.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://ae.colortex.cn

Py:   Counter(arr)
来源：http://mu.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://en.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pq.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yj.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cb.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://pi.haigaiapp.cn

Ruby: arr.tally
来源：http://pk.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hk.nicolike.cn

[D21] 判断是否包含某元素
来源：http://qp.nszjky.cn

Py:   x in arr
来源：http://qy.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://lr.521024.cn

JS:   arr.includes(x)
来源：http://wl.chemitech.net.cn

TS:   arr.includes(x)
来源：http://dl.hnjuh.cn

Java: list.contains(x)
来源：http://bj.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://ee.hahajie.cn

Ruby: arr.include?(x)
来源：http://eh.huixiangedu.cn

C#:   list.Contains(x)
来源：http://aa.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://qo.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xi.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sp.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ky.huixinmuqiang.cn

TS:   [...arr];
来源：http://wp.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://mc.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ih.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://no.szsharing.cn

C#:   new List<int>(list);
来源：http://mc.wgjwhj.cn

[D23] reduce 累积计算
来源：http://fu.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wj.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jh.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://er.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://de.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gr.shxzukj.cn

Go:   // 手写循环
来源：http://kx.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pp.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iy.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://wg.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uc.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kw.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mt.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tc.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mp.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nm.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gg.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qc.asd995.cn

[D25] Set 集合去重与交并差
来源：http://th.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ht.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cb.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sh.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eh.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://la.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yj.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gi.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yj.shxzskj.cn

[D26] 数组转字符串
来源：http://pk.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://fk.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://ut.521024.cn

JS:   arr.join(", ")
来源：http://px.asd995.cn

TS:   arr.join(", ")
来源：http://rc.huanxung.cn

Java: String.join(", ", list)
来源：http://xj.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://ky.asd995.cn

Ruby: arr.join(", ")
来源：http://sg.521024.cn

C#:   string.Join(", ", list)
来源：http://rc.nicolike.cn

================================================================================
来源：http://ii.asd995.cn

E. 字符串处理
来源：http://ow.szxytkj.cn

================================================================================
来源：http://xa.colortex.cn

[E01] 拼接字符串
来源：http://ay.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iu.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://an.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ar.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ht.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bb.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tp.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ho.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fx.bookmarksfly.cn

[E02] 重复字符串
来源：http://ig.asd995.cn

Py:   "ab" * 3
来源：http://uh.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://hf.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://fg.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://dz.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://kb.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://yh.bjjhwx.cn

Ruby: "ab" * 3
来源：http://wq.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ot.bjjhwx.cn

[E03] 截取子串
来源：http://wu.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ql.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gj.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ss.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://uq.hahajie.cn

Java: s.substring(1, 4)
来源：http://po.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vy.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mn.521024.cn

C#:   s.Substring(1, 3)
来源：http://hx.huanxung.cn

[E04] 查找子串位置
来源：http://jv.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://sr.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ai.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lb.hnjuh.cn

TS:   s.indexOf("x")
来源：http://zr.hahajie.cn

Java: s.indexOf("x")
来源：http://cz.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://rn.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://tn.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://uj.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oe.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cm.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kn.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wl.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vq.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xj.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gz.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hc.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dv.szxytkj.cn

[E06] 替换子串
来源：http://lu.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ls.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://gs.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tp.shxzukj.cn


<!-- 参考信息 -->