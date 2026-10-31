代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yu.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ay.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rm.huanxung.cn

Ruby: # 无泛型
来源：http://da.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ax.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://np.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vs.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://nv.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vx.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cg.chemitech.net.cn

Java: // 无解构
来源：http://ek.hahajie.cn

Go:   // 无解构
来源：http://jt.yuexingan06.cn

Ruby: a, b = pair
来源：http://et.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://pk.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ys.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cx.jianghongdianzi.cn

PHP:  // 无重载
来源：http://ny.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jh.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://pw.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ve.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://ah.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://tf.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ap.shxzukj.cn

================================================================================
来源：http://jy.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://wo.panjiajie.cn

================================================================================
来源：http://gs.521024.cn

[D01] 创建数组 / 列表
来源：http://ym.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iz.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ae.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mm.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mp.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nb.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://ak.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://sa.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vi.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://jk.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://na.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cg.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://sy.hnjuh.cn

TS:   arr.push(4);
来源：http://hs.haigaiapp.cn

Java: list.add(4);
来源：http://kj.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://be.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://al.szxytkj.cn

C#:   list.Add(4);
来源：http://um.nszjky.cn

[D03] 在指定位置插入元素
来源：http://fp.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://yd.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hy.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hd.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ym.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ob.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eq.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://up.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://cs.hahajie.cn

[D04] 删除元素
来源：http://oi.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nn.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oo.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://me.521024.cn

TS:   arr.splice(0, 1);
来源：http://ke.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ab.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cn.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yp.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gx.shtwfgs.cn

[D05] 访问与修改元素
来源：http://jz.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://om.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://be.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://do.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://mw.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://rw.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://pt.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cm.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yb.lnxyls.cn

[D06] 数组长度
来源：http://gu.wgjwhj.cn

Py:   len(arr)
来源：http://dm.colortex.cn

PHP:  count($arr);
来源：http://ns.bookmarksfly.cn

JS:   arr.length
来源：http://fb.haigaiapp.cn

TS:   arr.length
来源：http://rs.nicolike.cn

Java: list.size();
来源：http://mr.hahajie.cn

Go:   len(arr)
来源：http://ck.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://ms.colortex.cn

C#:   list.Count;
来源：http://zu.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://ro.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ry.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pt.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://mt.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ol.szxytkj.cn

Java: list.subList(1, 4);
来源：http://de.haigaiapp.cn

Go:   arr[1:4]
来源：http://wi.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://vk.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://cf.haigaiapp.cn

[D08] 合并两个数组
来源：http://va.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://yu.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ea.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gk.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://qq.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fw.hnjuh.cn

Go:   append(a, b...)
来源：http://zf.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://gx.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://wi.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://zv.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://jn.shtwfgs.cn

PHP:  sort($arr);
来源：http://iy.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fu.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hr.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sh.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lr.shxzukj.cn

Ruby: arr.sort
来源：http://yk.nicolike.cn

C#:   list.Sort();
来源：http://vj.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://un.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tl.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mz.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ar.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ae.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tj.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rq.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ql.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cx.wgjwhj.cn

[D11] 反转数组
来源：http://ha.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ql.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://oo.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jx.colortex.cn

TS:   [...arr].reverse();
来源：http://bx.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://xx.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://op.asd995.cn

Ruby: arr.reverse
来源：http://qi.nicolike.cn

C#:   list.Reverse();
来源：http://ea.huanxung.cn

[D12] 查找元素下标
来源：http://ka.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://ys.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fg.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vs.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ti.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ir.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://jp.jctech888.com.cn

Ruby: arr.index(x)
来源：http://vd.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://pc.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://jf.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ro.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mx.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://oq.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://pl.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ga.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qz.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cz.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ja.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://kx.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iw.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ic.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://kd.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://eh.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bq.gzmigu.cn

Go:   // 手写循环
来源：http://dl.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ka.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fk.huanxung.cn

[D15] 去重
来源：http://cm.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aw.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://ae.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://xb.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://yl.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vw.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zd.shtwfgs.cn

Ruby: arr.uniq
来源：http://sn.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://wf.haigaiapp.cn

[D16] 求和与平均值
来源：http://hs.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sg.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wj.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yi.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hy.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bj.huixiangedu.cn

Go:   // 手写循环累加
来源：http://wo.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qf.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://do.nszjky.cn

[D17] 最大值与最小值
来源：http://sm.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://ji.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://wr.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rg.nicolike.cn

TS:   Math.max(...arr);
来源：http://ua.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://il.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ll.asd995.cn

Ruby: arr.max;  arr.min
来源：http://nq.asd995.cn

C#:   list.Max();  list.Min()
来源：http://me.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://ac.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mk.521024.cn

PHP:  array_merge(...$nested);
来源：http://wm.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dn.szxytkj.cn

TS:   nested.flat();
来源：http://xi.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fz.hahajie.cn

Go:   // 手写双层循环
来源：http://yf.szxytkj.cn

Ruby: nested.flatten
来源：http://fq.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cd.gzmigu.cn

[D19] 按字段分组
来源：http://al.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://we.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://on.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qu.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xf.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://im.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://rs.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ca.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lq.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://my.521024.cn

Py:   Counter(arr)
来源：http://qh.huanxung.cn

PHP:  array_count_values($arr);
来源：http://gz.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gl.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cx.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tf.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ai.lnxyls.cn

Ruby: arr.tally
来源：http://dd.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cc.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://gj.shtwfgs.cn

Py:   x in arr
来源：http://fv.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://wu.nicolike.cn

JS:   arr.includes(x)
来源：http://sy.9csxet.cn

TS:   arr.includes(x)
来源：http://ez.huixinmuqiang.cn

Java: list.contains(x)
来源：http://av.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://bb.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://ly.asd995.cn

C#:   list.Contains(x)
来源：http://mp.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://ub.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fx.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hm.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cw.huixinmuqiang.cn

TS:   [...arr];
来源：http://eb.colortex.cn

Java: new ArrayList<>(list);
来源：http://lb.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://aa.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://yq.hahajie.cn

C#:   new List<int>(list);
来源：http://te.jctech888.com.cn

[D23] reduce 累积计算
来源：http://sj.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://af.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tp.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sj.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nn.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cy.muxihuayi.cn

Go:   // 手写循环
来源：http://ub.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uq.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dv.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://jv.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fd.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hg.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ua.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ht.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cs.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hd.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://un.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pa.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://wx.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fr.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sv.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ru.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zx.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pu.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cp.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ho.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://us.newstarts.cn

[D26] 数组转字符串
来源：http://sj.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://jx.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://hy.hahajie.cn

JS:   arr.join(", ")
来源：http://sm.hahajie.cn

TS:   arr.join(", ")
来源：http://ru.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://yg.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://jn.gzmigu.cn

Ruby: arr.join(", ")
来源：http://lp.nszjky.cn

C#:   string.Join(", ", list)
来源：http://wt.chemitech.net.cn

================================================================================
来源：http://eb.newstarts.cn

E. 字符串处理
来源：http://sb.hnjuh.cn

================================================================================
来源：http://vh.521024.cn

[E01] 拼接字符串
来源：http://uk.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dk.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://id.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vt.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xl.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fb.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jx.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sg.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bu.hnjuh.cn

[E02] 重复字符串
来源：http://qo.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://ct.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://yn.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://ow.szsharing.cn

TS:   "ab".repeat(3)
来源：http://wh.szsharing.cn

Java: "ab".repeat(3)
来源：http://jh.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://xd.muxihuayi.cn

Ruby: "ab" * 3
来源：http://qp.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ah.shxzskj.cn

[E03] 截取子串
来源：http://uh.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jk.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ue.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zh.szsharing.cn

TS:   s.slice(1, 4)
来源：http://xr.hahajie.cn

Java: s.substring(1, 4)
来源：http://rm.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cv.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cn.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://in.shtwfgs.cn

[E04] 查找子串位置
来源：http://la.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://xc.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://jx.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qo.newstarts.cn

TS:   s.indexOf("x")
来源：http://rk.asd995.cn

Java: s.indexOf("x")
来源：http://sp.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ml.huanxung.cn

Ruby: s.index("x")
来源：http://sx.asd995.cn

C#:   s.IndexOf("x")
来源：http://iw.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xc.521024.cn


<!-- 参考信息 -->