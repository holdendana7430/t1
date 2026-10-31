代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://pa.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://nj.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://qj.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kf.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://xk.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://zg.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ux.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://nz.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wi.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ms.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rp.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kc.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ei.9csxet.cn

Go:   func add(a, b int) int
来源：http://eb.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ma.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xz.nszjky.cn

[C14] 泛型函数
来源：http://bq.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://px.lnxyls.cn

PHP:  // 无泛型
来源：http://hn.colortex.cn

JS:   // 无泛型
来源：http://zh.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mo.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lm.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ur.hahajie.cn

Ruby: # 无泛型
来源：http://sz.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fy.szsharing.cn

[C15] 解构 / 展开参数
来源：http://gz.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pg.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://bg.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ph.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bc.hnjuh.cn

Java: // 无解构
来源：http://im.szsharing.cn

Go:   // 无解构
来源：http://ay.521024.cn

Ruby: a, b = pair
来源：http://uc.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://ca.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://ta.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sk.panjiajie.cn

PHP:  // 无重载
来源：http://vf.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yj.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ng.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mc.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://qt.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://oh.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yz.nicolike.cn

================================================================================
来源：http://hu.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://tj.521024.cn

================================================================================
来源：http://xx.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://wj.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iz.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dd.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vu.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ob.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zm.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://vj.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://uo.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://je.szsharing.cn

[D02] 追加元素到末尾
来源：http://uh.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oi.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fr.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://hf.szxytkj.cn

TS:   arr.push(4);
来源：http://gw.chemitech.net.cn

Java: list.add(4);
来源：http://pj.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://sy.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://bo.jctech888.com.cn

C#:   list.Add(4);
来源：http://tq.nszjky.cn

[D03] 在指定位置插入元素
来源：http://tj.521024.cn

Py:   arr.insert(0, 0)
来源：http://lz.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eg.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lp.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://ea.chemitech.net.cn

Java: list.add(0, 0);
来源：http://lt.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xp.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bb.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://vb.shtwfgs.cn

[D04] 删除元素
来源：http://yr.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ct.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xg.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zz.asd995.cn

TS:   arr.splice(0, 1);
来源：http://uv.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vf.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://so.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cf.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://we.9csxet.cn

[D05] 访问与修改元素
来源：http://hc.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://op.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ht.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hf.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://gf.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://fi.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://ck.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://my.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ca.jctech888.com.cn

[D06] 数组长度
来源：http://ca.colortex.cn

Py:   len(arr)
来源：http://lv.szsharing.cn

PHP:  count($arr);
来源：http://dd.jctech888.com.cn

JS:   arr.length
来源：http://nc.szsharing.cn

TS:   arr.length
来源：http://tn.haigaiapp.cn

Java: list.size();
来源：http://ta.szsharing.cn

Go:   len(arr)
来源：http://xh.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://wg.bjjhwx.cn

C#:   list.Count;
来源：http://df.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://ok.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nk.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yr.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://lo.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://ua.newstarts.cn

Java: list.subList(1, 4);
来源：http://lp.szxytkj.cn

Go:   arr[1:4]
来源：http://kd.colortex.cn

Ruby: arr[1, 3]
来源：http://aa.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ro.colortex.cn

[D08] 合并两个数组
来源：http://hq.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://ne.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://fo.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hm.shxzukj.cn

TS:   [...a, ...b];
来源：http://la.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rm.hnjuh.cn

Go:   append(a, b...)
来源：http://mq.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://lj.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://ws.asd995.cn

[D09] 排序（升序）
来源：http://tp.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://bb.szsharing.cn

PHP:  sort($arr);
来源：http://gg.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gc.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pg.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ap.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zz.szxytkj.cn

Ruby: arr.sort
来源：http://sr.bookmarksfly.cn

C#:   list.Sort();
来源：http://xc.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kv.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://og.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://su.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qx.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fq.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iq.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mz.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sv.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vs.9csxet.cn

[D11] 反转数组
来源：http://fj.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sy.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://hc.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gj.521024.cn

TS:   [...arr].reverse();
来源：http://te.9csxet.cn

Java: Collections.reverse(list);
来源：http://vx.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://hg.hnjuh.cn

Ruby: arr.reverse
来源：http://ef.shxzukj.cn

C#:   list.Reverse();
来源：http://ms.lnxyls.cn

[D12] 查找元素下标
来源：http://ez.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://hv.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zf.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pl.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rt.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zt.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://dz.bjjhwx.cn

Ruby: arr.index(x)
来源：http://qg.asd995.cn

C#:   list.IndexOf(x);
来源：http://vo.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://vj.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zb.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ro.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://ok.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://yz.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://an.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uv.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zr.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bt.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://so.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rn.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qz.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://zv.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://wo.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kt.521024.cn

Go:   // 手写循环
来源：http://fy.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dg.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xh.jctech888.com.cn

[D15] 去重
来源：http://pd.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tz.colortex.cn

PHP:  array_unique($arr);
来源：http://gf.newstarts.cn

JS:   [...new Set(arr)]
来源：http://bz.hahajie.cn

TS:   [...new Set(arr)]
来源：http://ny.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uo.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cl.szsharing.cn

Ruby: arr.uniq
来源：http://xz.521024.cn

C#:   list.Distinct().ToList()
来源：http://si.jctech888.com.cn

[D16] 求和与平均值
来源：http://gg.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ad.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ja.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://so.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ha.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nx.wgjwhj.cn

Go:   // 手写循环累加
来源：http://mc.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nc.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://na.lnxyls.cn

[D17] 最大值与最小值
来源：http://hv.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://fk.521024.cn

PHP:  max($arr);  min($arr);
来源：http://yh.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yz.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://mx.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jn.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mr.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://qv.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://vs.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://ht.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wm.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://yz.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://to.newstarts.cn

TS:   nested.flat();
来源：http://gz.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ap.521024.cn

Go:   // 手写双层循环
来源：http://fi.shxzskj.cn

Ruby: nested.flatten
来源：http://ef.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qi.huanxung.cn

[D19] 按字段分组
来源：http://lj.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ly.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pk.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lh.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://in.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ju.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://zd.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nm.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bi.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://va.huixiangedu.cn

Py:   Counter(arr)
来源：http://wz.nicolike.cn

PHP:  array_count_values($arr);
来源：http://ld.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://it.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vv.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ha.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://ih.9csxet.cn

Ruby: arr.tally
来源：http://kn.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dg.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://xc.bjjhwx.cn

Py:   x in arr
来源：http://ku.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://yv.colortex.cn

JS:   arr.includes(x)
来源：http://ag.nicolike.cn

TS:   arr.includes(x)
来源：http://pq.haigaiapp.cn

Java: list.contains(x)
来源：http://ge.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://md.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://go.521024.cn

C#:   list.Contains(x)
来源：http://nj.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://ln.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bf.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gc.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rc.shxzukj.cn

TS:   [...arr];
来源：http://xw.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://gb.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nn.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://mh.gzmigu.cn

C#:   new List<int>(list);
来源：http://cl.wgjwhj.cn

[D23] reduce 累积计算
来源：http://xq.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fs.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nq.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qe.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ol.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jc.muxihuayi.cn

Go:   // 手写循环
来源：http://ds.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kb.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oz.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://dq.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wo.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zp.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xc.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qi.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ie.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lw.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pc.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://we.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://yd.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ff.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hp.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lf.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xm.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gp.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ws.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://md.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cq.yuexingan06.cn

[D26] 数组转字符串
来源：http://mb.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://zp.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://kh.gzmigu.cn

JS:   arr.join(", ")
来源：http://as.szxytkj.cn

TS:   arr.join(", ")
来源：http://pc.haigaiapp.cn

Java: String.join(", ", list)
来源：http://hb.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://wb.asd995.cn

Ruby: arr.join(", ")
来源：http://ad.huanxung.cn

C#:   string.Join(", ", list)
来源：http://qf.newstarts.cn

================================================================================
来源：http://vk.newstarts.cn

E. 字符串处理
来源：http://le.shxzukj.cn

================================================================================
来源：http://fd.shtwfgs.cn

[E01] 拼接字符串
来源：http://qf.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tr.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nd.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://su.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yz.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vk.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fr.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kt.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ni.asd995.cn

[E02] 重复字符串
来源：http://do.nszjky.cn

Py:   "ab" * 3
来源：http://mm.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ex.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://tv.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://bo.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://dq.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://zc.bjjhwx.cn

Ruby: "ab" * 3
来源：http://cg.shxzskj.cn


<!-- 参考信息 -->