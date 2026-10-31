代发 wailian999

[C14] 泛型函数
来源：http://cq.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bb.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://cv.newstarts.cn

JS:   // 无泛型
来源：http://oq.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ks.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zy.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xi.haigaiapp.cn

Ruby: # 无泛型
来源：http://pi.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xu.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://uk.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ja.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://cw.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rj.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pd.bjjhwx.cn

Java: // 无解构
来源：http://rl.wgjwhj.cn

Go:   // 无解构
来源：http://cx.9csxet.cn

Ruby: a, b = pair
来源：http://ws.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://pi.hahajie.cn

[C16] 函数 / 方法重载
来源：http://yd.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yk.szsharing.cn

PHP:  // 无重载
来源：http://zi.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yy.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://sf.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uj.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://qr.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://dk.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oe.panjiajie.cn

================================================================================
来源：http://qv.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://rv.nicolike.cn

================================================================================
来源：http://zc.szsharing.cn

[D01] 创建数组 / 列表
来源：http://rh.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sc.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qr.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cs.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cq.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bj.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://ci.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://zx.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fn.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://hb.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rx.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ya.huanxung.cn

JS:   arr.push(4);
来源：http://yn.hahajie.cn

TS:   arr.push(4);
来源：http://nk.szxytkj.cn

Java: list.add(4);
来源：http://bi.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://hg.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://ir.hnjuh.cn

C#:   list.Add(4);
来源：http://os.colortex.cn

[D03] 在指定位置插入元素
来源：http://ze.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://jn.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eo.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hd.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ln.asd995.cn

Java: list.add(0, 0);
来源：http://sg.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iz.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yb.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://mj.szsharing.cn

[D04] 删除元素
来源：http://wp.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://is.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yl.yuntaijiaju.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ol.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://db.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://la.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vc.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xn.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sq.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://si.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bk.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qw.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xt.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ef.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://cb.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://yt.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cc.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uq.newstarts.cn

[D06] 数组长度
来源：http://wi.bookmarksfly.cn

Py:   len(arr)
来源：http://kp.colortex.cn

PHP:  count($arr);
来源：http://ku.yuexingan06.cn

JS:   arr.length
来源：http://en.jianghongdianzi.cn

TS:   arr.length
来源：http://cq.chemitech.net.cn

Java: list.size();
来源：http://zi.nicolike.cn

Go:   len(arr)
来源：http://hz.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://it.huixinmuqiang.cn

C#:   list.Count;
来源：http://pi.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://zl.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dv.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ne.521024.cn

JS:   arr.slice(1, 4);
来源：http://if.521024.cn

TS:   arr.slice(1, 4);
来源：http://sg.huanxung.cn

Java: list.subList(1, 4);
来源：http://fu.panjiajie.cn

Go:   arr[1:4]
来源：http://qy.hnjuh.cn

Ruby: arr[1, 3]
来源：http://vv.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://io.bookmarksfly.cn

[D08] 合并两个数组
来源：http://tl.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://xo.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://vw.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zh.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://gg.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lr.wgjwhj.cn

Go:   append(a, b...)
来源：http://qt.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://ti.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://kx.newstarts.cn

[D09] 排序（升序）
来源：http://sv.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://sk.shxzukj.cn

PHP:  sort($arr);
来源：http://om.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ln.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gt.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://re.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tu.521024.cn

Ruby: arr.sort
来源：http://hb.colortex.cn

C#:   list.Sort();
来源：http://kh.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bp.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ph.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yn.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xi.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gc.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wb.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ds.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ip.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yd.haigaiapp.cn

[D11] 反转数组
来源：http://wk.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fi.9csxet.cn

PHP:  array_reverse($arr);
来源：http://ch.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qo.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://rc.newstarts.cn

Java: Collections.reverse(list);
来源：http://np.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://li.huanxung.cn

Ruby: arr.reverse
来源：http://av.9csxet.cn

C#:   list.Reverse();
来源：http://sz.hnjuh.cn

[D12] 查找元素下标
来源：http://ru.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://ou.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lw.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bj.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eo.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uo.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://za.nicolike.cn

Ruby: arr.index(x)
来源：http://va.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://qy.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://zk.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xj.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wk.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://bn.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://ra.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gr.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pa.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xj.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ju.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://py.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ss.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dz.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://qz.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://lq.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dp.szxytkj.cn

Go:   // 手写循环
来源：http://px.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ht.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gf.jctech888.com.cn

[D15] 去重
来源：http://ju.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pl.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://jn.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://tq.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://fk.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nd.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hl.colortex.cn

Ruby: arr.uniq
来源：http://mc.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://xf.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://un.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vv.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jy.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wq.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rh.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tg.haigaiapp.cn

Go:   // 手写循环累加
来源：http://mv.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fi.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://cm.huixiangedu.cn

[D17] 最大值与最小值
来源：http://re.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://ft.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://px.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qp.9csxet.cn

TS:   Math.max(...arr);
来源：http://gz.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ur.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wq.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://wz.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://ct.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://lz.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kg.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://or.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sr.9csxet.cn

TS:   nested.flat();
来源：http://nj.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mk.colortex.cn

Go:   // 手写双层循环
来源：http://ft.bjjhwx.cn

Ruby: nested.flatten
来源：http://dc.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eu.newstarts.cn

[D19] 按字段分组
来源：http://pr.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rn.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vb.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pm.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xx.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bt.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ph.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://km.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pc.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://bn.szsharing.cn

Py:   Counter(arr)
来源：http://eu.nicolike.cn

PHP:  array_count_values($arr);
来源：http://nl.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pj.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pk.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zm.huanxung.cn

Go:   // 手写 map[T]int
来源：http://bj.nicolike.cn

Ruby: arr.tally
来源：http://zu.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cs.nicolike.cn

[D21] 判断是否包含某元素
来源：http://za.huixinmuqiang.cn

Py:   x in arr
来源：http://am.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://zl.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://sh.szsharing.cn

TS:   arr.includes(x)
来源：http://wb.szsharing.cn

Java: list.contains(x)
来源：http://en.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://cv.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://lx.shxzukj.cn

C#:   list.Contains(x)
来源：http://rk.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://pl.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vp.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cs.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wy.nicolike.cn

TS:   [...arr];
来源：http://gu.nicolike.cn

Java: new ArrayList<>(list);
来源：http://zx.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xy.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://fw.colortex.cn

C#:   new List<int>(list);
来源：http://gc.panjiajie.cn

[D23] reduce 累积计算
来源：http://tg.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gz.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hf.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wr.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qw.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://da.wgjwhj.cn

Go:   // 手写循环
来源：http://br.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kc.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://in.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://if.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xz.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cl.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yd.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zc.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rb.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zd.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dw.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ji.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://nl.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ys.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zt.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bg.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mm.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gl.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ce.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hg.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zk.hahajie.cn

[D26] 数组转字符串
来源：http://zo.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://ya.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://eb.yuexingan06.cn

JS:   arr.join(", ")
来源：http://lw.shtwfgs.cn

TS:   arr.join(", ")
来源：http://cp.haigaiapp.cn

Java: String.join(", ", list)
来源：http://gf.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://zn.nszjky.cn

Ruby: arr.join(", ")
来源：http://hy.colortex.cn

C#:   string.Join(", ", list)
来源：http://lj.yuexingan06.cn

================================================================================
来源：http://fc.shxzukj.cn

E. 字符串处理
来源：http://bi.jianghongdianzi.cn

================================================================================
来源：http://mv.bookmarksfly.cn

[E01] 拼接字符串
来源：http://ot.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qq.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lh.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lv.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wt.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kj.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hv.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ac.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zv.muxihuayi.cn

[E02] 重复字符串
来源：http://nc.lnxyls.cn

Py:   "ab" * 3
来源：http://zr.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://me.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://ww.szsharing.cn

TS:   "ab".repeat(3)
来源：http://lq.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://zw.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://xf.jctech888.com.cn

Ruby: "ab" * 3
来源：http://dh.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pk.lnxyls.cn

[E03] 截取子串
来源：http://hs.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lr.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wq.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nb.nszjky.cn

TS:   s.slice(1, 4)
来源：http://jo.szsharing.cn

Java: s.substring(1, 4)
来源：http://yy.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ms.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yp.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://gh.huanxung.cn

[E04] 查找子串位置
来源：http://qm.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://ml.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://gy.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sj.asd995.cn

TS:   s.indexOf("x")
来源：http://by.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://pr.9csxet.cn


<!-- 参考信息 -->