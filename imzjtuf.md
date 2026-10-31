代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cb.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yj.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hv.jctech888.com.cn

Ruby: # 无泛型
来源：http://uj.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ye.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://bb.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gv.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://np.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ql.gzmigu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bs.muxihuayi.cn

Java: // 无解构
来源：http://tk.asd995.cn

Go:   // 无解构
来源：http://ro.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://jx.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://ns.szsharing.cn

[C16] 函数 / 方法重载
来源：http://xu.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vx.panjiajie.cn

PHP:  // 无重载
来源：http://uh.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rc.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://ql.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://th.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://lm.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://gj.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vq.colortex.cn

================================================================================
来源：http://zq.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://da.jctech888.com.cn

================================================================================
来源：http://gu.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://wx.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gt.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xa.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ff.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://co.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://po.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://es.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://fq.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cn.szsharing.cn

[D02] 追加元素到末尾
来源：http://mi.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ak.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zn.521024.cn

JS:   arr.push(4);
来源：http://ze.newstarts.cn

TS:   arr.push(4);
来源：http://bg.jctech888.com.cn

Java: list.add(4);
来源：http://hb.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://ui.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://hw.521024.cn

C#:   list.Add(4);
来源：http://ab.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://ii.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://zo.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://en.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ce.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://un.huanxung.cn

Java: list.add(0, 0);
来源：http://em.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mm.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fq.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://hk.huixinmuqiang.cn

[D04] 删除元素
来源：http://ql.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rd.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yk.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lk.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://pe.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gv.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vz.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rj.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ku.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://wk.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qe.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vm.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://zd.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://lu.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://of.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yz.panjiajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zd.bookmarksfly.cn

[D06] 数组长度
来源：http://je.9csxet.cn

Py:   len(arr)
来源：http://yg.asd995.cn

PHP:  count($arr);
来源：http://mk.521024.cn

JS:   arr.length
来源：http://ct.lnxyls.cn

TS:   arr.length
来源：http://mo.shtwfgs.cn

Java: list.size();
来源：http://fy.huixinmuqiang.cn

Go:   len(arr)
来源：http://zq.newstarts.cn

Ruby: arr.length; arr.size
来源：http://kv.yuntaijiaju.cn

C#:   list.Count;
来源：http://oc.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://il.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qv.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ni.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://pp.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://wh.newstarts.cn

Java: list.subList(1, 4);
来源：http://wk.jctech888.com.cn

Go:   arr[1:4]
来源：http://xx.panjiajie.cn

Ruby: arr[1, 3]
来源：http://xa.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://wh.asd995.cn

[D08] 合并两个数组
来源：http://cb.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://ls.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://wl.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rz.chemitech.net.cn

TS:   [...a, ...b];
来源：http://xy.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bt.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://fd.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://dk.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://gj.hahajie.cn

[D09] 排序（升序）
来源：http://tr.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://uj.szxytkj.cn

PHP:  sort($arr);
来源：http://pl.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://re.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://re.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mf.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sp.jctech888.com.cn

Ruby: arr.sort
来源：http://lb.haigaiapp.cn

C#:   list.Sort();
来源：http://zl.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jm.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zu.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nj.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nu.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://op.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ud.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qj.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://se.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uw.wgjwhj.cn

[D11] 反转数组
来源：http://hi.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ty.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://sr.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vf.9csxet.cn

TS:   [...arr].reverse();
来源：http://fi.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://ae.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://to.hnjuh.cn

Ruby: arr.reverse
来源：http://gw.szsharing.cn

C#:   list.Reverse();
来源：http://zy.wgjwhj.cn

[D12] 查找元素下标
来源：http://iv.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://ui.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pl.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://md.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fj.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lk.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://eq.yuexingan06.cn

Ruby: arr.index(x)
来源：http://xd.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://vp.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://db.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xn.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jw.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://bb.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://os.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ag.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pe.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gk.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zz.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://sn.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qq.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ok.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://vm.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://pr.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ou.muxihuayi.cn

Go:   // 手写循环
来源：http://by.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yt.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zh.colortex.cn

[D15] 去重
来源：http://mh.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dm.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://bc.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://kn.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://ws.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zl.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xt.shxzskj.cn

Ruby: arr.uniq
来源：http://sy.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://tv.shxzskj.cn

[D16] 求和与平均值
来源：http://cq.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wk.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ql.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uv.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ln.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ey.9csxet.cn

Go:   // 手写循环累加
来源：http://rz.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://nf.hahajie.cn

[D17] 最大值与最小值
来源：http://nk.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://ww.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://tw.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ub.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://cx.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ft.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vk.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://pd.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://tz.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://yo.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aw.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://wa.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yn.huixiangedu.cn

TS:   nested.flat();
来源：http://kn.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://br.szxytkj.cn

Go:   // 手写双层循环
来源：http://mf.gzmigu.cn

Ruby: nested.flatten
来源：http://mm.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zz.colortex.cn

[D19] 按字段分组
来源：http://mi.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qi.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dr.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vd.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yf.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://te.521024.cn

Go:   // 手写 map[string][]T
来源：http://ga.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dv.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fs.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://xb.huixiangedu.cn

Py:   Counter(arr)
来源：http://ml.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://rm.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oe.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ke.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ex.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://ci.asd995.cn

Ruby: arr.tally
来源：http://ka.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zp.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://hj.newstarts.cn

Py:   x in arr
来源：http://gg.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://de.panjiajie.cn

JS:   arr.includes(x)
来源：http://kx.shxzukj.cn

TS:   arr.includes(x)
来源：http://qm.huanxung.cn

Java: list.contains(x)
来源：http://kg.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://ub.hahajie.cn

Ruby: arr.include?(x)
来源：http://sb.nicolike.cn

C#:   list.Contains(x)
来源：http://ce.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://sw.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sg.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ab.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jo.jctech888.com.cn

TS:   [...arr];
来源：http://wm.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://ci.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kn.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://ij.jctech888.com.cn

C#:   new List<int>(list);
来源：http://tw.chemitech.net.cn

[D23] reduce 累积计算
来源：http://ba.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://be.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ml.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ll.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rh.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kj.9csxet.cn

Go:   // 手写循环
来源：http://kt.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ms.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://od.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://de.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fl.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jx.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ii.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gh.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jj.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://du.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qv.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rm.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ru.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zb.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ka.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zh.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jm.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kq.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jr.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://li.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oz.hnjuh.cn

[D26] 数组转字符串
来源：http://pj.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://to.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://ng.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://ex.haigaiapp.cn

TS:   arr.join(", ")
来源：http://bl.lnxyls.cn

Java: String.join(", ", list)
来源：http://gz.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://zi.hahajie.cn

Ruby: arr.join(", ")
来源：http://ak.colortex.cn

C#:   string.Join(", ", list)
来源：http://wa.huixinmuqiang.cn

================================================================================
来源：http://nu.szxytkj.cn

E. 字符串处理
来源：http://pd.panjiajie.cn

================================================================================
来源：http://pb.jctech888.com.cn

[E01] 拼接字符串
来源：http://kb.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qv.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hq.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fg.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zd.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ej.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ds.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wl.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kp.haigaiapp.cn

[E02] 重复字符串
来源：http://gb.hahajie.cn

Py:   "ab" * 3
来源：http://qe.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://kn.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://wh.521024.cn

TS:   "ab".repeat(3)
来源：http://wk.szxytkj.cn

Java: "ab".repeat(3)
来源：http://wc.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://xp.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://cq.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gn.bjjhwx.cn

[E03] 截取子串
来源：http://ji.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kq.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qr.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fg.hahajie.cn

TS:   s.slice(1, 4)
来源：http://lz.nszjky.cn

Java: s.substring(1, 4)
来源：http://jf.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bw.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yh.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://pd.szxytkj.cn

[E04] 查找子串位置
来源：http://bu.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://zb.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://mb.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qi.521024.cn

TS:   s.indexOf("x")
来源：http://jc.chemitech.net.cn

Java: s.indexOf("x")
来源：http://xl.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://vw.szxytkj.cn

Ruby: s.index("x")
来源：http://fz.nszjky.cn

C#:   s.IndexOf("x")
来源：http://ps.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://su.chemitech.net.cn


<!-- 参考信息 -->