代发 wailian999

[C14] 泛型函数
来源：http://lc.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bi.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://yw.colortex.cn

JS:   // 无泛型
来源：http://pq.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ew.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zo.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jz.huanxung.cn

Ruby: # 无泛型
来源：http://zd.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qg.hahajie.cn

[C15] 解构 / 展开参数
来源：http://mb.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://br.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://wm.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hs.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ze.nszjky.cn

Java: // 无解构
来源：http://nv.nszjky.cn

Go:   // 无解构
来源：http://dh.haigaiapp.cn

Ruby: a, b = pair
来源：http://di.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://nd.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://bn.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rf.shxzukj.cn

PHP:  // 无重载
来源：http://vw.nicolike.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uv.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://bu.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ml.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://rd.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://xu.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cq.szxytkj.cn

================================================================================
来源：http://gx.asd995.cn

D. 数组 / 列表 / 集合
来源：http://ae.hnjuh.cn

================================================================================
来源：http://hs.szsharing.cn

[D01] 创建数组 / 列表
来源：http://pn.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://we.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kz.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ec.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dt.shtwfgs.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qw.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://qs.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://hn.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xk.huanxung.cn

[D02] 追加元素到末尾
来源：http://ki.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qi.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kg.panjiajie.cn

JS:   arr.push(4);
来源：http://ci.muxihuayi.cn

TS:   arr.push(4);
来源：http://rb.szxytkj.cn

Java: list.add(4);
来源：http://xp.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://cn.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://qr.jctech888.com.cn

C#:   list.Add(4);
来源：http://rg.newstarts.cn

[D03] 在指定位置插入元素
来源：http://rr.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://bd.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bg.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lh.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://pi.chemitech.net.cn

Java: list.add(0, 0);
来源：http://op.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://az.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rx.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://fx.521024.cn

[D04] 删除元素
来源：http://oo.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wa.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pa.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://as.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://kh.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ts.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vm.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mj.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tf.bjjhwx.cn

[D05] 访问与修改元素
来源：http://bt.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uz.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rt.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dv.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://lu.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://ff.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://bs.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wh.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hl.shtwfgs.cn

[D06] 数组长度
来源：http://vr.huanxung.cn

Py:   len(arr)
来源：http://cj.huixiangedu.cn

PHP:  count($arr);
来源：http://ux.colortex.cn

JS:   arr.length
来源：http://yx.colortex.cn

TS:   arr.length
来源：http://ck.lnxyls.cn

Java: list.size();
来源：http://qo.hnjuh.cn

Go:   len(arr)
来源：http://wl.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://yu.lnxyls.cn

C#:   list.Count;
来源：http://tz.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://te.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qs.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aw.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://if.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://gk.lnxyls.cn

Java: list.subList(1, 4);
来源：http://os.hnjuh.cn

Go:   arr[1:4]
来源：http://uy.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://si.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://ln.szsharing.cn

[D08] 合并两个数组
来源：http://le.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://bf.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://yp.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yf.nicolike.cn

TS:   [...a, ...b];
来源：http://pp.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mr.newstarts.cn

Go:   append(a, b...)
来源：http://pa.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://zm.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://bh.yuexingan06.cn

[D09] 排序（升序）
来源：http://lw.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sy.9csxet.cn

PHP:  sort($arr);
来源：http://bc.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tm.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ti.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kw.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wr.szxytkj.cn

Ruby: arr.sort
来源：http://ln.szxytkj.cn

C#:   list.Sort();
来源：http://sw.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xg.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qb.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ef.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jd.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ik.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ck.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rx.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vl.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://on.lnxyls.cn

[D11] 反转数组
来源：http://bz.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zu.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://wk.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vn.nszjky.cn

TS:   [...arr].reverse();
来源：http://wu.newstarts.cn

Java: Collections.reverse(list);
来源：http://qm.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://cc.yuexingan06.cn

Ruby: arr.reverse
来源：http://br.szsharing.cn

C#:   list.Reverse();
来源：http://se.nszjky.cn

[D12] 查找元素下标
来源：http://vi.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://ws.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ch.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wl.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://of.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yj.asd995.cn

Go:   slices.Index(arr, x)
来源：http://qr.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://qv.521024.cn

C#:   list.IndexOf(x);
来源：http://jq.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://je.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fu.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uu.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://ob.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://gt.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xy.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bt.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kp.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pg.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://pk.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gn.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://da.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://wp.521024.cn

TS:   arr.map(x => x * 2)
来源：http://hu.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://no.colortex.cn

Go:   // 手写循环
来源：http://gy.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ti.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lj.huixiangedu.cn

[D15] 去重
来源：http://nj.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ek.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://cj.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://of.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://nl.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lp.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pu.szxytkj.cn

Ruby: arr.uniq
来源：http://eh.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ex.wgjwhj.cn

[D16] 求和与平均值
来源：http://pn.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kl.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xw.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tg.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gv.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ul.hnjuh.cn

Go:   // 手写循环累加
来源：http://pq.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mu.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://cq.muxihuayi.cn

[D17] 最大值与最小值
来源：http://ob.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://dq.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://im.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rk.huanxung.cn

TS:   Math.max(...arr);
来源：http://cn.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bi.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tx.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://sv.asd995.cn

C#:   list.Max();  list.Min()
来源：http://na.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://ej.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ah.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://ym.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bn.gzmigu.cn

TS:   nested.flat();
来源：http://lh.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ns.nicolike.cn

Go:   // 手写双层循环
来源：http://ev.hahajie.cn

Ruby: nested.flatten
来源：http://kd.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xl.nszjky.cn

[D19] 按字段分组
来源：http://rk.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oe.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pf.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tb.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pj.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nb.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://df.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yd.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bz.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://bk.nszjky.cn

Py:   Counter(arr)
来源：http://dw.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://kr.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://av.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zz.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oc.521024.cn

Go:   // 手写 map[T]int
来源：http://zz.nicolike.cn

Ruby: arr.tally
来源：http://qe.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jz.newstarts.cn

[D21] 判断是否包含某元素
来源：http://gt.huixiangedu.cn

Py:   x in arr
来源：http://ow.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://xm.lnxyls.cn

JS:   arr.includes(x)
来源：http://gm.521024.cn

TS:   arr.includes(x)
来源：http://qg.colortex.cn

Java: list.contains(x)
来源：http://tz.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://jz.nszjky.cn

Ruby: arr.include?(x)
来源：http://je.yuexingan06.cn

C#:   list.Contains(x)
来源：http://yo.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://wt.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wj.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jm.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bh.chemitech.net.cn

TS:   [...arr];
来源：http://ny.nicolike.cn

Java: new ArrayList<>(list);
来源：http://gf.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iu.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://zu.huanxung.cn

C#:   new List<int>(list);
来源：http://fh.lnxyls.cn

[D23] reduce 累积计算
来源：http://wf.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mh.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gw.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://si.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kx.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://us.yuntaijiaju.cn

Go:   // 手写循环
来源：http://wp.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fb.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wj.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://hj.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ke.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gb.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ek.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zf.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fr.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tr.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rs.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tu.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ea.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ic.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gl.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mw.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://if.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ms.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://im.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fm.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cu.huixiangedu.cn

[D26] 数组转字符串
来源：http://iq.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://gi.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://lk.hahajie.cn

JS:   arr.join(", ")
来源：http://jl.haigaiapp.cn

TS:   arr.join(", ")
来源：http://ih.muxihuayi.cn

Java: String.join(", ", list)
来源：http://zl.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://pa.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://zl.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://gr.muxihuayi.cn

================================================================================
来源：http://vq.wgjwhj.cn

E. 字符串处理
来源：http://qb.gzmigu.cn

================================================================================
来源：http://xa.panjiajie.cn

[E01] 拼接字符串
来源：http://lp.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jk.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hx.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fm.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jl.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cm.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yw.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dq.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fw.yuexingan06.cn

[E02] 重复字符串
来源：http://ef.huanxung.cn

Py:   "ab" * 3
来源：http://we.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://ln.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://iv.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://wa.nszjky.cn

Java: "ab".repeat(3)
来源：http://ek.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://vg.newstarts.cn

Ruby: "ab" * 3
来源：http://yo.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jw.521024.cn

[E03] 截取子串
来源：http://il.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yv.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qu.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wa.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://yg.521024.cn

Java: s.substring(1, 4)
来源：http://zq.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eq.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pa.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://bm.bookmarksfly.cn

[E04] 查找子串位置
来源：http://cs.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://al.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://od.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yw.asd995.cn

TS:   s.indexOf("x")
来源：http://rg.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://xh.huixinmuqiang.cn


<!-- 参考信息 -->