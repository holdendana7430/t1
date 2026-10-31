代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://ss.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://xw.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zb.chemitech.net.cn

[C13] 类型声明 / 类型注解
来源：http://nn.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rm.haigaiapp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ga.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ve.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bq.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sm.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://zu.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://df.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cb.panjiajie.cn

[C14] 泛型函数
来源：http://ar.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kk.jctech888.com.cn

PHP:  // 无泛型
来源：http://ln.colortex.cn

JS:   // 无泛型
来源：http://en.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uv.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rt.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vg.nicolike.cn

Ruby: # 无泛型
来源：http://vv.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ws.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://ab.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uz.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://ks.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wr.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lb.nicolike.cn

Java: // 无解构
来源：http://uh.gzmigu.cn

Go:   // 无解构
来源：http://he.wgjwhj.cn

Ruby: a, b = pair
来源：http://gs.asd995.cn

C#:   var (a, b) = pair;
来源：http://ob.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://zy.muxihuayi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oo.szxytkj.cn

PHP:  // 无重载
来源：http://bp.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cv.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://ci.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vt.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://nr.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://bk.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ti.shtwfgs.cn

================================================================================
来源：http://ft.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://xo.521024.cn

================================================================================
来源：http://js.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://je.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://er.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kv.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jz.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fz.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dh.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://fg.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://bc.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pc.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://td.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pg.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xd.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://ob.shxzukj.cn

TS:   arr.push(4);
来源：http://ya.gzmigu.cn

Java: list.add(4);
来源：http://wn.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://ki.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://yp.shtwfgs.cn

C#:   list.Add(4);
来源：http://ym.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://gs.colortex.cn

Py:   arr.insert(0, 0)
来源：http://uz.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hq.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yh.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://hg.chemitech.net.cn

Java: list.add(0, 0);
来源：http://bb.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hw.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fs.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://ei.szxytkj.cn

[D04] 删除元素
来源：http://ac.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jh.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ya.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://of.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://ly.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mf.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fa.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vo.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sm.nicolike.cn

[D05] 访问与修改元素
来源：http://fa.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fi.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nd.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ok.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://fd.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://uv.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://od.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://be.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wn.9csxet.cn

[D06] 数组长度
来源：http://sq.huixinmuqiang.cn

Py:   len(arr)
来源：http://nu.haigaiapp.cn

PHP:  count($arr);
来源：http://dd.colortex.cn

JS:   arr.length
来源：http://wc.huixiangedu.cn

TS:   arr.length
来源：http://pe.szxytkj.cn

Java: list.size();
来源：http://kn.newstarts.cn

Go:   len(arr)
来源：http://wq.newstarts.cn

Ruby: arr.length; arr.size
来源：http://cx.jctech888.com.cn

C#:   list.Count;
来源：http://xs.huanxung.cn

[D07] 切片 / 取子数组
来源：http://mu.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kv.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ly.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://mb.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://du.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://uv.lnxyls.cn

Go:   arr[1:4]
来源：http://vy.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://gj.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://yn.nicolike.cn

[D08] 合并两个数组
来源：http://he.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://oh.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://zd.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xv.shtwfgs.cn

TS:   [...a, ...b];
来源：http://tk.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yr.521024.cn

Go:   append(a, b...)
来源：http://qc.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://ag.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://iy.huixiangedu.cn

[D09] 排序（升序）
来源：http://tn.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://yp.haigaiapp.cn

PHP:  sort($arr);
来源：http://yc.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vt.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tt.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rh.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qn.bjjhwx.cn

Ruby: arr.sort
来源：http://eo.hahajie.cn

C#:   list.Sort();
来源：http://jl.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xz.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yf.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cz.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://np.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ac.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qj.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rt.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ei.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lm.haigaiapp.cn

[D11] 反转数组
来源：http://af.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wh.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://qk.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bv.hnjuh.cn

TS:   [...arr].reverse();
来源：http://ga.szxytkj.cn

Java: Collections.reverse(list);
来源：http://md.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://jq.shxzukj.cn

Ruby: arr.reverse
来源：http://yp.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://uj.muxihuayi.cn

[D12] 查找元素下标
来源：http://tw.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://yi.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dc.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pp.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oe.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hb.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://mx.nicolike.cn

Ruby: arr.index(x)
来源：http://ej.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://sj.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://oz.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jo.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wm.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://rr.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://pc.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mi.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jw.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mv.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yy.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://ck.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ie.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ce.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://xl.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://dn.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ik.gzmigu.cn

Go:   // 手写循环
来源：http://gh.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pg.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nk.asd995.cn

[D15] 去重
来源：http://fq.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kg.colortex.cn

PHP:  array_unique($arr);
来源：http://zu.newstarts.cn

JS:   [...new Set(arr)]
来源：http://pn.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://cp.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tq.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ex.hnjuh.cn

Ruby: arr.uniq
来源：http://ue.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://qi.newstarts.cn

[D16] 求和与平均值
来源：http://qw.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fl.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ez.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xk.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oo.521024.cn

Go:   // 手写循环累加
来源：http://lj.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vb.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://cy.jctech888.com.cn

[D17] 最大值与最小值
来源：http://on.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://qj.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://yw.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dy.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://gr.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ji.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xy.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://nc.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://ri.colortex.cn

[D18] 扁平化嵌套数组
来源：http://na.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fo.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://wv.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qa.panjiajie.cn

TS:   nested.flat();
来源：http://qs.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xh.newstarts.cn

Go:   // 手写双层循环
来源：http://mz.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://yx.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://az.jctech888.com.cn

[D19] 按字段分组
来源：http://xq.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xe.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://li.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qg.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nu.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pk.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://zm.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ke.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vj.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://wz.shtwfgs.cn

Py:   Counter(arr)
来源：http://bm.newstarts.cn

PHP:  array_count_values($arr);
来源：http://xm.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://me.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vl.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lm.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://ke.jctech888.com.cn

Ruby: arr.tally
来源：http://ly.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fu.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://rh.asd995.cn

Py:   x in arr
来源：http://ve.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://oq.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://sb.nszjky.cn

TS:   arr.includes(x)
来源：http://bo.bjjhwx.cn

Java: list.contains(x)
来源：http://dn.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://np.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://nz.lnxyls.cn

C#:   list.Contains(x)
来源：http://ny.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://bx.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mr.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wt.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://og.bookmarksfly.cn

TS:   [...arr];
来源：http://dt.newstarts.cn

Java: new ArrayList<>(list);
来源：http://yo.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zz.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://kl.asd995.cn

C#:   new List<int>(list);
来源：http://zv.huixiangedu.cn

[D23] reduce 累积计算
来源：http://jm.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ic.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iq.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ek.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://av.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qg.bookmarksfly.cn

Go:   // 手写循环
来源：http://oi.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qe.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xn.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://rt.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fy.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gn.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nm.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kg.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fc.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ld.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kn.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mt.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://ap.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xb.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pw.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hx.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fn.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gz.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qs.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jm.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xn.shtwfgs.cn

[D26] 数组转字符串
来源：http://yf.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://vf.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://xc.chemitech.net.cn

JS:   arr.join(", ")
来源：http://qv.szxytkj.cn

TS:   arr.join(", ")
来源：http://qy.bjjhwx.cn

Java: String.join(", ", list)
来源：http://gq.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://uu.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://zg.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://vo.haigaiapp.cn

================================================================================
来源：http://co.huanxung.cn

E. 字符串处理
来源：http://qp.bookmarksfly.cn

================================================================================
来源：http://qr.jctech888.com.cn

[E01] 拼接字符串
来源：http://gl.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ky.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hi.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://as.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uc.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zi.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vx.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ub.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oq.szxytkj.cn

[E02] 重复字符串
来源：http://de.muxihuayi.cn

Py:   "ab" * 3
来源：http://jv.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://fw.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://it.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://zu.9csxet.cn

Java: "ab".repeat(3)
来源：http://vi.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://gi.hnjuh.cn

Ruby: "ab" * 3
来源：http://pk.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pr.bjjhwx.cn

[E03] 截取子串
来源：http://rh.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dc.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nb.lnxyls.cn


<!-- 参考信息 -->