代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ls.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hc.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://el.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://mx.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rm.9csxet.cn

[C15] 解构 / 展开参数
来源：http://hx.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qg.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://fn.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://do.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ra.yuntaijiaju.cn

Java: // 无解构
来源：http://is.yuntaijiaju.cn

Go:   // 无解构
来源：http://eh.jctech888.com.cn

Ruby: a, b = pair
来源：http://vk.521024.cn

C#:   var (a, b) = pair;
来源：http://hr.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://la.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vg.wgjwhj.cn

PHP:  // 无重载
来源：http://ha.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mw.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://hw.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tu.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://hy.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://em.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ae.shtwfgs.cn

================================================================================
来源：http://pz.asd995.cn

D. 数组 / 列表 / 集合
来源：http://ec.yuexingan06.cn

================================================================================
来源：http://cd.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://os.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qq.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ru.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vv.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uv.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://di.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://il.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://rg.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yh.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://en.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://de.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uq.gzmigu.cn

JS:   arr.push(4);
来源：http://qa.hnjuh.cn

TS:   arr.push(4);
来源：http://zc.newstarts.cn

Java: list.add(4);
来源：http://mz.jianghongdianzi.cn

Go:   arr = append(arr, 4)
来源：http://wt.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://rx.bjjhwx.cn

C#:   list.Add(4);
来源：http://md.521024.cn

[D03] 在指定位置插入元素
来源：http://fk.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://ix.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ny.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pe.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://gm.colortex.cn

Java: list.add(0, 0);
来源：http://ny.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oy.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kc.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://yg.shtwfgs.cn

[D04] 删除元素
来源：http://ui.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sz.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tj.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tg.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://lw.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ik.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wv.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wt.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jq.nicolike.cn

[D05] 访问与修改元素
来源：http://mm.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ez.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rf.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gt.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://rh.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://mp.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://vd.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qf.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rt.jianghongdianzi.cn

[D06] 数组长度
来源：http://og.nszjky.cn

Py:   len(arr)
来源：http://ph.szsharing.cn

PHP:  count($arr);
来源：http://ko.chemitech.net.cn

JS:   arr.length
来源：http://xc.shxzukj.cn

TS:   arr.length
来源：http://lc.huanxung.cn

Java: list.size();
来源：http://ls.hahajie.cn

Go:   len(arr)
来源：http://ts.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://lp.newstarts.cn

C#:   list.Count;
来源：http://rz.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://kt.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yb.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zv.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://yw.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://ec.shxzukj.cn

Java: list.subList(1, 4);
来源：http://uj.bjjhwx.cn

Go:   arr[1:4]
来源：http://bz.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://sd.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://ov.lnxyls.cn

[D08] 合并两个数组
来源：http://qb.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://hd.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://mc.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://co.bjjhwx.cn

TS:   [...a, ...b];
来源：http://qc.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ep.chemitech.net.cn

Go:   append(a, b...)
来源：http://zs.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://er.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://qt.chemitech.net.cn

[D09] 排序（升序）
来源：http://xb.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://zw.szxytkj.cn

PHP:  sort($arr);
来源：http://rc.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fm.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vj.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wt.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xj.gzmigu.cn

Ruby: arr.sort
来源：http://sa.asd995.cn

C#:   list.Sort();
来源：http://fq.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dn.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iv.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zi.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xp.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ql.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gt.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xe.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oq.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dc.lnxyls.cn

[D11] 反转数组
来源：http://hx.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wt.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://vu.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oo.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://tb.szxytkj.cn

Java: Collections.reverse(list);
来源：http://rb.asd995.cn

Go:   slices.Reverse(arr)
来源：http://lp.lnxyls.cn

Ruby: arr.reverse
来源：http://oe.szsharing.cn

C#:   list.Reverse();
来源：http://ml.wgjwhj.cn

[D12] 查找元素下标
来源：http://sk.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://hn.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dm.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xd.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sy.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ag.asd995.cn

Go:   slices.Index(arr, x)
来源：http://sk.panjiajie.cn

Ruby: arr.index(x)
来源：http://kf.nszjky.cn

C#:   list.IndexOf(x);
来源：http://wo.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://rl.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fq.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vi.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://hp.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://ra.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tc.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ns.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://du.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yp.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://ee.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tg.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fj.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://wx.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://ye.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ms.lnxyls.cn

Go:   // 手写循环
来源：http://ep.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://do.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lk.bookmarksfly.cn

[D15] 去重
来源：http://oh.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oz.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://ir.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://qp.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://yo.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://df.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lt.muxihuayi.cn

Ruby: arr.uniq
来源：http://qw.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://ka.wgjwhj.cn

[D16] 求和与平均值
来源：http://lt.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gn.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ih.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vs.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uz.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iy.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://zv.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vf.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://ce.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://vf.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://qx.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://fc.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pb.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://lc.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pq.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kt.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://jo.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://ba.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://lc.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dh.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://sd.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://df.huanxung.cn

TS:   nested.flat();
来源：http://fe.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://np.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://sh.9csxet.cn

Ruby: nested.flatten
来源：http://eu.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eu.521024.cn

[D19] 按字段分组
来源：http://gf.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gx.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qh.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hv.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://as.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vz.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://yi.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tn.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://en.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://fq.chemitech.net.cn

Py:   Counter(arr)
来源：http://lx.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://dy.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://co.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://an.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tn.521024.cn

Go:   // 手写 map[T]int
来源：http://sv.huixinmuqiang.cn

Ruby: arr.tally
来源：http://yt.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sz.huanxung.cn

[D21] 判断是否包含某元素
来源：http://un.9csxet.cn

Py:   x in arr
来源：http://wl.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://bn.gzmigu.cn

JS:   arr.includes(x)
来源：http://ao.newstarts.cn

TS:   arr.includes(x)
来源：http://ji.yuntaijiaju.cn

Java: list.contains(x)
来源：http://cu.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://gp.hnjuh.cn

Ruby: arr.include?(x)
来源：http://tr.asd995.cn

C#:   list.Contains(x)
来源：http://nb.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://zv.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vq.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ku.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sx.nicolike.cn

TS:   [...arr];
来源：http://nm.nszjky.cn

Java: new ArrayList<>(list);
来源：http://ti.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ay.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://bp.haigaiapp.cn

C#:   new List<int>(list);
来源：http://lz.jctech888.com.cn

[D23] reduce 累积计算
来源：http://bk.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://st.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wg.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ln.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ea.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fm.huixiangedu.cn

Go:   // 手写循环
来源：http://jp.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fs.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qr.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://cu.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tb.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ez.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ae.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ip.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wy.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://am.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gc.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bp.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://cv.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pc.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jf.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wr.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://es.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vw.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fq.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kh.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ez.asd995.cn

[D26] 数组转字符串
来源：http://ao.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://mf.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://jl.shtwfgs.cn

JS:   arr.join(", ")
来源：http://ce.chemitech.net.cn

TS:   arr.join(", ")
来源：http://sn.shtwfgs.cn

Java: String.join(", ", list)
来源：http://bu.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://zi.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://fp.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://ia.gzmigu.cn

================================================================================
来源：http://gw.newstarts.cn

E. 字符串处理
来源：http://mh.panjiajie.cn

================================================================================
来源：http://go.asd995.cn

[E01] 拼接字符串
来源：http://wc.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zt.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vn.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dw.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yz.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vf.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yo.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pw.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://us.shxzskj.cn

[E02] 重复字符串
来源：http://nn.wgjwhj.cn

Py:   "ab" * 3
来源：http://zi.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://wf.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://nr.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://hz.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://kw.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://te.colortex.cn

Ruby: "ab" * 3
来源：http://aw.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fp.521024.cn

[E03] 截取子串
来源：http://tp.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cn.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://td.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ap.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://sy.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://dq.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gb.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rf.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://lm.lnxyls.cn

[E04] 查找子串位置
来源：http://la.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://yn.521024.cn

PHP:  strpos($s, "x");
来源：http://cv.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wk.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://lx.shxzskj.cn

Java: s.indexOf("x")
来源：http://xx.colortex.cn

Go:   strings.Index(s, "x")
来源：http://dc.shxzukj.cn

Ruby: s.index("x")
来源：http://hb.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://ou.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ec.hnjuh.cn


<!-- 参考信息 -->