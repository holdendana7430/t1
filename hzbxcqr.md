代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wv.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://gl.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jp.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://zd.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cz.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yj.hnjuh.cn

Java: // 无解构
来源：http://sd.hahajie.cn

Go:   // 无解构
来源：http://jx.521024.cn

Ruby: a, b = pair
来源：http://px.newstarts.cn

C#:   var (a, b) = pair;
来源：http://wu.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://bn.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rq.lnxyls.cn

PHP:  // 无重载
来源：http://cc.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wh.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://of.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gz.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://kp.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://ff.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cf.nszjky.cn

================================================================================
来源：http://cg.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://wf.hnjuh.cn

================================================================================
来源：http://so.nszjky.cn

[D01] 创建数组 / 列表
来源：http://ch.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://no.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oq.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fc.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nv.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oe.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://bj.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://qt.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://of.newstarts.cn

[D02] 追加元素到末尾
来源：http://eh.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fq.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gu.gzmigu.cn

JS:   arr.push(4);
来源：http://dn.lnxyls.cn

TS:   arr.push(4);
来源：http://kz.huixiangedu.cn

Java: list.add(4);
来源：http://dh.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://tg.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://qt.nicolike.cn

C#:   list.Add(4);
来源：http://vk.nszjky.cn

[D03] 在指定位置插入元素
来源：http://cy.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://et.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ju.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ex.colortex.cn

TS:   arr.splice(0, 0, 0);
来源：http://ee.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://es.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mk.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oy.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://gz.szxytkj.cn

[D04] 删除元素
来源：http://bp.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hd.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://no.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ov.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://qm.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jt.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://av.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lv.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qz.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://tj.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lq.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sx.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bu.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://yy.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://tc.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://ft.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://td.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sa.shxzskj.cn

[D06] 数组长度
来源：http://cr.521024.cn

Py:   len(arr)
来源：http://yr.nszjky.cn

PHP:  count($arr);
来源：http://ei.szsharing.cn

JS:   arr.length
来源：http://me.colortex.cn

TS:   arr.length
来源：http://yu.wgjwhj.cn

Java: list.size();
来源：http://ia.szxytkj.cn

Go:   len(arr)
来源：http://fy.muxihuayi.cn

Ruby: arr.length; arr.size
来源：http://kr.szxytkj.cn

C#:   list.Count;
来源：http://vr.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://fd.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vp.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hx.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://vz.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://qp.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://yg.lnxyls.cn

Go:   arr[1:4]
来源：http://tn.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://zc.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://xs.521024.cn

[D08] 合并两个数组
来源：http://mq.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://wz.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://ef.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://po.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://ms.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jt.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ke.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://mi.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://ws.nicolike.cn

[D09] 排序（升序）
来源：http://dk.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fc.szsharing.cn

PHP:  sort($arr);
来源：http://fz.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yc.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tg.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uk.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yw.shxzukj.cn

Ruby: arr.sort
来源：http://dr.haigaiapp.cn

C#:   list.Sort();
来源：http://qh.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kj.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mo.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ls.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://to.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mp.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bb.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xi.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nh.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qu.gzmigu.cn

[D11] 反转数组
来源：http://sh.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lq.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://pp.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cb.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://yl.szxytkj.cn

Java: Collections.reverse(list);
来源：http://re.521024.cn

Go:   slices.Reverse(arr)
来源：http://uf.asd995.cn

Ruby: arr.reverse
来源：http://uw.nicolike.cn

C#:   list.Reverse();
来源：http://wg.shtwfgs.cn

[D12] 查找元素下标
来源：http://zx.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://zm.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pd.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wh.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qv.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fx.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://mv.asd995.cn

Ruby: arr.index(x)
来源：http://sy.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://wo.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://sz.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oh.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hc.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://nc.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://pk.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sb.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uz.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wy.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oc.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://it.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ap.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gc.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://bl.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://bc.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bg.asd995.cn

Go:   // 手写循环
来源：http://ci.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ax.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vp.panjiajie.cn

[D15] 去重
来源：http://hm.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gu.huanxung.cn

PHP:  array_unique($arr);
来源：http://tx.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://or.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://xd.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wk.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cx.hnjuh.cn

Ruby: arr.uniq
来源：http://hz.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://gg.szsharing.cn

[D16] 求和与平均值
来源：http://lp.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://be.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jg.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://so.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rr.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ow.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ey.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://en.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://bn.szsharing.cn

[D17] 最大值与最小值
来源：http://hz.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://wh.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://vc.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vc.szsharing.cn

TS:   Math.max(...arr);
来源：http://vf.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jq.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oj.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://wa.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://yd.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://hr.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wt.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://tg.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wy.jianghongdianzi.cn

TS:   nested.flat();
来源：http://wu.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xf.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://yn.wgjwhj.cn

Ruby: nested.flatten
来源：http://sd.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cc.yuntaijiaju.cn

[D19] 按字段分组
来源：http://ry.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kd.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dc.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xt.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ev.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yb.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://jo.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rc.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bw.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://pl.nszjky.cn

Py:   Counter(arr)
来源：http://ic.szsharing.cn

PHP:  array_count_values($arr);
来源：http://ba.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pl.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lo.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aj.asd995.cn

Go:   // 手写 map[T]int
来源：http://hs.szsharing.cn

Ruby: arr.tally
来源：http://lr.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wi.newstarts.cn

[D21] 判断是否包含某元素
来源：http://gx.huixiangedu.cn

Py:   x in arr
来源：http://wp.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://mv.asd995.cn

JS:   arr.includes(x)
来源：http://hk.wgjwhj.cn

TS:   arr.includes(x)
来源：http://po.shxzskj.cn

Java: list.contains(x)
来源：http://xf.521024.cn

Go:   slices.Contains(arr, x)
来源：http://yc.hahajie.cn

Ruby: arr.include?(x)
来源：http://fc.newstarts.cn

C#:   list.Contains(x)
来源：http://hc.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://hh.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jc.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gw.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://za.bookmarksfly.cn

TS:   [...arr];
来源：http://ut.nicolike.cn

Java: new ArrayList<>(list);
来源：http://kl.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gj.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://st.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://rf.haigaiapp.cn

[D23] reduce 累积计算
来源：http://nh.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iy.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gm.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dg.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yg.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cb.colortex.cn

Go:   // 手写循环
来源：http://es.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ib.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wb.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://tn.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://et.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ij.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lb.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://re.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sy.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uw.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://br.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zk.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://yt.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rc.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iz.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://io.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sn.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tj.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ls.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sh.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ii.colortex.cn

[D26] 数组转字符串
来源：http://ul.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://wn.colortex.cn

PHP:  implode(", ", $arr);
来源：http://sf.lnxyls.cn

JS:   arr.join(", ")
来源：http://cx.panjiajie.cn

TS:   arr.join(", ")
来源：http://ch.panjiajie.cn

Java: String.join(", ", list)
来源：http://nw.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://fm.asd995.cn

Ruby: arr.join(", ")
来源：http://oh.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://nq.nszjky.cn

================================================================================
来源：http://ef.shtwfgs.cn

E. 字符串处理
来源：http://ju.jctech888.com.cn

================================================================================
来源：http://st.nicolike.cn

[E01] 拼接字符串
来源：http://sr.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yh.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qu.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zs.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dx.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xr.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gq.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wg.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://du.jctech888.com.cn

[E02] 重复字符串
来源：http://ey.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://xq.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://yt.nicolike.cn

JS:   "ab".repeat(3)
来源：http://zl.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ua.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://za.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://sq.colortex.cn

Ruby: "ab" * 3
来源：http://it.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fb.huixiangedu.cn

[E03] 截取子串
来源：http://gb.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lb.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ri.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mn.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://wd.asd995.cn

Java: s.substring(1, 4)
来源：http://yk.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ss.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zf.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://vp.nszjky.cn

[E04] 查找子串位置
来源：http://un.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://kj.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://dt.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xp.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://sa.521024.cn

Java: s.indexOf("x")
来源：http://it.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://sw.huanxung.cn

Ruby: s.index("x")
来源：http://cb.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://eq.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ji.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xj.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nh.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fc.yuntaijiaju.cn


<!-- 参考信息 -->