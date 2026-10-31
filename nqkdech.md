代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nd.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pi.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ua.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ld.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://to.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ju.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kt.muxihuayi.cn

[C14] 泛型函数
来源：http://rb.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dq.muxihuayi.cn

PHP:  // 无泛型
来源：http://ar.chemitech.net.cn

JS:   // 无泛型
来源：http://mm.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pj.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gr.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pn.muxihuayi.cn

Ruby: # 无泛型
来源：http://lz.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kb.nszjky.cn

[C15] 解构 / 展开参数
来源：http://ov.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ju.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://ro.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cr.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qb.szsharing.cn

Java: // 无解构
来源：http://dd.haigaiapp.cn

Go:   // 无解构
来源：http://tw.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://sr.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://xr.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://it.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zo.chemitech.net.cn

PHP:  // 无重载
来源：http://jh.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ab.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://sd.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://za.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://sz.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://qn.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ig.nszjky.cn

================================================================================
来源：http://aq.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://li.shtwfgs.cn

================================================================================
来源：http://ef.9csxet.cn

[D01] 创建数组 / 列表
来源：http://uz.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vl.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://az.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iy.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vd.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gg.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://td.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://gs.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cc.nicolike.cn

[D02] 追加元素到末尾
来源：http://ey.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rn.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qt.nicolike.cn

JS:   arr.push(4);
来源：http://nt.hahajie.cn

TS:   arr.push(4);
来源：http://az.huanxung.cn

Java: list.add(4);
来源：http://zi.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ah.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://nv.colortex.cn

C#:   list.Add(4);
来源：http://sb.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://ri.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://ec.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bk.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zt.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://vf.9csxet.cn

Java: list.add(0, 0);
来源：http://sh.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ws.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lh.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://ym.hahajie.cn

[D04] 删除元素
来源：http://ev.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wh.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fs.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vw.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://ei.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ov.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ij.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rf.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ni.colortex.cn

[D05] 访问与修改元素
来源：http://lr.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wz.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ff.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wx.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://zc.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://lp.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://dg.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fa.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xi.9csxet.cn

[D06] 数组长度
来源：http://au.colortex.cn

Py:   len(arr)
来源：http://md.bjjhwx.cn

PHP:  count($arr);
来源：http://xk.shxzskj.cn

JS:   arr.length
来源：http://tf.muxihuayi.cn

TS:   arr.length
来源：http://lu.yuntaijiaju.cn

Java: list.size();
来源：http://le.bookmarksfly.cn

Go:   len(arr)
来源：http://we.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://ak.wgjwhj.cn

C#:   list.Count;
来源：http://cf.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://rp.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ru.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nz.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://oh.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://ag.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://ri.nicolike.cn

Go:   arr[1:4]
来源：http://fr.shxzskj.cn

Ruby: arr[1, 3]
来源：http://oy.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://hs.muxihuayi.cn

[D08] 合并两个数组
来源：http://ss.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://fu.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://ex.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://se.colortex.cn

TS:   [...a, ...b];
来源：http://gz.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://do.shxzukj.cn

Go:   append(a, b...)
来源：http://cq.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://ku.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://nm.asd995.cn

[D09] 排序（升序）
来源：http://if.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://gz.jctech888.com.cn

PHP:  sort($arr);
来源：http://jl.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hw.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lm.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tp.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://en.shxzukj.cn

Ruby: arr.sort
来源：http://jk.szxytkj.cn

C#:   list.Sort();
来源：http://au.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bm.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tm.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://et.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xh.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qd.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bd.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tb.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nb.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qf.huixiangedu.cn

[D11] 反转数组
来源：http://qy.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bx.huanxung.cn

PHP:  array_reverse($arr);
来源：http://du.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mv.nicolike.cn

TS:   [...arr].reverse();
来源：http://mw.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://ga.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://ro.haigaiapp.cn

Ruby: arr.reverse
来源：http://ra.hahajie.cn

C#:   list.Reverse();
来源：http://yi.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://mz.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://xg.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ka.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://is.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oj.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xk.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://uu.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://hw.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://gq.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://ok.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zj.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dz.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://fn.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://tm.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sq.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vf.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://el.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ta.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://me.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xs.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mz.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://kv.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://jf.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ev.jctech888.com.cn

Go:   // 手写循环
来源：http://el.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ji.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://is.9csxet.cn

[D15] 去重
来源：http://dl.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yy.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://mw.nicolike.cn

JS:   [...new Set(arr)]
来源：http://rs.newstarts.cn

TS:   [...new Set(arr)]
来源：http://uk.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://za.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://az.newstarts.cn

Ruby: arr.uniq
来源：http://qi.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://uo.newstarts.cn

[D16] 求和与平均值
来源：http://pt.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://im.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vz.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fa.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mr.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gl.shxzskj.cn

Go:   // 手写循环累加
来源：http://ac.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hm.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://zm.asd995.cn

[D17] 最大值与最小值
来源：http://dh.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://zu.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://tj.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wk.colortex.cn

TS:   Math.max(...arr);
来源：http://be.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bb.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hv.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://eg.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://ky.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://um.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gi.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://ur.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hn.shxzukj.cn

TS:   nested.flat();
来源：http://da.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://em.521024.cn

Go:   // 手写双层循环
来源：http://wl.colortex.cn

Ruby: nested.flatten
来源：http://cv.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qo.szsharing.cn

[D19] 按字段分组
来源：http://ye.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://al.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rb.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pt.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mf.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yr.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://ed.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://am.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lc.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://em.lnxyls.cn

Py:   Counter(arr)
来源：http://jp.asd995.cn

PHP:  array_count_values($arr);
来源：http://ne.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lf.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wj.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ai.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://ii.bjjhwx.cn

Ruby: arr.tally
来源：http://jr.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vh.asd995.cn

[D21] 判断是否包含某元素
来源：http://qd.shxzskj.cn

Py:   x in arr
来源：http://ew.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://bd.bjjhwx.cn

JS:   arr.includes(x)
来源：http://qb.gzmigu.cn

TS:   arr.includes(x)
来源：http://uj.yuntaijiaju.cn

Java: list.contains(x)
来源：http://ob.521024.cn

Go:   slices.Contains(arr, x)
来源：http://dw.hnjuh.cn

Ruby: arr.include?(x)
来源：http://fo.muxihuayi.cn

C#:   list.Contains(x)
来源：http://ju.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://bp.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mm.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zg.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mu.jctech888.com.cn

TS:   [...arr];
来源：http://ya.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://lz.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lc.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://ym.shxzskj.cn

C#:   new List<int>(list);
来源：http://mm.shxzukj.cn

[D23] reduce 累积计算
来源：http://ki.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ei.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ng.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vr.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kr.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bq.521024.cn

Go:   // 手写循环
来源：http://ua.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nq.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nu.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://td.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pn.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dn.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ev.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hk.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aa.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dm.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://is.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rc.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://oc.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pl.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ep.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vb.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wz.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wl.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://un.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tl.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mk.gzmigu.cn

[D26] 数组转字符串
来源：http://lu.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://hl.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://kx.shxzskj.cn

JS:   arr.join(", ")
来源：http://tv.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://xr.szsharing.cn

Java: String.join(", ", list)
来源：http://ve.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://zi.gzmigu.cn

Ruby: arr.join(", ")
来源：http://fa.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://bk.9csxet.cn

================================================================================
来源：http://vf.huixiangedu.cn

E. 字符串处理
来源：http://iw.yuexingan06.cn

================================================================================
来源：http://ib.shxzskj.cn

[E01] 拼接字符串
来源：http://dc.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lw.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vy.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kh.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ze.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hx.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ra.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vx.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yn.nicolike.cn

[E02] 重复字符串
来源：http://xg.szxytkj.cn

Py:   "ab" * 3
来源：http://ck.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://ms.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://kt.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://th.shxzukj.cn

Java: "ab".repeat(3)
来源：http://bo.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://nc.shtwfgs.cn

Ruby: "ab" * 3
来源：http://af.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://th.yuntaijiaju.cn

[E03] 截取子串
来源：http://xg.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rt.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ux.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wd.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://to.521024.cn

Java: s.substring(1, 4)
来源：http://go.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bh.lnxyls.cn


<!-- 参考信息 -->