代发 wailian999

Java: list.size();
来源：http://bf.asd995.cn

Go:   len(arr)
来源：http://ck.nszjky.cn

Ruby: arr.length; arr.size
来源：http://bc.bookmarksfly.cn

C#:   list.Count;
来源：http://da.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://xp.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hd.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qv.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://nn.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://lx.nszjky.cn

Java: list.subList(1, 4);
来源：http://el.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://ur.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://wk.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://aa.yuexingan06.cn

[D08] 合并两个数组
来源：http://gz.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://ou.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://pz.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cu.nicolike.cn

TS:   [...a, ...b];
来源：http://dy.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://md.szxytkj.cn

Go:   append(a, b...)
来源：http://wn.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://vu.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://ta.colortex.cn

[D09] 排序（升序）
来源：http://ko.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vd.huixiangedu.cn

PHP:  sort($arr);
来源：http://os.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ux.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://im.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ux.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hv.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ss.huanxung.cn

C#:   list.Sort();
来源：http://tk.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bl.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bo.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bw.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://np.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xu.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fp.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cq.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yb.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ol.lnxyls.cn

[D11] 反转数组
来源：http://lx.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nr.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://an.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ww.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://xs.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://se.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://nh.panjiajie.cn

Ruby: arr.reverse
来源：http://ih.lnxyls.cn

C#:   list.Reverse();
来源：http://jb.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://tm.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://cp.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ik.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cm.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nb.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gz.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://zn.yuexingan06.cn

Ruby: arr.index(x)
来源：http://xz.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://hn.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://qa.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ha.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ev.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://qv.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://qg.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dz.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eb.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hi.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gg.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://dh.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ps.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bi.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://lh.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://or.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qn.huixinmuqiang.cn

Go:   // 手写循环
来源：http://fg.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ec.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ii.9csxet.cn

[D15] 去重
来源：http://uh.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ii.gzmigu.cn

PHP:  array_unique($arr);
来源：http://hq.huanxung.cn

JS:   [...new Set(arr)]
来源：http://ee.colortex.cn

TS:   [...new Set(arr)]
来源：http://da.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://va.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yz.hnjuh.cn

Ruby: arr.uniq
来源：http://gi.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://iy.muxihuayi.cn

[D16] 求和与平均值
来源：http://pp.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nv.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iu.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://am.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wa.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nk.szsharing.cn

Go:   // 手写循环累加
来源：http://mr.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cj.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://jh.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://iz.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://nk.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://og.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sz.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://nw.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vj.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kg.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://nv.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://hr.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://tn.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://do.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://zp.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ry.haigaiapp.cn

TS:   nested.flat();
来源：http://yi.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fh.huixiangedu.cn

Go:   // 手写双层循环
来源：http://ll.nszjky.cn

Ruby: nested.flatten
来源：http://ec.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://it.szxytkj.cn

[D19] 按字段分组
来源：http://rz.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tw.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eb.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qj.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ww.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sb.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://pn.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://av.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sf.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://bd.colortex.cn

Py:   Counter(arr)
来源：http://bu.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://nb.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nx.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xd.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://di.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://oj.asd995.cn

Ruby: arr.tally
来源：http://kh.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dn.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://cq.hnjuh.cn

Py:   x in arr
来源：http://ni.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://gi.nicolike.cn

JS:   arr.includes(x)
来源：http://bh.shxzskj.cn

TS:   arr.includes(x)
来源：http://rx.jctech888.com.cn

Java: list.contains(x)
来源：http://yv.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://sr.panjiajie.cn

Ruby: arr.include?(x)
来源：http://fx.lnxyls.cn

C#:   list.Contains(x)
来源：http://el.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://hw.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bk.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xo.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nx.szxytkj.cn

TS:   [...arr];
来源：http://zg.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://ov.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oc.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://yd.hnjuh.cn

C#:   new List<int>(list);
来源：http://kf.szxytkj.cn

[D23] reduce 累积计算
来源：http://ag.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qd.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zh.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pw.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hy.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nm.bjjhwx.cn

Go:   // 手写循环
来源：http://qp.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tk.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://po.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://lb.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cu.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qi.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gk.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bu.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://am.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ef.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nh.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uj.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://ik.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ie.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fb.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fj.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cm.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gy.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://of.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wz.521024.cn

[D26] 数组转字符串
来源：http://us.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://hz.asd995.cn

PHP:  implode(", ", $arr);
来源：http://lu.haigaiapp.cn

JS:   arr.join(", ")
来源：http://xu.nicolike.cn

TS:   arr.join(", ")
来源：http://ku.nszjky.cn

Java: String.join(", ", list)
来源：http://tj.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://ko.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://uc.nicolike.cn

C#:   string.Join(", ", list)
来源：http://qx.9csxet.cn

================================================================================
来源：http://ql.szxytkj.cn

E. 字符串处理
来源：http://wg.jianghongdianzi.cn

================================================================================
来源：http://ju.nszjky.cn

[E01] 拼接字符串
来源：http://pl.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dg.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mo.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qd.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aj.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dp.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hh.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vv.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cu.bookmarksfly.cn

[E02] 重复字符串
来源：http://nb.bookmarksfly.cn

Py:   "ab" * 3
来源：http://uj.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://mt.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://sp.huanxung.cn

TS:   "ab".repeat(3)
来源：http://of.newstarts.cn

Java: "ab".repeat(3)
来源：http://iy.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://ya.wgjwhj.cn

Ruby: "ab" * 3
来源：http://wk.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gm.bjjhwx.cn

[E03] 截取子串
来源：http://cq.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bt.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uy.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sg.9csxet.cn

TS:   s.slice(1, 4)
来源：http://sz.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://xe.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sn.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vi.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://kl.chemitech.net.cn

[E04] 查找子串位置
来源：http://wz.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://uu.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://vi.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ql.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://pq.jctech888.com.cn

Java: s.indexOf("x")
来源：http://lt.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://cc.huixiangedu.cn

Ruby: s.index("x")
来源：http://fx.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://tk.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://go.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lo.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lc.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qo.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ir.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mg.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ce.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rq.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gw.yuexingan06.cn

[E06] 替换子串
来源：http://zq.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ta.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://fm.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zt.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://xz.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vc.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rk.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cy.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://xa.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://lf.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ol.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ko.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fm.shxzukj.cn

TS:   s.split(",")
来源：http://zz.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xy.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nv.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://zt.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bo.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://gx.9csxet.cn

Py:   ",".join(items)
来源：http://ip.szxytkj.cn

PHP:  implode(",", $items);
来源：http://dq.bjjhwx.cn

JS:   items.join(",")
来源：http://ri.huixinmuqiang.cn

TS:   items.join(",")
来源：http://qc.chemitech.net.cn

Java: String.join(",", items)
来源：http://dg.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://xn.colortex.cn

Ruby: items.join(",")
来源：http://to.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://ob.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://rt.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pe.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ni.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zw.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://nt.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://qo.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vg.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nl.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ie.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://np.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hc.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fq.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://zr.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://pz.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://qm.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sp.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lv.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zt.gzmigu.cn

[E11] 反转字符串
来源：http://xy.panjiajie.cn

Py:   s[::-1]
来源：http://qr.shxzskj.cn

PHP:  strrev($s);
来源：http://ul.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ij.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://rt.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nz.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ne.lnxyls.cn

Ruby: s.reverse
来源：http://bm.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://te.hahajie.cn

[E12] 统计某字符出现次数
来源：http://rd.jctech888.com.cn

Py:   s.count("a")
来源：http://ho.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://cj.hahajie.cn

JS:   s.split("a").length - 1
来源：http://or.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://vx.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qd.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://fq.nszjky.cn

Ruby: s.count("a")
来源：http://jn.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://tt.shxzukj.cn

[E13] 逐字符遍历
来源：http://ws.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://wn.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jb.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wz.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://il.bookmarksfly.cn


<!-- 参考信息 -->