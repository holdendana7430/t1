代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://ag.nicolike.cn

Go:   func add(a, b int) int
来源：http://mt.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cd.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ky.521024.cn

[C14] 泛型函数
来源：http://jr.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hj.shxzskj.cn

PHP:  // 无泛型
来源：http://iq.jianghongdianzi.cn

JS:   // 无泛型
来源：http://su.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wm.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ex.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iq.haigaiapp.cn

Ruby: # 无泛型
来源：http://jn.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bv.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://ve.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ql.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://rt.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xy.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ll.shxzukj.cn

Java: // 无解构
来源：http://mm.muxihuayi.cn

Go:   // 无解构
来源：http://ww.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://hi.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://gy.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://jl.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dg.yuexingan06.cn

PHP:  // 无重载
来源：http://kl.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sc.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://hf.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hq.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://wg.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://ht.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ul.huixiangedu.cn

================================================================================
来源：http://vj.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://kg.shxzukj.cn

================================================================================
来源：http://cq.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://tk.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xx.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lz.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ts.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mr.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eb.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://or.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://qi.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://el.lnxyls.cn

[D02] 追加元素到末尾
来源：http://vf.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jz.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uj.colortex.cn

JS:   arr.push(4);
来源：http://en.yuexingan06.cn

TS:   arr.push(4);
来源：http://gp.huixiangedu.cn

Java: list.add(4);
来源：http://ll.521024.cn

Go:   arr = append(arr, 4)
来源：http://wu.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://rd.shxzskj.cn

C#:   list.Add(4);
来源：http://lm.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://yl.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://yv.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gz.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qc.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://gx.nicolike.cn

Java: list.add(0, 0);
来源：http://hb.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jw.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://te.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://va.shxzskj.cn

[D04] 删除元素
来源：http://xp.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uc.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ng.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xq.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://ni.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://le.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uw.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nh.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://me.colortex.cn

[D05] 访问与修改元素
来源：http://vh.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wo.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gt.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ia.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://kk.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://qc.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://mj.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qy.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sa.lnxyls.cn

[D06] 数组长度
来源：http://bu.nicolike.cn

Py:   len(arr)
来源：http://by.haigaiapp.cn

PHP:  count($arr);
来源：http://ow.shxzskj.cn

JS:   arr.length
来源：http://tn.bjjhwx.cn

TS:   arr.length
来源：http://tx.shxzukj.cn

Java: list.size();
来源：http://so.gzmigu.cn

Go:   len(arr)
来源：http://sf.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://ji.huanxung.cn

C#:   list.Count;
来源：http://ry.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://bs.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ty.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hu.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://bm.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://lw.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://tj.nszjky.cn

Go:   arr[1:4]
来源：http://di.szsharing.cn

Ruby: arr[1, 3]
来源：http://al.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://dn.521024.cn

[D08] 合并两个数组
来源：http://jp.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://re.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://yp.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vf.hahajie.cn

TS:   [...a, ...b];
来源：http://ld.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fz.9csxet.cn

Go:   append(a, b...)
来源：http://yt.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://am.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://ko.bookmarksfly.cn

[D09] 排序（升序）
来源：http://gd.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sq.hahajie.cn

PHP:  sort($arr);
来源：http://ek.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pk.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fx.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uo.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ve.colortex.cn

Ruby: arr.sort
来源：http://hs.colortex.cn

C#:   list.Sort();
来源：http://je.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jo.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://en.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vn.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rm.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pc.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xu.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vj.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ab.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fj.huixinmuqiang.cn

[D11] 反转数组
来源：http://ww.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dc.521024.cn

PHP:  array_reverse($arr);
来源：http://ru.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hl.hahajie.cn

TS:   [...arr].reverse();
来源：http://nq.panjiajie.cn

Java: Collections.reverse(list);
来源：http://fm.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://xz.bookmarksfly.cn

Ruby: arr.reverse
来源：http://he.wgjwhj.cn

C#:   list.Reverse();
来源：http://xa.chemitech.net.cn

[D12] 查找元素下标
来源：http://kp.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://db.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://op.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nn.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lx.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hk.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://hn.szxytkj.cn

Ruby: arr.index(x)
来源：http://nj.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://qi.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://jw.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cd.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ga.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://sj.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://an.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wv.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cp.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gh.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dx.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://le.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vs.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vj.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://tn.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://nj.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yx.wgjwhj.cn

Go:   // 手写循环
来源：http://om.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wc.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wu.yuntaijiaju.cn

[D15] 去重
来源：http://cm.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sl.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://rq.hahajie.cn

JS:   [...new Set(arr)]
来源：http://eo.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://qq.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ch.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://um.szsharing.cn

Ruby: arr.uniq
来源：http://lm.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://qx.gzmigu.cn

[D16] 求和与平均值
来源：http://op.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ch.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dj.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zb.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gz.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bs.szsharing.cn

Go:   // 手写循环累加
来源：http://te.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nr.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://gd.szsharing.cn

[D17] 最大值与最小值
来源：http://dt.521024.cn

Py:   max(arr);  min(arr)
来源：http://om.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://ul.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tk.hnjuh.cn

TS:   Math.max(...arr);
来源：http://fl.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dz.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://au.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://ou.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://fr.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://wd.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xl.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://zj.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://id.nszjky.cn

TS:   nested.flat();
来源：http://dg.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://so.newstarts.cn

Go:   // 手写双层循环
来源：http://fp.nicolike.cn

Ruby: nested.flatten
来源：http://st.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pt.yuntaijiaju.cn

[D19] 按字段分组
来源：http://fz.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jh.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dc.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uy.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eo.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oo.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://oz.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sv.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bk.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://ip.huixiangedu.cn

Py:   Counter(arr)
来源：http://wg.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://ii.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zp.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zy.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://al.9csxet.cn

Go:   // 手写 map[T]int
来源：http://ib.huixiangedu.cn

Ruby: arr.tally
来源：http://hn.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gf.szsharing.cn

[D21] 判断是否包含某元素
来源：http://qd.wgjwhj.cn

Py:   x in arr
来源：http://ig.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://up.wgjwhj.cn

JS:   arr.includes(x)
来源：http://ss.hahajie.cn

TS:   arr.includes(x)
来源：http://sb.szsharing.cn

Java: list.contains(x)
来源：http://fy.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://vo.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://rw.jctech888.com.cn

C#:   list.Contains(x)
来源：http://tq.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://vi.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kx.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://za.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gz.yuntaijiaju.cn

TS:   [...arr];
来源：http://yw.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://mj.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dv.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://ne.jctech888.com.cn

C#:   new List<int>(list);
来源：http://tc.521024.cn

[D23] reduce 累积计算
来源：http://ap.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jc.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vr.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://od.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rw.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ls.nszjky.cn

Go:   // 手写循环
来源：http://ao.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bv.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ua.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://lr.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hw.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kj.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://la.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yr.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dx.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zw.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jz.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rh.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://eg.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ho.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://my.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dm.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gk.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hq.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zh.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kn.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ng.hnjuh.cn

[D26] 数组转字符串
来源：http://bc.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ar.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://bo.chemitech.net.cn

JS:   arr.join(", ")
来源：http://ii.huanxung.cn

TS:   arr.join(", ")
来源：http://wo.asd995.cn

Java: String.join(", ", list)
来源：http://hv.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://jk.newstarts.cn

Ruby: arr.join(", ")
来源：http://my.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://rg.nicolike.cn

================================================================================
来源：http://pr.bjjhwx.cn

E. 字符串处理
来源：http://bo.nszjky.cn

================================================================================
来源：http://qg.szxytkj.cn

[E01] 拼接字符串
来源：http://bw.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pz.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qh.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jj.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iq.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://js.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oh.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pj.shtwfgs.cn

[E02] 重复字符串
来源：http://af.nicolike.cn

Py:   "ab" * 3
来源：http://oe.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://fm.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://yp.hahajie.cn

TS:   "ab".repeat(3)
来源：http://lu.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://bw.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://xx.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://lo.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jn.521024.cn

[E03] 截取子串
来源：http://wf.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wa.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ws.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sv.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://og.szsharing.cn

Java: s.substring(1, 4)
来源：http://sc.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yn.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://fm.nicolike.cn

[E04] 查找子串位置
来源：http://ig.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://km.gzmigu.cn


<!-- 参考信息 -->