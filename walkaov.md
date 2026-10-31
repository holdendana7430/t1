代发 wailian999

[D07] 切片 / 取子数组
来源：http://ee.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bg.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bs.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://bx.colortex.cn

TS:   arr.slice(1, 4);
来源：http://rj.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://un.yuexingan06.cn

Go:   arr[1:4]
来源：http://jp.shxzskj.cn

Ruby: arr[1, 3]
来源：http://zf.521024.cn

C#:   list.GetRange(1, 3);
来源：http://vl.521024.cn

[D08] 合并两个数组
来源：http://tt.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://lt.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://ew.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pg.shtwfgs.cn

TS:   [...a, ...b];
来源：http://jk.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fq.wgjwhj.cn

Go:   append(a, b...)
来源：http://pu.yuexingan06.cn

Ruby: a + b;  a.concat(b)
来源：http://eb.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://yp.szxytkj.cn

[D09] 排序（升序）
来源：http://kj.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://qw.hahajie.cn

PHP:  sort($arr);
来源：http://db.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bf.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kl.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qh.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wb.yuntaijiaju.cn

Ruby: arr.sort
来源：http://ug.newstarts.cn

C#:   list.Sort();
来源：http://ii.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mk.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xb.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lh.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ky.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bc.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sh.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zs.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://au.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yz.szsharing.cn

[D11] 反转数组
来源：http://rj.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xr.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://gc.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dh.nicolike.cn

TS:   [...arr].reverse();
来源：http://lb.muxihuayi.cn

Java: Collections.reverse(list);
来源：http://vh.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://yd.jctech888.com.cn

Ruby: arr.reverse
来源：http://bs.jctech888.com.cn

C#:   list.Reverse();
来源：http://hj.huanxung.cn

[D12] 查找元素下标
来源：http://ce.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://ly.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://if.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rc.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fq.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://jq.bjjhwx.cn

Ruby: arr.index(x)
来源：http://uj.newstarts.cn

C#:   list.IndexOf(x);
来源：http://rw.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://dz.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ge.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qf.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://ef.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://am.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sm.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yc.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ji.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ko.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://lh.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://is.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://so.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://bx.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://fc.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sy.muxihuayi.cn

Go:   // 手写循环
来源：http://ds.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lj.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://en.bookmarksfly.cn

[D15] 去重
来源：http://ae.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jx.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://nn.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://gu.9csxet.cn

TS:   [...new Set(arr)]
来源：http://tt.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ok.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cp.yuexingan06.cn

Ruby: arr.uniq
来源：http://yr.521024.cn

C#:   list.Distinct().ToList()
来源：http://bx.chemitech.net.cn

[D16] 求和与平均值
来源：http://si.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ps.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mv.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dt.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://if.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bu.haigaiapp.cn

Go:   // 手写循环累加
来源：http://yn.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wg.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://ev.521024.cn

[D17] 最大值与最小值
来源：http://kj.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://cs.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://pv.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eu.9csxet.cn

TS:   Math.max(...arr);
来源：http://ad.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sk.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ap.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://qe.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://op.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://uk.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yv.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://oa.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fa.lnxyls.cn

TS:   nested.flat();
来源：http://lz.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://di.shtwfgs.cn

Go:   // 手写双层循环
来源：http://xm.huanxung.cn

Ruby: nested.flatten
来源：http://fx.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uy.nszjky.cn

[D19] 按字段分组
来源：http://po.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sz.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lm.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yt.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ht.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cs.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://ff.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jx.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aj.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://zd.szsharing.cn

Py:   Counter(arr)
来源：http://ai.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://st.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ow.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yu.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mu.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://kh.521024.cn

Ruby: arr.tally
来源：http://dv.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sa.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://ob.yuexingan06.cn

Py:   x in arr
来源：http://hh.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://rr.huanxung.cn

JS:   arr.includes(x)
来源：http://ws.colortex.cn

TS:   arr.includes(x)
来源：http://fc.yuntaijiaju.cn

Java: list.contains(x)
来源：http://zo.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://is.9csxet.cn

Ruby: arr.include?(x)
来源：http://bm.huixiangedu.cn

C#:   list.Contains(x)
来源：http://ib.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://am.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bj.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rj.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ej.panjiajie.cn

TS:   [...arr];
来源：http://yw.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://vx.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tf.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://xh.hnjuh.cn

C#:   new List<int>(list);
来源：http://lm.szsharing.cn

[D23] reduce 累积计算
来源：http://fz.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kw.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dd.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ui.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tx.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nh.bookmarksfly.cn

Go:   // 手写循环
来源：http://zl.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://no.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iv.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://sm.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ps.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xb.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xe.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xv.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uc.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ox.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tk.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nw.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://vz.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eu.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yu.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kj.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qt.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ev.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bd.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mx.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hu.gzmigu.cn

[D26] 数组转字符串
来源：http://wb.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://ns.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://jt.haigaiapp.cn

JS:   arr.join(", ")
来源：http://ay.chemitech.net.cn

TS:   arr.join(", ")
来源：http://kk.521024.cn

Java: String.join(", ", list)
来源：http://da.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://pt.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://uw.nszjky.cn

C#:   string.Join(", ", list)
来源：http://pz.yuntaijiaju.cn

================================================================================
来源：http://jx.shtwfgs.cn

E. 字符串处理
来源：http://ao.521024.cn

================================================================================
来源：http://lb.haigaiapp.cn

[E01] 拼接字符串
来源：http://ij.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zk.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lr.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lk.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ce.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vr.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ct.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bj.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ey.bookmarksfly.cn

[E02] 重复字符串
来源：http://pf.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://bp.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://cz.9csxet.cn

JS:   "ab".repeat(3)
来源：http://di.hahajie.cn

TS:   "ab".repeat(3)
来源：http://wp.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://ij.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://gl.szsharing.cn

Ruby: "ab" * 3
来源：http://bf.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cj.shxzskj.cn

[E03] 截取子串
来源：http://am.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kj.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ne.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aa.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://bn.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://pf.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tr.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tb.asd995.cn

C#:   s.Substring(1, 3)
来源：http://cu.jctech888.com.cn

[E04] 查找子串位置
来源：http://gh.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://hv.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ep.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tu.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://ae.haigaiapp.cn

Java: s.indexOf("x")
来源：http://yf.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://ds.huixiangedu.cn

Ruby: s.index("x")
来源：http://qx.colortex.cn

C#:   s.IndexOf("x")
来源：http://io.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ig.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lp.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pn.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sn.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://su.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bi.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tg.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://il.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mm.yuexingan06.cn

[E06] 替换子串
来源：http://ds.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://po.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://fy.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://te.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://zo.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sw.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ya.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nw.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://tn.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://de.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://me.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bt.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tt.yuexingan06.cn

TS:   s.split(",")
来源：http://hl.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zg.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xg.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://si.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://az.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://om.haigaiapp.cn

Py:   ",".join(items)
来源：http://qi.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://ag.gzmigu.cn

JS:   items.join(",")
来源：http://nj.hnjuh.cn

TS:   items.join(",")
来源：http://vn.nszjky.cn

Java: String.join(",", items)
来源：http://oh.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://vj.chemitech.net.cn

Ruby: items.join(",")
来源：http://hy.shxzskj.cn

C#:   string.Join(",", items)
来源：http://fr.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://xl.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lw.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hi.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://kf.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://we.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://aq.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zp.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rp.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jd.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://fr.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tk.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ze.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://mb.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://hz.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://oo.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mz.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tz.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://es.jianghongdianzi.cn

[E11] 反转字符串
来源：http://tx.hahajie.cn

Py:   s[::-1]
来源：http://eq.huanxung.cn

PHP:  strrev($s);
来源：http://il.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://aa.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://zu.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ba.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zx.nicolike.cn

Ruby: s.reverse
来源：http://hi.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lt.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://ua.nszjky.cn

Py:   s.count("a")
来源：http://ea.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://mc.colortex.cn

JS:   s.split("a").length - 1
来源：http://cc.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://pl.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://te.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://zm.asd995.cn

Ruby: s.count("a")
来源：http://vu.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://wo.yuexingan06.cn

[E13] 逐字符遍历
来源：http://wk.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://we.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tp.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cb.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://um.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kq.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hq.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eo.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tm.muxihuayi.cn


<!-- 参考信息 -->