代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://dl.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://sq.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://qh.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sl.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://sp.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://ep.chemitech.net.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kv.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://pz.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rm.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tw.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ti.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yr.szxytkj.cn

Go:   func add(a, b int) int
来源：http://lq.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mh.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pz.huanxung.cn

[C14] 泛型函数
来源：http://ug.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eh.nicolike.cn

PHP:  // 无泛型
来源：http://mq.yuntaijiaju.cn

JS:   // 无泛型
来源：http://il.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yd.chemitech.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dd.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zl.szxytkj.cn

Ruby: # 无泛型
来源：http://hy.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jp.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://ty.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xg.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://cq.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ae.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zm.szxytkj.cn

Java: // 无解构
来源：http://xc.bjjhwx.cn

Go:   // 无解构
来源：http://sl.bjjhwx.cn

Ruby: a, b = pair
来源：http://ve.newstarts.cn

C#:   var (a, b) = pair;
来源：http://pq.hahajie.cn

[C16] 函数 / 方法重载
来源：http://lr.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://my.nicolike.cn

PHP:  // 无重载
来源：http://fq.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xv.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://uv.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nu.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://xp.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://fr.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tg.colortex.cn

================================================================================
来源：http://hn.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://jr.yuntaijiaju.cn

================================================================================
来源：http://db.521024.cn

[D01] 创建数组 / 列表
来源：http://jz.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zz.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iq.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://er.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nj.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yx.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://ld.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://dt.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ss.asd995.cn

[D02] 追加元素到末尾
来源：http://xs.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ri.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ob.shxzukj.cn

JS:   arr.push(4);
来源：http://zv.bjjhwx.cn

TS:   arr.push(4);
来源：http://am.nszjky.cn

Java: list.add(4);
来源：http://ah.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ht.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://hb.gzmigu.cn

C#:   list.Add(4);
来源：http://lq.colortex.cn

[D03] 在指定位置插入元素
来源：http://jr.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://sr.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lw.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bo.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://wf.szsharing.cn

Java: list.add(0, 0);
来源：http://et.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://iy.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xk.asd995.cn

C#:   list.Insert(0, 0);
来源：http://qx.yuntaijiaju.cn

[D04] 删除元素
来源：http://vb.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kf.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ka.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zi.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://yi.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gz.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ds.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ax.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uv.521024.cn

[D05] 访问与修改元素
来源：http://ku.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iu.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kc.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fp.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://hi.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://ez.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://xj.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zt.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ck.gzmigu.cn

[D06] 数组长度
来源：http://fp.shxzukj.cn

Py:   len(arr)
来源：http://ef.hnjuh.cn

PHP:  count($arr);
来源：http://lw.szxytkj.cn

JS:   arr.length
来源：http://ze.hahajie.cn

TS:   arr.length
来源：http://jp.nszjky.cn

Java: list.size();
来源：http://ya.huixiangedu.cn

Go:   len(arr)
来源：http://el.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://no.nszjky.cn

C#:   list.Count;
来源：http://ec.nicolike.cn

[D07] 切片 / 取子数组
来源：http://sp.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tc.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wg.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://wm.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://yj.asd995.cn

Java: list.subList(1, 4);
来源：http://zd.bookmarksfly.cn

Go:   arr[1:4]
来源：http://wi.newstarts.cn

Ruby: arr[1, 3]
来源：http://ms.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://xb.colortex.cn

[D08] 合并两个数组
来源：http://xu.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://pu.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://sv.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eh.shxzskj.cn

TS:   [...a, ...b];
来源：http://ek.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ko.bjjhwx.cn

Go:   append(a, b...)
来源：http://fp.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://iw.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://tz.colortex.cn

[D09] 排序（升序）
来源：http://fs.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ww.shxzskj.cn

PHP:  sort($arr);
来源：http://sh.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lb.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bj.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vr.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yv.shxzskj.cn

Ruby: arr.sort
来源：http://lp.hnjuh.cn

C#:   list.Sort();
来源：http://id.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pr.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vo.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gf.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://an.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qs.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dn.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pk.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sg.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ct.hahajie.cn

[D11] 反转数组
来源：http://pd.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yg.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://zm.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cj.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://xa.shxzskj.cn

Java: Collections.reverse(list);
来源：http://ae.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://aa.gzmigu.cn

Ruby: arr.reverse
来源：http://we.szxytkj.cn

C#:   list.Reverse();
来源：http://yz.huanxung.cn

[D12] 查找元素下标
来源：http://ns.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://en.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tb.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mp.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dk.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://we.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://ly.szsharing.cn

Ruby: arr.index(x)
来源：http://rn.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://kx.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://im.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yc.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ax.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://bc.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://qi.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jf.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jg.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ok.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xn.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://wz.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zm.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jl.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://vd.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://gk.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qz.yuexingan06.cn

Go:   // 手写循环
来源：http://yr.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iy.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://by.muxihuayi.cn

[D15] 去重
来源：http://ng.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gc.lnxyls.cn

PHP:  array_unique($arr);
来源：http://es.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://gd.szsharing.cn

TS:   [...new Set(arr)]
来源：http://up.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ss.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yc.yuexingan06.cn

Ruby: arr.uniq
来源：http://pv.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://oq.panjiajie.cn

[D16] 求和与平均值
来源：http://yq.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zi.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mc.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://by.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xl.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kb.hahajie.cn

Go:   // 手写循环累加
来源：http://er.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://go.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://cm.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://yn.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://fn.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://va.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ef.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://mj.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ns.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ok.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://tc.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://xv.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://wd.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yf.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://pc.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gb.shxzukj.cn

TS:   nested.flat();
来源：http://tp.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xj.lnxyls.cn

Go:   // 手写双层循环
来源：http://rg.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://vs.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qk.colortex.cn

[D19] 按字段分组
来源：http://iz.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xx.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sk.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hj.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://az.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sg.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://nb.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ap.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ve.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://kf.huixiangedu.cn

Py:   Counter(arr)
来源：http://tg.huanxung.cn

PHP:  array_count_values($arr);
来源：http://wz.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bo.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mq.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ie.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://iv.hahajie.cn

Ruby: arr.tally
来源：http://ox.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qo.asd995.cn

[D21] 判断是否包含某元素
来源：http://hu.haigaiapp.cn

Py:   x in arr
来源：http://ps.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://gq.nicolike.cn

JS:   arr.includes(x)
来源：http://vc.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://lj.hahajie.cn

Java: list.contains(x)
来源：http://ty.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://mx.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://mc.521024.cn

C#:   list.Contains(x)
来源：http://lg.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://pi.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kq.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ap.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wd.bookmarksfly.cn

TS:   [...arr];
来源：http://zu.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://sd.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jd.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://vg.panjiajie.cn

C#:   new List<int>(list);
来源：http://zu.9csxet.cn

[D23] reduce 累积计算
来源：http://sl.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sm.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kr.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ag.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dt.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ig.shtwfgs.cn

Go:   // 手写循环
来源：http://rv.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ya.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ae.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://jq.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bo.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vm.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ba.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pn.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dt.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mi.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://af.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zg.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://zn.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nv.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fs.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xk.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jz.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sw.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dh.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bm.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ql.panjiajie.cn

[D26] 数组转字符串
来源：http://db.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://mc.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://ek.shtwfgs.cn

JS:   arr.join(", ")
来源：http://ls.gzmigu.cn

TS:   arr.join(", ")
来源：http://us.nicolike.cn

Java: String.join(", ", list)
来源：http://qr.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://tw.newstarts.cn

Ruby: arr.join(", ")
来源：http://ra.nicolike.cn

C#:   string.Join(", ", list)
来源：http://ay.521024.cn

================================================================================
来源：http://eq.shxzskj.cn

E. 字符串处理
来源：http://jb.newstarts.cn

================================================================================
来源：http://al.huanxung.cn

[E01] 拼接字符串
来源：http://bc.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lx.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jt.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xp.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dv.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fo.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ku.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zj.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lo.szxytkj.cn

[E02] 重复字符串
来源：http://qo.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://oh.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ax.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://ru.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://uy.521024.cn

Java: "ab".repeat(3)
来源：http://dp.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://ui.nszjky.cn

Ruby: "ab" * 3
来源：http://ee.wgjwhj.cn


<!-- 参考信息 -->