代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yz.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://so.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pu.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vx.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mm.newstarts.cn

Go:   func add(a, b int) int
来源：http://lz.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://on.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tq.yuntaijiaju.cn

[C14] 泛型函数
来源：http://zi.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://om.szxytkj.cn

PHP:  // 无泛型
来源：http://kv.panjiajie.cn

JS:   // 无泛型
来源：http://ev.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oa.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ma.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zu.huanxung.cn

Ruby: # 无泛型
来源：http://vy.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ul.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://nn.chemitech.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ps.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://nr.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ss.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uv.bookmarksfly.cn

Java: // 无解构
来源：http://pw.nicolike.cn

Go:   // 无解构
来源：http://hp.bookmarksfly.cn

Ruby: a, b = pair
来源：http://ov.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://so.newstarts.cn

[C16] 函数 / 方法重载
来源：http://dk.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rn.panjiajie.cn

PHP:  // 无重载
来源：http://ai.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zn.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://wt.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hp.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://no.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://mv.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://si.hnjuh.cn

================================================================================
来源：http://ql.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://vy.yuexingan06.cn

================================================================================
来源：http://mu.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://pu.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xk.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ar.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://os.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vi.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jp.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://xg.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://vd.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kz.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://ek.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pc.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zu.newstarts.cn

JS:   arr.push(4);
来源：http://sv.panjiajie.cn

TS:   arr.push(4);
来源：http://td.huixiangedu.cn

Java: list.add(4);
来源：http://ku.asd995.cn

Go:   arr = append(arr, 4)
来源：http://tl.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://gv.521024.cn

C#:   list.Add(4);
来源：http://ay.521024.cn

[D03] 在指定位置插入元素
来源：http://uv.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://yq.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ax.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lh.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://kl.jctech888.com.cn

Java: list.add(0, 0);
来源：http://zw.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xh.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xs.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://cc.haigaiapp.cn

[D04] 删除元素
来源：http://fb.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mj.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wx.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ia.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://ah.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jj.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fs.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://is.chemitech.net.cn

[D05] 访问与修改元素
来源：http://hl.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ie.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ye.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ld.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://tu.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ox.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://pm.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://on.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ha.haigaiapp.cn

[D06] 数组长度
来源：http://hw.bookmarksfly.cn

Py:   len(arr)
来源：http://ti.szxytkj.cn

PHP:  count($arr);
来源：http://vf.muxihuayi.cn

JS:   arr.length
来源：http://nf.colortex.cn

TS:   arr.length
来源：http://fa.521024.cn

Java: list.size();
来源：http://uk.gzmigu.cn

Go:   len(arr)
来源：http://xz.newstarts.cn

Ruby: arr.length; arr.size
来源：http://pa.wgjwhj.cn

C#:   list.Count;
来源：http://ko.wgjwhj.cn

[D07] 切片 / 取子数组
来源：http://zo.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vs.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tr.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://tx.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://cw.asd995.cn

Java: list.subList(1, 4);
来源：http://ya.nszjky.cn

Go:   arr[1:4]
来源：http://hl.colortex.cn

Ruby: arr[1, 3]
来源：http://om.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://pf.gzmigu.cn

[D08] 合并两个数组
来源：http://ww.521024.cn

Py:   a + b;  a.extend(b)
来源：http://yj.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://ti.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yg.nszjky.cn

TS:   [...a, ...b];
来源：http://pi.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wy.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://dv.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://hi.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://pu.muxihuayi.cn

[D09] 排序（升序）
来源：http://uv.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://bn.gzmigu.cn

PHP:  sort($arr);
来源：http://gs.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jp.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yn.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ua.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jt.newstarts.cn

Ruby: arr.sort
来源：http://ib.muxihuayi.cn

C#:   list.Sort();
来源：http://uk.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://er.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ju.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yq.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fs.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bw.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wd.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tf.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xj.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bo.yuntaijiaju.cn

[D11] 反转数组
来源：http://ve.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yf.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://yz.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yt.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://oh.gzmigu.cn

Java: Collections.reverse(list);
来源：http://eo.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://to.huanxung.cn

Ruby: arr.reverse
来源：http://ko.nszjky.cn

C#:   list.Reverse();
来源：http://jm.huanxung.cn

[D12] 查找元素下标
来源：http://lh.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://dl.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ri.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ld.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hb.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uh.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://dx.huanxung.cn

Ruby: arr.index(x)
来源：http://yo.521024.cn

C#:   list.IndexOf(x);
来源：http://ay.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://ue.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qk.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qy.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://vh.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://cl.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ks.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bg.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hu.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://li.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://os.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tp.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://di.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://hv.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://hf.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vy.gzmigu.cn

Go:   // 手写循环
来源：http://iq.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lj.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://up.haigaiapp.cn

[D15] 去重
来源：http://qh.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lu.huanxung.cn

PHP:  array_unique($arr);
来源：http://wp.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://na.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://va.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uh.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://in.nicolike.cn

Ruby: arr.uniq
来源：http://dh.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://no.wgjwhj.cn

[D16] 求和与平均值
来源：http://pk.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://md.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fq.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fp.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rh.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gg.wgjwhj.cn

Go:   // 手写循环累加
来源：http://cw.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fd.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://yw.wgjwhj.cn

[D17] 最大值与最小值
来源：http://wx.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://wr.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://nm.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://en.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://km.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zj.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vv.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://al.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://nm.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://hi.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bz.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://jn.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iv.muxihuayi.cn

TS:   nested.flat();
来源：http://qf.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rf.szxytkj.cn

Go:   // 手写双层循环
来源：http://el.shxzskj.cn

Ruby: nested.flatten
来源：http://an.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yy.szxytkj.cn

[D19] 按字段分组
来源：http://kg.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jx.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ja.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rj.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rk.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wz.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://da.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ap.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ri.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://ii.newstarts.cn

Py:   Counter(arr)
来源：http://jc.szsharing.cn

PHP:  array_count_values($arr);
来源：http://bf.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ea.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ye.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ts.nszjky.cn

Go:   // 手写 map[T]int
来源：http://ee.szxytkj.cn

Ruby: arr.tally
来源：http://uu.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ov.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ru.chemitech.net.cn

Py:   x in arr
来源：http://qv.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://do.huixiangedu.cn

JS:   arr.includes(x)
来源：http://ak.nszjky.cn

TS:   arr.includes(x)
来源：http://yk.9csxet.cn

Java: list.contains(x)
来源：http://kn.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://na.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://kl.colortex.cn

C#:   list.Contains(x)
来源：http://yd.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://lm.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tw.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nr.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zz.nszjky.cn

TS:   [...arr];
来源：http://bj.bjjhwx.cn

Java: new ArrayList<>(list);
来源：http://hs.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rh.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://fa.chemitech.net.cn

C#:   new List<int>(list);
来源：http://cq.gzmigu.cn

[D23] reduce 累积计算
来源：http://je.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://su.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mw.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nn.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qm.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ga.9csxet.cn

Go:   // 手写循环
来源：http://ua.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rd.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rm.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://cr.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nu.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qg.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tj.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bi.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ol.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pb.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hl.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rz.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://tu.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bo.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qm.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wl.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ba.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rf.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ca.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vw.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ca.muxihuayi.cn

[D26] 数组转字符串
来源：http://li.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://cu.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://ee.shxzskj.cn

JS:   arr.join(", ")
来源：http://yf.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://vq.shxzukj.cn

Java: String.join(", ", list)
来源：http://vw.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://nd.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://dm.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://be.yuexingan06.cn

================================================================================
来源：http://he.hahajie.cn

E. 字符串处理
来源：http://gf.shxzskj.cn

================================================================================
来源：http://cg.bookmarksfly.cn

[E01] 拼接字符串
来源：http://kl.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ed.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://np.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ps.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pl.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tx.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ay.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ov.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vx.lnxyls.cn

[E02] 重复字符串
来源：http://fr.bookmarksfly.cn

Py:   "ab" * 3
来源：http://ri.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://ep.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://ti.szsharing.cn

TS:   "ab".repeat(3)
来源：http://ac.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://ew.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://hu.jctech888.com.cn

Ruby: "ab" * 3
来源：http://pk.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bi.huixiangedu.cn

[E03] 截取子串
来源：http://ri.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rh.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ru.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://he.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://ic.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://cz.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bi.bjjhwx.cn


<!-- 参考信息 -->