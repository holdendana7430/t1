代发 wailian999

Ruby: a, b = pair
来源：http://mz.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://fe.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://fh.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jk.huixiangedu.cn

PHP:  // 无重载
来源：http://nc.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yb.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://gi.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hd.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://tw.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://hl.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bn.yuntaijiaju.cn

================================================================================
来源：http://rb.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://kg.hnjuh.cn

================================================================================
来源：http://im.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://rc.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ff.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://be.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://af.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yq.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tu.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://al.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://dl.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ru.gzmigu.cn

[D02] 追加元素到末尾
来源：http://vx.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gz.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dh.muxihuayi.cn

JS:   arr.push(4);
来源：http://ye.9csxet.cn

TS:   arr.push(4);
来源：http://vy.bookmarksfly.cn

Java: list.add(4);
来源：http://ny.huanxung.cn

Go:   arr = append(arr, 4)
来源：http://rh.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://lt.huanxung.cn

C#:   list.Add(4);
来源：http://ma.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://pk.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://nf.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qc.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://um.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://sl.hnjuh.cn

Java: list.add(0, 0);
来源：http://ma.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jv.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ii.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://kz.huixiangedu.cn

[D04] 删除元素
来源：http://ef.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hp.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://by.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jl.asd995.cn

TS:   arr.splice(0, 1);
来源：http://qf.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ju.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ln.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tu.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pj.shxzukj.cn

[D05] 访问与修改元素
来源：http://ob.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eh.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wc.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://id.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://ye.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://cm.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ml.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kh.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lw.haigaiapp.cn

[D06] 数组长度
来源：http://gv.jctech888.com.cn

Py:   len(arr)
来源：http://lp.shxzskj.cn

PHP:  count($arr);
来源：http://tu.nicolike.cn

JS:   arr.length
来源：http://bp.asd995.cn

TS:   arr.length
来源：http://jw.haigaiapp.cn

Java: list.size();
来源：http://aa.chemitech.net.cn

Go:   len(arr)
来源：http://bx.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://yc.hnjuh.cn

C#:   list.Count;
来源：http://qm.nszjky.cn

[D07] 切片 / 取子数组
来源：http://et.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nq.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gu.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://gc.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://oe.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://tk.huixiangedu.cn

Go:   arr[1:4]
来源：http://wk.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://xl.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://cn.newstarts.cn

[D08] 合并两个数组
来源：http://ag.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://ad.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://xa.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://np.shxzukj.cn

TS:   [...a, ...b];
来源：http://ql.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uc.shxzukj.cn

Go:   append(a, b...)
来源：http://wy.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://km.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://rf.lnxyls.cn

[D09] 排序（升序）
来源：http://hm.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ir.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://mo.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ao.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mg.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://la.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://us.muxihuayi.cn

Ruby: arr.sort
来源：http://ww.huixiangedu.cn

C#:   list.Sort();
来源：http://ki.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nt.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ks.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bk.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fs.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hl.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ml.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jb.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ad.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ff.521024.cn

[D11] 反转数组
来源：http://if.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gg.szsharing.cn

PHP:  array_reverse($arr);
来源：http://ja.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lt.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://mp.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://nz.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://kz.nszjky.cn

Ruby: arr.reverse
来源：http://qv.haigaiapp.cn

C#:   list.Reverse();
来源：http://np.huixiangedu.cn

[D12] 查找元素下标
来源：http://qy.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://ka.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nj.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gn.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pb.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vw.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ag.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ix.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://nh.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://zc.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sp.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cp.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://sr.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://xo.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pm.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yo.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lw.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nd.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://vy.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ie.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ub.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://ey.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://nr.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oq.nicolike.cn

Go:   // 手写循环
来源：http://oo.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vo.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xb.hahajie.cn

[D15] 去重
来源：http://fj.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mj.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://ii.521024.cn

JS:   [...new Set(arr)]
来源：http://yk.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://bf.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pw.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ma.szsharing.cn

Ruby: arr.uniq
来源：http://sa.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://xw.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://fi.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ic.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nu.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mo.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pw.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ks.shxzukj.cn

Go:   // 手写循环累加
来源：http://da.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wn.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://cp.huanxung.cn

[D17] 最大值与最小值
来源：http://sh.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://qa.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://mj.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ut.colortex.cn

TS:   Math.max(...arr);
来源：http://ia.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sn.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ea.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://wh.asd995.cn

C#:   list.Max();  list.Min()
来源：http://lk.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://yr.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hu.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://gr.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ur.huanxung.cn

TS:   nested.flat();
来源：http://nu.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ut.huixiangedu.cn

Go:   // 手写双层循环
来源：http://yr.lnxyls.cn

Ruby: nested.flatten
来源：http://nb.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sn.huanxung.cn

[D19] 按字段分组
来源：http://gx.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ph.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gq.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://km.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pg.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pb.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://rq.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lf.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ra.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://tj.muxihuayi.cn

Py:   Counter(arr)
来源：http://zh.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://ms.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kt.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ix.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ai.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://gs.bjjhwx.cn

Ruby: arr.tally
来源：http://gw.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cb.hahajie.cn

[D21] 判断是否包含某元素
来源：http://jn.bookmarksfly.cn

Py:   x in arr
来源：http://tj.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://wu.huanxung.cn

JS:   arr.includes(x)
来源：http://fe.hahajie.cn

TS:   arr.includes(x)
来源：http://jv.bookmarksfly.cn

Java: list.contains(x)
来源：http://nt.521024.cn

Go:   slices.Contains(arr, x)
来源：http://ql.hahajie.cn

Ruby: arr.include?(x)
来源：http://rh.hnjuh.cn

C#:   list.Contains(x)
来源：http://vr.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://nn.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kn.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://th.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qy.szsharing.cn

TS:   [...arr];
来源：http://fs.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://ex.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://st.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://fj.shxzukj.cn

C#:   new List<int>(list);
来源：http://ic.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://ip.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lp.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hr.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ru.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://do.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gr.newstarts.cn

Go:   // 手写循环
来源：http://il.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bp.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fj.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://um.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fu.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xo.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://li.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://au.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uw.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zd.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hb.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zc.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ti.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ia.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ae.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lw.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ax.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bj.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qp.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qe.wgjwhj.cn

[D26] 数组转字符串
来源：http://yx.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://pd.colortex.cn

PHP:  implode(", ", $arr);
来源：http://ar.jctech888.com.cn

JS:   arr.join(", ")
来源：http://fm.bjjhwx.cn

TS:   arr.join(", ")
来源：http://zb.wgjwhj.cn

Java: String.join(", ", list)
来源：http://cg.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ke.panjiajie.cn

Ruby: arr.join(", ")
来源：http://wg.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://kx.colortex.cn

================================================================================
来源：http://yp.jianghongdianzi.cn

E. 字符串处理
来源：http://pc.gzmigu.cn

================================================================================
来源：http://qf.szsharing.cn

[E01] 拼接字符串
来源：http://ro.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mq.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ys.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://or.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://md.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bq.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ym.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://os.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hd.huixiangedu.cn

[E02] 重复字符串
来源：http://qa.huixiangedu.cn

Py:   "ab" * 3
来源：http://gr.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://by.asd995.cn

JS:   "ab".repeat(3)
来源：http://iw.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://hk.shxzskj.cn

Java: "ab".repeat(3)
来源：http://re.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://ja.shxzskj.cn

Ruby: "ab" * 3
来源：http://zy.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wc.gzmigu.cn

[E03] 截取子串
来源：http://qh.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mu.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ml.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ay.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://um.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://cv.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yl.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dp.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://pz.huixiangedu.cn

[E04] 查找子串位置
来源：http://co.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://yk.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://zw.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nz.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://cv.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://ro.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://mc.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://de.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://lx.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uz.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gl.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://to.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://je.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fk.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pc.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gf.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uy.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://px.szxytkj.cn

[E06] 替换子串
来源：http://sk.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rv.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ap.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cq.huixinmuqiang.cn


<!-- 参考信息 -->