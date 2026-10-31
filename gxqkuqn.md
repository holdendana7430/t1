代发 wailian999

[C14] 泛型函数
来源：http://no.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://or.huanxung.cn

PHP:  // 无泛型
来源：http://ji.colortex.cn

JS:   // 无泛型
来源：http://xv.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hs.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yo.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yo.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://vu.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://et.521024.cn

[C15] 解构 / 展开参数
来源：http://nw.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kf.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://kf.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tg.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uf.hahajie.cn

Java: // 无解构
来源：http://pt.panjiajie.cn

Go:   // 无解构
来源：http://gb.huixiangedu.cn

Ruby: a, b = pair
来源：http://vz.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://lx.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://vm.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zp.haigaiapp.cn

PHP:  // 无重载
来源：http://ha.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ss.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://ww.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lr.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://go.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://qa.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wn.huanxung.cn

================================================================================
来源：http://tc.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://po.huixinmuqiang.cn

================================================================================
来源：http://ra.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://gi.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ld.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mm.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rx.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ll.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ke.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://hy.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://vv.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ke.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://hv.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jr.panjiajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mp.muxihuayi.cn

JS:   arr.push(4);
来源：http://dj.asd995.cn

TS:   arr.push(4);
来源：http://bc.haigaiapp.cn

Java: list.add(4);
来源：http://sj.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://ds.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://ee.nicolike.cn

C#:   list.Add(4);
来源：http://fy.521024.cn

[D03] 在指定位置插入元素
来源：http://au.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://da.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yu.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xu.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://mf.colortex.cn

Java: list.add(0, 0);
来源：http://fy.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kb.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://br.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://em.wgjwhj.cn

[D04] 删除元素
来源：http://wc.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lo.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ef.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vt.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://xr.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hx.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ok.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zh.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xk.panjiajie.cn

[D05] 访问与修改元素
来源：http://de.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ds.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cc.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://il.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://jr.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://es.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ji.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kr.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sw.haigaiapp.cn

[D06] 数组长度
来源：http://jz.yuntaijiaju.cn

Py:   len(arr)
来源：http://ay.nicolike.cn

PHP:  count($arr);
来源：http://wj.nicolike.cn

JS:   arr.length
来源：http://ks.szxytkj.cn

TS:   arr.length
来源：http://hi.szxytkj.cn

Java: list.size();
来源：http://hp.shxzukj.cn

Go:   len(arr)
来源：http://ea.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://eo.9csxet.cn

C#:   list.Count;
来源：http://yt.huanxung.cn

[D07] 切片 / 取子数组
来源：http://kg.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sn.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ax.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://zf.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://mi.szsharing.cn

Java: list.subList(1, 4);
来源：http://af.bjjhwx.cn

Go:   arr[1:4]
来源：http://hb.9csxet.cn

Ruby: arr[1, 3]
来源：http://xq.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://wr.szxytkj.cn

[D08] 合并两个数组
来源：http://jn.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://dc.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://fs.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tt.newstarts.cn

TS:   [...a, ...b];
来源：http://ht.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ob.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://bj.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://mu.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://md.huanxung.cn

[D09] 排序（升序）
来源：http://wv.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://iy.gzmigu.cn

PHP:  sort($arr);
来源：http://sm.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dz.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://au.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sv.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rk.huixiangedu.cn

Ruby: arr.sort
来源：http://qa.wgjwhj.cn

C#:   list.Sort();
来源：http://hy.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iy.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ca.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ac.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jr.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sx.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ak.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://am.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lw.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ws.szxytkj.cn

[D11] 反转数组
来源：http://ol.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ox.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://vu.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ku.shxzukj.cn

TS:   [...arr].reverse();
来源：http://my.shxzukj.cn

Java: Collections.reverse(list);
来源：http://nr.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://ra.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://rz.panjiajie.cn

C#:   list.Reverse();
来源：http://sk.huanxung.cn

[D12] 查找元素下标
来源：http://yh.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://jv.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xm.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hy.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tp.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jo.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://ne.huanxung.cn

Ruby: arr.index(x)
来源：http://mt.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ly.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://xe.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bj.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yp.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://dk.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://ra.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dn.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ac.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://px.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xy.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://al.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ad.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xa.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ll.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://xw.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://st.shtwfgs.cn

Go:   // 手写循环
来源：http://ce.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://se.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jb.9csxet.cn

[D15] 去重
来源：http://gh.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://du.newstarts.cn

PHP:  array_unique($arr);
来源：http://wg.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://vq.nicolike.cn

TS:   [...new Set(arr)]
来源：http://bc.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://az.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nx.shxzukj.cn

Ruby: arr.uniq
来源：http://ai.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://hh.hnjuh.cn

[D16] 求和与平均值
来源：http://gs.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fz.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ch.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://re.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zq.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gf.bjjhwx.cn

Go:   // 手写循环累加
来源：http://kl.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://il.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://cb.bjjhwx.cn

[D17] 最大值与最小值
来源：http://on.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://kd.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://sl.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sa.shxzskj.cn

TS:   Math.max(...arr);
来源：http://te.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qn.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fj.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://sq.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://zt.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://cn.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://td.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://dq.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wn.gzmigu.cn

TS:   nested.flat();
来源：http://ec.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wu.chemitech.net.cn

Go:   // 手写双层循环
来源：http://ol.hnjuh.cn

Ruby: nested.flatten
来源：http://fx.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gm.shxzskj.cn

[D19] 按字段分组
来源：http://xf.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ez.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ix.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iq.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kh.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://di.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ze.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ye.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yf.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://tk.shtwfgs.cn

Py:   Counter(arr)
来源：http://hl.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://vc.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fe.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vz.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qp.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://xt.wgjwhj.cn

Ruby: arr.tally
来源：http://oq.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wi.hahajie.cn

[D21] 判断是否包含某元素
来源：http://fe.huixinmuqiang.cn

Py:   x in arr
来源：http://oz.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://fc.huixiangedu.cn

JS:   arr.includes(x)
来源：http://uv.wgjwhj.cn

TS:   arr.includes(x)
来源：http://pj.asd995.cn

Java: list.contains(x)
来源：http://pn.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://qk.521024.cn

Ruby: arr.include?(x)
来源：http://fj.nicolike.cn

C#:   list.Contains(x)
来源：http://wo.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://xg.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zj.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qo.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://up.yuntaijiaju.cn

TS:   [...arr];
来源：http://th.szsharing.cn

Java: new ArrayList<>(list);
来源：http://nu.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fd.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://qw.muxihuayi.cn

C#:   new List<int>(list);
来源：http://pm.haigaiapp.cn

[D23] reduce 累积计算
来源：http://du.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://br.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mh.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cz.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nk.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yp.huixinmuqiang.cn

Go:   // 手写循环
来源：http://vn.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dc.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xn.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://pp.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yg.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tk.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eh.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sr.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qe.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fa.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uj.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ea.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ah.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vu.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qo.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ws.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://um.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uo.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mh.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ys.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dy.hahajie.cn

[D26] 数组转字符串
来源：http://gg.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://gb.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://yt.bjjhwx.cn

JS:   arr.join(", ")
来源：http://bl.wgjwhj.cn

TS:   arr.join(", ")
来源：http://fn.gzmigu.cn

Java: String.join(", ", list)
来源：http://sf.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://ar.nicolike.cn

Ruby: arr.join(", ")
来源：http://yj.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://bd.yuexingan06.cn

================================================================================
来源：http://oq.szsharing.cn

E. 字符串处理
来源：http://oz.yuntaijiaju.cn

================================================================================
来源：http://so.szxytkj.cn

[E01] 拼接字符串
来源：http://ah.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pp.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yo.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sm.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eo.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sa.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bt.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pm.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ho.9csxet.cn

[E02] 重复字符串
来源：http://ev.panjiajie.cn

Py:   "ab" * 3
来源：http://jt.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://hb.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://pj.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://fi.huanxung.cn

Java: "ab".repeat(3)
来源：http://ze.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://mw.shxzukj.cn

Ruby: "ab" * 3
来源：http://fi.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://up.nicolike.cn

[E03] 截取子串
来源：http://bt.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fv.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tm.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ur.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://rl.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://pc.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rm.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ni.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://sp.nicolike.cn

[E04] 查找子串位置
来源：http://dl.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://mq.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://ju.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oh.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://pa.muxihuayi.cn

Java: s.indexOf("x")
来源：http://ap.nszjky.cn


<!-- 参考信息 -->