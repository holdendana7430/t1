代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yo.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vd.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yj.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sz.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ff.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://fc.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bt.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hn.bjjhwx.cn

[C14] 泛型函数
来源：http://uf.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sy.nicolike.cn

PHP:  // 无泛型
来源：http://hh.jctech888.com.cn

JS:   // 无泛型
来源：http://zv.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xy.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mc.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nj.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://yz.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ik.colortex.cn

[C15] 解构 / 展开参数
来源：http://cd.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sa.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://me.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://np.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tb.haigaiapp.cn

Java: // 无解构
来源：http://yr.9csxet.cn

Go:   // 无解构
来源：http://xt.szsharing.cn

Ruby: a, b = pair
来源：http://je.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://ys.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://cj.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bs.bjjhwx.cn

PHP:  // 无重载
来源：http://hi.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fh.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://jh.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lt.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://lo.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://zx.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gh.colortex.cn

================================================================================
来源：http://cd.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://hq.9csxet.cn

================================================================================
来源：http://zu.huanxung.cn

[D01] 创建数组 / 列表
来源：http://fa.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lz.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oc.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://du.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zz.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tn.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://de.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://bp.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aj.panjiajie.cn

[D02] 追加元素到末尾
来源：http://rv.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xr.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hy.muxihuayi.cn

JS:   arr.push(4);
来源：http://pi.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://oz.yuexingan06.cn

Java: list.add(4);
来源：http://pd.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://mc.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://yu.9csxet.cn

C#:   list.Add(4);
来源：http://mt.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://nm.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://ha.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dm.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mr.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ms.shxzukj.cn

Java: list.add(0, 0);
来源：http://hc.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sx.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ks.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://fq.shxzskj.cn

[D04] 删除元素
来源：http://xz.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lv.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hy.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fc.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://rz.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://co.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vt.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fn.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ig.yuexingan06.cn

[D05] 访问与修改元素
来源：http://wq.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://su.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iv.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mz.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ed.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://yz.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://hv.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lw.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://za.nszjky.cn

[D06] 数组长度
来源：http://oz.huanxung.cn

Py:   len(arr)
来源：http://sg.jctech888.com.cn

PHP:  count($arr);
来源：http://zz.huixinmuqiang.cn

JS:   arr.length
来源：http://tq.lnxyls.cn

TS:   arr.length
来源：http://qq.gzmigu.cn

Java: list.size();
来源：http://zh.yuntaijiaju.cn

Go:   len(arr)
来源：http://sl.nicolike.cn

Ruby: arr.length; arr.size
来源：http://bh.nszjky.cn

C#:   list.Count;
来源：http://ef.nicolike.cn

[D07] 切片 / 取子数组
来源：http://ty.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nf.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://on.colortex.cn

JS:   arr.slice(1, 4);
来源：http://op.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://gi.521024.cn

Java: list.subList(1, 4);
来源：http://hv.huixiangedu.cn

Go:   arr[1:4]
来源：http://jc.hnjuh.cn

Ruby: arr[1, 3]
来源：http://lb.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://kr.asd995.cn

[D08] 合并两个数组
来源：http://vn.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://zq.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://zv.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vl.9csxet.cn

TS:   [...a, ...b];
来源：http://oa.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fa.huanxung.cn

Go:   append(a, b...)
来源：http://cg.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://pf.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://fv.bookmarksfly.cn

[D09] 排序（升序）
来源：http://ne.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://xa.bjjhwx.cn

PHP:  sort($arr);
来源：http://bj.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ht.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gc.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jl.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qt.9csxet.cn

Ruby: arr.sort
来源：http://ik.nszjky.cn

C#:   list.Sort();
来源：http://aj.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fv.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ik.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qu.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gn.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://se.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ec.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://la.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ar.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nc.asd995.cn

[D11] 反转数组
来源：http://ni.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hk.nicolike.cn

PHP:  array_reverse($arr);
来源：http://il.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rp.lnxyls.cn

TS:   [...arr].reverse();
来源：http://hk.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://zx.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://qk.newstarts.cn

Ruby: arr.reverse
来源：http://mc.muxihuayi.cn

C#:   list.Reverse();
来源：http://oa.chemitech.net.cn

[D12] 查找元素下标
来源：http://fs.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://bu.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gb.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vo.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xg.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lk.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://na.hnjuh.cn

Ruby: arr.index(x)
来源：http://ia.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://ir.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://md.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xc.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://by.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://fv.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://uf.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hb.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://et.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://li.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://th.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://ca.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yt.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fv.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ye.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://kc.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wx.hahajie.cn

Go:   // 手写循环
来源：http://ih.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sv.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zw.szsharing.cn

[D15] 去重
来源：http://ne.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://is.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://bw.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://gv.9csxet.cn

TS:   [...new Set(arr)]
来源：http://bn.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lv.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sh.gzmigu.cn

Ruby: arr.uniq
来源：http://zp.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ew.shtwfgs.cn

[D16] 求和与平均值
来源：http://qh.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tn.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fm.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mm.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gs.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wm.szxytkj.cn

Go:   // 手写循环累加
来源：http://lh.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iw.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ow.panjiajie.cn

[D17] 最大值与最小值
来源：http://ut.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://ve.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://qx.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xn.hnjuh.cn

TS:   Math.max(...arr);
来源：http://ns.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jz.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aa.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://wv.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://vb.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://hv.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mj.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://yc.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nj.huixiangedu.cn

TS:   nested.flat();
来源：http://py.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://si.huanxung.cn

Go:   // 手写双层循环
来源：http://uh.jctech888.com.cn

Ruby: nested.flatten
来源：http://px.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tl.yuntaijiaju.cn

[D19] 按字段分组
来源：http://az.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tl.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ji.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ti.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fq.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xm.panjiajie.cn

Go:   // 手写 map[string][]T
来源：http://hg.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bc.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cj.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://xy.huixiangedu.cn

Py:   Counter(arr)
来源：http://lh.hahajie.cn

PHP:  array_count_values($arr);
来源：http://hl.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zk.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uf.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://il.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://ik.gzmigu.cn

Ruby: arr.tally
来源：http://wv.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ng.huanxung.cn

[D21] 判断是否包含某元素
来源：http://jc.panjiajie.cn

Py:   x in arr
来源：http://tl.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://bd.shtwfgs.cn

JS:   arr.includes(x)
来源：http://nh.hnjuh.cn

TS:   arr.includes(x)
来源：http://rm.nicolike.cn

Java: list.contains(x)
来源：http://zs.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://so.huanxung.cn

Ruby: arr.include?(x)
来源：http://ck.chemitech.net.cn

C#:   list.Contains(x)
来源：http://vc.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://zx.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wm.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mf.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cl.nicolike.cn

TS:   [...arr];
来源：http://vr.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://fg.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ci.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://iz.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://ir.hahajie.cn

[D23] reduce 累积计算
来源：http://vt.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pg.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ao.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fd.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mm.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gh.haigaiapp.cn

Go:   // 手写循环
来源：http://sm.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fz.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ij.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://to.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gg.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://of.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://za.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tv.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://py.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wf.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rx.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zb.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://gi.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mz.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jv.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://on.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ku.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ap.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zc.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xp.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jb.wgjwhj.cn

[D26] 数组转字符串
来源：http://bo.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://fc.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://jp.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://mq.shtwfgs.cn

TS:   arr.join(", ")
来源：http://cf.nszjky.cn

Java: String.join(", ", list)
来源：http://yu.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://cw.asd995.cn

Ruby: arr.join(", ")
来源：http://kf.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://oo.colortex.cn

================================================================================
来源：http://oq.jctech888.com.cn

E. 字符串处理
来源：http://dy.jctech888.com.cn

================================================================================
来源：http://rx.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://ms.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hl.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xo.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ve.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wc.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://we.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pw.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://za.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uw.haigaiapp.cn

[E02] 重复字符串
来源：http://jz.nicolike.cn

Py:   "ab" * 3
来源：http://gh.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://in.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://nv.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://wu.gzmigu.cn

Java: "ab".repeat(3)
来源：http://ne.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://gg.shxzukj.cn

Ruby: "ab" * 3
来源：http://lt.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lz.nicolike.cn

[E03] 截取子串
来源：http://mp.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ik.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iz.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xg.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://ge.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://zz.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cj.gzmigu.cn


<!-- 参考信息 -->