代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fx.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sx.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sw.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jf.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://re.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://rn.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://me.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mk.nicolike.cn

[C14] 泛型函数
来源：http://kx.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xz.bookmarksfly.cn

PHP:  // 无泛型
来源：http://py.shxzukj.cn

JS:   // 无泛型
来源：http://zf.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dy.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://os.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cy.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://pj.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cv.nicolike.cn

[C15] 解构 / 展开参数
来源：http://vk.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lk.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://ar.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rm.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kr.521024.cn

Java: // 无解构
来源：http://nb.panjiajie.cn

Go:   // 无解构
来源：http://qz.colortex.cn

Ruby: a, b = pair
来源：http://sm.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://ou.521024.cn

[C16] 函数 / 方法重载
来源：http://fg.colortex.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qg.wgjwhj.cn

PHP:  // 无重载
来源：http://wl.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nv.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://gw.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://oj.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ft.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://dv.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ri.nszjky.cn

================================================================================
来源：http://jl.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://fo.asd995.cn

================================================================================
来源：http://rv.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://id.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wp.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pu.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zx.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fb.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://us.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://yb.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://lr.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ne.shxzukj.cn

[D02] 追加元素到末尾
来源：http://vv.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tf.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tq.wgjwhj.cn

JS:   arr.push(4);
来源：http://ts.asd995.cn

TS:   arr.push(4);
来源：http://od.shtwfgs.cn

Java: list.add(4);
来源：http://xw.colortex.cn

Go:   arr = append(arr, 4)
来源：http://jt.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://sk.nszjky.cn

C#:   list.Add(4);
来源：http://bs.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://lk.colortex.cn

Py:   arr.insert(0, 0)
来源：http://df.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eh.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dj.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://vh.shxzukj.cn

Java: list.add(0, 0);
来源：http://eb.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://aj.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vt.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://nl.chemitech.net.cn

[D04] 删除元素
来源：http://zg.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fh.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mc.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nn.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://es.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qi.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ty.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ra.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ug.wgjwhj.cn

[D05] 访问与修改元素
来源：http://np.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fd.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rq.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bj.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://il.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://ly.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://pq.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wt.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bb.asd995.cn

[D06] 数组长度
来源：http://ra.521024.cn

Py:   len(arr)
来源：http://fr.muxihuayi.cn

PHP:  count($arr);
来源：http://qd.nicolike.cn

JS:   arr.length
来源：http://sh.shxzskj.cn

TS:   arr.length
来源：http://on.bookmarksfly.cn

Java: list.size();
来源：http://wa.muxihuayi.cn

Go:   len(arr)
来源：http://ls.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://fw.shxzukj.cn

C#:   list.Count;
来源：http://kl.huanxung.cn

[D07] 切片 / 取子数组
来源：http://ov.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rn.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tn.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://rt.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://uo.gzmigu.cn

Java: list.subList(1, 4);
来源：http://og.panjiajie.cn

Go:   arr[1:4]
来源：http://hh.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://wr.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://dj.nicolike.cn

[D08] 合并两个数组
来源：http://gq.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://kb.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://gv.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lo.9csxet.cn

TS:   [...a, ...b];
来源：http://en.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oh.bookmarksfly.cn

Go:   append(a, b...)
来源：http://je.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://cl.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://xm.521024.cn

[D09] 排序（升序）
来源：http://ud.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://la.panjiajie.cn

PHP:  sort($arr);
来源：http://vu.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tx.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iq.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pg.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tb.jctech888.com.cn

Ruby: arr.sort
来源：http://nd.hnjuh.cn

C#:   list.Sort();
来源：http://lq.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kf.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ef.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fo.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yq.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lb.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ue.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lo.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ol.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://to.colortex.cn

[D11] 反转数组
来源：http://eb.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dc.colortex.cn

PHP:  array_reverse($arr);
来源：http://we.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sc.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://hu.gzmigu.cn

Java: Collections.reverse(list);
来源：http://ip.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://wc.szsharing.cn

Ruby: arr.reverse
来源：http://nt.hahajie.cn

C#:   list.Reverse();
来源：http://mo.nicolike.cn

[D12] 查找元素下标
来源：http://ps.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://yb.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dd.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hb.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://di.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://um.asd995.cn

Go:   slices.Index(arr, x)
来源：http://uj.yuexingan06.cn

Ruby: arr.index(x)
来源：http://aq.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://vt.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://td.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ym.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pj.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://wc.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://af.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qw.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ix.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uq.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hr.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ar.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ob.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ku.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://cv.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://au.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://re.gzmigu.cn

Go:   // 手写循环
来源：http://sd.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vb.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yt.nicolike.cn

[D15] 去重
来源：http://ev.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bf.shxzukj.cn

PHP:  array_unique($arr);
来源：http://du.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://qd.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://st.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eq.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jq.panjiajie.cn

Ruby: arr.uniq
来源：http://tz.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://is.bookmarksfly.cn

[D16] 求和与平均值
来源：http://zc.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yv.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dc.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ys.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ga.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ra.shxzskj.cn

Go:   // 手写循环累加
来源：http://fy.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ms.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://aw.bjjhwx.cn

[D17] 最大值与最小值
来源：http://rk.colortex.cn

Py:   max(arr);  min(arr)
来源：http://dn.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://uw.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://de.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://eo.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dv.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://en.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://fo.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://bn.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://sj.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hx.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://ur.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hc.muxihuayi.cn

TS:   nested.flat();
来源：http://vd.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jg.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://ar.szsharing.cn

Ruby: nested.flatten
来源：http://ya.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vd.asd995.cn

[D19] 按字段分组
来源：http://uk.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kp.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ih.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wr.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ta.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gy.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://qg.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rg.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nq.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://hb.shtwfgs.cn

Py:   Counter(arr)
来源：http://by.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://ye.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uw.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://po.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lh.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://ri.bookmarksfly.cn

Ruby: arr.tally
来源：http://ea.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hv.asd995.cn

[D21] 判断是否包含某元素
来源：http://dc.haigaiapp.cn

Py:   x in arr
来源：http://lk.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://ax.huixiangedu.cn

JS:   arr.includes(x)
来源：http://ci.9csxet.cn

TS:   arr.includes(x)
来源：http://tz.jianghongdianzi.cn

Java: list.contains(x)
来源：http://tu.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://xd.panjiajie.cn

Ruby: arr.include?(x)
来源：http://vm.bjjhwx.cn

C#:   list.Contains(x)
来源：http://cs.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://bw.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gt.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ns.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://og.huixiangedu.cn

TS:   [...arr];
来源：http://zz.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://sh.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://id.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ge.asd995.cn

C#:   new List<int>(list);
来源：http://sn.shxzskj.cn

[D23] reduce 累积计算
来源：http://st.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cq.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sh.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fe.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://df.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vy.nicolike.cn

Go:   // 手写循环
来源：http://lb.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jn.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rc.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://ca.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://np.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ut.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bl.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mj.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sk.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nk.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yn.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ee.521024.cn

[D25] Set 集合去重与交并差
来源：http://qk.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oi.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ru.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ne.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qp.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wb.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yj.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wi.bookmarksfly.cn

[D26] 数组转字符串
来源：http://tu.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://zw.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://hd.shxzukj.cn

JS:   arr.join(", ")
来源：http://jk.521024.cn

TS:   arr.join(", ")
来源：http://az.shxzskj.cn

Java: String.join(", ", list)
来源：http://rv.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://wr.lnxyls.cn

Ruby: arr.join(", ")
来源：http://mz.huanxung.cn

C#:   string.Join(", ", list)
来源：http://wh.szxytkj.cn

================================================================================
来源：http://qf.jianghongdianzi.cn

E. 字符串处理
来源：http://uw.shxzskj.cn

================================================================================
来源：http://fk.nszjky.cn

[E01] 拼接字符串
来源：http://rn.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kh.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ep.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pg.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://li.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tw.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xs.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pr.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wp.hnjuh.cn

[E02] 重复字符串
来源：http://io.9csxet.cn

Py:   "ab" * 3
来源：http://jb.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://st.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://xi.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://jg.nszjky.cn

Java: "ab".repeat(3)
来源：http://fp.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://tp.muxihuayi.cn

Ruby: "ab" * 3
来源：http://al.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qa.nicolike.cn

[E03] 截取子串
来源：http://ga.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vn.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wg.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vb.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://ac.colortex.cn

Java: s.substring(1, 4)
来源：http://dk.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jz.nszjky.cn


<!-- 参考信息 -->