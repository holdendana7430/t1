代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://ha.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://jk.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ov.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://vo.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ou.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xr.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ec.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lw.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wg.huanxung.cn

Go:   func add(a, b int) int
来源：http://eb.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hn.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fg.9csxet.cn

[C14] 泛型函数
来源：http://xa.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qy.nicolike.cn

PHP:  // 无泛型
来源：http://tf.hahajie.cn

JS:   // 无泛型
来源：http://sf.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qa.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rt.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gm.huanxung.cn

Ruby: # 无泛型
来源：http://cz.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://le.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://he.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mk.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ey.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ou.muxihuayi.cn

Java: // 无解构
来源：http://kp.huixinmuqiang.cn

Go:   // 无解构
来源：http://si.bjjhwx.cn

Ruby: a, b = pair
来源：http://ov.szsharing.cn

C#:   var (a, b) = pair;
来源：http://ww.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ne.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rl.shxzskj.cn

PHP:  // 无重载
来源：http://gq.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qs.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://hz.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vc.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://xd.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://jq.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ia.asd995.cn

================================================================================
来源：http://pa.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://pr.huanxung.cn

================================================================================
来源：http://fs.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://se.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://li.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pf.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nt.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tj.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ee.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://sv.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://du.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://es.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://jg.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ti.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jd.hahajie.cn

JS:   arr.push(4);
来源：http://og.huanxung.cn

TS:   arr.push(4);
来源：http://uy.nszjky.cn

Java: list.add(4);
来源：http://cy.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://on.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://te.gzmigu.cn

C#:   list.Add(4);
来源：http://oc.szsharing.cn

[D03] 在指定位置插入元素
来源：http://wj.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://pv.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vl.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ck.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://cy.9csxet.cn

Java: list.add(0, 0);
来源：http://hp.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yx.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ny.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://hk.panjiajie.cn

[D04] 删除元素
来源：http://vt.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mf.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cd.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://td.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://ui.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yv.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bb.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rh.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kj.shxzskj.cn

[D05] 访问与修改元素
来源：http://yp.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fq.muxihuayi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wp.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dl.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://dl.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://eo.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://pw.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ai.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iy.bjjhwx.cn

[D06] 数组长度
来源：http://cw.haigaiapp.cn

Py:   len(arr)
来源：http://zx.shxzskj.cn

PHP:  count($arr);
来源：http://sl.muxihuayi.cn

JS:   arr.length
来源：http://qn.asd995.cn

TS:   arr.length
来源：http://xx.jctech888.com.cn

Java: list.size();
来源：http://oi.newstarts.cn

Go:   len(arr)
来源：http://fh.nszjky.cn

Ruby: arr.length; arr.size
来源：http://df.muxihuayi.cn

C#:   list.Count;
来源：http://ul.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://kp.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wm.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ib.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://wr.colortex.cn

TS:   arr.slice(1, 4);
来源：http://oe.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://yl.nicolike.cn

Go:   arr[1:4]
来源：http://wl.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://fb.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://as.hahajie.cn

[D08] 合并两个数组
来源：http://cu.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://qh.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ou.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wg.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://mv.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bh.newstarts.cn

Go:   append(a, b...)
来源：http://ko.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://rr.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://pr.wgjwhj.cn

[D09] 排序（升序）
来源：http://gc.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://zh.shxzukj.cn

PHP:  sort($arr);
来源：http://nz.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ok.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cq.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yf.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yi.haigaiapp.cn

Ruby: arr.sort
来源：http://no.shxzskj.cn

C#:   list.Sort();
来源：http://vw.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wq.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oy.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yg.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bs.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xu.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lv.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qw.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://df.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ji.bookmarksfly.cn

[D11] 反转数组
来源：http://yo.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dq.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://up.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://in.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://qk.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://mj.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://ao.shxzskj.cn

Ruby: arr.reverse
来源：http://ub.szxytkj.cn

C#:   list.Reverse();
来源：http://va.hnjuh.cn

[D12] 查找元素下标
来源：http://wt.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://ib.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ej.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zn.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lc.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tx.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://gq.bjjhwx.cn

Ruby: arr.index(x)
来源：http://ij.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://lv.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://bx.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://us.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eo.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://dp.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://oj.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cv.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xn.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://em.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wx.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://gg.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ae.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xf.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://zf.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ax.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ro.hahajie.cn

Go:   // 手写循环
来源：http://pk.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vz.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eq.bjjhwx.cn

[D15] 去重
来源：http://ju.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vl.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://jp.asd995.cn

JS:   [...new Set(arr)]
来源：http://sa.nicolike.cn

TS:   [...new Set(arr)]
来源：http://nm.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gd.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cn.bookmarksfly.cn

Ruby: arr.uniq
来源：http://fr.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://gg.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://vs.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yg.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wi.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gy.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hg.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://em.shxzskj.cn

Go:   // 手写循环累加
来源：http://yc.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zy.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://ub.shxzskj.cn

[D17] 最大值与最小值
来源：http://mx.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://yb.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://ll.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gk.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://pr.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hk.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gz.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://va.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://qs.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://oz.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gk.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://pr.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fx.bjjhwx.cn

TS:   nested.flat();
来源：http://hb.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mo.haigaiapp.cn

Go:   // 手写双层循环
来源：http://hb.wgjwhj.cn

Ruby: nested.flatten
来源：http://hk.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lj.shxzskj.cn

[D19] 按字段分组
来源：http://td.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yc.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zr.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qu.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mj.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sv.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://sb.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nq.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ay.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://fp.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://ja.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://ie.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nx.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xz.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hk.9csxet.cn

Go:   // 手写 map[T]int
来源：http://fs.panjiajie.cn

Ruby: arr.tally
来源：http://dn.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xw.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://vw.szxytkj.cn

Py:   x in arr
来源：http://gt.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://ch.521024.cn

JS:   arr.includes(x)
来源：http://ri.jctech888.com.cn

TS:   arr.includes(x)
来源：http://gf.lnxyls.cn

Java: list.contains(x)
来源：http://rf.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://xd.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://wi.shtwfgs.cn

C#:   list.Contains(x)
来源：http://zs.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://dj.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pu.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xu.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aw.muxihuayi.cn

TS:   [...arr];
来源：http://ba.9csxet.cn

Java: new ArrayList<>(list);
来源：http://kg.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wl.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://rv.colortex.cn

C#:   new List<int>(list);
来源：http://dz.shxzskj.cn

[D23] reduce 累积计算
来源：http://nl.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hr.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dw.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://be.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ef.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://np.yuexingan06.cn

Go:   // 手写循环
来源：http://iu.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dr.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yq.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://uu.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://br.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://by.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yz.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rc.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fg.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yt.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tw.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uv.521024.cn

[D25] Set 集合去重与交并差
来源：http://fy.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vz.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qj.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gs.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jd.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ig.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mt.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fc.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bc.colortex.cn

[D26] 数组转字符串
来源：http://px.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://mv.colortex.cn

PHP:  implode(", ", $arr);
来源：http://vz.jctech888.com.cn

JS:   arr.join(", ")
来源：http://pn.yuexingan06.cn

TS:   arr.join(", ")
来源：http://ll.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://iy.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://lt.shxzskj.cn

Ruby: arr.join(", ")
来源：http://fl.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://yy.jianghongdianzi.cn

================================================================================
来源：http://nv.shtwfgs.cn

E. 字符串处理
来源：http://hi.yuexingan06.cn

================================================================================
来源：http://qt.521024.cn

[E01] 拼接字符串
来源：http://jl.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ih.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kv.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://of.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://or.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sw.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://od.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://my.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hx.nicolike.cn

[E02] 重复字符串
来源：http://qk.huanxung.cn

Py:   "ab" * 3
来源：http://jw.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://pe.nszjky.cn

JS:   "ab".repeat(3)
来源：http://ch.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://al.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://ct.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://lk.gzmigu.cn

Ruby: "ab" * 3
来源：http://iw.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yc.colortex.cn

[E03] 截取子串
来源：http://zc.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ts.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hi.huixinmuqiang.cn


<!-- 参考信息 -->