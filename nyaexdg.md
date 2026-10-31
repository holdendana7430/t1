代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://yq.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://pr.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ft.521024.cn

[C13] 类型声明 / 类型注解
来源：http://hx.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ah.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dx.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xa.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ag.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jx.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://oy.wgjwhj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sb.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ke.colortex.cn

[C14] 泛型函数
来源：http://mo.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://em.yuexingan06.cn

PHP:  // 无泛型
来源：http://yo.lnxyls.cn

JS:   // 无泛型
来源：http://fo.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fz.muxihuayi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://og.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tx.hnjuh.cn

Ruby: # 无泛型
来源：http://mg.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vz.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://gb.yuntaijiaju.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ml.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://qm.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lg.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nf.yuntaijiaju.cn

Java: // 无解构
来源：http://ea.yuexingan06.cn

Go:   // 无解构
来源：http://or.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://jq.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://gh.szsharing.cn

[C16] 函数 / 方法重载
来源：http://lj.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xr.yuntaijiaju.cn

PHP:  // 无重载
来源：http://rd.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ep.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://pd.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yd.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://oo.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://bj.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rq.wgjwhj.cn

================================================================================
来源：http://kq.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://zd.haigaiapp.cn

================================================================================
来源：http://dg.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://cc.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zt.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ma.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://us.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ha.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tk.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://ed.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ud.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qp.panjiajie.cn

[D02] 追加元素到末尾
来源：http://nk.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ua.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rs.nszjky.cn

JS:   arr.push(4);
来源：http://nc.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://zd.colortex.cn

Java: list.add(4);
来源：http://kw.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://jm.9csxet.cn

Ruby: arr << 4; arr.push(5)
来源：http://zy.9csxet.cn

C#:   list.Add(4);
来源：http://vx.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://ix.asd995.cn

Py:   arr.insert(0, 0)
来源：http://nd.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sd.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nx.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://we.wgjwhj.cn

Java: list.add(0, 0);
来源：http://wb.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ea.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tf.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://ju.szxytkj.cn

[D04] 删除元素
来源：http://kv.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kr.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wb.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wj.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://kl.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://is.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vl.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xm.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rc.szsharing.cn

[D05] 访问与修改元素
来源：http://mk.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://be.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ou.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ip.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://vw.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://rc.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://ce.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://no.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ej.nicolike.cn

[D06] 数组长度
来源：http://de.newstarts.cn

Py:   len(arr)
来源：http://er.hahajie.cn

PHP:  count($arr);
来源：http://qr.wgjwhj.cn

JS:   arr.length
来源：http://jb.521024.cn

TS:   arr.length
来源：http://ch.wgjwhj.cn

Java: list.size();
来源：http://sl.gzmigu.cn

Go:   len(arr)
来源：http://oh.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://uv.haigaiapp.cn

C#:   list.Count;
来源：http://tv.nicolike.cn

[D07] 切片 / 取子数组
来源：http://rn.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://le.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pu.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://yk.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://ln.shxzskj.cn

Java: list.subList(1, 4);
来源：http://eg.chemitech.net.cn

Go:   arr[1:4]
来源：http://ck.szxytkj.cn

Ruby: arr[1, 3]
来源：http://cw.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://hp.bjjhwx.cn

[D08] 合并两个数组
来源：http://yq.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://jk.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://pk.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://or.szxytkj.cn

TS:   [...a, ...b];
来源：http://fc.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ov.gzmigu.cn

Go:   append(a, b...)
来源：http://ob.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://ri.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://jk.lnxyls.cn

[D09] 排序（升序）
来源：http://da.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://vv.szsharing.cn

PHP:  sort($arr);
来源：http://yy.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oi.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zd.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lw.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yj.panjiajie.cn

Ruby: arr.sort
来源：http://yi.muxihuayi.cn

C#:   list.Sort();
来源：http://ww.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mq.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rz.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aw.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oq.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nf.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sv.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ej.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ct.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vp.hahajie.cn

[D11] 反转数组
来源：http://rz.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yk.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://ob.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dv.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://hz.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://qg.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://ne.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://ez.nicolike.cn

C#:   list.Reverse();
来源：http://cs.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://ea.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://go.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rv.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ui.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://me.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ns.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://xo.shxzukj.cn

Ruby: arr.index(x)
来源：http://bz.521024.cn

C#:   list.IndexOf(x);
来源：http://ks.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://po.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fh.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pz.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://it.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://yd.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yp.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gd.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lx.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vf.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://an.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zo.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hn.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://zl.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://uz.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ih.9csxet.cn

Go:   // 手写循环
来源：http://ty.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vy.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sx.wgjwhj.cn

[D15] 去重
来源：http://zb.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fl.asd995.cn

PHP:  array_unique($arr);
来源：http://tk.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://li.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://fj.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nx.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ye.shxzskj.cn

Ruby: arr.uniq
来源：http://aa.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://sa.newstarts.cn

[D16] 求和与平均值
来源：http://gb.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uv.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rz.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bq.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ef.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://im.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dc.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://gb.chemitech.net.cn

[D17] 最大值与最小值
来源：http://on.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://ds.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://vd.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yz.hnjuh.cn

TS:   Math.max(...arr);
来源：http://hu.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nv.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kx.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://lr.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://zf.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://ph.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://av.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://sq.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cy.shtwfgs.cn

TS:   nested.flat();
来源：http://sj.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kl.jctech888.com.cn

Go:   // 手写双层循环
来源：http://mq.huanxung.cn

Ruby: nested.flatten
来源：http://or.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wr.hnjuh.cn

[D19] 按字段分组
来源：http://fg.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cc.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sm.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rr.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sb.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ia.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://rf.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fv.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gd.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://ie.shxzukj.cn

Py:   Counter(arr)
来源：http://jw.huanxung.cn

PHP:  array_count_values($arr);
来源：http://ag.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://in.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nj.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bm.hahajie.cn

Go:   // 手写 map[T]int
来源：http://ed.muxihuayi.cn

Ruby: arr.tally
来源：http://ak.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sg.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://gi.jianghongdianzi.cn

Py:   x in arr
来源：http://ut.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://ji.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://pp.jctech888.com.cn

TS:   arr.includes(x)
来源：http://rm.colortex.cn

Java: list.contains(x)
来源：http://fb.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://ki.asd995.cn

Ruby: arr.include?(x)
来源：http://bc.521024.cn

C#:   list.Contains(x)
来源：http://ms.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://ci.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kw.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dv.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xl.bookmarksfly.cn

TS:   [...arr];
来源：http://ve.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://dy.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://me.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://pm.nicolike.cn

C#:   new List<int>(list);
来源：http://vk.asd995.cn

[D23] reduce 累积计算
来源：http://ap.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tw.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ps.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hm.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oz.huixinmuqiang.cn

Go:   // 手写循环
来源：http://qx.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ly.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mm.521024.cn

[D24] 字典 / Map 基本操作
来源：http://ff.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ve.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tf.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qk.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xd.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bt.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vj.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oy.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cj.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://fd.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sl.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jn.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ue.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gf.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vl.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://em.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qm.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cc.gzmigu.cn

[D26] 数组转字符串
来源：http://rd.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://bv.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://en.lnxyls.cn

JS:   arr.join(", ")
来源：http://qz.bjjhwx.cn

TS:   arr.join(", ")
来源：http://co.newstarts.cn

Java: String.join(", ", list)
来源：http://vt.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://vk.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://of.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://tc.yuntaijiaju.cn

================================================================================
来源：http://tx.jctech888.com.cn

E. 字符串处理
来源：http://ot.yuexingan06.cn

================================================================================
来源：http://bc.asd995.cn

[E01] 拼接字符串
来源：http://qn.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://es.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sx.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ro.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lk.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wr.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rs.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pr.nszjky.cn

[E02] 重复字符串
来源：http://pk.9csxet.cn

Py:   "ab" * 3
来源：http://cy.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://gp.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://ji.newstarts.cn

TS:   "ab".repeat(3)
来源：http://py.shxzskj.cn

Java: "ab".repeat(3)
来源：http://ez.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://mw.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://dz.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pv.jianghongdianzi.cn

[E03] 截取子串
来源：http://vp.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xf.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qm.521024.cn


<!-- 参考信息 -->