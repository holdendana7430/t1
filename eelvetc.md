代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://fd.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://ox.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uc.jianghongdianzi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hm.9csxet.cn

[C14] 泛型函数
来源：http://by.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bz.shtwfgs.cn

PHP:  // 无泛型
来源：http://ea.szsharing.cn

JS:   // 无泛型
来源：http://lm.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ku.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bs.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vm.muxihuayi.cn

Ruby: # 无泛型
来源：http://aj.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fl.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://pr.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vu.asd995.cn

PHP:  [$a, $b] = $pair;
来源：http://de.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qg.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://th.huixiangedu.cn

Java: // 无解构
来源：http://ww.huanxung.cn

Go:   // 无解构
来源：http://ki.hnjuh.cn

Ruby: a, b = pair
来源：http://jg.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://ud.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://wm.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ou.bjjhwx.cn

PHP:  // 无重载
来源：http://hd.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://da.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://er.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://za.huixinmuqiang.cn

Go:   // 无重载：用不同函数名
来源：http://vt.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ol.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jl.haigaiapp.cn

================================================================================
来源：http://eh.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://xw.colortex.cn

================================================================================
来源：http://ab.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://jd.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zd.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lq.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yp.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jv.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://er.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://bw.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://pn.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mk.szsharing.cn

[D02] 追加元素到末尾
来源：http://th.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uo.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gy.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://nr.newstarts.cn

TS:   arr.push(4);
来源：http://co.hahajie.cn

Java: list.add(4);
来源：http://ie.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://aw.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://zc.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://ec.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ko.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://pe.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qx.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gq.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://lt.521024.cn

Java: list.add(0, 0);
来源：http://wn.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fj.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dq.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://cl.bjjhwx.cn

[D04] 删除元素
来源：http://sl.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ca.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rf.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bd.asd995.cn

TS:   arr.splice(0, 1);
来源：http://am.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ce.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fz.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wb.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aw.colortex.cn

[D05] 访问与修改元素
来源：http://zg.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xt.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://le.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://br.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://lc.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://ff.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://jg.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wx.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dg.gzmigu.cn

[D06] 数组长度
来源：http://pu.9csxet.cn

Py:   len(arr)
来源：http://gr.haigaiapp.cn

PHP:  count($arr);
来源：http://fq.jctech888.com.cn

JS:   arr.length
来源：http://id.chemitech.net.cn

TS:   arr.length
来源：http://vb.bookmarksfly.cn

Java: list.size();
来源：http://ig.huixiangedu.cn

Go:   len(arr)
来源：http://bc.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://gv.yuexingan06.cn

C#:   list.Count;
来源：http://iu.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://va.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mh.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ie.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://kc.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://pp.nicolike.cn

Java: list.subList(1, 4);
来源：http://bw.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://pd.szxytkj.cn

Ruby: arr[1, 3]
来源：http://fd.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://wu.nszjky.cn

[D08] 合并两个数组
来源：http://gf.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://hq.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://xd.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://we.szsharing.cn

TS:   [...a, ...b];
来源：http://ih.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://co.521024.cn

Go:   append(a, b...)
来源：http://ks.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://cn.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://hz.haigaiapp.cn

[D09] 排序（升序）
来源：http://uy.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ak.bookmarksfly.cn

PHP:  sort($arr);
来源：http://vq.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://my.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ae.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://id.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fa.9csxet.cn

Ruby: arr.sort
来源：http://he.colortex.cn

C#:   list.Sort();
来源：http://nm.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fr.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://px.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pe.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://it.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://au.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://go.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xi.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ln.chemitech.net.cn

[D11] 反转数组
来源：http://xx.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wi.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://pd.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gw.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://fe.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://zl.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://ex.shtwfgs.cn

Ruby: arr.reverse
来源：http://fa.nszjky.cn

C#:   list.Reverse();
来源：http://ft.shxzskj.cn

[D12] 查找元素下标
来源：http://bo.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://en.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ym.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yj.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ue.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xz.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://oj.521024.cn

Ruby: arr.index(x)
来源：http://hn.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://ya.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://uq.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tq.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bu.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://xr.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://qd.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://io.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oe.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://az.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jr.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://xn.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://su.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://od.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://xc.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://cm.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tt.wgjwhj.cn

Go:   // 手写循环
来源：http://oo.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zz.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qh.nicolike.cn

[D15] 去重
来源：http://te.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qp.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ve.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://ag.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://es.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fv.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tm.newstarts.cn

Ruby: arr.uniq
来源：http://iq.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://ca.muxihuayi.cn

[D16] 求和与平均值
来源：http://ey.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ca.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xq.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yz.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xf.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ef.panjiajie.cn

Go:   // 手写循环累加
来源：http://vs.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jr.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://el.haigaiapp.cn

[D17] 最大值与最小值
来源：http://na.521024.cn

Py:   max(arr);  min(arr)
来源：http://gh.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://ci.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fk.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://or.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vg.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ss.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ry.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://rp.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://cn.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qg.huixiangedu.cn

PHP:  array_merge(...$nested);
来源：http://er.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oq.yuexingan06.cn

TS:   nested.flat();
来源：http://oq.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gs.chemitech.net.cn

Go:   // 手写双层循环
来源：http://vs.szxytkj.cn

Ruby: nested.flatten
来源：http://qr.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://io.huixiangedu.cn

[D19] 按字段分组
来源：http://gy.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jy.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jk.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lu.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aa.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bn.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://mz.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ds.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zx.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://ti.nicolike.cn

Py:   Counter(arr)
来源：http://fz.hahajie.cn

PHP:  array_count_values($arr);
来源：http://ox.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fq.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pa.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xd.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://vu.hahajie.cn

Ruby: arr.tally
来源：http://jj.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kl.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://zh.asd995.cn

Py:   x in arr
来源：http://qo.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://bc.panjiajie.cn

JS:   arr.includes(x)
来源：http://mz.szxytkj.cn

TS:   arr.includes(x)
来源：http://ge.newstarts.cn

Java: list.contains(x)
来源：http://wy.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://db.szxytkj.cn

Ruby: arr.include?(x)
来源：http://ts.bjjhwx.cn

C#:   list.Contains(x)
来源：http://lo.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://dz.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fj.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qc.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://op.yuntaijiaju.cn

TS:   [...arr];
来源：http://ha.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://kp.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ti.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://pc.shxzskj.cn

C#:   new List<int>(list);
来源：http://yl.hnjuh.cn

[D23] reduce 累积计算
来源：http://cw.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vv.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fw.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ne.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cu.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vx.nszjky.cn

Go:   // 手写循环
来源：http://ol.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ru.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://is.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://bh.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ke.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xb.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ri.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://il.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ok.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://up.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ou.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qq.asd995.cn

[D25] Set 集合去重与交并差
来源：http://mq.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hy.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hl.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eq.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gn.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qh.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pm.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xr.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://or.wgjwhj.cn

[D26] 数组转字符串
来源：http://vs.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://rn.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://aj.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://ok.gzmigu.cn

TS:   arr.join(", ")
来源：http://vh.nszjky.cn

Java: String.join(", ", list)
来源：http://oe.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://pz.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://gd.nicolike.cn

C#:   string.Join(", ", list)
来源：http://yp.shxzskj.cn

================================================================================
来源：http://eb.asd995.cn

E. 字符串处理
来源：http://bn.shtwfgs.cn

================================================================================
来源：http://bb.panjiajie.cn

[E01] 拼接字符串
来源：http://ym.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nc.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tr.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wd.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://va.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oj.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ga.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pk.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oy.hahajie.cn

[E02] 重复字符串
来源：http://rs.shxzukj.cn

Py:   "ab" * 3
来源：http://vi.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://cg.asd995.cn

JS:   "ab".repeat(3)
来源：http://vg.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://wy.9csxet.cn

Java: "ab".repeat(3)
来源：http://jv.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ab.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://ua.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iw.yuexingan06.cn

[E03] 截取子串
来源：http://dl.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ko.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ka.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gn.asd995.cn

TS:   s.slice(1, 4)
来源：http://dh.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://wp.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bn.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cr.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://uf.bjjhwx.cn

[E04] 查找子串位置
来源：http://bw.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://ih.bookmarksfly.cn


<!-- 参考信息 -->