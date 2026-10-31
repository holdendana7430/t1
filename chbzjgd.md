代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://cv.szsharing.cn

C#:   using System.Text;
来源：http://ae.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://na.huixiangedu.cn

Py:   (lambda: print("run"))()
来源：http://lq.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://zu.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://en.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://ki.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://an.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://nx.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://lu.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pb.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://wb.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sn.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nn.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vb.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ks.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ht.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://zw.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ut.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://un.asd995.cn

[C14] 泛型函数
来源：http://gg.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://br.panjiajie.cn

PHP:  // 无泛型
来源：http://tk.huixiangedu.cn

JS:   // 无泛型
来源：http://su.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cg.9csxet.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qj.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dt.bookmarksfly.cn

Ruby: # 无泛型
来源：http://je.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yw.9csxet.cn

[C15] 解构 / 展开参数
来源：http://od.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ox.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://wn.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zf.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ed.yuexingan06.cn

Java: // 无解构
来源：http://jq.hahajie.cn

Go:   // 无解构
来源：http://sn.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://he.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://ie.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://cf.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mr.panjiajie.cn

PHP:  // 无重载
来源：http://nl.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xl.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://uj.hahajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xf.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://jg.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://gx.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cd.yuntaijiaju.cn

================================================================================
来源：http://ve.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://qs.9csxet.cn

================================================================================
来源：http://mh.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://dj.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nd.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bi.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oo.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wc.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vn.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://dz.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://gb.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gv.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://px.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://id.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xi.hnjuh.cn

JS:   arr.push(4);
来源：http://ix.panjiajie.cn

TS:   arr.push(4);
来源：http://gj.shtwfgs.cn

Java: list.add(4);
来源：http://nl.asd995.cn

Go:   arr = append(arr, 4)
来源：http://zb.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://nm.shxzskj.cn

C#:   list.Add(4);
来源：http://kh.hahajie.cn

[D03] 在指定位置插入元素
来源：http://vp.colortex.cn

Py:   arr.insert(0, 0)
来源：http://wb.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bl.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rv.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://hd.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://wh.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ha.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://it.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://il.shxzukj.cn

[D04] 删除元素
来源：http://bk.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nq.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xr.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ti.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://up.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vw.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vu.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cg.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qk.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://uh.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sv.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oe.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qt.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://pe.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://cr.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://wr.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wk.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://me.shxzukj.cn

[D06] 数组长度
来源：http://sb.lnxyls.cn

Py:   len(arr)
来源：http://vm.yuexingan06.cn

PHP:  count($arr);
来源：http://hb.jianghongdianzi.cn

JS:   arr.length
来源：http://cm.wgjwhj.cn

TS:   arr.length
来源：http://oi.huanxung.cn

Java: list.size();
来源：http://mp.huixiangedu.cn

Go:   len(arr)
来源：http://mm.521024.cn

Ruby: arr.length; arr.size
来源：http://ba.nszjky.cn

C#:   list.Count;
来源：http://vx.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://hs.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zu.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nu.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://hj.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://wo.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://ss.huanxung.cn

Go:   arr[1:4]
来源：http://ru.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://or.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://qi.shxzukj.cn

[D08] 合并两个数组
来源：http://yj.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://uw.521024.cn

PHP:  array_merge($a, $b);
来源：http://my.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tc.haigaiapp.cn

TS:   [...a, ...b];
来源：http://cl.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rb.wgjwhj.cn

Go:   append(a, b...)
来源：http://zx.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://tq.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://is.wgjwhj.cn

[D09] 排序（升序）
来源：http://pt.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ww.9csxet.cn

PHP:  sort($arr);
来源：http://mm.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ka.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tx.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ix.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ti.colortex.cn

Ruby: arr.sort
来源：http://pa.jctech888.com.cn

C#:   list.Sort();
来源：http://sq.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hl.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wq.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yt.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://is.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iv.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ap.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://al.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zu.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tp.nszjky.cn

[D11] 反转数组
来源：http://ms.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sx.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://ju.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dk.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://zu.szxytkj.cn

Java: Collections.reverse(list);
来源：http://ur.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://ug.haigaiapp.cn

Ruby: arr.reverse
来源：http://aw.gzmigu.cn

C#:   list.Reverse();
来源：http://lx.bjjhwx.cn

[D12] 查找元素下标
来源：http://pz.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://bl.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uv.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gg.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fs.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ej.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://mc.nicolike.cn

Ruby: arr.index(x)
来源：http://rf.9csxet.cn

C#:   list.IndexOf(x);
来源：http://kc.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://kw.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xk.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oh.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://im.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://wp.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rl.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nu.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zz.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oi.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://bc.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xl.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uf.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://ay.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://bb.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vv.bookmarksfly.cn

Go:   // 手写循环
来源：http://cx.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bg.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chemitech.net.cn

[D15] 去重
来源：http://pd.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sw.shxzukj.cn

PHP:  array_unique($arr);
来源：http://ia.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://oq.9csxet.cn

TS:   [...new Set(arr)]
来源：http://hl.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qa.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vk.wgjwhj.cn

Ruby: arr.uniq
来源：http://sr.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://xh.hnjuh.cn

[D16] 求和与平均值
来源：http://uy.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xa.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fz.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mi.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jp.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uj.lnxyls.cn

Go:   // 手写循环累加
来源：http://ip.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rv.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://tk.hahajie.cn

[D17] 最大值与最小值
来源：http://aa.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://pj.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://ux.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pb.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://qi.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vi.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://sl.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://pl.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://bk.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://em.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://sd.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dw.gzmigu.cn

TS:   nested.flat();
来源：http://pr.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pg.haigaiapp.cn

Go:   // 手写双层循环
来源：http://st.shtwfgs.cn

Ruby: nested.flatten
来源：http://gb.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mi.chemitech.net.cn

[D19] 按字段分组
来源：http://hj.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uk.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uq.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qp.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lv.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rk.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://jr.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gg.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nv.asd995.cn

[D20] 统计每个元素出现次数
来源：http://hn.hahajie.cn

Py:   Counter(arr)
来源：http://pg.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://mb.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yg.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gg.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ak.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://tl.yuexingan06.cn

Ruby: arr.tally
来源：http://wo.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hw.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://qj.lnxyls.cn

Py:   x in arr
来源：http://bz.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://tj.panjiajie.cn

JS:   arr.includes(x)
来源：http://go.yuexingan06.cn

TS:   arr.includes(x)
来源：http://we.bjjhwx.cn

Java: list.contains(x)
来源：http://fa.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://hs.huanxung.cn

Ruby: arr.include?(x)
来源：http://lq.nicolike.cn

C#:   list.Contains(x)
来源：http://je.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://wn.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wj.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ti.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xp.nicolike.cn

TS:   [...arr];
来源：http://ia.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://wr.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rz.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://kb.nicolike.cn

C#:   new List<int>(list);
来源：http://bs.huanxung.cn

[D23] reduce 累积计算
来源：http://ku.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gm.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fm.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mw.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ho.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://io.newstarts.cn

Go:   // 手写循环
来源：http://py.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lm.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ij.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://ce.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tl.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://es.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wv.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://he.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vx.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bm.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ec.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://js.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://vy.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ek.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ey.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vb.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ww.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zj.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sm.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rs.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qt.shxzukj.cn

[D26] 数组转字符串
来源：http://md.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://sq.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://fq.szsharing.cn

JS:   arr.join(", ")
来源：http://xc.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://pu.shtwfgs.cn

Java: String.join(", ", list)
来源：http://rn.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://lm.huanxung.cn

Ruby: arr.join(", ")
来源：http://zd.nicolike.cn

C#:   string.Join(", ", list)
来源：http://be.hahajie.cn

================================================================================
来源：http://yh.lnxyls.cn

E. 字符串处理
来源：http://tj.colortex.cn

================================================================================
来源：http://ed.bjjhwx.cn

[E01] 拼接字符串
来源：http://or.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zq.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vc.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xh.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://na.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xm.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gp.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bd.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rq.nszjky.cn

[E02] 重复字符串
来源：http://eu.shxzukj.cn

Py:   "ab" * 3
来源：http://ts.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://yv.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://nx.yuntaijiaju.cn


<!-- 参考信息 -->