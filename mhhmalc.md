代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://jk.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://hk.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bg.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pf.yuexingan06.cn

[C14] 泛型函数
来源：http://of.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tj.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://no.jctech888.com.cn

JS:   // 无泛型
来源：http://it.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rl.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eo.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wt.yuexingan06.cn

Ruby: # 无泛型
来源：http://uz.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nl.nszjky.cn

[C15] 解构 / 展开参数
来源：http://mx.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gq.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://yb.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jq.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ce.nicolike.cn

Java: // 无解构
来源：http://xv.huanxung.cn

Go:   // 无解构
来源：http://sz.asd995.cn

Ruby: a, b = pair
来源：http://fw.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://wa.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://mq.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://an.bookmarksfly.cn

PHP:  // 无重载
来源：http://ds.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ov.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://ks.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://is.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://jp.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://xi.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ob.shxzskj.cn

================================================================================
来源：http://wd.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://kc.jianghongdianzi.cn

================================================================================
来源：http://tl.nszjky.cn

[D01] 创建数组 / 列表
来源：http://ui.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xx.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ye.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cb.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qd.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zv.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://lc.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://om.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://na.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://eg.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rz.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pm.panjiajie.cn

JS:   arr.push(4);
来源：http://rb.wgjwhj.cn

TS:   arr.push(4);
来源：http://bb.szxytkj.cn

Java: list.add(4);
来源：http://tr.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://hm.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://an.bookmarksfly.cn

C#:   list.Add(4);
来源：http://xn.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://fn.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://vv.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://af.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zo.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://wb.szsharing.cn

Java: list.add(0, 0);
来源：http://xy.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tc.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://up.asd995.cn

C#:   list.Insert(0, 0);
来源：http://wn.panjiajie.cn

[D04] 删除元素
来源：http://zz.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yl.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zc.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zk.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://iy.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pz.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ey.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cn.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xi.bjjhwx.cn

[D05] 访问与修改元素
来源：http://vd.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wn.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dd.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rs.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://ys.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://se.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://ge.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uy.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fp.yuexingan06.cn

[D06] 数组长度
来源：http://dc.shxzukj.cn

Py:   len(arr)
来源：http://ok.bookmarksfly.cn

PHP:  count($arr);
来源：http://hr.gzmigu.cn

JS:   arr.length
来源：http://ig.huixinmuqiang.cn

TS:   arr.length
来源：http://am.yuexingan06.cn

Java: list.size();
来源：http://xn.yuntaijiaju.cn

Go:   len(arr)
来源：http://st.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://mb.lnxyls.cn

C#:   list.Count;
来源：http://yr.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://iu.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vm.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pm.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://ag.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://ez.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://eu.shxzukj.cn

Go:   arr[1:4]
来源：http://td.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://hg.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://fc.lnxyls.cn

[D08] 合并两个数组
来源：http://jh.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://ey.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://ax.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iq.newstarts.cn

TS:   [...a, ...b];
来源：http://qn.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ud.szxytkj.cn

Go:   append(a, b...)
来源：http://sr.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://hp.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://rw.nicolike.cn

[D09] 排序（升序）
来源：http://qf.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://en.szsharing.cn

PHP:  sort($arr);
来源：http://db.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hr.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://in.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://og.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xa.yuntaijiaju.cn

Ruby: arr.sort
来源：http://sy.yuntaijiaju.cn

C#:   list.Sort();
来源：http://fc.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vs.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ab.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://np.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kz.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sq.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ce.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jh.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ne.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xp.jianghongdianzi.cn

[D11] 反转数组
来源：http://wf.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bw.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://kd.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xj.panjiajie.cn

TS:   [...arr].reverse();
来源：http://zc.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://cq.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://qp.colortex.cn

Ruby: arr.reverse
来源：http://yn.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://ag.bjjhwx.cn

[D12] 查找元素下标
来源：http://za.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://cq.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kc.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kf.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aq.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hf.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://vr.newstarts.cn

Ruby: arr.index(x)
来源：http://jf.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ej.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://ny.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dr.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cb.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://yf.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://bv.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yi.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jj.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://og.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cz.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://gw.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xu.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tg.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://dy.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://it.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zx.9csxet.cn

Go:   // 手写循环
来源：http://hz.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yi.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mr.bookmarksfly.cn

[D15] 去重
来源：http://sn.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qo.asd995.cn

PHP:  array_unique($arr);
来源：http://gt.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://mg.hahajie.cn

TS:   [...new Set(arr)]
来源：http://it.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pa.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zo.hnjuh.cn

Ruby: arr.uniq
来源：http://eq.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://aj.shxzskj.cn

[D16] 求和与平均值
来源：http://ku.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wu.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jw.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ro.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ke.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nx.huixiangedu.cn

Go:   // 手写循环累加
来源：http://aa.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pg.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://kf.szxytkj.cn

[D17] 最大值与最小值
来源：http://wz.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://ri.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://ys.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rc.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://ah.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qz.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zw.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://bn.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://jv.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://zw.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rl.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://uk.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fq.shtwfgs.cn

TS:   nested.flat();
来源：http://ls.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ab.521024.cn

Go:   // 手写双层循环
来源：http://te.colortex.cn

Ruby: nested.flatten
来源：http://pc.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mc.9csxet.cn

[D19] 按字段分组
来源：http://vh.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vl.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hv.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iy.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://um.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xs.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://cn.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zu.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wx.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://pw.bookmarksfly.cn

Py:   Counter(arr)
来源：http://ic.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://qs.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qp.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ji.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://yg.muxihuayi.cn

Ruby: arr.tally
来源：http://vg.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uw.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://hn.asd995.cn

Py:   x in arr
来源：http://om.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://nm.nicolike.cn

JS:   arr.includes(x)
来源：http://bu.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://hs.panjiajie.cn

Java: list.contains(x)
来源：http://rg.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://vi.szxytkj.cn

Ruby: arr.include?(x)
来源：http://hp.gzmigu.cn

C#:   list.Contains(x)
来源：http://jv.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://hf.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yy.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ey.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tp.panjiajie.cn

TS:   [...arr];
来源：http://sr.huanxung.cn

Java: new ArrayList<>(list);
来源：http://va.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iy.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://rh.szsharing.cn

C#:   new List<int>(list);
来源：http://ey.muxihuayi.cn

[D23] reduce 累积计算
来源：http://zb.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nc.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://le.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bu.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tr.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xu.bookmarksfly.cn

Go:   // 手写循环
来源：http://co.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tk.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dg.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://al.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://th.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kk.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zb.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bg.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yo.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gc.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xz.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nh.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://or.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ju.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rf.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yv.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yp.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ub.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fl.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wu.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gb.nszjky.cn

[D26] 数组转字符串
来源：http://zv.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://mc.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://kc.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://xt.nszjky.cn

TS:   arr.join(", ")
来源：http://ak.shxzskj.cn

Java: String.join(", ", list)
来源：http://ha.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://kn.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://sj.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://tg.hahajie.cn

================================================================================
来源：http://yw.huixinmuqiang.cn

E. 字符串处理
来源：http://xm.9csxet.cn

================================================================================
来源：http://ef.panjiajie.cn

[E01] 拼接字符串
来源：http://qw.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dg.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sh.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fc.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fk.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fz.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://df.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ir.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nj.haigaiapp.cn

[E02] 重复字符串
来源：http://ut.shxzukj.cn

Py:   "ab" * 3
来源：http://py.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://oq.521024.cn

JS:   "ab".repeat(3)
来源：http://hm.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://gs.nszjky.cn

Java: "ab".repeat(3)
来源：http://lp.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://kv.jctech888.com.cn

Ruby: "ab" * 3
来源：http://rx.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oz.yuexingan06.cn

[E03] 截取子串
来源：http://nz.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eu.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yw.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yy.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://tr.shxzukj.cn

Java: s.substring(1, 4)
来源：http://on.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vu.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tf.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://ja.gzmigu.cn

[E04] 查找子串位置
来源：http://gr.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://az.panjiajie.cn


<!-- 参考信息 -->