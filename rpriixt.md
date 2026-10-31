代发 wailian999

D. 数组 / 列表 / 集合
来源：http://on.szsharing.cn

================================================================================
来源：http://tl.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://ih.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cx.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nz.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gl.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ki.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sy.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://hu.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://ge.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cz.lnxyls.cn

[D02] 追加元素到末尾
来源：http://ge.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rc.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ea.jctech888.com.cn

JS:   arr.push(4);
来源：http://ee.muxihuayi.cn

TS:   arr.push(4);
来源：http://gy.shxzukj.cn

Java: list.add(4);
来源：http://wo.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://cm.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://bu.nszjky.cn

C#:   list.Add(4);
来源：http://wc.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://sh.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://tt.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://te.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hs.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ii.asd995.cn

Java: list.add(0, 0);
来源：http://yh.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gj.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vt.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://pw.gzmigu.cn

[D04] 删除元素
来源：http://uc.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nd.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wh.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://we.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://fs.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iu.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://je.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wp.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ha.shtwfgs.cn

[D05] 访问与修改元素
来源：http://af.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mp.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xa.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ou.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://mi.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://rg.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ux.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dh.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bx.hahajie.cn

[D06] 数组长度
来源：http://kr.huixiangedu.cn

Py:   len(arr)
来源：http://ai.huixiangedu.cn

PHP:  count($arr);
来源：http://hy.yuntaijiaju.cn

JS:   arr.length
来源：http://gx.colortex.cn

TS:   arr.length
来源：http://oi.yuexingan06.cn

Java: list.size();
来源：http://yo.shxzukj.cn

Go:   len(arr)
来源：http://sc.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://nz.shtwfgs.cn

C#:   list.Count;
来源：http://kp.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://si.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bt.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sw.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://px.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://tj.9csxet.cn

Java: list.subList(1, 4);
来源：http://uj.jctech888.com.cn

Go:   arr[1:4]
来源：http://od.521024.cn

Ruby: arr[1, 3]
来源：http://op.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://dg.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://iu.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://bp.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://us.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tj.asd995.cn

TS:   [...a, ...b];
来源：http://sy.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://po.bjjhwx.cn

Go:   append(a, b...)
来源：http://ai.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://lc.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://bf.shtwfgs.cn

[D09] 排序（升序）
来源：http://oa.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://li.asd995.cn

PHP:  sort($arr);
来源：http://wv.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mt.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tl.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://my.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fq.bookmarksfly.cn

Ruby: arr.sort
来源：http://ou.shxzskj.cn

C#:   list.Sort();
来源：http://tu.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ok.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qn.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mx.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ic.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uy.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ap.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zt.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oq.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lp.jctech888.com.cn

[D11] 反转数组
来源：http://vp.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qa.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://bc.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fy.panjiajie.cn

TS:   [...arr].reverse();
来源：http://cs.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://xr.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://vq.yuexingan06.cn

Ruby: arr.reverse
来源：http://qb.shtwfgs.cn

C#:   list.Reverse();
来源：http://rd.bookmarksfly.cn

[D12] 查找元素下标
来源：http://or.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://bz.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ab.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bh.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hx.nicolike.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ak.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://in.nicolike.cn

Ruby: arr.index(x)
来源：http://ex.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ax.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://rq.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://le.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://or.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://yu.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://ai.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pk.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yx.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xh.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wq.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://eb.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sh.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lm.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://vs.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://xm.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zb.nszjky.cn

Go:   // 手写循环
来源：http://hp.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vb.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bq.panjiajie.cn

[D15] 去重
来源：http://ef.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jk.colortex.cn

PHP:  array_unique($arr);
来源：http://zf.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://wx.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://of.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://za.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://he.bookmarksfly.cn

Ruby: arr.uniq
来源：http://pc.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://ju.shtwfgs.cn

[D16] 求和与平均值
来源：http://sx.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yr.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://og.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iv.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bf.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yl.lnxyls.cn

Go:   // 手写循环累加
来源：http://fp.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lk.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://sn.szxytkj.cn

[D17] 最大值与最小值
来源：http://pq.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://jd.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://sh.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://in.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://fw.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bd.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wz.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://sq.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://wh.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://uw.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tm.asd995.cn

PHP:  array_merge(...$nested);
来源：http://mm.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oy.hahajie.cn

TS:   nested.flat();
来源：http://tm.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vd.muxihuayi.cn

Go:   // 手写双层循环
来源：http://om.hahajie.cn

Ruby: nested.flatten
来源：http://rs.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xd.chemitech.net.cn

[D19] 按字段分组
来源：http://po.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://li.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://re.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qq.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fo.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ux.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://my.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eu.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hc.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://hc.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://pb.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://ee.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ca.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nr.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nh.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://ms.colortex.cn

Ruby: arr.tally
来源：http://aj.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xk.huanxung.cn

[D21] 判断是否包含某元素
来源：http://bj.shtwfgs.cn

Py:   x in arr
来源：http://jt.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://uh.panjiajie.cn

JS:   arr.includes(x)
来源：http://rb.nszjky.cn

TS:   arr.includes(x)
来源：http://ev.9csxet.cn

Java: list.contains(x)
来源：http://gn.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://zk.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://rc.shxzskj.cn

C#:   list.Contains(x)
来源：http://kd.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://nb.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dj.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gk.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://he.9csxet.cn

TS:   [...arr];
来源：http://jo.hahajie.cn

Java: new ArrayList<>(list);
来源：http://ei.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xs.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://ys.yuexingan06.cn

C#:   new List<int>(list);
来源：http://qu.asd995.cn

[D23] reduce 累积计算
来源：http://uf.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xq.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jc.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pl.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://px.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fm.colortex.cn

Go:   // 手写循环
来源：http://dz.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cw.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sj.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://hh.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dv.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ki.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lo.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://id.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mw.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ro.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vt.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vd.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://yd.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jp.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jy.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ke.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kt.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ku.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qu.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vi.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ar.haigaiapp.cn

[D26] 数组转字符串
来源：http://dz.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://zr.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://fj.shxzukj.cn

JS:   arr.join(", ")
来源：http://dx.nszjky.cn

TS:   arr.join(", ")
来源：http://iw.newstarts.cn

Java: String.join(", ", list)
来源：http://uc.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://do.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://ew.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://yt.jianghongdianzi.cn

================================================================================
来源：http://pg.521024.cn

E. 字符串处理
来源：http://mk.wgjwhj.cn

================================================================================
来源：http://fd.szxytkj.cn

[E01] 拼接字符串
来源：http://mf.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ln.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fw.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xw.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zo.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://re.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mq.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://py.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://io.hahajie.cn

[E02] 重复字符串
来源：http://ep.colortex.cn

Py:   "ab" * 3
来源：http://vf.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://bt.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://vo.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://in.asd995.cn

Java: "ab".repeat(3)
来源：http://vj.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://li.nicolike.cn

Ruby: "ab" * 3
来源：http://cq.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hn.jctech888.com.cn

[E03] 截取子串
来源：http://co.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kw.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bg.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://op.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://yn.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://cg.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pc.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ch.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://df.colortex.cn

[E04] 查找子串位置
来源：http://nb.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://cf.newstarts.cn

PHP:  strpos($s, "x");
来源：http://iz.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ad.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://ln.szxytkj.cn

Java: s.indexOf("x")
来源：http://fr.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://hg.lnxyls.cn

Ruby: s.index("x")
来源：http://tq.asd995.cn

C#:   s.IndexOf("x")
来源：http://de.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://br.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wy.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://df.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ng.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mn.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zf.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ng.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zj.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oy.szsharing.cn

[E06] 替换子串
来源：http://hg.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gv.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://qw.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kq.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://em.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bc.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oc.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ru.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://xn.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://yy.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ek.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mh.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://du.huixiangedu.cn

TS:   s.split(",")
来源：http://hv.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qk.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xn.szxytkj.cn


<!-- 参考信息 -->