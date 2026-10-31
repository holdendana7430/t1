代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zo.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uw.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xp.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kw.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://rp.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://nb.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hp.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://cz.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iv.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qi.hahajie.cn

JS:   arr.push(4);
来源：http://fx.huixiangedu.cn

TS:   arr.push(4);
来源：http://qf.yuexingan06.cn

Java: list.add(4);
来源：http://sf.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://xt.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://he.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://hh.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://hs.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://br.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rt.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lk.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://ik.wgjwhj.cn

Java: list.add(0, 0);
来源：http://qq.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ns.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lt.asd995.cn

C#:   list.Insert(0, 0);
来源：http://wz.shxzskj.cn

[D04] 删除元素
来源：http://jg.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cw.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ee.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pf.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://xd.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://im.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jk.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dq.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://or.muxihuayi.cn

[D05] 访问与修改元素
来源：http://rm.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://al.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ls.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://su.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://ae.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://ou.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://ci.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tr.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ma.521024.cn

[D06] 数组长度
来源：http://be.gzmigu.cn

Py:   len(arr)
来源：http://rd.shtwfgs.cn

PHP:  count($arr);
来源：http://vf.9csxet.cn

JS:   arr.length
来源：http://gs.colortex.cn

TS:   arr.length
来源：http://uv.szsharing.cn

Java: list.size();
来源：http://cl.huanxung.cn

Go:   len(arr)
来源：http://nk.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://yf.wgjwhj.cn

C#:   list.Count;
来源：http://hy.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://bc.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yk.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hj.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://gp.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://nr.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://dv.9csxet.cn

Go:   arr[1:4]
来源：http://bh.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://hh.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://mx.jctech888.com.cn

[D08] 合并两个数组
来源：http://gh.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://lq.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://yt.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kh.panjiajie.cn

TS:   [...a, ...b];
来源：http://hs.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ui.521024.cn

Go:   append(a, b...)
来源：http://ad.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://bx.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://om.muxihuayi.cn

[D09] 排序（升序）
来源：http://sc.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://oj.shxzukj.cn

PHP:  sort($arr);
来源：http://hq.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hs.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hx.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bh.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tj.gzmigu.cn

Ruby: arr.sort
来源：http://nf.colortex.cn

C#:   list.Sort();
来源：http://us.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qt.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ll.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ru.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zv.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jw.nszjky.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bo.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zz.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nf.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hs.hnjuh.cn

[D11] 反转数组
来源：http://gr.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jt.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://dn.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://po.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://nr.shxzukj.cn

Java: Collections.reverse(list);
来源：http://sb.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://wh.jctech888.com.cn

Ruby: arr.reverse
来源：http://eu.shtwfgs.cn

C#:   list.Reverse();
来源：http://he.9csxet.cn

[D12] 查找元素下标
来源：http://el.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://yi.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nn.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rq.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cz.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wl.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://xv.jctech888.com.cn

Ruby: arr.index(x)
来源：http://lf.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://vf.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://wv.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pa.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fy.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://bn.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://qm.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zf.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hn.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oi.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lb.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://tt.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qn.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://da.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://ix.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ag.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qj.shxzukj.cn

Go:   // 手写循环
来源：http://zd.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zu.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ql.shtwfgs.cn

[D15] 去重
来源：http://fv.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xb.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://jp.colortex.cn

JS:   [...new Set(arr)]
来源：http://nt.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://wh.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ik.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wf.shxzukj.cn

Ruby: arr.uniq
来源：http://ou.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://qf.newstarts.cn

[D16] 求和与平均值
来源：http://uw.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ae.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tz.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ge.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ot.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aa.huanxung.cn

Go:   // 手写循环累加
来源：http://kp.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wd.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://gn.haigaiapp.cn

[D17] 最大值与最小值
来源：http://bx.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://ix.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://rp.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ps.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://gt.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gv.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dz.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://wz.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://jp.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://od.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://np.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ly.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cc.yuexingan06.cn

TS:   nested.flat();
来源：http://sd.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://im.muxihuayi.cn

Go:   // 手写双层循环
来源：http://wb.chemitech.net.cn

Ruby: nested.flatten
来源：http://hs.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ew.shxzskj.cn

[D19] 按字段分组
来源：http://pa.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zj.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ji.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rn.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zj.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nd.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://mv.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zh.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eo.521024.cn

[D20] 统计每个元素出现次数
来源：http://yj.gzmigu.cn

Py:   Counter(arr)
来源：http://kq.szsharing.cn

PHP:  array_count_values($arr);
来源：http://qz.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ev.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://du.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://li.asd995.cn

Go:   // 手写 map[T]int
来源：http://ly.gzmigu.cn

Ruby: arr.tally
来源：http://zo.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fg.nszjky.cn

[D21] 判断是否包含某元素
来源：http://kv.shxzskj.cn

Py:   x in arr
来源：http://mh.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://ch.9csxet.cn

JS:   arr.includes(x)
来源：http://xy.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://wu.lnxyls.cn

Java: list.contains(x)
来源：http://uv.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://hd.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://op.wgjwhj.cn

C#:   list.Contains(x)
来源：http://nl.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://fu.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ca.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bj.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ba.bookmarksfly.cn

TS:   [...arr];
来源：http://dl.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://zl.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nx.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://yz.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://gi.muxihuayi.cn

[D23] reduce 累积计算
来源：http://nz.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://us.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jt.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://px.szsharing.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pw.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zn.wgjwhj.cn

Go:   // 手写循环
来源：http://jh.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yj.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hd.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://fy.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xn.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cz.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mu.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ux.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zk.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pt.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ul.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ey.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://ww.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qi.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wh.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://at.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kp.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ir.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hj.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ti.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rl.gzmigu.cn

[D26] 数组转字符串
来源：http://qp.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ie.asd995.cn

PHP:  implode(", ", $arr);
来源：http://qc.haigaiapp.cn

JS:   arr.join(", ")
来源：http://on.shtwfgs.cn

TS:   arr.join(", ")
来源：http://va.shtwfgs.cn

Java: String.join(", ", list)
来源：http://xc.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://at.colortex.cn

Ruby: arr.join(", ")
来源：http://jz.nicolike.cn

C#:   string.Join(", ", list)
来源：http://oh.jianghongdianzi.cn

================================================================================
来源：http://au.hahajie.cn

E. 字符串处理
来源：http://hp.shtwfgs.cn

================================================================================
来源：http://hn.gzmigu.cn

[E01] 拼接字符串
来源：http://ky.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uk.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hd.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cj.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vv.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dy.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wp.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ys.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ih.9csxet.cn

[E02] 重复字符串
来源：http://st.shxzskj.cn

Py:   "ab" * 3
来源：http://ad.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://cp.huanxung.cn

JS:   "ab".repeat(3)
来源：http://ks.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://rf.gzmigu.cn

Java: "ab".repeat(3)
来源：http://tx.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://am.jctech888.com.cn

Ruby: "ab" * 3
来源：http://fw.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ku.huixiangedu.cn

[E03] 截取子串
来源：http://zd.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://na.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zy.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nm.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://ww.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://rs.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ny.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mx.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://dk.521024.cn

[E04] 查找子串位置
来源：http://gn.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://le.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://vo.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jc.hnjuh.cn

TS:   s.indexOf("x")
来源：http://dt.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://mr.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ag.chemitech.net.cn

Ruby: s.index("x")
来源：http://jc.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://fg.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://me.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nb.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zz.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://za.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gn.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ls.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vc.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://by.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ib.bjjhwx.cn

[E06] 替换子串
来源：http://dm.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ky.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://gj.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://le.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://lz.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ov.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ni.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bn.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://so.521024.cn

[E07] 按分隔符拆分
来源：http://fh.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pq.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nx.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://us.huixiangedu.cn

TS:   s.split(",")
来源：http://kz.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rc.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tr.asd995.cn

Ruby: s.split(",");  s.split
来源：http://fv.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qx.colortex.cn

[E08] 数组按分隔符合并
来源：http://ys.huanxung.cn

Py:   ",".join(items)
来源：http://rs.bookmarksfly.cn


<!-- 参考信息 -->