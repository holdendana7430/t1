代发 wailian999

[D03] 在指定位置插入元素
来源：http://kz.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://eq.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nv.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wh.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://xz.shxzskj.cn

Java: list.add(0, 0);
来源：http://ka.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hm.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://np.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://ik.shtwfgs.cn

[D04] 删除元素
来源：http://nl.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qt.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sd.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wi.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://bq.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yb.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xq.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jd.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yn.nicolike.cn

[D05] 访问与修改元素
来源：http://ts.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rc.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://no.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qt.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://tr.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://tz.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://kp.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kk.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wu.jctech888.com.cn

[D06] 数组长度
来源：http://iv.gzmigu.cn

Py:   len(arr)
来源：http://xf.bookmarksfly.cn

PHP:  count($arr);
来源：http://zq.wgjwhj.cn

JS:   arr.length
来源：http://hy.huixinmuqiang.cn

TS:   arr.length
来源：http://wr.bookmarksfly.cn

Java: list.size();
来源：http://kp.gzmigu.cn

Go:   len(arr)
来源：http://km.szsharing.cn

Ruby: arr.length; arr.size
来源：http://bs.szxytkj.cn

C#:   list.Count;
来源：http://dt.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://bx.hahajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gq.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gs.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://fe.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://oy.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://uw.bjjhwx.cn

Go:   arr[1:4]
来源：http://xv.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://bi.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://td.nszjky.cn

[D08] 合并两个数组
来源：http://gi.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://kw.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://iy.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rm.yuexingan06.cn

TS:   [...a, ...b];
来源：http://tx.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ge.nszjky.cn

Go:   append(a, b...)
来源：http://sw.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://sh.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://qr.szxytkj.cn

[D09] 排序（升序）
来源：http://mi.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://wm.hnjuh.cn

PHP:  sort($arr);
来源：http://kr.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pi.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://th.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mi.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oc.jianghongdianzi.cn

Ruby: arr.sort
来源：http://lm.huixiangedu.cn

C#:   list.Sort();
来源：http://qm.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://to.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xa.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qa.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tq.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ga.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oh.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pn.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nl.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gz.hahajie.cn

[D11] 反转数组
来源：http://ee.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vw.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://fy.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bc.lnxyls.cn

TS:   [...arr].reverse();
来源：http://ma.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://ri.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://tu.wgjwhj.cn

Ruby: arr.reverse
来源：http://tr.panjiajie.cn

C#:   list.Reverse();
来源：http://ai.521024.cn

[D12] 查找元素下标
来源：http://sj.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://gn.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ic.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rm.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nz.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wf.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://tw.haigaiapp.cn

Ruby: arr.index(x)
来源：http://qh.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://yf.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://jx.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bi.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gu.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://pz.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://uo.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bw.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dl.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qk.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ze.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://nb.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nk.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://av.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://zy.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://ps.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vx.panjiajie.cn

Go:   // 手写循环
来源：http://kn.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nx.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gv.szxytkj.cn

[D15] 去重
来源：http://ve.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nr.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://vc.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://lg.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://sz.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qg.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cj.shxzskj.cn

Ruby: arr.uniq
来源：http://iw.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://gj.gzmigu.cn

[D16] 求和与平均值
来源：http://jh.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ow.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zn.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bp.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ke.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iy.jctech888.com.cn

Go:   // 手写循环累加
来源：http://ey.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fk.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://as.9csxet.cn

[D17] 最大值与最小值
来源：http://ml.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://ue.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://uq.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cl.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://vj.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jf.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tl.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://oz.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://lb.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://hs.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ms.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://zp.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fq.newstarts.cn

TS:   nested.flat();
来源：http://id.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rd.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://mi.bookmarksfly.cn

Ruby: nested.flatten
来源：http://ql.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ad.nicolike.cn

[D19] 按字段分组
来源：http://jj.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gw.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://er.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pt.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zz.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gw.asd995.cn

Go:   // 手写 map[string][]T
来源：http://lp.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://et.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bp.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://ok.shxzskj.cn

Py:   Counter(arr)
来源：http://vn.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://wk.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fb.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hs.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hv.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://cq.colortex.cn

Ruby: arr.tally
来源：http://ze.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bn.9csxet.cn

[D21] 判断是否包含某元素
来源：http://zu.nicolike.cn

Py:   x in arr
来源：http://tz.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://uq.huixiangedu.cn

JS:   arr.includes(x)
来源：http://zh.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ha.huixiangedu.cn

Java: list.contains(x)
来源：http://yz.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://hd.nszjky.cn

Ruby: arr.include?(x)
来源：http://xm.nicolike.cn

C#:   list.Contains(x)
来源：http://ef.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://wr.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oj.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fs.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gx.bjjhwx.cn

TS:   [...arr];
来源：http://ge.nszjky.cn

Java: new ArrayList<>(list);
来源：http://iw.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gr.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://lj.muxihuayi.cn

C#:   new List<int>(list);
来源：http://tu.9csxet.cn

[D23] reduce 累积计算
来源：http://ge.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yz.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eh.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sv.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xh.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xh.chemitech.net.cn

Go:   // 手写循环
来源：http://rt.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xd.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xm.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://cd.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oj.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yp.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qp.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qd.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xh.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mw.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sb.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bv.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://wv.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qb.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mj.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ki.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sf.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iw.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fo.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xq.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uk.huanxung.cn

[D26] 数组转字符串
来源：http://ym.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://ab.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://zk.huanxung.cn

JS:   arr.join(", ")
来源：http://jg.nszjky.cn

TS:   arr.join(", ")
来源：http://uj.panjiajie.cn

Java: String.join(", ", list)
来源：http://gx.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://te.lnxyls.cn

Ruby: arr.join(", ")
来源：http://oi.newstarts.cn

C#:   string.Join(", ", list)
来源：http://st.jctech888.com.cn

================================================================================
来源：http://qg.szsharing.cn

E. 字符串处理
来源：http://zl.shtwfgs.cn

================================================================================
来源：http://qh.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://xn.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qe.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ol.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bk.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vx.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gn.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xl.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bz.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gw.huixiangedu.cn

[E02] 重复字符串
来源：http://iv.wgjwhj.cn

Py:   "ab" * 3
来源：http://qq.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://zr.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://rt.9csxet.cn

TS:   "ab".repeat(3)
来源：http://an.panjiajie.cn

Java: "ab".repeat(3)
来源：http://yd.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://yr.muxihuayi.cn

Ruby: "ab" * 3
来源：http://fy.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xe.yuexingan06.cn

[E03] 截取子串
来源：http://tv.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://op.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gr.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ln.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://kp.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://fq.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bz.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zj.colortex.cn

C#:   s.Substring(1, 3)
来源：http://af.chemitech.net.cn

[E04] 查找子串位置
来源：http://ep.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://mu.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://qk.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gd.hahajie.cn

TS:   s.indexOf("x")
来源：http://xs.hnjuh.cn

Java: s.indexOf("x")
来源：http://aj.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://to.muxihuayi.cn

Ruby: s.index("x")
来源：http://qy.huanxung.cn

C#:   s.IndexOf("x")
来源：http://gr.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bl.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ug.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vs.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ca.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://om.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mv.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pj.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://go.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vd.haigaiapp.cn

[E06] 替换子串
来源：http://pt.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dt.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ek.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qh.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://tp.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ru.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hy.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://re.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://hw.panjiajie.cn

[E07] 按分隔符拆分
来源：http://vu.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ot.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xn.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bs.shxzukj.cn

TS:   s.split(",")
来源：http://le.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ha.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vp.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://js.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cq.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://fl.huixiangedu.cn

Py:   ",".join(items)
来源：http://wk.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://ve.hahajie.cn

JS:   items.join(",")
来源：http://zk.hahajie.cn

TS:   items.join(",")
来源：http://hn.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://yf.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://tm.chemitech.net.cn

Ruby: items.join(",")
来源：http://is.huanxung.cn

C#:   string.Join(",", items)
来源：http://na.asd995.cn

[E09] 去除所有空白字符
来源：http://lv.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ze.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ox.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://ba.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ar.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://vu.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sh.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ru.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yb.shtwfgs.cn


<!-- 参考信息 -->