代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vo.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ar.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lc.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sl.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ri.9csxet.cn

Go:   func add(a, b int) int
来源：http://sl.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ut.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dq.asd995.cn

[C14] 泛型函数
来源：http://nm.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pw.muxihuayi.cn

PHP:  // 无泛型
来源：http://rh.bookmarksfly.cn

JS:   // 无泛型
来源：http://za.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ke.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xf.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ph.lnxyls.cn

Ruby: # 无泛型
来源：http://cs.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fy.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://jy.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bh.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://ph.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sq.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ao.bookmarksfly.cn

Java: // 无解构
来源：http://eo.chemitech.net.cn

Go:   // 无解构
来源：http://we.bookmarksfly.cn

Ruby: a, b = pair
来源：http://gr.9csxet.cn

C#:   var (a, b) = pair;
来源：http://so.nicolike.cn

[C16] 函数 / 方法重载
来源：http://pf.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tn.shxzskj.cn

PHP:  // 无重载
来源：http://ud.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uv.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://zv.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dw.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://gn.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://vr.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hq.shxzskj.cn

================================================================================
来源：http://ej.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://hv.hnjuh.cn

================================================================================
来源：http://sz.colortex.cn

[D01] 创建数组 / 列表
来源：http://se.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sf.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ga.newstarts.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://at.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lt.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sd.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://xl.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://or.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mw.lnxyls.cn

[D02] 追加元素到末尾
来源：http://hz.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xa.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rw.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://ud.bookmarksfly.cn

TS:   arr.push(4);
来源：http://zb.nicolike.cn

Java: list.add(4);
来源：http://ag.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://yh.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://rg.nszjky.cn

C#:   list.Add(4);
来源：http://ru.nicolike.cn

[D03] 在指定位置插入元素
来源：http://vs.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://jq.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vv.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dn.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://ms.hahajie.cn

Java: list.add(0, 0);
来源：http://fb.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qn.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ez.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://ti.huixiangedu.cn

[D04] 删除元素
来源：http://vz.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jw.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uk.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hr.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://xg.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://os.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sk.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jm.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hg.szsharing.cn

[D05] 访问与修改元素
来源：http://wx.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yi.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qa.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tl.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://qa.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://oh.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://lj.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rf.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rb.gzmigu.cn

[D06] 数组长度
来源：http://pu.521024.cn

Py:   len(arr)
来源：http://kv.yuntaijiaju.cn

PHP:  count($arr);
来源：http://xf.hnjuh.cn

JS:   arr.length
来源：http://wf.chemitech.net.cn

TS:   arr.length
来源：http://ob.9csxet.cn

Java: list.size();
来源：http://mp.asd995.cn

Go:   len(arr)
来源：http://yu.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://wa.huanxung.cn

C#:   list.Count;
来源：http://hd.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://qw.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zg.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jh.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://xn.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://yl.huanxung.cn

Java: list.subList(1, 4);
来源：http://jt.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://ax.gzmigu.cn

Ruby: arr[1, 3]
来源：http://wd.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://ru.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://mg.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://bg.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ky.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dh.wgjwhj.cn

TS:   [...a, ...b];
来源：http://ex.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tn.bjjhwx.cn

Go:   append(a, b...)
来源：http://ek.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://in.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://gp.colortex.cn

[D09] 排序（升序）
来源：http://xy.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://aa.haigaiapp.cn

PHP:  sort($arr);
来源：http://tu.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fu.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://in.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ho.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nz.nszjky.cn

Ruby: arr.sort
来源：http://lv.huanxung.cn

C#:   list.Sort();
来源：http://wt.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uu.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ee.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vk.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ga.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tr.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sa.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yw.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://py.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ji.hahajie.cn

[D11] 反转数组
来源：http://sn.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ln.huanxung.cn

PHP:  array_reverse($arr);
来源：http://tx.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cs.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://xg.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://hh.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://nj.hahajie.cn

Ruby: arr.reverse
来源：http://th.panjiajie.cn

C#:   list.Reverse();
来源：http://qe.muxihuayi.cn

[D12] 查找元素下标
来源：http://et.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://gy.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ay.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oy.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nc.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yy.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://uh.bjjhwx.cn

Ruby: arr.index(x)
来源：http://oe.szsharing.cn

C#:   list.IndexOf(x);
来源：http://da.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://im.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tl.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gj.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://jb.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://cd.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cc.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ir.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ry.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gy.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://sx.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yk.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jz.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://pz.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://lh.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ql.colortex.cn

Go:   // 手写循环
来源：http://zk.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xo.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ex.muxihuayi.cn

[D15] 去重
来源：http://io.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vi.nszjky.cn

PHP:  array_unique($arr);
来源：http://xi.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ln.nicolike.cn

TS:   [...new Set(arr)]
来源：http://fr.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ux.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dp.szxytkj.cn

Ruby: arr.uniq
来源：http://nh.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://ad.521024.cn

[D16] 求和与平均值
来源：http://yi.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://op.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://li.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ks.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hc.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mk.bjjhwx.cn

Go:   // 手写循环累加
来源：http://jt.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ij.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://ev.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://xp.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://wi.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://nm.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://en.newstarts.cn

TS:   Math.max(...arr);
来源：http://ku.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ro.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ol.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://hi.colortex.cn

C#:   list.Max();  list.Min()
来源：http://hm.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://gw.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dk.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://tx.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tt.gzmigu.cn

TS:   nested.flat();
来源：http://di.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sl.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://kn.panjiajie.cn

Ruby: nested.flatten
来源：http://pm.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ms.lnxyls.cn

[D19] 按字段分组
来源：http://aq.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vb.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xa.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bl.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ym.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hr.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://gq.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://md.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oc.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://vh.huanxung.cn

Py:   Counter(arr)
来源：http://fr.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://bn.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ac.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tf.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nv.asd995.cn

Go:   // 手写 map[T]int
来源：http://sx.shxzukj.cn

Ruby: arr.tally
来源：http://sn.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tn.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://et.bjjhwx.cn

Py:   x in arr
来源：http://wt.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://vp.lnxyls.cn

JS:   arr.includes(x)
来源：http://cr.nszjky.cn

TS:   arr.includes(x)
来源：http://vh.gzmigu.cn

Java: list.contains(x)
来源：http://uc.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://cv.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://nj.hnjuh.cn

C#:   list.Contains(x)
来源：http://vv.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ty.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tu.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ei.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tf.panjiajie.cn

TS:   [...arr];
来源：http://sp.521024.cn

Java: new ArrayList<>(list);
来源：http://yu.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oq.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://ai.nicolike.cn

C#:   new List<int>(list);
来源：http://lo.bjjhwx.cn

[D23] reduce 累积计算
来源：http://oe.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xp.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dx.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://os.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vc.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ml.9csxet.cn

Go:   // 手写循环
来源：http://dr.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iy.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ts.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://mz.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sp.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cm.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cw.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://be.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gx.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xp.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://el.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ve.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://dz.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pz.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bb.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rt.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ib.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dg.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hr.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pc.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lt.bjjhwx.cn

[D26] 数组转字符串
来源：http://ba.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://bp.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://sn.nszjky.cn

JS:   arr.join(", ")
来源：http://gn.colortex.cn

TS:   arr.join(", ")
来源：http://al.szsharing.cn

Java: String.join(", ", list)
来源：http://da.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://nh.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://rm.nicolike.cn

C#:   string.Join(", ", list)
来源：http://um.asd995.cn

================================================================================
来源：http://zf.chemitech.net.cn

E. 字符串处理
来源：http://ek.huixinmuqiang.cn

================================================================================
来源：http://cr.shtwfgs.cn

[E01] 拼接字符串
来源：http://ei.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xk.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ya.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ro.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://al.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ny.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ls.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ox.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tk.szsharing.cn

[E02] 重复字符串
来源：http://vj.nicolike.cn

Py:   "ab" * 3
来源：http://ev.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://do.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://ey.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://il.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://ed.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://dq.panjiajie.cn

Ruby: "ab" * 3
来源：http://gx.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://va.haigaiapp.cn

[E03] 截取子串
来源：http://ey.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://di.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ht.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ab.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://nu.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://bo.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ld.shtwfgs.cn


<!-- 参考信息 -->