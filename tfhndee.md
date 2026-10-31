代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ef.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://en.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fh.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hg.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://td.lnxyls.cn

Go:   func add(a, b int) int
来源：http://dx.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://px.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zn.hahajie.cn

[C14] 泛型函数
来源：http://hz.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sr.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://oz.jctech888.com.cn

JS:   // 无泛型
来源：http://qu.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yx.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yd.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uv.haigaiapp.cn

Ruby: # 无泛型
来源：http://ug.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vp.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://wb.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ae.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://ce.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ko.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://od.huanxung.cn

Java: // 无解构
来源：http://fm.nicolike.cn

Go:   // 无解构
来源：http://ox.nicolike.cn

Ruby: a, b = pair
来源：http://rn.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://rd.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ti.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xc.nszjky.cn

PHP:  // 无重载
来源：http://vk.yuntaijiaju.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ta.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://nu.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://se.521024.cn

Go:   // 无重载：用不同函数名
来源：http://dp.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://bh.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ll.hnjuh.cn

================================================================================
来源：http://kw.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://ns.wgjwhj.cn

================================================================================
来源：http://qu.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://qg.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ux.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mc.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sf.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yh.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kx.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://vc.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://cx.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mx.shxzukj.cn

[D02] 追加元素到末尾
来源：http://pj.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gk.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ed.newstarts.cn

JS:   arr.push(4);
来源：http://li.shtwfgs.cn

TS:   arr.push(4);
来源：http://hk.huanxung.cn

Java: list.add(4);
来源：http://fv.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://ux.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://so.szsharing.cn

C#:   list.Add(4);
来源：http://yh.newstarts.cn

[D03] 在指定位置插入元素
来源：http://tq.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://ww.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ua.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xy.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://gf.chemitech.net.cn

Java: list.add(0, 0);
来源：http://tk.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cq.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zd.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://ao.huixiangedu.cn

[D04] 删除元素
来源：http://di.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bb.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rs.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ah.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://lv.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ar.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ep.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jr.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kr.shtwfgs.cn

[D05] 访问与修改元素
来源：http://lb.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yu.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bl.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ao.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://zo.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://wq.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://yn.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xd.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sw.jianghongdianzi.cn

[D06] 数组长度
来源：http://er.szsharing.cn

Py:   len(arr)
来源：http://qj.szsharing.cn

PHP:  count($arr);
来源：http://rm.huanxung.cn

JS:   arr.length
来源：http://pv.jctech888.com.cn

TS:   arr.length
来源：http://ii.haigaiapp.cn

Java: list.size();
来源：http://ga.521024.cn

Go:   len(arr)
来源：http://nu.colortex.cn

Ruby: arr.length; arr.size
来源：http://ag.asd995.cn

C#:   list.Count;
来源：http://az.szsharing.cn

[D07] 切片 / 取子数组
来源：http://dc.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://it.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vb.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://fp.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://yi.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://zi.asd995.cn

Go:   arr[1:4]
来源：http://bq.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://bh.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://be.asd995.cn

[D08] 合并两个数组
来源：http://az.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://dx.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://wy.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fv.9csxet.cn

TS:   [...a, ...b];
来源：http://rs.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qq.hnjuh.cn

Go:   append(a, b...)
来源：http://uc.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://hk.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://st.shtwfgs.cn

[D09] 排序（升序）
来源：http://jv.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://gv.hahajie.cn

PHP:  sort($arr);
来源：http://jg.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tl.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fe.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://at.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://el.hahajie.cn

Ruby: arr.sort
来源：http://rr.haigaiapp.cn

C#:   list.Sort();
来源：http://zh.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ok.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fu.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ya.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ke.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wo.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pm.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vj.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rn.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uy.bjjhwx.cn

[D11] 反转数组
来源：http://jh.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sn.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://lx.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yc.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://co.hahajie.cn

Java: Collections.reverse(list);
来源：http://gp.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://ml.jctech888.com.cn

Ruby: arr.reverse
来源：http://jz.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://ec.yuexingan06.cn

[D12] 查找元素下标
来源：http://kg.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://wu.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yr.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ik.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://le.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vq.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://zb.haigaiapp.cn

Ruby: arr.index(x)
来源：http://py.521024.cn

C#:   list.IndexOf(x);
来源：http://md.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://ah.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jz.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yl.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://cg.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://lf.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vd.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rs.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://te.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lg.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://sx.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eg.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://js.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ja.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://th.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://by.panjiajie.cn

Go:   // 手写循环
来源：http://sw.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ia.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jx.bjjhwx.cn

[D15] 去重
来源：http://re.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fq.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://kr.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://yz.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://ak.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bq.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://km.nicolike.cn

Ruby: arr.uniq
来源：http://cw.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://pi.chemitech.net.cn

[D16] 求和与平均值
来源：http://kl.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hu.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wj.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vq.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iw.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xa.hahajie.cn

Go:   // 手写循环累加
来源：http://lu.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yd.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://ki.muxihuayi.cn

[D17] 最大值与最小值
来源：http://bb.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://yb.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://tb.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uj.panjiajie.cn

TS:   Math.max(...arr);
来源：http://ge.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sz.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kc.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://xw.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://rb.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://cj.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xp.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://ad.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hv.bookmarksfly.cn

TS:   nested.flat();
来源：http://ga.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oe.jctech888.com.cn

Go:   // 手写双层循环
来源：http://mt.shtwfgs.cn

Ruby: nested.flatten
来源：http://ue.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ys.huixinmuqiang.cn

[D19] 按字段分组
来源：http://xz.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ko.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mw.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lg.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wg.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nw.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://cd.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zf.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nx.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://vs.newstarts.cn

Py:   Counter(arr)
来源：http://pd.hahajie.cn

PHP:  array_count_values($arr);
来源：http://zx.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ny.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bk.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fh.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://hj.jianghongdianzi.cn

Ruby: arr.tally
来源：http://ll.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lw.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://gr.jianghongdianzi.cn

Py:   x in arr
来源：http://xe.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://tw.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://my.gzmigu.cn

TS:   arr.includes(x)
来源：http://kv.asd995.cn

Java: list.contains(x)
来源：http://zp.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://gj.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://gt.chemitech.net.cn

C#:   list.Contains(x)
来源：http://ps.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://ov.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jv.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gc.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qj.bjjhwx.cn

TS:   [...arr];
来源：http://va.hahajie.cn

Java: new ArrayList<>(list);
来源：http://rp.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vy.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://bz.hahajie.cn

C#:   new List<int>(list);
来源：http://mp.bjjhwx.cn

[D23] reduce 累积计算
来源：http://bu.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wc.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wn.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://at.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://el.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fu.yuntaijiaju.cn

Go:   // 手写循环
来源：http://nr.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yj.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hg.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://qh.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gy.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qt.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kw.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kh.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mz.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wv.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rt.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gs.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://zk.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://el.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bo.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fv.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://os.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qj.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qb.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pl.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ix.9csxet.cn

[D26] 数组转字符串
来源：http://xk.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://ed.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://nu.yuexingan06.cn

JS:   arr.join(", ")
来源：http://yh.haigaiapp.cn

TS:   arr.join(", ")
来源：http://ry.yuexingan06.cn

Java: String.join(", ", list)
来源：http://rf.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ic.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://gx.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://sn.chemitech.net.cn

================================================================================
来源：http://ke.shxzukj.cn

E. 字符串处理
来源：http://iz.hnjuh.cn

================================================================================
来源：http://jm.hahajie.cn

[E01] 拼接字符串
来源：http://aq.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ga.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tb.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ro.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hy.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qo.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bn.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ws.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ys.haigaiapp.cn

[E02] 重复字符串
来源：http://ds.szxytkj.cn

Py:   "ab" * 3
来源：http://js.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://ql.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://im.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://ps.shxzukj.cn

Java: "ab".repeat(3)
来源：http://ev.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://jj.nszjky.cn

Ruby: "ab" * 3
来源：http://tn.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bj.shtwfgs.cn

[E03] 截取子串
来源：http://mo.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eq.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uo.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xd.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://mu.521024.cn

Java: s.substring(1, 4)
来源：http://hg.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lr.shxzukj.cn


<!-- 参考信息 -->