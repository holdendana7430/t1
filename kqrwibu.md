代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://oo.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://wc.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ot.9csxet.cn

================================================================================
来源：http://yy.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://ge.lnxyls.cn

================================================================================
来源：http://vd.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://uf.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zv.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qv.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pz.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cl.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://np.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://sj.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://hv.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mu.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://cr.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ex.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cq.521024.cn

JS:   arr.push(4);
来源：http://rg.newstarts.cn

TS:   arr.push(4);
来源：http://aw.huixinmuqiang.cn

Java: list.add(4);
来源：http://uh.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://fe.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://jq.bjjhwx.cn

C#:   list.Add(4);
来源：http://ml.asd995.cn

[D03] 在指定位置插入元素
来源：http://pr.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://jr.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aj.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://za.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://rp.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://bp.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qk.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ag.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://sc.muxihuayi.cn

[D04] 删除元素
来源：http://gk.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fl.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fg.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jw.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://cp.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ze.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pp.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bk.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ln.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://lm.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zz.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ps.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uv.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://pz.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://dm.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://zh.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uh.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iu.huixiangedu.cn

[D06] 数组长度
来源：http://wr.szsharing.cn

Py:   len(arr)
来源：http://lq.muxihuayi.cn

PHP:  count($arr);
来源：http://zn.asd995.cn

JS:   arr.length
来源：http://kl.hahajie.cn

TS:   arr.length
来源：http://ah.bjjhwx.cn

Java: list.size();
来源：http://ut.szsharing.cn

Go:   len(arr)
来源：http://cc.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://td.shxzukj.cn

C#:   list.Count;
来源：http://es.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://mf.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bh.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wq.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://mh.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://kw.lnxyls.cn

Java: list.subList(1, 4);
来源：http://nn.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://bt.gzmigu.cn

Ruby: arr[1, 3]
来源：http://tx.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://xd.panjiajie.cn

[D08] 合并两个数组
来源：http://wi.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://va.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://xm.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tz.colortex.cn

TS:   [...a, ...b];
来源：http://nm.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gy.bookmarksfly.cn

Go:   append(a, b...)
来源：http://ll.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://qr.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://mf.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://qg.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://fz.9csxet.cn

PHP:  sort($arr);
来源：http://hh.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gk.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cm.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qo.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xl.lnxyls.cn

Ruby: arr.sort
来源：http://ig.hnjuh.cn

C#:   list.Sort();
来源：http://cp.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bv.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vy.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qb.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ce.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tl.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hy.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lt.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bw.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wz.huixiangedu.cn

[D11] 反转数组
来源：http://cs.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://di.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://xt.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jt.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://be.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://kh.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://ex.shxzukj.cn

Ruby: arr.reverse
来源：http://aj.bookmarksfly.cn

C#:   list.Reverse();
来源：http://em.hahajie.cn

[D12] 查找元素下标
来源：http://na.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://nm.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qf.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yn.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ic.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://na.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://gf.huanxung.cn

Ruby: arr.index(x)
来源：http://zf.nicolike.cn

C#:   list.IndexOf(x);
来源：http://jo.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://ml.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kb.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bl.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://lb.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://xx.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aw.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dz.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ll.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rq.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://xh.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cm.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bj.521024.cn

JS:   arr.map(x => x * 2)
来源：http://oj.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://ux.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pw.jctech888.com.cn

Go:   // 手写循环
来源：http://xl.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gh.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hi.hnjuh.cn

[D15] 去重
来源：http://xj.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hy.newstarts.cn

PHP:  array_unique($arr);
来源：http://vt.nszjky.cn

JS:   [...new Set(arr)]
来源：http://qu.9csxet.cn

TS:   [...new Set(arr)]
来源：http://lx.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tg.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://di.wgjwhj.cn

Ruby: arr.uniq
来源：http://mq.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://my.asd995.cn

[D16] 求和与平均值
来源：http://xb.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gc.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://af.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yr.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wf.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ko.9csxet.cn

Go:   // 手写循环累加
来源：http://mh.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jd.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://db.521024.cn

[D17] 最大值与最小值
来源：http://zx.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://iy.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://zr.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ac.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://cr.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ul.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eq.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://fa.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://qa.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://ew.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rg.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ry.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jn.bookmarksfly.cn

TS:   nested.flat();
来源：http://rt.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sm.colortex.cn

Go:   // 手写双层循环
来源：http://jc.9csxet.cn

Ruby: nested.flatten
来源：http://sb.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xs.huixinmuqiang.cn

[D19] 按字段分组
来源：http://nd.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qn.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://av.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mj.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nd.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zk.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://or.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vb.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sk.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://lm.9csxet.cn

Py:   Counter(arr)
来源：http://po.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://jk.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dd.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sl.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cd.nszjky.cn

Go:   // 手写 map[T]int
来源：http://uj.panjiajie.cn

Ruby: arr.tally
来源：http://ol.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ad.asd995.cn

[D21] 判断是否包含某元素
来源：http://fl.chemitech.net.cn

Py:   x in arr
来源：http://jp.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://di.hahajie.cn

JS:   arr.includes(x)
来源：http://gf.shxzukj.cn

TS:   arr.includes(x)
来源：http://du.asd995.cn

Java: list.contains(x)
来源：http://gv.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://ms.hnjuh.cn

Ruby: arr.include?(x)
来源：http://st.newstarts.cn

C#:   list.Contains(x)
来源：http://iz.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://xb.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ms.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ef.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ju.muxihuayi.cn

TS:   [...arr];
来源：http://vw.521024.cn

Java: new ArrayList<>(list);
来源：http://vf.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bu.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://rw.haigaiapp.cn

C#:   new List<int>(list);
来源：http://rm.panjiajie.cn

[D23] reduce 累积计算
来源：http://ct.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://go.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ws.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tb.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pq.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://da.bookmarksfly.cn

Go:   // 手写循环
来源：http://hy.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sq.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cf.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://sv.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zm.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://at.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zf.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rk.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wb.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hs.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lq.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ha.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ti.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kl.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hg.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ex.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ph.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nj.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://su.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lr.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hf.colortex.cn

[D26] 数组转字符串
来源：http://at.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://sl.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://er.gzmigu.cn

JS:   arr.join(", ")
来源：http://qg.nszjky.cn

TS:   arr.join(", ")
来源：http://lw.colortex.cn

Java: String.join(", ", list)
来源：http://pr.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://ae.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://gk.9csxet.cn

C#:   string.Join(", ", list)
来源：http://ub.nicolike.cn

================================================================================
来源：http://fa.szxytkj.cn

E. 字符串处理
来源：http://cm.bookmarksfly.cn

================================================================================
来源：http://ta.9csxet.cn

[E01] 拼接字符串
来源：http://ks.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kq.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ry.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fa.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dh.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ds.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uk.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mf.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nm.521024.cn

[E02] 重复字符串
来源：http://ox.shxzukj.cn

Py:   "ab" * 3
来源：http://uq.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://hi.szsharing.cn

JS:   "ab".repeat(3)
来源：http://lg.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://hi.shxzskj.cn

Java: "ab".repeat(3)
来源：http://gr.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://ex.lnxyls.cn

Ruby: "ab" * 3
来源：http://cx.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bh.shtwfgs.cn

[E03] 截取子串
来源：http://an.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://af.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ur.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pu.nszjky.cn

TS:   s.slice(1, 4)
来源：http://be.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://sk.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gl.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ne.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://yi.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://nx.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://do.asd995.cn

PHP:  strpos($s, "x");
来源：http://kd.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yj.panjiajie.cn

TS:   s.indexOf("x")
来源：http://ou.hnjuh.cn

Java: s.indexOf("x")
来源：http://gi.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://er.wgjwhj.cn

Ruby: s.index("x")
来源：http://nf.huanxung.cn

C#:   s.IndexOf("x")
来源：http://rq.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wx.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vw.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uy.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gk.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xt.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://on.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zg.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ds.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ib.521024.cn

[E06] 替换子串
来源：http://nh.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rg.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ai.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aq.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://gj.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cs.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tc.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zt.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://wf.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://yd.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pf.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xm.asd995.cn


<!-- 参考信息 -->