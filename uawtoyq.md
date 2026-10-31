代发 wailian999

PHP:  // 无重载
来源：http://tg.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hv.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://za.panjiajie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zb.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://pd.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://pj.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ax.gzmigu.cn

================================================================================
来源：http://yf.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://nf.huixiangedu.cn

================================================================================
来源：http://rw.huanxung.cn

[D01] 创建数组 / 列表
来源：http://zj.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pp.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rm.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pp.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ay.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gi.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://cd.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://rz.shxzskj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dp.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://bv.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ef.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hg.bookmarksfly.cn

JS:   arr.push(4);
来源：http://ca.gzmigu.cn

TS:   arr.push(4);
来源：http://tj.chemitech.net.cn

Java: list.add(4);
来源：http://ly.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://od.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://lv.newstarts.cn

C#:   list.Add(4);
来源：http://oe.huanxung.cn

[D03] 在指定位置插入元素
来源：http://tv.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://ra.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nk.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jn.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://ew.muxihuayi.cn

Java: list.add(0, 0);
来源：http://ql.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sx.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://by.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://vj.yuntaijiaju.cn

[D04] 删除元素
来源：http://gk.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lw.nicolike.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iw.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ch.asd995.cn

TS:   arr.splice(0, 1);
来源：http://yh.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mi.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wi.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jl.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wt.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://za.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ar.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kf.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qu.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://bn.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://yk.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://sa.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yh.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vv.shtwfgs.cn

[D06] 数组长度
来源：http://dt.szxytkj.cn

Py:   len(arr)
来源：http://sb.hahajie.cn

PHP:  count($arr);
来源：http://xx.shxzskj.cn

JS:   arr.length
来源：http://gs.huixinmuqiang.cn

TS:   arr.length
来源：http://tf.hnjuh.cn

Java: list.size();
来源：http://km.huixinmuqiang.cn

Go:   len(arr)
来源：http://qz.szsharing.cn

Ruby: arr.length; arr.size
来源：http://rh.muxihuayi.cn

C#:   list.Count;
来源：http://ri.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://xy.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ni.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oh.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://hh.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://so.asd995.cn

Java: list.subList(1, 4);
来源：http://zh.newstarts.cn

Go:   arr[1:4]
来源：http://ci.panjiajie.cn

Ruby: arr[1, 3]
来源：http://jw.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://vz.nicolike.cn

[D08] 合并两个数组
来源：http://eg.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://ew.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://bl.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ac.huanxung.cn

TS:   [...a, ...b];
来源：http://hk.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hh.haigaiapp.cn

Go:   append(a, b...)
来源：http://zo.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://gd.huixiangedu.cn

C#:   a.Concat(b).ToList()
来源：http://fg.asd995.cn

[D09] 排序（升序）
来源：http://td.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://mk.521024.cn

PHP:  sort($arr);
来源：http://pu.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jy.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mm.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tf.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tj.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ms.panjiajie.cn

C#:   list.Sort();
来源：http://fu.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pz.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zc.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qh.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cy.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ha.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rm.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ne.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aa.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://km.shxzskj.cn

[D11] 反转数组
来源：http://jj.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rv.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://uu.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jg.asd995.cn

TS:   [...arr].reverse();
来源：http://ue.panjiajie.cn

Java: Collections.reverse(list);
来源：http://eo.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://kv.colortex.cn

Ruby: arr.reverse
来源：http://ys.nicolike.cn

C#:   list.Reverse();
来源：http://el.nszjky.cn

[D12] 查找元素下标
来源：http://af.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://tf.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wh.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yp.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://my.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yr.asd995.cn

Go:   slices.Index(arr, x)
来源：http://gn.huixiangedu.cn

Ruby: arr.index(x)
来源：http://px.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://ga.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://fv.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rf.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ms.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://ly.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://vi.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qd.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://in.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ff.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vo.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://we.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ez.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uo.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://rq.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://dz.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fx.9csxet.cn

Go:   // 手写循环
来源：http://xz.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uc.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wn.shtwfgs.cn

[D15] 去重
来源：http://hg.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sx.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://nw.nszjky.cn

JS:   [...new Set(arr)]
来源：http://sg.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://vz.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sk.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xu.bookmarksfly.cn

Ruby: arr.uniq
来源：http://lz.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://de.yuexingan06.cn

[D16] 求和与平均值
来源：http://yx.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xj.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://np.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qd.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://se.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hs.bjjhwx.cn

Go:   // 手写循环累加
来源：http://wt.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://um.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://ap.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://ti.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://sf.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://ow.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hk.newstarts.cn

TS:   Math.max(...arr);
来源：http://ur.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://id.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fk.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://gp.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://ng.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://hv.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xg.521024.cn

PHP:  array_merge(...$nested);
来源：http://ue.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ox.hnjuh.cn

TS:   nested.flat();
来源：http://pi.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vr.shxzskj.cn

Go:   // 手写双层循环
来源：http://cc.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://lg.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fn.shxzskj.cn

[D19] 按字段分组
来源：http://ao.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xt.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ak.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://io.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gt.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zj.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://ym.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qr.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qy.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://lg.nszjky.cn

Py:   Counter(arr)
来源：http://xq.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://ni.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kh.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cm.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pr.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://qx.huixiangedu.cn

Ruby: arr.tally
来源：http://dr.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fo.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://ag.9csxet.cn

Py:   x in arr
来源：http://yd.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://hh.szsharing.cn

JS:   arr.includes(x)
来源：http://yw.colortex.cn

TS:   arr.includes(x)
来源：http://st.hahajie.cn

Java: list.contains(x)
来源：http://mc.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://cn.panjiajie.cn

Ruby: arr.include?(x)
来源：http://ph.colortex.cn

C#:   list.Contains(x)
来源：http://bq.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://ej.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fy.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tk.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fi.szsharing.cn

TS:   [...arr];
来源：http://pn.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://nx.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oa.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://gd.szsharing.cn

C#:   new List<int>(list);
来源：http://jf.hahajie.cn

[D23] reduce 累积计算
来源：http://wq.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dw.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://no.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ij.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ch.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vw.hnjuh.cn

Go:   // 手写循环
来源：http://rx.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cx.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zs.521024.cn

[D24] 字典 / Map 基本操作
来源：http://zk.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://on.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ph.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qi.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bq.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ko.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://us.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gf.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yl.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://yt.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vl.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dp.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cq.huanxung.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ut.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://we.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sz.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sh.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://io.hnjuh.cn

[D26] 数组转字符串
来源：http://gb.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://fv.521024.cn

PHP:  implode(", ", $arr);
来源：http://ab.jctech888.com.cn

JS:   arr.join(", ")
来源：http://xq.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://pr.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://ml.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://dr.521024.cn

Ruby: arr.join(", ")
来源：http://zh.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://nk.521024.cn

================================================================================
来源：http://zl.huixinmuqiang.cn

E. 字符串处理
来源：http://jf.yuexingan06.cn

================================================================================
来源：http://bf.huixiangedu.cn

[E01] 拼接字符串
来源：http://oz.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qb.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dh.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fq.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tg.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://we.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fg.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zb.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rw.panjiajie.cn

[E02] 重复字符串
来源：http://it.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://tx.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://yr.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://ju.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://an.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://ab.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ri.shxzukj.cn

Ruby: "ab" * 3
来源：http://yy.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oa.gzmigu.cn

[E03] 截取子串
来源：http://vi.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mb.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://op.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dq.9csxet.cn

TS:   s.slice(1, 4)
来源：http://jl.asd995.cn

Java: s.substring(1, 4)
来源：http://de.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nc.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://db.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://rs.shxzukj.cn

[E04] 查找子串位置
来源：http://iu.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://fo.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://tl.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://re.shxzukj.cn

TS:   s.indexOf("x")
来源：http://as.szsharing.cn

Java: s.indexOf("x")
来源：http://aq.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://pw.haigaiapp.cn

Ruby: s.index("x")
来源：http://bd.huanxung.cn

C#:   s.IndexOf("x")
来源：http://or.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://es.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ai.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lv.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bv.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hb.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oq.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wc.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ic.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://en.haigaiapp.cn

[E06] 替换子串
来源：http://hy.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://md.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ak.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zd.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://kc.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oj.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://og.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mp.shtwfgs.cn


<!-- 参考信息 -->