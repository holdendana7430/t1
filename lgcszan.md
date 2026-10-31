代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qe.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ut.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bt.9csxet.cn

Ruby: # 无泛型
来源：http://mv.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tx.nszjky.cn

[C15] 解构 / 展开参数
来源：http://qu.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lg.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ed.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qz.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fh.yuexingan06.cn

Java: // 无解构
来源：http://hx.yuntaijiaju.cn

Go:   // 无解构
来源：http://oi.szsharing.cn

Ruby: a, b = pair
来源：http://jb.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://ua.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://tu.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cj.muxihuayi.cn

PHP:  // 无重载
来源：http://ko.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mm.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://ci.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://at.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://fc.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://bd.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fk.nszjky.cn

================================================================================
来源：http://uf.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://xw.gzmigu.cn

================================================================================
来源：http://kl.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://ok.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://im.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ga.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pj.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hy.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hj.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://sp.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://xi.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yh.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://tu.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fz.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ca.asd995.cn

JS:   arr.push(4);
来源：http://me.gzmigu.cn

TS:   arr.push(4);
来源：http://az.shtwfgs.cn

Java: list.add(4);
来源：http://zr.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ad.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ze.521024.cn

C#:   list.Add(4);
来源：http://xd.szsharing.cn

[D03] 在指定位置插入元素
来源：http://rb.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://yy.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ac.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uc.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ui.shtwfgs.cn

Java: list.add(0, 0);
来源：http://ff.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ay.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uj.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://aa.shxzukj.cn

[D04] 删除元素
来源：http://bm.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nb.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kr.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sr.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://tz.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ia.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fo.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ul.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://go.muxihuayi.cn

[D05] 访问与修改元素
来源：http://ok.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ya.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sv.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dn.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://uc.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bn.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://rc.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://em.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://if.szsharing.cn

[D06] 数组长度
来源：http://ge.newstarts.cn

Py:   len(arr)
来源：http://yp.lnxyls.cn

PHP:  count($arr);
来源：http://rl.jianghongdianzi.cn

JS:   arr.length
来源：http://gu.asd995.cn

TS:   arr.length
来源：http://fg.shxzukj.cn

Java: list.size();
来源：http://yo.bookmarksfly.cn

Go:   len(arr)
来源：http://si.szsharing.cn

Ruby: arr.length; arr.size
来源：http://fa.haigaiapp.cn

C#:   list.Count;
来源：http://qd.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://xn.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oq.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eu.colortex.cn

JS:   arr.slice(1, 4);
来源：http://mj.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://hf.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://nq.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://fv.lnxyls.cn

Ruby: arr[1, 3]
来源：http://qm.521024.cn

C#:   list.GetRange(1, 3);
来源：http://zq.shxzukj.cn

[D08] 合并两个数组
来源：http://hl.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://uq.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://rs.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fk.nszjky.cn

TS:   [...a, ...b];
来源：http://cn.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ns.lnxyls.cn

Go:   append(a, b...)
来源：http://km.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://uf.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://ad.shtwfgs.cn

[D09] 排序（升序）
来源：http://oo.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://fz.huixiangedu.cn

PHP:  sort($arr);
来源：http://cs.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nn.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://er.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fq.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sr.lnxyls.cn

Ruby: arr.sort
来源：http://bf.bookmarksfly.cn

C#:   list.Sort();
来源：http://hk.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iu.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://io.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bq.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ql.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ll.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iw.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jp.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pd.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wx.nszjky.cn

[D11] 反转数组
来源：http://xj.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ro.9csxet.cn

PHP:  array_reverse($arr);
来源：http://ax.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jr.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://xs.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://yi.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://ss.shxzskj.cn

Ruby: arr.reverse
来源：http://ms.521024.cn

C#:   list.Reverse();
来源：http://nx.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://yd.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://cv.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fu.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://po.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ok.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://da.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://mn.huixiangedu.cn

Ruby: arr.index(x)
来源：http://bf.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://nt.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://bq.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wg.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gn.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://lu.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://at.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ru.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oj.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yu.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://em.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://xg.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://as.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vt.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://kd.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://uw.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lm.yuexingan06.cn

Go:   // 手写循环
来源：http://ai.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jg.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zf.nicolike.cn

[D15] 去重
来源：http://sq.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tr.shxzukj.cn

PHP:  array_unique($arr);
来源：http://dr.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://ym.asd995.cn

TS:   [...new Set(arr)]
来源：http://jg.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bj.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wb.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://vp.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://bx.yuexingan06.cn

[D16] 求和与平均值
来源：http://df.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ir.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ou.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rm.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nn.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eh.panjiajie.cn

Go:   // 手写循环累加
来源：http://oc.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ri.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://en.szsharing.cn

[D17] 最大值与最小值
来源：http://dw.521024.cn

Py:   max(arr);  min(arr)
来源：http://iv.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://uu.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://st.newstarts.cn

TS:   Math.max(...arr);
来源：http://gd.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vq.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ih.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://ye.colortex.cn

C#:   list.Max();  list.Min()
来源：http://dh.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://ds.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wp.521024.cn

PHP:  array_merge(...$nested);
来源：http://cl.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dq.asd995.cn

TS:   nested.flat();
来源：http://hs.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pm.szxytkj.cn

Go:   // 手写双层循环
来源：http://fl.9csxet.cn

Ruby: nested.flatten
来源：http://hx.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wu.huixiangedu.cn

[D19] 按字段分组
来源：http://lv.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ix.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ji.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yz.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wb.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ic.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://av.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://we.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sb.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://sk.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://dd.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://pr.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hs.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://og.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://gp.szxytkj.cn

Ruby: arr.tally
来源：http://es.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ko.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://by.shtwfgs.cn

Py:   x in arr
来源：http://to.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://il.asd995.cn

JS:   arr.includes(x)
来源：http://ad.9csxet.cn

TS:   arr.includes(x)
来源：http://ez.nszjky.cn

Java: list.contains(x)
来源：http://jd.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://ph.asd995.cn

Ruby: arr.include?(x)
来源：http://wk.lnxyls.cn

C#:   list.Contains(x)
来源：http://sh.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://uo.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://po.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hv.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rd.shtwfgs.cn

TS:   [...arr];
来源：http://zr.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://zz.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ic.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://jb.nszjky.cn

C#:   new List<int>(list);
来源：http://kx.521024.cn

[D23] reduce 累积计算
来源：http://im.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qg.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xl.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ty.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://te.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zw.bjjhwx.cn

Go:   // 手写循环
来源：http://ei.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kl.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xg.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://mp.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sv.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hr.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://us.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ck.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oy.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mi.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ot.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rm.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://yy.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jo.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fd.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ul.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dk.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jr.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://om.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hg.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lh.newstarts.cn

[D26] 数组转字符串
来源：http://kg.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://wk.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://ot.gzmigu.cn

JS:   arr.join(", ")
来源：http://zp.nszjky.cn

TS:   arr.join(", ")
来源：http://wm.hahajie.cn

Java: String.join(", ", list)
来源：http://fl.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://jy.colortex.cn

Ruby: arr.join(", ")
来源：http://jv.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://jt.panjiajie.cn

================================================================================
来源：http://jc.huanxung.cn

E. 字符串处理
来源：http://xp.huixinmuqiang.cn

================================================================================
来源：http://zi.muxihuayi.cn

[E01] 拼接字符串
来源：http://pq.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mi.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ug.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://it.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://er.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sy.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hy.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ct.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qg.9csxet.cn

[E02] 重复字符串
来源：http://wz.asd995.cn

Py:   "ab" * 3
来源：http://hu.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://mk.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://qu.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://br.nszjky.cn

Java: "ab".repeat(3)
来源：http://nt.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://nn.asd995.cn

Ruby: "ab" * 3
来源：http://fo.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ws.shxzukj.cn

[E03] 截取子串
来源：http://av.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://da.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gz.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uv.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://yi.gzmigu.cn

Java: s.substring(1, 4)
来源：http://od.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ef.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jv.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://bz.nszjky.cn

[E04] 查找子串位置
来源：http://gm.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://fm.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://mi.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zo.shxzukj.cn

TS:   s.indexOf("x")
来源：http://ao.chemitech.net.cn

Java: s.indexOf("x")
来源：http://oj.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://se.haigaiapp.cn

Ruby: s.index("x")
来源：http://wk.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://lh.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cp.nszjky.cn


<!-- 参考信息 -->