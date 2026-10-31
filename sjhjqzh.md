代发 wailian999

Java: list.size();
来源：http://vr.huanxung.cn

Go:   len(arr)
来源：http://nj.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://yg.shxzskj.cn

C#:   list.Count;
来源：http://rt.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://aj.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ri.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pt.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://yb.colortex.cn

TS:   arr.slice(1, 4);
来源：http://hz.hnjuh.cn

Java: list.subList(1, 4);
来源：http://oj.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ro.szxytkj.cn

Ruby: arr[1, 3]
来源：http://kj.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://gk.wgjwhj.cn

[D08] 合并两个数组
来源：http://lo.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://we.asd995.cn

PHP:  array_merge($a, $b);
来源：http://zp.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kf.hahajie.cn

TS:   [...a, ...b];
来源：http://oy.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zm.hnjuh.cn

Go:   append(a, b...)
来源：http://mh.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://cp.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://vf.wgjwhj.cn

[D09] 排序（升序）
来源：http://xy.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ax.yuexingan06.cn

PHP:  sort($arr);
来源：http://dl.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mj.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pc.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vg.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ke.szsharing.cn

Ruby: arr.sort
来源：http://iy.lnxyls.cn

C#:   list.Sort();
来源：http://sx.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://no.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oe.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qf.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ps.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vi.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cd.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vd.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ls.newstarts.cn

[D11] 反转数组
来源：http://dc.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pm.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://ia.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nk.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://ni.huanxung.cn

Java: Collections.reverse(list);
来源：http://lm.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://vm.shtwfgs.cn

Ruby: arr.reverse
来源：http://qg.panjiajie.cn

C#:   list.Reverse();
来源：http://ox.newstarts.cn

[D12] 查找元素下标
来源：http://hc.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://lr.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ka.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://li.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jc.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sr.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://ur.nszjky.cn

Ruby: arr.index(x)
来源：http://bf.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://jy.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://tk.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oq.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ze.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://cd.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://so.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rg.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://px.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hb.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qw.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://jg.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hq.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ty.521024.cn

JS:   arr.map(x => x * 2)
来源：http://rf.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://yc.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lt.shtwfgs.cn

Go:   // 手写循环
来源：http://lx.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ab.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fu.shxzskj.cn

[D15] 去重
来源：http://bv.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gv.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://jr.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://is.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://bg.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wf.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pc.panjiajie.cn

Ruby: arr.uniq
来源：http://pj.asd995.cn

C#:   list.Distinct().ToList()
来源：http://ql.bjjhwx.cn

[D16] 求和与平均值
来源：http://dp.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zy.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jm.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ya.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fa.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dn.shtwfgs.cn

Go:   // 手写循环累加
来源：http://wg.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://po.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://xg.panjiajie.cn

[D17] 最大值与最小值
来源：http://bb.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://lo.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://yv.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://so.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://qw.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fk.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uc.colortex.cn

Ruby: arr.max;  arr.min
来源：http://zr.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://ij.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://pz.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cp.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://zb.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bv.nszjky.cn

TS:   nested.flat();
来源：http://tv.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gc.asd995.cn

Go:   // 手写双层循环
来源：http://wa.gzmigu.cn

Ruby: nested.flatten
来源：http://uw.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hu.hahajie.cn

[D19] 按字段分组
来源：http://ae.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tj.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pt.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xt.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xl.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dq.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://hu.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ol.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://az.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://yw.colortex.cn

Py:   Counter(arr)
来源：http://rw.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://lg.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kw.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wh.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cq.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://lm.shxzukj.cn

Ruby: arr.tally
来源：http://ev.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cn.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://ge.colortex.cn

Py:   x in arr
来源：http://zl.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://cu.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://fa.szxytkj.cn

TS:   arr.includes(x)
来源：http://mw.jctech888.com.cn

Java: list.contains(x)
来源：http://eh.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://kd.jianghongdianzi.cn

Ruby: arr.include?(x)
来源：http://rb.haigaiapp.cn

C#:   list.Contains(x)
来源：http://xb.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://co.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ya.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ps.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://so.jctech888.com.cn

TS:   [...arr];
来源：http://sb.colortex.cn

Java: new ArrayList<>(list);
来源：http://qt.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bb.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://dn.wgjwhj.cn

C#:   new List<int>(list);
来源：http://ac.shxzukj.cn

[D23] reduce 累积计算
来源：http://te.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bf.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gn.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bx.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vx.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kx.muxihuayi.cn

Go:   // 手写循环
来源：http://no.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fa.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cs.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://kd.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rj.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://es.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hw.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pp.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yz.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hg.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ii.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sc.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://ft.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ot.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sk.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bv.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bp.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qp.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lj.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qu.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bj.chemitech.net.cn

[D26] 数组转字符串
来源：http://ar.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://rp.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://wk.shxzskj.cn

JS:   arr.join(", ")
来源：http://fp.haigaiapp.cn

TS:   arr.join(", ")
来源：http://rr.newstarts.cn

Java: String.join(", ", list)
来源：http://ig.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://xx.szsharing.cn

Ruby: arr.join(", ")
来源：http://fc.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://th.nicolike.cn

================================================================================
来源：http://ym.haigaiapp.cn

E. 字符串处理
来源：http://cy.gzmigu.cn

================================================================================
来源：http://zn.chemitech.net.cn

[E01] 拼接字符串
来源：http://bo.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hy.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://at.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zd.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rx.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kz.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://es.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gk.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nn.huixiangedu.cn

[E02] 重复字符串
来源：http://bh.9csxet.cn

Py:   "ab" * 3
来源：http://ot.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://jt.szsharing.cn

JS:   "ab".repeat(3)
来源：http://pm.colortex.cn

TS:   "ab".repeat(3)
来源：http://dx.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://pc.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://uj.9csxet.cn

Ruby: "ab" * 3
来源：http://wv.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ee.nicolike.cn

[E03] 截取子串
来源：http://wp.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nt.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zl.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hq.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://kx.szsharing.cn

Java: s.substring(1, 4)
来源：http://zq.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ca.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mj.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://vw.yuexingan06.cn

[E04] 查找子串位置
来源：http://lf.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://df.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://at.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://na.nicolike.cn

TS:   s.indexOf("x")
来源：http://iz.newstarts.cn

Java: s.indexOf("x")
来源：http://nq.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://xb.colortex.cn

Ruby: s.index("x")
来源：http://dt.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://bz.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ql.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wp.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vu.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bl.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kl.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uj.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zt.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iy.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kg.521024.cn

[E06] 替换子串
来源：http://ry.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lp.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://ey.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uh.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://ds.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yv.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vh.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vp.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://kb.shxzukj.cn

[E07] 按分隔符拆分
来源：http://xh.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wy.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gv.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tf.szsharing.cn

TS:   s.split(",")
来源：http://od.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cl.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yy.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://lp.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cu.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://xu.shxzukj.cn

Py:   ",".join(items)
来源：http://ck.colortex.cn

PHP:  implode(",", $items);
来源：http://yr.hnjuh.cn

JS:   items.join(",")
来源：http://jm.newstarts.cn

TS:   items.join(",")
来源：http://pl.haigaiapp.cn

Java: String.join(",", items)
来源：http://bq.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://xo.szxytkj.cn

Ruby: items.join(",")
来源：http://lh.521024.cn

C#:   string.Join(",", items)
来源：http://zd.hnjuh.cn

[E09] 去除所有空白字符
来源：http://iu.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://et.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jp.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://qn.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://ln.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://rl.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yz.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pc.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://as.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://jh.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pk.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wa.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://wg.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://hb.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://or.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ex.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zn.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xw.shtwfgs.cn

[E11] 反转字符串
来源：http://le.colortex.cn

Py:   s[::-1]
来源：http://ku.lnxyls.cn

PHP:  strrev($s);
来源：http://cg.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://xb.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://im.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zv.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ps.wgjwhj.cn

Ruby: s.reverse
来源：http://wu.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nh.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://kd.521024.cn

Py:   s.count("a")
来源：http://hp.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://ik.huanxung.cn

JS:   s.split("a").length - 1
来源：http://sl.asd995.cn

TS:   s.split("a").length - 1
来源：http://hn.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://po.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://pl.huixiangedu.cn

Ruby: s.count("a")
来源：http://nl.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://aa.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ez.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://xs.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ys.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gr.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rx.wgjwhj.cn


<!-- 参考信息 -->