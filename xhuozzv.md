代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://tv.521024.cn

Go:   func add(a, b int) int
来源：http://ab.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ft.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eo.shxzukj.cn

[C14] 泛型函数
来源：http://vo.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fy.bookmarksfly.cn

PHP:  // 无泛型
来源：http://nn.huanxung.cn

JS:   // 无泛型
来源：http://ap.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ao.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ou.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ma.huanxung.cn

Ruby: # 无泛型
来源：http://kt.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ma.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://ni.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xt.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://iy.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rr.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ue.huanxung.cn

Java: // 无解构
来源：http://ce.hnjuh.cn

Go:   // 无解构
来源：http://in.hnjuh.cn

Ruby: a, b = pair
来源：http://ip.huanxung.cn

C#:   var (a, b) = pair;
来源：http://dx.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://dr.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gq.asd995.cn

PHP:  // 无重载
来源：http://gr.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hd.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ci.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pd.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://pj.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://zc.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://va.nszjky.cn

================================================================================
来源：http://oq.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://sz.panjiajie.cn

================================================================================
来源：http://sr.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://nw.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rw.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zq.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iy.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kx.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pk.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://jd.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://kn.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wu.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ge.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lf.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qw.newstarts.cn

JS:   arr.push(4);
来源：http://xw.chemitech.net.cn

TS:   arr.push(4);
来源：http://rf.jianghongdianzi.cn

Java: list.add(4);
来源：http://vo.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://pg.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://em.bjjhwx.cn

C#:   list.Add(4);
来源：http://km.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://jx.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://ty.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cg.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kd.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://af.shxzskj.cn

Java: list.add(0, 0);
来源：http://if.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://og.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xz.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://yg.asd995.cn

[D04] 删除元素
来源：http://od.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oi.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uo.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pz.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://yy.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vu.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gg.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://du.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rg.huanxung.cn

[D05] 访问与修改元素
来源：http://gb.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://km.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hx.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fi.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://an.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://pq.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://we.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ug.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ck.huanxung.cn

[D06] 数组长度
来源：http://ox.gzmigu.cn

Py:   len(arr)
来源：http://nu.huixinmuqiang.cn

PHP:  count($arr);
来源：http://ld.huixiangedu.cn

JS:   arr.length
来源：http://zb.yuexingan06.cn

TS:   arr.length
来源：http://rg.9csxet.cn

Java: list.size();
来源：http://jx.shxzskj.cn

Go:   len(arr)
来源：http://fx.nszjky.cn

Ruby: arr.length; arr.size
来源：http://yc.chemitech.net.cn

C#:   list.Count;
来源：http://fr.521024.cn

[D07] 切片 / 取子数组
来源：http://lz.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yl.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gh.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://vk.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://ai.gzmigu.cn

Java: list.subList(1, 4);
来源：http://aw.nicolike.cn

Go:   arr[1:4]
来源：http://wh.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://wf.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://ex.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://ua.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://td.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://op.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pd.nszjky.cn

TS:   [...a, ...b];
来源：http://pm.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://re.lnxyls.cn

Go:   append(a, b...)
来源：http://vf.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://hj.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://hu.panjiajie.cn

[D09] 排序（升序）
来源：http://kh.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://tw.panjiajie.cn

PHP:  sort($arr);
来源：http://ri.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cu.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ww.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://re.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ls.bjjhwx.cn

Ruby: arr.sort
来源：http://zw.muxihuayi.cn

C#:   list.Sort();
来源：http://qx.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tg.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nr.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lf.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ul.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aw.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ku.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wn.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uu.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://je.nszjky.cn

[D11] 反转数组
来源：http://wo.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hq.asd995.cn

PHP:  array_reverse($arr);
来源：http://ce.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ze.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://zb.panjiajie.cn

Java: Collections.reverse(list);
来源：http://yb.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://ra.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://yi.szsharing.cn

C#:   list.Reverse();
来源：http://uj.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://ds.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://jq.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pq.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://un.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xs.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iz.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://mt.szxytkj.cn

Ruby: arr.index(x)
来源：http://jy.9csxet.cn

C#:   list.IndexOf(x);
来源：http://eb.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://hg.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tt.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mc.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ou.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://gh.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://th.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tb.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mi.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vq.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://ja.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mz.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pn.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://oj.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://kh.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kh.shxzukj.cn

Go:   // 手写循环
来源：http://xi.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wk.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uu.gzmigu.cn

[D15] 去重
来源：http://sg.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ih.hnjuh.cn

PHP:  array_unique($arr);
来源：http://sg.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://tj.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://gc.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qr.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ss.nszjky.cn

Ruby: arr.uniq
来源：http://kb.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://zm.521024.cn

[D16] 求和与平均值
来源：http://pi.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ud.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wr.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kp.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jb.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://az.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ip.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uw.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://hu.9csxet.cn

[D17] 最大值与最小值
来源：http://wn.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://nu.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://mg.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://re.nicolike.cn

TS:   Math.max(...arr);
来源：http://ih.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lg.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://in.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://ax.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://lf.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://lo.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://al.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://eg.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wp.9csxet.cn

TS:   nested.flat();
来源：http://ac.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ec.yuexingan06.cn

Go:   // 手写双层循环
来源：http://wg.asd995.cn

Ruby: nested.flatten
来源：http://jz.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://en.huanxung.cn

[D19] 按字段分组
来源：http://np.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lz.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kk.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ld.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://np.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://do.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://eb.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zz.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ob.asd995.cn

[D20] 统计每个元素出现次数
来源：http://bj.newstarts.cn

Py:   Counter(arr)
来源：http://dp.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://sp.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xs.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ik.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sl.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://qk.asd995.cn

Ruby: arr.tally
来源：http://nt.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cb.asd995.cn

[D21] 判断是否包含某元素
来源：http://yh.bookmarksfly.cn

Py:   x in arr
来源：http://gz.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://le.huanxung.cn

JS:   arr.includes(x)
来源：http://kq.shxzukj.cn

TS:   arr.includes(x)
来源：http://fp.hnjuh.cn

Java: list.contains(x)
来源：http://tt.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://cw.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://ow.haigaiapp.cn

C#:   list.Contains(x)
来源：http://cr.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://wv.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ge.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xz.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tn.bjjhwx.cn

TS:   [...arr];
来源：http://ar.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://wi.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gv.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://nq.bjjhwx.cn

C#:   new List<int>(list);
来源：http://fx.muxihuayi.cn

[D23] reduce 累积计算
来源：http://iq.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://be.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ji.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jh.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dp.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fw.nszjky.cn

Go:   // 手写循环
来源：http://mp.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lh.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kl.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://jg.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fn.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sm.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ux.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wb.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cm.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gw.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sy.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tf.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://qo.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ot.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lm.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ig.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vf.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xr.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ny.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jj.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qa.shtwfgs.cn

[D26] 数组转字符串
来源：http://mq.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://kq.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://as.jctech888.com.cn

JS:   arr.join(", ")
来源：http://ft.lnxyls.cn

TS:   arr.join(", ")
来源：http://bw.colortex.cn

Java: String.join(", ", list)
来源：http://an.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://qp.nszjky.cn

Ruby: arr.join(", ")
来源：http://ni.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://mc.nicolike.cn

================================================================================
来源：http://od.haigaiapp.cn

E. 字符串处理
来源：http://ys.newstarts.cn

================================================================================
来源：http://qr.panjiajie.cn

[E01] 拼接字符串
来源：http://wi.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qy.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bo.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fx.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ec.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bw.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://we.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dl.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jk.hnjuh.cn

[E02] 重复字符串
来源：http://ls.asd995.cn

Py:   "ab" * 3
来源：http://fi.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://ed.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://uv.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://jn.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://ci.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://yw.shxzskj.cn

Ruby: "ab" * 3
来源：http://ek.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dq.szxytkj.cn

[E03] 截取子串
来源：http://bw.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hs.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vq.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sq.huanxung.cn

TS:   s.slice(1, 4)
来源：http://ma.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://cj.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qs.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iv.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://lc.shxzukj.cn

[E04] 查找子串位置
来源：http://gg.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://rp.colortex.cn


<!-- 参考信息 -->