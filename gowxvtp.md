代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://ic.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://df.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xz.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://wb.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kn.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://in.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jv.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uk.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vn.szsharing.cn

Go:   func add(a, b int) int
来源：http://wj.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ee.lnxyls.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nc.shxzskj.cn

[C14] 泛型函数
来源：http://jn.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xs.shxzskj.cn

PHP:  // 无泛型
来源：http://iq.hnjuh.cn

JS:   // 无泛型
来源：http://lz.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ky.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bj.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lq.bjjhwx.cn

Ruby: # 无泛型
来源：http://ut.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bs.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://fo.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kp.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://qv.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rq.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lf.szsharing.cn

Java: // 无解构
来源：http://nv.colortex.cn

Go:   // 无解构
来源：http://ux.hnjuh.cn

Ruby: a, b = pair
来源：http://re.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://ky.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://kl.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iu.huanxung.cn

PHP:  // 无重载
来源：http://yd.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wz.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://le.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sv.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://mg.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://va.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sb.panjiajie.cn

================================================================================
来源：http://hs.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://pe.yuexingan06.cn

================================================================================
来源：http://fb.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://bo.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bt.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zg.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://om.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yp.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ba.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://xs.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://wp.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vy.shxzskj.cn

[D02] 追加元素到末尾
来源：http://ai.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gp.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ij.hnjuh.cn

JS:   arr.push(4);
来源：http://kz.shxzukj.cn

TS:   arr.push(4);
来源：http://md.huanxung.cn

Java: list.add(4);
来源：http://gk.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://iv.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://sm.bookmarksfly.cn

C#:   list.Add(4);
来源：http://qo.szsharing.cn

[D03] 在指定位置插入元素
来源：http://zc.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://ps.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jg.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kd.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://uc.newstarts.cn

Java: list.add(0, 0);
来源：http://hd.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ol.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vo.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://im.nicolike.cn

[D04] 删除元素
来源：http://hh.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sx.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fe.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tw.asd995.cn

TS:   arr.splice(0, 1);
来源：http://ed.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jo.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xb.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fl.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qb.hahajie.cn

[D05] 访问与修改元素
来源：http://me.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ec.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://st.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ma.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://vq.hnjuh.cn

Java: list.get(0); list.set(0, 9);
来源：http://bv.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://mg.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://we.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yd.panjiajie.cn

[D06] 数组长度
来源：http://wz.newstarts.cn

Py:   len(arr)
来源：http://to.521024.cn

PHP:  count($arr);
来源：http://oo.shtwfgs.cn

JS:   arr.length
来源：http://mu.panjiajie.cn

TS:   arr.length
来源：http://nl.huixiangedu.cn

Java: list.size();
来源：http://oh.nszjky.cn

Go:   len(arr)
来源：http://tb.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://lm.gzmigu.cn

C#:   list.Count;
来源：http://fi.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://sf.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fv.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fs.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://yd.colortex.cn

TS:   arr.slice(1, 4);
来源：http://yg.szsharing.cn

Java: list.subList(1, 4);
来源：http://li.shxzukj.cn

Go:   arr[1:4]
来源：http://qd.hnjuh.cn

Ruby: arr[1, 3]
来源：http://ih.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://hg.asd995.cn

[D08] 合并两个数组
来源：http://ks.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://nl.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://cw.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yl.jctech888.com.cn

TS:   [...a, ...b];
来源：http://fe.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jg.muxihuayi.cn

Go:   append(a, b...)
来源：http://of.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://lr.521024.cn

C#:   a.Concat(b).ToList()
来源：http://hc.hnjuh.cn

[D09] 排序（升序）
来源：http://zn.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ow.asd995.cn

PHP:  sort($arr);
来源：http://hw.shtwfgs.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sj.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sm.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://du.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vz.chemitech.net.cn

Ruby: arr.sort
来源：http://mx.panjiajie.cn

C#:   list.Sort();
来源：http://cf.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wb.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://an.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nu.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vb.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gu.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ai.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xb.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yy.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tt.gzmigu.cn

[D11] 反转数组
来源：http://vy.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lz.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://bb.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jy.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://gm.panjiajie.cn

Java: Collections.reverse(list);
来源：http://nt.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://mz.muxihuayi.cn

Ruby: arr.reverse
来源：http://hk.newstarts.cn

C#:   list.Reverse();
来源：http://vz.shtwfgs.cn

[D12] 查找元素下标
来源：http://tv.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://nu.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wp.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yz.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ff.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gu.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://jv.haigaiapp.cn

Ruby: arr.index(x)
来源：http://qn.521024.cn

C#:   list.IndexOf(x);
来源：http://fl.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://km.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bv.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://up.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://tn.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://wu.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mk.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zo.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yz.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qx.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://ee.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yd.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tc.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://al.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://dy.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rz.bjjhwx.cn

Go:   // 手写循环
来源：http://it.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cf.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lk.hnjuh.cn

[D15] 去重
来源：http://cz.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xo.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://oc.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://yt.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://mo.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pn.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://de.asd995.cn

Ruby: arr.uniq
来源：http://up.521024.cn

C#:   list.Distinct().ToList()
来源：http://za.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://uc.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rf.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cl.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://un.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ll.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aa.9csxet.cn

Go:   // 手写循环累加
来源：http://my.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://us.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://js.nszjky.cn

[D17] 最大值与最小值
来源：http://ro.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://kf.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://pb.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vo.panjiajie.cn

TS:   Math.max(...arr);
来源：http://li.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yn.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hq.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://nl.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://pv.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://st.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sy.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://hb.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uf.nicolike.cn

TS:   nested.flat();
来源：http://nc.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://et.huanxung.cn

Go:   // 手写双层循环
来源：http://fq.jctech888.com.cn

Ruby: nested.flatten
来源：http://xz.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uv.shxzskj.cn

[D19] 按字段分组
来源：http://dx.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ok.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dl.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cb.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oe.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tm.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://mu.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cu.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pm.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://vw.huanxung.cn

Py:   Counter(arr)
来源：http://eq.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://rf.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://al.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://el.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aw.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://rp.haigaiapp.cn

Ruby: arr.tally
来源：http://ih.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aa.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://ic.bookmarksfly.cn

Py:   x in arr
来源：http://zs.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://cf.bjjhwx.cn

JS:   arr.includes(x)
来源：http://yy.hnjuh.cn

TS:   arr.includes(x)
来源：http://bh.haigaiapp.cn

Java: list.contains(x)
来源：http://pe.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://ak.szsharing.cn

Ruby: arr.include?(x)
来源：http://hw.shtwfgs.cn

C#:   list.Contains(x)
来源：http://lp.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://bq.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ch.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ke.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dq.shtwfgs.cn

TS:   [...arr];
来源：http://nb.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://rm.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ms.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://rx.colortex.cn

C#:   new List<int>(list);
来源：http://nn.asd995.cn

[D23] reduce 累积计算
来源：http://zj.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qi.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xv.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hc.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gc.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cg.9csxet.cn

Go:   // 手写循环
来源：http://nk.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bp.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ox.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://hj.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ov.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pm.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dd.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ux.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qt.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vn.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kh.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ah.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://ei.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rr.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://im.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ph.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zq.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bb.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vh.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sl.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pz.bookmarksfly.cn

[D26] 数组转字符串
来源：http://td.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://vr.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://ia.haigaiapp.cn

JS:   arr.join(", ")
来源：http://pf.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://ic.521024.cn

Java: String.join(", ", list)
来源：http://bc.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://bl.521024.cn

Ruby: arr.join(", ")
来源：http://wn.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://jd.asd995.cn

================================================================================
来源：http://wm.nicolike.cn

E. 字符串处理
来源：http://tp.huixiangedu.cn

================================================================================
来源：http://xw.yuexingan06.cn

[E01] 拼接字符串
来源：http://xn.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dz.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jr.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tn.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ab.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ut.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ro.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ea.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rq.szxytkj.cn

[E02] 重复字符串
来源：http://jf.asd995.cn

Py:   "ab" * 3
来源：http://su.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://rl.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://qb.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://fd.shxzukj.cn

Java: "ab".repeat(3)
来源：http://lv.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://ew.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://vm.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lr.jianghongdianzi.cn

[E03] 截取子串
来源：http://oq.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ae.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wv.muxihuayi.cn


<!-- 参考信息 -->