代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rz.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kf.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mx.hnjuh.cn

Ruby: # 无泛型
来源：http://ca.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://by.asd995.cn

[C15] 解构 / 展开参数
来源：http://ld.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ue.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://ap.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dt.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rf.nszjky.cn

Java: // 无解构
来源：http://hx.wgjwhj.cn

Go:   // 无解构
来源：http://op.szxytkj.cn

Ruby: a, b = pair
来源：http://oi.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://uc.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://xr.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ye.huixiangedu.cn

PHP:  // 无重载
来源：http://mf.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ga.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://ei.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mn.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://fr.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://ie.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mn.asd995.cn

================================================================================
来源：http://zk.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://cf.colortex.cn

================================================================================
来源：http://ww.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://fi.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wa.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ey.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cq.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qj.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vi.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://qm.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://le.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wz.nicolike.cn

[D02] 追加元素到末尾
来源：http://cd.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tv.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yw.szxytkj.cn

JS:   arr.push(4);
来源：http://xo.muxihuayi.cn

TS:   arr.push(4);
来源：http://qc.521024.cn

Java: list.add(4);
来源：http://yk.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://am.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://qi.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://kn.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://fb.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://sa.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wv.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iz.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://gs.muxihuayi.cn

Java: list.add(0, 0);
来源：http://vx.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ka.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://se.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://ql.newstarts.cn

[D04] 删除元素
来源：http://vh.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zo.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://at.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://as.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://ny.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kt.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pm.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vu.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nn.9csxet.cn

[D05] 访问与修改元素
来源：http://ml.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wf.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dt.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bz.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://vh.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ba.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://rn.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zw.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nr.chemitech.net.cn

[D06] 数组长度
来源：http://xu.chemitech.net.cn

Py:   len(arr)
来源：http://jn.bjjhwx.cn

PHP:  count($arr);
来源：http://uq.hnjuh.cn

JS:   arr.length
来源：http://yo.bjjhwx.cn

TS:   arr.length
来源：http://dr.bookmarksfly.cn

Java: list.size();
来源：http://qe.jianghongdianzi.cn

Go:   len(arr)
来源：http://yj.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://zt.huanxung.cn

C#:   list.Count;
来源：http://nj.521024.cn

[D07] 切片 / 取子数组
来源：http://jc.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xc.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ig.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://zc.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://wq.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ln.haigaiapp.cn

Go:   arr[1:4]
来源：http://ck.521024.cn

Ruby: arr[1, 3]
来源：http://fl.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://qw.lnxyls.cn

[D08] 合并两个数组
来源：http://nk.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://sm.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://mc.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nc.shxzskj.cn

TS:   [...a, ...b];
来源：http://pz.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tm.asd995.cn

Go:   append(a, b...)
来源：http://wg.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://gw.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://nm.jctech888.com.cn

[D09] 排序（升序）
来源：http://od.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://vy.shxzukj.cn

PHP:  sort($arr);
来源：http://cf.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kv.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vd.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nm.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zh.nicolike.cn

Ruby: arr.sort
来源：http://np.panjiajie.cn

C#:   list.Sort();
来源：http://mw.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ff.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iv.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ya.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sf.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cf.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://it.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iy.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tc.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hg.hnjuh.cn

[D11] 反转数组
来源：http://eh.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xm.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://gz.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kx.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://us.hahajie.cn

Java: Collections.reverse(list);
来源：http://zg.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://bs.huanxung.cn

Ruby: arr.reverse
来源：http://wz.haigaiapp.cn

C#:   list.Reverse();
来源：http://ok.yuexingan06.cn

[D12] 查找元素下标
来源：http://tg.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://wg.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fw.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ut.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://es.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://du.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://tg.wgjwhj.cn

Ruby: arr.index(x)
来源：http://cm.asd995.cn

C#:   list.IndexOf(x);
来源：http://ev.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://tm.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qv.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nx.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://zn.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://cp.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://my.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://go.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sf.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ax.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://xm.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xy.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mf.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://fu.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://qk.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ps.muxihuayi.cn

Go:   // 手写循环
来源：http://jd.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ve.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gy.shxzukj.cn

[D15] 去重
来源：http://rn.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tm.521024.cn

PHP:  array_unique($arr);
来源：http://tf.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://xm.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://hw.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://at.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://na.colortex.cn

Ruby: arr.uniq
来源：http://ba.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://nz.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://uy.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qi.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pj.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fc.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bz.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://om.panjiajie.cn

Go:   // 手写循环累加
来源：http://ub.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://el.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://vx.hahajie.cn

[D17] 最大值与最小值
来源：http://aj.colortex.cn

Py:   max(arr);  min(arr)
来源：http://hj.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://ac.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cm.nszjky.cn

TS:   Math.max(...arr);
来源：http://wc.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bl.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dc.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://py.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://gw.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://qt.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jt.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://lq.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nz.szsharing.cn

TS:   nested.flat();
来源：http://yj.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jn.chemitech.net.cn

Go:   // 手写双层循环
来源：http://ys.gzmigu.cn

Ruby: nested.flatten
来源：http://ki.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eb.muxihuayi.cn

[D19] 按字段分组
来源：http://pj.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pr.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sh.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uw.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kc.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mc.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://xi.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ak.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aj.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://hl.wgjwhj.cn

Py:   Counter(arr)
来源：http://kx.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://bx.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tz.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nu.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ge.nicolike.cn

Go:   // 手写 map[T]int
来源：http://du.shtwfgs.cn

Ruby: arr.tally
来源：http://ym.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vs.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://cb.szxytkj.cn

Py:   x in arr
来源：http://zr.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://xm.521024.cn

JS:   arr.includes(x)
来源：http://as.muxihuayi.cn

TS:   arr.includes(x)
来源：http://qh.bjjhwx.cn

Java: list.contains(x)
来源：http://rr.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://yf.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://st.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://lf.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://tm.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wt.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wu.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nt.szsharing.cn

TS:   [...arr];
来源：http://nd.9csxet.cn

Java: new ArrayList<>(list);
来源：http://tk.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://as.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://qe.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://dn.hahajie.cn

[D23] reduce 累积计算
来源：http://xb.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://co.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://li.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gl.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qr.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gy.newstarts.cn

Go:   // 手写循环
来源：http://py.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kh.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://el.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://iu.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cv.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sc.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ql.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eu.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nu.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ie.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ch.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rd.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://ao.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dt.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lo.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zf.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rr.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sz.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rz.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sq.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zs.wgjwhj.cn

[D26] 数组转字符串
来源：http://le.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://ui.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://cw.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://xl.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://nr.hahajie.cn

Java: String.join(", ", list)
来源：http://qc.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://we.lnxyls.cn

Ruby: arr.join(", ")
来源：http://cz.colortex.cn

C#:   string.Join(", ", list)
来源：http://aj.szxytkj.cn

================================================================================
来源：http://ju.hnjuh.cn

E. 字符串处理
来源：http://vl.jianghongdianzi.cn

================================================================================
来源：http://lj.chemitech.net.cn

[E01] 拼接字符串
来源：http://kc.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mc.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://an.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qz.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nn.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ku.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xr.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rk.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dy.shxzukj.cn

[E02] 重复字符串
来源：http://za.huixiangedu.cn

Py:   "ab" * 3
来源：http://br.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://ta.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://xb.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://bs.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://ut.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://fz.shxzukj.cn

Ruby: "ab" * 3
来源：http://gn.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dj.muxihuayi.cn

[E03] 截取子串
来源：http://zy.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vw.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ah.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://he.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://bq.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://yy.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cv.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cz.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://tt.jctech888.com.cn

[E04] 查找子串位置
来源：http://tj.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://sj.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://dw.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cz.asd995.cn

TS:   s.indexOf("x")
来源：http://we.hahajie.cn

Java: s.indexOf("x")
来源：http://yy.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://oi.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://sx.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://yb.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bn.huanxung.cn


<!-- 参考信息 -->