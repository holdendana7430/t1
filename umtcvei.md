代发 wailian999

Java: list.size();
来源：http://yf.asd995.cn

Go:   len(arr)
来源：http://cc.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://yr.hahajie.cn

C#:   list.Count;
来源：http://an.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://cq.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hr.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dt.asd995.cn

JS:   arr.slice(1, 4);
来源：http://ra.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://vf.521024.cn

Java: list.subList(1, 4);
来源：http://ca.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://gs.newstarts.cn

Ruby: arr[1, 3]
来源：http://bs.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://rl.gzmigu.cn

[D08] 合并两个数组
来源：http://ig.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://mg.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://bl.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ay.521024.cn

TS:   [...a, ...b];
来源：http://tt.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wf.jctech888.com.cn

Go:   append(a, b...)
来源：http://of.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://tg.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://ih.hnjuh.cn

[D09] 排序（升序）
来源：http://pj.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://mq.lnxyls.cn

PHP:  sort($arr);
来源：http://qh.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yt.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qz.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oy.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pl.asd995.cn

Ruby: arr.sort
来源：http://sn.muxihuayi.cn

C#:   list.Sort();
来源：http://pz.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ku.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://it.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dw.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yj.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hk.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gq.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wh.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zw.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wh.gzmigu.cn

[D11] 反转数组
来源：http://pr.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aa.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://al.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vr.shxzukj.cn

TS:   [...arr].reverse();
来源：http://wr.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://jx.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://hx.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://ir.521024.cn

C#:   list.Reverse();
来源：http://ud.lnxyls.cn

[D12] 查找元素下标
来源：http://ce.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://no.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vf.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yk.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mm.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qj.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://iw.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://or.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://rw.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://so.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rh.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rf.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://qv.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://zw.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vz.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kr.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pp.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gq.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://ai.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hl.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://es.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://xv.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://yl.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zd.asd995.cn

Go:   // 手写循环
来源：http://bh.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tt.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ix.shxzukj.cn

[D15] 去重
来源：http://yg.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kc.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://lv.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://zt.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://xr.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hj.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xl.haigaiapp.cn

Ruby: arr.uniq
来源：http://lt.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://cn.wgjwhj.cn

[D16] 求和与平均值
来源：http://ql.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pm.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xl.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://al.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gv.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ui.hahajie.cn

Go:   // 手写循环累加
来源：http://eh.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ot.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://fo.asd995.cn

[D17] 最大值与最小值
来源：http://hu.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://as.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://as.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wf.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://nv.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mu.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ac.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://yj.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ug.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://ja.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://km.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://uj.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ew.huixinmuqiang.cn

TS:   nested.flat();
来源：http://na.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dz.haigaiapp.cn

Go:   // 手写双层循环
来源：http://bm.muxihuayi.cn

Ruby: nested.flatten
来源：http://ww.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cr.521024.cn

[D19] 按字段分组
来源：http://ty.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kb.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://de.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ox.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uf.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://re.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://ps.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bv.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ue.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://ap.lnxyls.cn

Py:   Counter(arr)
来源：http://dy.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://cc.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nx.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ah.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nu.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://nv.nicolike.cn

Ruby: arr.tally
来源：http://ql.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jh.huanxung.cn

[D21] 判断是否包含某元素
来源：http://yi.hahajie.cn

Py:   x in arr
来源：http://lh.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://wr.lnxyls.cn

JS:   arr.includes(x)
来源：http://yk.gzmigu.cn

TS:   arr.includes(x)
来源：http://ov.haigaiapp.cn

Java: list.contains(x)
来源：http://lv.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://to.szsharing.cn

Ruby: arr.include?(x)
来源：http://qw.shxzskj.cn

C#:   list.Contains(x)
来源：http://vr.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ap.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rv.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://md.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fc.huanxung.cn

TS:   [...arr];
来源：http://fz.newstarts.cn

Java: new ArrayList<>(list);
来源：http://pr.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nq.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://gw.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://hy.szxytkj.cn

[D23] reduce 累积计算
来源：http://bd.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sd.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ff.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fl.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nm.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ae.lnxyls.cn

Go:   // 手写循环
来源：http://gn.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ad.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://my.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://bn.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bp.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wk.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ak.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nr.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://db.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oa.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://he.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cv.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ad.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rn.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cp.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://um.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://by.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sa.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://az.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jl.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lx.shxzukj.cn

[D26] 数组转字符串
来源：http://yl.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://xr.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://sv.szxytkj.cn

JS:   arr.join(", ")
来源：http://mg.9csxet.cn

TS:   arr.join(", ")
来源：http://et.colortex.cn

Java: String.join(", ", list)
来源：http://vz.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://vn.nicolike.cn

Ruby: arr.join(", ")
来源：http://tt.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://wj.jctech888.com.cn

================================================================================
来源：http://nc.shtwfgs.cn

E. 字符串处理
来源：http://ai.shxzukj.cn

================================================================================
来源：http://ew.muxihuayi.cn

[E01] 拼接字符串
来源：http://qt.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mu.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qb.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ve.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ft.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yu.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jg.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qh.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mq.bjjhwx.cn

[E02] 重复字符串
来源：http://zi.gzmigu.cn

Py:   "ab" * 3
来源：http://bn.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://xd.nicolike.cn

JS:   "ab".repeat(3)
来源：http://og.nicolike.cn

TS:   "ab".repeat(3)
来源：http://ke.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://qn.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://av.bjjhwx.cn

Ruby: "ab" * 3
来源：http://lx.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yz.asd995.cn

[E03] 截取子串
来源：http://rb.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://as.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cp.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zw.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://qu.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://sj.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ee.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lx.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://cq.huanxung.cn

[E04] 查找子串位置
来源：http://va.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ps.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://qj.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yo.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://gd.nicolike.cn

Java: s.indexOf("x")
来源：http://nh.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://ax.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://st.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://us.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ar.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lw.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qz.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ne.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aw.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mi.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oh.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vb.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tk.bjjhwx.cn

[E06] 替换子串
来源：http://gn.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://it.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://tq.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://si.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ud.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cp.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wn.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hu.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://jp.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://qe.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://um.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xd.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qf.huixinmuqiang.cn

TS:   s.split(",")
来源：http://eh.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vg.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ai.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://lg.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ch.newstarts.cn

[E08] 数组按分隔符合并
来源：http://ux.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://eu.521024.cn

PHP:  implode(",", $items);
来源：http://ii.521024.cn

JS:   items.join(",")
来源：http://ji.jianghongdianzi.cn

TS:   items.join(",")
来源：http://gq.huanxung.cn

Java: String.join(",", items)
来源：http://jh.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://yi.asd995.cn

Ruby: items.join(",")
来源：http://ub.panjiajie.cn

C#:   string.Join(",", items)
来源：http://eq.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://uq.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mx.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jd.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://dr.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://vg.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://xq.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://df.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lx.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xv.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://ee.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://un.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ag.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://td.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://ic.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://uv.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://in.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gv.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tz.hahajie.cn

[E11] 反转字符串
来源：http://cc.panjiajie.cn

Py:   s[::-1]
来源：http://pq.panjiajie.cn

PHP:  strrev($s);
来源：http://io.colortex.cn

JS:   [...s].reverse().join("")
来源：http://zf.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://hv.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cd.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dw.chemitech.net.cn

Ruby: s.reverse
来源：http://az.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zg.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://sc.asd995.cn

Py:   s.count("a")
来源：http://xh.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://ou.521024.cn

JS:   s.split("a").length - 1
来源：http://ri.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://dt.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tq.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://hs.panjiajie.cn

Ruby: s.count("a")
来源：http://ce.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://xx.panjiajie.cn

[E13] 逐字符遍历
来源：http://kv.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://iv.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aa.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iw.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mk.521024.cn


<!-- 参考信息 -->