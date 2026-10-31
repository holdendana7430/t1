代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://be.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://iz.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ss.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://un.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tb.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vd.hahajie.cn

Java: // 无解构
来源：http://wk.bookmarksfly.cn

Go:   // 无解构
来源：http://ms.shxzukj.cn

Ruby: a, b = pair
来源：http://xr.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://pt.szsharing.cn

[C16] 函数 / 方法重载
来源：http://ih.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nz.chemitech.net.cn

PHP:  // 无重载
来源：http://jb.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lx.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://tw.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zn.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://js.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://gr.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hd.nicolike.cn

================================================================================
来源：http://yx.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://cu.muxihuayi.cn

================================================================================
来源：http://cq.asd995.cn

[D01] 创建数组 / 列表
来源：http://dd.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iv.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ju.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ey.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yy.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vz.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://af.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://oo.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gd.shxzukj.cn

[D02] 追加元素到末尾
来源：http://un.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://om.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ep.szxytkj.cn

JS:   arr.push(4);
来源：http://su.hnjuh.cn

TS:   arr.push(4);
来源：http://mp.panjiajie.cn

Java: list.add(4);
来源：http://um.asd995.cn

Go:   arr = append(arr, 4)
来源：http://cb.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://tp.hahajie.cn

C#:   list.Add(4);
来源：http://zf.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://xh.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://xr.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tf.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ej.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://bt.szxytkj.cn

Java: list.add(0, 0);
来源：http://cy.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mc.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zc.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://an.huixinmuqiang.cn

[D04] 删除元素
来源：http://ld.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yr.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rp.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gp.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://hx.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://em.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zq.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tc.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://re.jctech888.com.cn

[D05] 访问与修改元素
来源：http://ig.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jv.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ko.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jk.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://tt.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://xb.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://zp.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kq.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://px.lnxyls.cn

[D06] 数组长度
来源：http://us.yuntaijiaju.cn

Py:   len(arr)
来源：http://iq.szsharing.cn

PHP:  count($arr);
来源：http://fc.bjjhwx.cn

JS:   arr.length
来源：http://td.hnjuh.cn

TS:   arr.length
来源：http://ke.shtwfgs.cn

Java: list.size();
来源：http://yq.hahajie.cn

Go:   len(arr)
来源：http://cs.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://ca.huixinmuqiang.cn

C#:   list.Count;
来源：http://wl.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://ab.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vf.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uv.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://mc.colortex.cn

TS:   arr.slice(1, 4);
来源：http://rk.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://bf.chemitech.net.cn

Go:   arr[1:4]
来源：http://hf.lnxyls.cn

Ruby: arr[1, 3]
来源：http://cm.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://yg.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://xj.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://cr.yuntaijiaju.cn

PHP:  array_merge($a, $b);
来源：http://fz.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://io.hahajie.cn

TS:   [...a, ...b];
来源：http://ce.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gj.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://qv.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://uu.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://cz.nicolike.cn

[D09] 排序（升序）
来源：http://kt.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://lk.shxzukj.cn

PHP:  sort($arr);
来源：http://mg.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tm.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kj.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bg.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ce.panjiajie.cn

Ruby: arr.sort
来源：http://ka.shtwfgs.cn

C#:   list.Sort();
来源：http://po.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ie.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rv.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qa.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eb.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://py.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oy.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sd.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ua.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bz.panjiajie.cn

[D11] 反转数组
来源：http://mv.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bj.nicolike.cn

PHP:  array_reverse($arr);
来源：http://hd.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ss.szsharing.cn

TS:   [...arr].reverse();
来源：http://ds.colortex.cn

Java: Collections.reverse(list);
来源：http://gy.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://jf.huixiangedu.cn

Ruby: arr.reverse
来源：http://nc.bjjhwx.cn

C#:   list.Reverse();
来源：http://yf.szxytkj.cn

[D12] 查找元素下标
来源：http://ix.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://jx.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sp.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ee.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ud.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ve.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://rx.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://qy.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://ha.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://jj.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bc.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uv.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://xp.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://bn.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qf.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://is.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sb.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uu.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://bu.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://li.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kw.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://gu.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://zt.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ol.shtwfgs.cn

Go:   // 手写循环
来源：http://yq.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://md.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vb.jctech888.com.cn

[D15] 去重
来源：http://gn.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ra.hnjuh.cn

PHP:  array_unique($arr);
来源：http://pm.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://xx.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ba.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kg.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nr.szxytkj.cn

Ruby: arr.uniq
来源：http://kq.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://lh.colortex.cn

[D16] 求和与平均值
来源：http://aj.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bc.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fu.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rh.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sc.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hp.hnjuh.cn

Go:   // 手写循环累加
来源：http://ek.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xa.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://gc.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://do.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://ag.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://hg.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vi.hahajie.cn

TS:   Math.max(...arr);
来源：http://nx.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mb.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://me.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ts.colortex.cn

C#:   list.Max();  list.Min()
来源：http://gg.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://ru.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bu.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://va.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ei.haigaiapp.cn

TS:   nested.flat();
来源：http://ri.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gx.huixiangedu.cn

Go:   // 手写双层循环
来源：http://ue.chemitech.net.cn

Ruby: nested.flatten
来源：http://ki.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ho.521024.cn

[D19] 按字段分组
来源：http://zm.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cr.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ls.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cf.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ll.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ep.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://eq.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sm.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kg.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://pn.hahajie.cn

Py:   Counter(arr)
来源：http://dj.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://yb.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fn.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ac.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zk.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://gz.9csxet.cn

Ruby: arr.tally
来源：http://ui.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oj.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://ni.jianghongdianzi.cn

Py:   x in arr
来源：http://fb.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://bc.asd995.cn

JS:   arr.includes(x)
来源：http://wy.asd995.cn

TS:   arr.includes(x)
来源：http://bb.yuexingan06.cn

Java: list.contains(x)
来源：http://kh.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://ji.gzmigu.cn

Ruby: arr.include?(x)
来源：http://kn.wgjwhj.cn

C#:   list.Contains(x)
来源：http://mz.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://ig.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nc.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sg.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jc.9csxet.cn

TS:   [...arr];
来源：http://eg.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://uf.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vs.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://za.szsharing.cn

C#:   new List<int>(list);
来源：http://wb.szsharing.cn

[D23] reduce 累积计算
来源：http://dh.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lo.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bn.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mv.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uw.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jk.chemitech.net.cn

Go:   // 手写循环
来源：http://yk.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tx.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ow.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://ax.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sw.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qt.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bt.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lp.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ej.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yc.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hr.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://es.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://wg.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rq.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yc.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mo.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yb.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vi.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dt.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bv.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vk.9csxet.cn

[D26] 数组转字符串
来源：http://xc.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://mp.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://pb.hnjuh.cn

JS:   arr.join(", ")
来源：http://nf.shxzskj.cn

TS:   arr.join(", ")
来源：http://yd.521024.cn

Java: String.join(", ", list)
来源：http://ls.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://qx.colortex.cn

Ruby: arr.join(", ")
来源：http://nt.9csxet.cn

C#:   string.Join(", ", list)
来源：http://sn.jianghongdianzi.cn

================================================================================
来源：http://yo.yuexingan06.cn

E. 字符串处理
来源：http://vl.szxytkj.cn

================================================================================
来源：http://qp.shtwfgs.cn

[E01] 拼接字符串
来源：http://vp.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sv.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tl.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lq.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aq.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tv.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ws.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qc.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zn.hahajie.cn

[E02] 重复字符串
来源：http://gk.hnjuh.cn

Py:   "ab" * 3
来源：http://pk.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://zd.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://lr.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://zl.newstarts.cn

Java: "ab".repeat(3)
来源：http://mn.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://ad.haigaiapp.cn

Ruby: "ab" * 3
来源：http://jn.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ep.wgjwhj.cn

[E03] 截取子串
来源：http://fc.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vn.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ct.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zl.9csxet.cn

TS:   s.slice(1, 4)
来源：http://kn.hnjuh.cn

Java: s.substring(1, 4)
来源：http://zy.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://le.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lo.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://dp.panjiajie.cn

[E04] 查找子串位置
来源：http://pt.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://tk.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://vo.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rx.lnxyls.cn

TS:   s.indexOf("x")
来源：http://in.huixiangedu.cn

Java: s.indexOf("x")
来源：http://mh.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://kl.hahajie.cn

Ruby: s.index("x")
来源：http://hc.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://rf.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ie.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tc.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uf.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qj.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nz.asd995.cn


<!-- 参考信息 -->