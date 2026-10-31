代发 wailian999

PHP:  // 无重载
来源：http://kt.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vc.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://pz.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kn.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://bm.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://ee.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zr.yuntaijiaju.cn

================================================================================
来源：http://vs.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://wk.wgjwhj.cn

================================================================================
来源：http://la.newstarts.cn

[D01] 创建数组 / 列表
来源：http://hf.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qq.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://in.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ny.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yi.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://to.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://rk.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://rs.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kv.szxytkj.cn

[D02] 追加元素到末尾
来源：http://uj.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://je.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://om.jctech888.com.cn

JS:   arr.push(4);
来源：http://td.colortex.cn

TS:   arr.push(4);
来源：http://ea.bookmarksfly.cn

Java: list.add(4);
来源：http://tk.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://rv.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://hm.hahajie.cn

C#:   list.Add(4);
来源：http://ne.colortex.cn

[D03] 在指定位置插入元素
来源：http://bc.colortex.cn

Py:   arr.insert(0, 0)
来源：http://sh.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://he.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ll.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://ai.521024.cn

Java: list.add(0, 0);
来源：http://un.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ck.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lp.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://aq.shtwfgs.cn

[D04] 删除元素
来源：http://gt.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bq.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fi.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qw.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://wc.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gd.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://td.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uw.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vh.hahajie.cn

[D05] 访问与修改元素
来源：http://bu.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xn.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kb.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xk.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://pc.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://ir.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://xv.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bo.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mp.lnxyls.cn

[D06] 数组长度
来源：http://zl.huixinmuqiang.cn

Py:   len(arr)
来源：http://lw.9csxet.cn

PHP:  count($arr);
来源：http://kq.jctech888.com.cn

JS:   arr.length
来源：http://ty.jctech888.com.cn

TS:   arr.length
来源：http://pg.shxzskj.cn

Java: list.size();
来源：http://tj.haigaiapp.cn

Go:   len(arr)
来源：http://ft.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://ky.asd995.cn

C#:   list.Count;
来源：http://xk.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://pb.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dk.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fn.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://yp.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://oj.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://zk.bookmarksfly.cn

Go:   arr[1:4]
来源：http://nb.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://bk.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://bq.9csxet.cn

[D08] 合并两个数组
来源：http://nz.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://go.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://ad.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nf.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://bh.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yi.muxihuayi.cn

Go:   append(a, b...)
来源：http://bw.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://he.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://bm.bjjhwx.cn

[D09] 排序（升序）
来源：http://br.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://bi.yuexingan06.cn

PHP:  sort($arr);
来源：http://ql.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gw.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pq.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://is.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xs.jianghongdianzi.cn

Ruby: arr.sort
来源：http://lo.huixinmuqiang.cn

C#:   list.Sort();
来源：http://ph.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qq.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rk.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jf.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dv.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gc.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://du.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hl.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sd.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oz.panjiajie.cn

[D11] 反转数组
来源：http://bd.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ls.9csxet.cn

PHP:  array_reverse($arr);
来源：http://rr.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tw.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://cp.szsharing.cn

Java: Collections.reverse(list);
来源：http://eq.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://df.chemitech.net.cn

Ruby: arr.reverse
来源：http://rf.lnxyls.cn

C#:   list.Reverse();
来源：http://mx.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://pf.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://hf.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://id.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tw.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jh.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rs.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://qz.hahajie.cn

Ruby: arr.index(x)
来源：http://ht.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://dv.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://ol.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bn.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tq.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://yc.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://gg.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zx.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cp.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mp.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tr.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://bc.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xy.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dz.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://qq.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://or.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vq.newstarts.cn

Go:   // 手写循环
来源：http://kf.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oj.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lw.9csxet.cn

[D15] 去重
来源：http://cq.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jq.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://ar.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://de.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://qe.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://no.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rb.haigaiapp.cn

Ruby: arr.uniq
来源：http://hn.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://qq.521024.cn

[D16] 求和与平均值
来源：http://du.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qo.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vq.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hn.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tq.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vm.yuexingan06.cn

Go:   // 手写循环累加
来源：http://dg.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://on.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ee.nszjky.cn

[D17] 最大值与最小值
来源：http://ry.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://dd.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://hc.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wg.9csxet.cn

TS:   Math.max(...arr);
来源：http://cm.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pq.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rm.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://og.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://as.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://lq.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ou.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://ve.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zd.yuexingan06.cn

TS:   nested.flat();
来源：http://yv.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xz.szsharing.cn

Go:   // 手写双层循环
来源：http://zp.lnxyls.cn

Ruby: nested.flatten
来源：http://mx.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zd.muxihuayi.cn

[D19] 按字段分组
来源：http://ob.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ce.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qs.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://px.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oc.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gw.asd995.cn

Go:   // 手写 map[string][]T
来源：http://qy.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://as.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hb.asd995.cn

[D20] 统计每个元素出现次数
来源：http://kr.nszjky.cn

Py:   Counter(arr)
来源：http://jv.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://uo.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hv.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://su.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sv.521024.cn

Go:   // 手写 map[T]int
来源：http://rn.huanxung.cn

Ruby: arr.tally
来源：http://mg.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kb.szsharing.cn

[D21] 判断是否包含某元素
来源：http://qf.yuntaijiaju.cn

Py:   x in arr
来源：http://rr.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://iz.asd995.cn

JS:   arr.includes(x)
来源：http://kj.huixiangedu.cn

TS:   arr.includes(x)
来源：http://js.shxzukj.cn

Java: list.contains(x)
来源：http://ot.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://ol.szxytkj.cn

Ruby: arr.include?(x)
来源：http://ih.gzmigu.cn

C#:   list.Contains(x)
来源：http://yq.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://ui.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hj.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pv.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ak.asd995.cn

TS:   [...arr];
来源：http://xj.521024.cn

Java: new ArrayList<>(list);
来源：http://iv.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://om.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://nm.nszjky.cn

C#:   new List<int>(list);
来源：http://lk.lnxyls.cn

[D23] reduce 累积计算
来源：http://ky.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fb.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mp.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wl.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xs.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qn.521024.cn

Go:   // 手写循环
来源：http://ta.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bv.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://md.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://se.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rv.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vj.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lq.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lu.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ov.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lm.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oq.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cm.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://bg.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uh.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fp.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jq.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://if.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zy.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://if.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qu.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kh.bjjhwx.cn

[D26] 数组转字符串
来源：http://pq.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://ua.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://km.haigaiapp.cn

JS:   arr.join(", ")
来源：http://oa.huanxung.cn

TS:   arr.join(", ")
来源：http://qe.521024.cn

Java: String.join(", ", list)
来源：http://lu.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://gz.nszjky.cn

Ruby: arr.join(", ")
来源：http://kw.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://lu.huixiangedu.cn

================================================================================
来源：http://zj.hnjuh.cn

E. 字符串处理
来源：http://ml.bookmarksfly.cn

================================================================================
来源：http://az.shxzskj.cn

[E01] 拼接字符串
来源：http://dt.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gh.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ne.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hn.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lm.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cf.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qg.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://il.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://te.lnxyls.cn

[E02] 重复字符串
来源：http://ii.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://nj.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://ds.nszjky.cn

JS:   "ab".repeat(3)
来源：http://rq.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ba.nicolike.cn

Java: "ab".repeat(3)
来源：http://bo.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://du.shxzskj.cn

Ruby: "ab" * 3
来源：http://em.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sq.asd995.cn

[E03] 截取子串
来源：http://va.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hm.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jr.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ot.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://el.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://rq.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bh.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wu.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://ut.jctech888.com.cn

[E04] 查找子串位置
来源：http://ym.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://lz.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://dj.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ho.521024.cn

TS:   s.indexOf("x")
来源：http://dy.huixiangedu.cn

Java: s.indexOf("x")
来源：http://bz.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://lr.asd995.cn

Ruby: s.index("x")
来源：http://ks.colortex.cn

C#:   s.IndexOf("x")
来源：http://mc.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ye.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ir.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sc.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gm.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ni.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fe.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tu.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rg.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ib.bookmarksfly.cn

[E06] 替换子串
来源：http://ew.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dp.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://xx.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fa.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://od.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ks.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mq.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pf.9csxet.cn


<!-- 参考信息 -->