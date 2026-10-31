代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yw.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://lc.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ux.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mx.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://do.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dw.lnxyls.cn

[D05] 访问与修改元素
来源：http://ec.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hj.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fi.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ud.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://wx.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://lj.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ur.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mf.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hu.lnxyls.cn

[D06] 数组长度
来源：http://th.huixinmuqiang.cn

Py:   len(arr)
来源：http://kh.huanxung.cn

PHP:  count($arr);
来源：http://st.szsharing.cn

JS:   arr.length
来源：http://jn.huixinmuqiang.cn

TS:   arr.length
来源：http://vs.nicolike.cn

Java: list.size();
来源：http://ky.chemitech.net.cn

Go:   len(arr)
来源：http://tk.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://jb.asd995.cn

C#:   list.Count;
来源：http://vn.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://xd.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nj.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tp.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://wz.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://zc.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://vg.bjjhwx.cn

Go:   arr[1:4]
来源：http://rg.newstarts.cn

Ruby: arr[1, 3]
来源：http://mb.521024.cn

C#:   list.GetRange(1, 3);
来源：http://tq.lnxyls.cn

[D08] 合并两个数组
来源：http://je.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://sp.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://lu.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fm.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://vx.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bn.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://ky.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ml.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://dr.shxzukj.cn

[D09] 排序（升序）
来源：http://nb.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://nk.jctech888.com.cn

PHP:  sort($arr);
来源：http://gk.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sn.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ua.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zg.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lj.yuntaijiaju.cn

Ruby: arr.sort
来源：http://vh.huixinmuqiang.cn

C#:   list.Sort();
来源：http://bu.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ki.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bm.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zk.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oc.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rn.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jk.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bk.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mn.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rz.haigaiapp.cn

[D11] 反转数组
来源：http://nx.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tx.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://af.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hu.shxzukj.cn

TS:   [...arr].reverse();
来源：http://kg.9csxet.cn

Java: Collections.reverse(list);
来源：http://cf.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://ii.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://xc.bjjhwx.cn

C#:   list.Reverse();
来源：http://wb.haigaiapp.cn

[D12] 查找元素下标
来源：http://fk.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://bx.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://et.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://co.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ht.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zf.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://dv.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://rh.colortex.cn

C#:   list.IndexOf(x);
来源：http://fs.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://ch.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kc.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bo.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://ko.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://qi.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://av.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sy.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ao.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jn.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://ow.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ad.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hj.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://yj.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://kx.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gu.hnjuh.cn

Go:   // 手写循环
来源：http://it.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nw.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wf.hnjuh.cn

[D15] 去重
来源：http://ob.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eu.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://si.nszjky.cn

JS:   [...new Set(arr)]
来源：http://on.hahajie.cn

TS:   [...new Set(arr)]
来源：http://lj.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://am.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ce.shxzskj.cn

Ruby: arr.uniq
来源：http://xk.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://cs.hahajie.cn

[D16] 求和与平均值
来源：http://rx.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://la.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qn.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fe.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jk.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xf.wgjwhj.cn

Go:   // 手写循环累加
来源：http://xe.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ck.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://bm.lnxyls.cn

[D17] 最大值与最小值
来源：http://fu.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://wg.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://zo.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://in.hnjuh.cn

TS:   Math.max(...arr);
来源：http://xi.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pa.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cu.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://ix.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://qx.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://gg.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vn.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://wi.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vo.newstarts.cn

TS:   nested.flat();
来源：http://au.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bl.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://sh.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://cp.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hr.huixinmuqiang.cn

[D19] 按字段分组
来源：http://pr.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zo.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kj.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://el.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yy.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ev.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://wu.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cc.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kf.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://wq.panjiajie.cn

Py:   Counter(arr)
来源：http://pi.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://nm.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zh.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ci.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://es.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://re.bjjhwx.cn

Ruby: arr.tally
来源：http://ex.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hn.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://xv.panjiajie.cn

Py:   x in arr
来源：http://fm.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://lt.jctech888.com.cn

JS:   arr.includes(x)
来源：http://ux.chemitech.net.cn

TS:   arr.includes(x)
来源：http://cb.bookmarksfly.cn

Java: list.contains(x)
来源：http://jf.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://wn.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://cm.shxzskj.cn

C#:   list.Contains(x)
来源：http://sk.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://lt.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nk.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kt.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fd.shtwfgs.cn

TS:   [...arr];
来源：http://iv.asd995.cn

Java: new ArrayList<>(list);
来源：http://rr.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jk.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://bd.newstarts.cn

C#:   new List<int>(list);
来源：http://fw.yuexingan06.cn

[D23] reduce 累积计算
来源：http://hl.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ib.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bs.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yt.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ix.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dl.huanxung.cn

Go:   // 手写循环
来源：http://td.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pu.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mf.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://oh.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fm.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rn.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oe.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bl.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://na.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sz.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pf.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vw.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://xm.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://on.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wb.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wz.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sv.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bu.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jc.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jd.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tn.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ro.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://vr.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://ow.9csxet.cn

JS:   arr.join(", ")
来源：http://yk.yuexingan06.cn

TS:   arr.join(", ")
来源：http://st.hahajie.cn

Java: String.join(", ", list)
来源：http://jo.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://rt.panjiajie.cn

Ruby: arr.join(", ")
来源：http://br.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://mx.jctech888.com.cn

================================================================================
来源：http://bw.asd995.cn

E. 字符串处理
来源：http://ds.asd995.cn

================================================================================
来源：http://kt.521024.cn

[E01] 拼接字符串
来源：http://or.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://py.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qs.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xc.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://op.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vq.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ot.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hw.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wf.jianghongdianzi.cn

[E02] 重复字符串
来源：http://cl.panjiajie.cn

Py:   "ab" * 3
来源：http://wh.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://wy.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://qq.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://zy.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://rq.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://ho.szxytkj.cn

Ruby: "ab" * 3
来源：http://zb.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sy.bookmarksfly.cn

[E03] 截取子串
来源：http://rs.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ed.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sv.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ef.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://xh.lnxyls.cn

Java: s.substring(1, 4)
来源：http://qp.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qg.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fx.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://cw.nicolike.cn

[E04] 查找子串位置
来源：http://mt.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://kc.hahajie.cn

PHP:  strpos($s, "x");
来源：http://yn.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xx.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://gw.9csxet.cn

Java: s.indexOf("x")
来源：http://ss.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://nj.lnxyls.cn

Ruby: s.index("x")
来源：http://qg.huanxung.cn

C#:   s.IndexOf("x")
来源：http://qm.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cf.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://so.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cq.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://es.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ys.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ic.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ef.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zu.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qb.yuexingan06.cn

[E06] 替换子串
来源：http://kr.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xq.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://vk.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qh.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://gt.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ja.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nj.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jn.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ro.lnxyls.cn

[E07] 按分隔符拆分
来源：http://mi.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vd.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ny.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wu.szsharing.cn

TS:   s.split(",")
来源：http://ez.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xg.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ar.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://qw.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://me.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://fj.shxzukj.cn

Py:   ",".join(items)
来源：http://qz.hnjuh.cn

PHP:  implode(",", $items);
来源：http://cp.bookmarksfly.cn

JS:   items.join(",")
来源：http://pz.chemitech.net.cn

TS:   items.join(",")
来源：http://au.shxzskj.cn

Java: String.join(",", items)
来源：http://km.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://yr.huixiangedu.cn

Ruby: items.join(",")
来源：http://jx.shxzskj.cn

C#:   string.Join(",", items)
来源：http://dj.9csxet.cn

[E09] 去除所有空白字符
来源：http://pw.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://su.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qe.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://vy.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://ff.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://mn.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sf.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zl.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vk.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://io.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yj.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vx.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://yg.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://lk.hahajie.cn

Java: String.format("%03d", 7)
来源：http://hv.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wv.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vy.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sf.shtwfgs.cn

[E11] 反转字符串
来源：http://at.huanxung.cn

Py:   s[::-1]
来源：http://vk.panjiajie.cn

PHP:  strrev($s);
来源：http://np.shxzukj.cn


<!-- 参考信息 -->