代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ti.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ae.nicolike.cn

Java: // 无解构
来源：http://rq.bjjhwx.cn

Go:   // 无解构
来源：http://jo.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://wx.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://sn.asd995.cn

[C16] 函数 / 方法重载
来源：http://ul.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xg.lnxyls.cn

PHP:  // 无重载
来源：http://ws.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ow.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://dp.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gj.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://dr.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://sz.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ye.gzmigu.cn

================================================================================
来源：http://ux.asd995.cn

D. 数组 / 列表 / 集合
来源：http://mj.wgjwhj.cn

================================================================================
来源：http://vk.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://kp.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ui.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fu.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ps.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cj.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ko.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://mn.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://hk.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vo.szsharing.cn

[D02] 追加元素到末尾
来源：http://aq.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yf.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kw.nszjky.cn

JS:   arr.push(4);
来源：http://vs.nszjky.cn

TS:   arr.push(4);
来源：http://wt.huanxung.cn

Java: list.add(4);
来源：http://yt.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://po.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://jm.haigaiapp.cn

C#:   list.Add(4);
来源：http://kz.hahajie.cn

[D03] 在指定位置插入元素
来源：http://ll.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://or.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kw.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lb.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://zv.nicolike.cn

Java: list.add(0, 0);
来源：http://zs.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nw.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cf.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://uc.nszjky.cn

[D04] 删除元素
来源：http://pf.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sf.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hp.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bi.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://hs.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ff.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ot.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vo.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://za.shxzskj.cn

[D05] 访问与修改元素
来源：http://vb.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wk.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fj.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://au.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://oc.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://sz.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://xh.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dj.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cs.521024.cn

[D06] 数组长度
来源：http://al.huixiangedu.cn

Py:   len(arr)
来源：http://xf.bjjhwx.cn

PHP:  count($arr);
来源：http://hq.nicolike.cn

JS:   arr.length
来源：http://an.9csxet.cn

TS:   arr.length
来源：http://qn.huanxung.cn

Java: list.size();
来源：http://mz.jianghongdianzi.cn

Go:   len(arr)
来源：http://vd.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://ka.wgjwhj.cn

C#:   list.Count;
来源：http://oe.521024.cn

[D07] 切片 / 取子数组
来源：http://fi.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://de.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tu.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://eq.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://cu.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://ok.huanxung.cn

Go:   arr[1:4]
来源：http://cl.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://nn.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://em.shxzskj.cn

[D08] 合并两个数组
来源：http://dp.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://rk.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://qs.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sp.haigaiapp.cn

TS:   [...a, ...b];
来源：http://yt.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vc.521024.cn

Go:   append(a, b...)
来源：http://hk.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://zx.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ay.shtwfgs.cn

[D09] 排序（升序）
来源：http://vm.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://qe.muxihuayi.cn

PHP:  sort($arr);
来源：http://zw.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ru.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hu.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rg.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://td.bookmarksfly.cn

Ruby: arr.sort
来源：http://hi.lnxyls.cn

C#:   list.Sort();
来源：http://yr.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ff.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pz.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://km.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oh.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://at.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qx.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bt.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dt.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ox.colortex.cn

[D11] 反转数组
来源：http://tn.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pm.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://dx.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vl.szxytkj.cn

TS:   [...arr].reverse();
来源：http://dy.nszjky.cn

Java: Collections.reverse(list);
来源：http://pa.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://ik.gzmigu.cn

Ruby: arr.reverse
来源：http://mp.chemitech.net.cn

C#:   list.Reverse();
来源：http://do.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://xa.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://jg.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://py.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uh.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kh.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dw.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://gk.newstarts.cn

Ruby: arr.index(x)
来源：http://gv.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://wj.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://ts.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xf.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ri.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://mp.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://lt.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bq.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mn.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hw.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gd.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://dr.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://db.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ox.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://tf.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://is.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rk.newstarts.cn

Go:   // 手写循环
来源：http://mm.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tq.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://de.shxzukj.cn

[D15] 去重
来源：http://eg.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bg.9csxet.cn

PHP:  array_unique($arr);
来源：http://lj.szsharing.cn

JS:   [...new Set(arr)]
来源：http://zl.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://zr.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jn.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xz.nicolike.cn

Ruby: arr.uniq
来源：http://qj.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://ct.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://xx.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bh.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://td.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://di.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ob.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mz.panjiajie.cn

Go:   // 手写循环累加
来源：http://di.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qb.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://oy.shxzskj.cn

[D17] 最大值与最小值
来源：http://bm.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://gw.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://py.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wr.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://gg.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bn.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kz.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ul.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://jb.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://no.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ge.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://uo.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eu.shxzskj.cn

TS:   nested.flat();
来源：http://tg.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gm.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://yw.lnxyls.cn

Ruby: nested.flatten
来源：http://mg.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yi.bookmarksfly.cn

[D19] 按字段分组
来源：http://wn.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xc.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://et.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xo.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kx.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sv.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://wy.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mk.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ed.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://sz.asd995.cn

Py:   Counter(arr)
来源：http://zm.newstarts.cn

PHP:  array_count_values($arr);
来源：http://tb.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://py.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pn.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nx.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://pm.nicolike.cn

Ruby: arr.tally
来源：http://ne.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gy.newstarts.cn

[D21] 判断是否包含某元素
来源：http://va.shxzukj.cn

Py:   x in arr
来源：http://fw.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://tg.asd995.cn

JS:   arr.includes(x)
来源：http://ig.nicolike.cn

TS:   arr.includes(x)
来源：http://nh.huixiangedu.cn

Java: list.contains(x)
来源：http://br.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://dr.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://rj.asd995.cn

C#:   list.Contains(x)
来源：http://dk.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://bm.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xn.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lm.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nd.panjiajie.cn

TS:   [...arr];
来源：http://in.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://yx.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tg.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://fp.shxzukj.cn

C#:   new List<int>(list);
来源：http://wg.szxytkj.cn

[D23] reduce 累积计算
来源：http://jd.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vu.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eb.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nn.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://do.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cy.yuntaijiaju.cn

Go:   // 手写循环
来源：http://kb.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://co.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ci.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://vo.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bi.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oe.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rw.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fa.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ju.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sf.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uf.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qm.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://hh.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vs.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pf.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://io.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jh.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ip.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lx.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dr.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sj.colortex.cn

[D26] 数组转字符串
来源：http://xt.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://ng.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://uy.szsharing.cn

JS:   arr.join(", ")
来源：http://so.shxzukj.cn

TS:   arr.join(", ")
来源：http://dy.chemitech.net.cn

Java: String.join(", ", list)
来源：http://pm.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://do.nicolike.cn

Ruby: arr.join(", ")
来源：http://az.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://gz.hnjuh.cn

================================================================================
来源：http://kz.szxytkj.cn

E. 字符串处理
来源：http://qq.shxzskj.cn

================================================================================
来源：http://yo.panjiajie.cn

[E01] 拼接字符串
来源：http://kp.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ye.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sv.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://js.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yw.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kv.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nu.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vp.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gt.haigaiapp.cn

[E02] 重复字符串
来源：http://hr.shxzskj.cn

Py:   "ab" * 3
来源：http://tp.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://gl.newstarts.cn

JS:   "ab".repeat(3)
来源：http://so.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://rl.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://sd.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ua.9csxet.cn

Ruby: "ab" * 3
来源：http://bg.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ar.szxytkj.cn

[E03] 截取子串
来源：http://vs.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qi.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ie.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zr.nicolike.cn

TS:   s.slice(1, 4)
来源：http://kd.521024.cn

Java: s.substring(1, 4)
来源：http://ns.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wm.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ri.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://rg.shxzskj.cn

[E04] 查找子串位置
来源：http://ax.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://jv.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://vl.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qd.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://tp.shxzskj.cn

Java: s.indexOf("x")
来源：http://ny.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://ue.yuexingan06.cn

Ruby: s.index("x")
来源：http://bh.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://mt.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cv.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uh.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ms.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kc.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ww.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ij.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ox.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gt.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gy.521024.cn


<!-- 参考信息 -->