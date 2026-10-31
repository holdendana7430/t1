代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://ih.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://gj.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://sh.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tp.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://cf.521024.cn

Ruby: -> { puts "run" }.call
来源：http://uf.hahajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ca.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://ow.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rj.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kj.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qs.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xk.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xo.szxytkj.cn

Go:   func add(a, b int) int
来源：http://tw.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ja.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wk.shxzskj.cn

[C14] 泛型函数
来源：http://uq.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kl.newstarts.cn

PHP:  // 无泛型
来源：http://hr.muxihuayi.cn

JS:   // 无泛型
来源：http://je.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ls.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ht.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tu.szxytkj.cn

Ruby: # 无泛型
来源：http://vd.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xh.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://ev.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tb.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://mz.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sp.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wi.huixiangedu.cn

Java: // 无解构
来源：http://va.shtwfgs.cn

Go:   // 无解构
来源：http://zr.nszjky.cn

Ruby: a, b = pair
来源：http://wr.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://bt.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://yh.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zf.shtwfgs.cn

PHP:  // 无重载
来源：http://tb.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lp.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://cj.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://de.521024.cn

Go:   // 无重载：用不同函数名
来源：http://gf.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://ry.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lc.shxzskj.cn

================================================================================
来源：http://ll.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://td.szxytkj.cn

================================================================================
来源：http://rq.szsharing.cn

[D01] 创建数组 / 列表
来源：http://nd.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tk.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rc.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ry.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mv.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://do.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://da.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://ms.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ij.521024.cn

[D02] 追加元素到末尾
来源：http://io.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ru.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vz.muxihuayi.cn

JS:   arr.push(4);
来源：http://wh.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://ia.wgjwhj.cn

Java: list.add(4);
来源：http://jw.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://ru.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://eg.bookmarksfly.cn

C#:   list.Add(4);
来源：http://jc.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://yt.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://lf.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ba.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zr.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://rj.szxytkj.cn

Java: list.add(0, 0);
来源：http://bu.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kz.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ke.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://ia.gzmigu.cn

[D04] 删除元素
来源：http://wa.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xt.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ef.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ui.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://ze.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oq.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dg.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vu.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ef.521024.cn

[D05] 访问与修改元素
来源：http://wn.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wy.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pd.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bh.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://gx.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://ld.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://px.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pl.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ai.jianghongdianzi.cn

[D06] 数组长度
来源：http://wa.huanxung.cn

Py:   len(arr)
来源：http://dj.huanxung.cn

PHP:  count($arr);
来源：http://rx.bjjhwx.cn

JS:   arr.length
来源：http://ni.wgjwhj.cn

TS:   arr.length
来源：http://md.yuntaijiaju.cn

Java: list.size();
来源：http://wt.asd995.cn

Go:   len(arr)
来源：http://rj.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://wu.521024.cn

C#:   list.Count;
来源：http://qi.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://wn.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vj.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bu.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://pw.colortex.cn

TS:   arr.slice(1, 4);
来源：http://wz.lnxyls.cn

Java: list.subList(1, 4);
来源：http://vf.haigaiapp.cn

Go:   arr[1:4]
来源：http://ts.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://xe.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://bw.nszjky.cn

[D08] 合并两个数组
来源：http://gy.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://zs.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://uw.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wg.gzmigu.cn

TS:   [...a, ...b];
来源：http://nf.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ol.panjiajie.cn

Go:   append(a, b...)
来源：http://op.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://fp.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://bn.wgjwhj.cn

[D09] 排序（升序）
来源：http://na.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://au.chemitech.net.cn

PHP:  sort($arr);
来源：http://eu.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ez.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rj.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mi.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dm.huanxung.cn

Ruby: arr.sort
来源：http://yh.szxytkj.cn

C#:   list.Sort();
来源：http://ml.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jd.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qo.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hb.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vb.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rq.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://re.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wk.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kj.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pq.yuexingan06.cn

[D11] 反转数组
来源：http://ez.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ag.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://pw.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lk.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://kz.colortex.cn

Java: Collections.reverse(list);
来源：http://cm.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://gr.jctech888.com.cn

Ruby: arr.reverse
来源：http://zs.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://gk.shtwfgs.cn

[D12] 查找元素下标
来源：http://fs.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://ov.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ld.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nd.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qu.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mf.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://fs.bjjhwx.cn

Ruby: arr.index(x)
来源：http://fk.colortex.cn

C#:   list.IndexOf(x);
来源：http://nw.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://gv.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mb.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rg.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://af.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://hu.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dn.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dw.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fv.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xp.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://mp.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ip.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rt.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://qg.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://fd.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ar.newstarts.cn

Go:   // 手写循环
来源：http://is.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ke.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gy.muxihuayi.cn

[D15] 去重
来源：http://hs.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xx.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://rt.colortex.cn

JS:   [...new Set(arr)]
来源：http://ad.nszjky.cn

TS:   [...new Set(arr)]
来源：http://ra.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pe.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ti.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://xl.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://kd.huanxung.cn

[D16] 求和与平均值
来源：http://mb.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ki.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://up.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rl.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cj.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mh.huanxung.cn

Go:   // 手写循环累加
来源：http://ot.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tr.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://pd.shxzskj.cn

[D17] 最大值与最小值
来源：http://pt.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://yn.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://uz.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://px.lnxyls.cn

TS:   Math.max(...arr);
来源：http://io.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://of.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ci.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://dg.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://lq.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://ip.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uj.colortex.cn

PHP:  array_merge(...$nested);
来源：http://ng.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fe.huanxung.cn

TS:   nested.flat();
来源：http://ph.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vj.hnjuh.cn

Go:   // 手写双层循环
来源：http://cu.wgjwhj.cn

Ruby: nested.flatten
来源：http://sr.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://et.haigaiapp.cn

[D19] 按字段分组
来源：http://km.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xl.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dw.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ue.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jj.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ac.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://rm.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jq.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xi.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://lx.huanxung.cn

Py:   Counter(arr)
来源：http://pa.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://ro.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fh.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ym.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pi.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://yc.haigaiapp.cn

Ruby: arr.tally
来源：http://hy.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zo.huanxung.cn

[D21] 判断是否包含某元素
来源：http://tu.bookmarksfly.cn

Py:   x in arr
来源：http://ts.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://dz.newstarts.cn

JS:   arr.includes(x)
来源：http://cs.bjjhwx.cn

TS:   arr.includes(x)
来源：http://kg.lnxyls.cn

Java: list.contains(x)
来源：http://eq.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://av.colortex.cn

Ruby: arr.include?(x)
来源：http://kk.wgjwhj.cn

C#:   list.Contains(x)
来源：http://rf.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://lb.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gh.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pt.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uv.lnxyls.cn

TS:   [...arr];
来源：http://qf.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://ah.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ez.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://ei.hnjuh.cn

C#:   new List<int>(list);
来源：http://ow.bjjhwx.cn

[D23] reduce 累积计算
来源：http://jj.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kd.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sg.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zf.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ji.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vo.jctech888.com.cn

Go:   // 手写循环
来源：http://fd.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uf.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hs.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://fz.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vz.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cx.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sh.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ql.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zf.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ec.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xe.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bu.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://jw.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rh.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bv.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ex.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ky.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bm.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uo.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://se.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://as.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://al.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://vn.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://mm.hahajie.cn

JS:   arr.join(", ")
来源：http://ri.521024.cn

TS:   arr.join(", ")
来源：http://ga.colortex.cn

Java: String.join(", ", list)
来源：http://bh.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://uz.9csxet.cn

Ruby: arr.join(", ")
来源：http://kh.9csxet.cn

C#:   string.Join(", ", list)
来源：http://lr.shtwfgs.cn

================================================================================
来源：http://ur.jianghongdianzi.cn

E. 字符串处理
来源：http://xr.haigaiapp.cn

================================================================================
来源：http://sp.haigaiapp.cn

[E01] 拼接字符串
来源：http://fm.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yf.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jq.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zi.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fr.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kb.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bi.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qg.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cj.huixiangedu.cn

[E02] 重复字符串
来源：http://lv.shtwfgs.cn

Py:   "ab" * 3
来源：http://cu.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://td.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://ag.521024.cn

TS:   "ab".repeat(3)
来源：http://zc.gzmigu.cn

Java: "ab".repeat(3)
来源：http://jl.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ya.huixiangedu.cn

Ruby: "ab" * 3
来源：http://wq.gzmigu.cn


<!-- 参考信息 -->