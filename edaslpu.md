代发 wailian999

Py:   len(arr)
来源：http://of.muxihuayi.cn

PHP:  count($arr);
来源：http://pw.shxzskj.cn

JS:   arr.length
来源：http://yw.nicolike.cn

TS:   arr.length
来源：http://el.hahajie.cn

Java: list.size();
来源：http://ws.colortex.cn

Go:   len(arr)
来源：http://mm.newstarts.cn

Ruby: arr.length; arr.size
来源：http://yu.szsharing.cn

C#:   list.Count;
来源：http://kb.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://fi.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pl.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qv.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://yu.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://xi.shxzskj.cn

Java: list.subList(1, 4);
来源：http://ug.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://qx.nszjky.cn

Ruby: arr[1, 3]
来源：http://ir.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://hb.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://bx.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://lx.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://ik.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yb.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://ih.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://to.szxytkj.cn

Go:   append(a, b...)
来源：http://yd.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://yn.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://vu.shxzukj.cn

[D09] 排序（升序）
来源：http://ll.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://pf.asd995.cn

PHP:  sort($arr);
来源：http://do.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sz.asd995.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wp.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rr.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://op.521024.cn

Ruby: arr.sort
来源：http://fv.hnjuh.cn

C#:   list.Sort();
来源：http://po.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vw.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gn.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wy.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xc.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yx.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hh.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vh.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cm.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cu.shxzukj.cn

[D11] 反转数组
来源：http://hi.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cy.szsharing.cn

PHP:  array_reverse($arr);
来源：http://zc.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vw.gzmigu.cn

TS:   [...arr].reverse();
来源：http://yl.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://zo.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://hc.asd995.cn

Ruby: arr.reverse
来源：http://xj.hnjuh.cn

C#:   list.Reverse();
来源：http://qb.lnxyls.cn

[D12] 查找元素下标
来源：http://hu.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://zd.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xk.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bj.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ed.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://co.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://bl.shxzukj.cn

Ruby: arr.index(x)
来源：http://qw.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://ez.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://ey.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uf.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jy.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://fx.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://lj.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ps.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jp.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kd.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zu.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://ye.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ns.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://va.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://ag.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://we.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qq.bookmarksfly.cn

Go:   // 手写循环
来源：http://se.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fe.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pv.bjjhwx.cn

[D15] 去重
来源：http://ud.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qu.hnjuh.cn

PHP:  array_unique($arr);
来源：http://oj.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://wb.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://wr.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uk.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://te.shxzskj.cn

Ruby: arr.uniq
来源：http://ip.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ls.gzmigu.cn

[D16] 求和与平均值
来源：http://ow.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tn.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://el.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qi.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ty.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jq.panjiajie.cn

Go:   // 手写循环累加
来源：http://au.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lg.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://nx.521024.cn

[D17] 最大值与最小值
来源：http://xm.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://qx.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://cg.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mf.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://mn.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vm.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kp.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://bm.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://np.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://su.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ie.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://tv.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sc.hahajie.cn

TS:   nested.flat();
来源：http://mr.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gd.jctech888.com.cn

Go:   // 手写双层循环
来源：http://mb.gzmigu.cn

Ruby: nested.flatten
来源：http://mw.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ah.gzmigu.cn

[D19] 按字段分组
来源：http://hz.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aj.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eg.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://we.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ql.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xa.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://gt.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bh.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vz.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://nd.wgjwhj.cn

Py:   Counter(arr)
来源：http://dl.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://on.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rl.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tl.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xk.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://lr.asd995.cn

Ruby: arr.tally
来源：http://pm.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wm.newstarts.cn

[D21] 判断是否包含某元素
来源：http://ad.colortex.cn

Py:   x in arr
来源：http://bk.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://ea.521024.cn

JS:   arr.includes(x)
来源：http://ak.colortex.cn

TS:   arr.includes(x)
来源：http://si.colortex.cn

Java: list.contains(x)
来源：http://rx.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://xo.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://gk.bjjhwx.cn

C#:   list.Contains(x)
来源：http://sj.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://zg.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wj.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://he.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tq.newstarts.cn

TS:   [...arr];
来源：http://jn.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://zz.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xe.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://ov.szsharing.cn

C#:   new List<int>(list);
来源：http://ef.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://dq.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lb.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ib.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zu.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ns.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xg.colortex.cn

Go:   // 手写循环
来源：http://iw.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qh.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cl.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://xr.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pm.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bt.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ug.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hk.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lr.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mq.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hx.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uy.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://rq.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kx.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://am.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qc.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dk.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yw.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://np.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bl.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zq.lnxyls.cn

[D26] 数组转字符串
来源：http://fy.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://tw.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://se.shtwfgs.cn

JS:   arr.join(", ")
来源：http://xi.huixiangedu.cn

TS:   arr.join(", ")
来源：http://gb.wgjwhj.cn

Java: String.join(", ", list)
来源：http://tt.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://py.shxzukj.cn

Ruby: arr.join(", ")
来源：http://vu.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://bs.colortex.cn

================================================================================
来源：http://ns.szxytkj.cn

E. 字符串处理
来源：http://ut.newstarts.cn

================================================================================
来源：http://ft.shxzskj.cn

[E01] 拼接字符串
来源：http://yg.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gr.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tc.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://du.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ta.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ns.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dr.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ix.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bn.bookmarksfly.cn

[E02] 重复字符串
来源：http://sb.chemitech.net.cn

Py:   "ab" * 3
来源：http://bz.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://re.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://nz.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://lh.colortex.cn

Java: "ab".repeat(3)
来源：http://hh.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://fp.shxzukj.cn

Ruby: "ab" * 3
来源：http://zf.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jm.muxihuayi.cn

[E03] 截取子串
来源：http://yk.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wy.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xm.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rm.521024.cn

TS:   s.slice(1, 4)
来源：http://fm.szsharing.cn

Java: s.substring(1, 4)
来源：http://zl.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gi.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oy.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://le.yuexingan06.cn

[E04] 查找子串位置
来源：http://di.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://nz.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://jl.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vd.nicolike.cn

TS:   s.indexOf("x")
来源：http://na.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://st.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://rs.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://ov.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://wt.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jq.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qt.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://go.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://af.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mi.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ds.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sd.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jm.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zr.hahajie.cn

[E06] 替换子串
来源：http://qq.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yo.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://wu.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fz.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://jw.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hu.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kg.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qn.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://ph.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://dy.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://it.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bu.shxzskj.cn

TS:   s.split(",")
来源：http://bh.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lx.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wv.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://vm.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zq.asd995.cn

[E08] 数组按分隔符合并
来源：http://je.muxihuayi.cn

Py:   ",".join(items)
来源：http://ri.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://zs.gzmigu.cn

JS:   items.join(",")
来源：http://hl.wgjwhj.cn

TS:   items.join(",")
来源：http://zj.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://jr.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://mx.huanxung.cn

Ruby: items.join(",")
来源：http://ba.lnxyls.cn

C#:   string.Join(",", items)
来源：http://xb.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ej.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qt.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sc.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://jr.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://ir.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://pc.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sr.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ks.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xs.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://je.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rl.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yk.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://rd.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://bp.szsharing.cn

Java: String.format("%03d", 7)
来源：http://at.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pz.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kl.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ab.shxzukj.cn

[E11] 反转字符串
来源：http://xh.shtwfgs.cn

Py:   s[::-1]
来源：http://at.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://on.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://os.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://vb.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lb.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dt.szsharing.cn

Ruby: s.reverse
来源：http://hp.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kv.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://dg.bjjhwx.cn

Py:   s.count("a")
来源：http://lx.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://le.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://sm.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://nt.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uy.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://ob.9csxet.cn

Ruby: s.count("a")
来源：http://oy.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://as.szsharing.cn

[E13] 逐字符遍历
来源：http://pz.jianghongdianzi.cn


<!-- 参考信息 -->