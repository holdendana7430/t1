代发 wailian999

[D07] 切片 / 取子数组
来源：http://oa.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ug.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sn.colortex.cn

JS:   arr.slice(1, 4);
来源：http://vx.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://np.nszjky.cn

Java: list.subList(1, 4);
来源：http://rh.shxzukj.cn

Go:   arr[1:4]
来源：http://am.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://ya.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://rp.huixiangedu.cn

[D08] 合并两个数组
来源：http://pp.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://pa.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://sp.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://om.shxzskj.cn

TS:   [...a, ...b];
来源：http://kx.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mr.huixiangedu.cn

Go:   append(a, b...)
来源：http://ev.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://jl.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://wj.shxzukj.cn

[D09] 排序（升序）
来源：http://in.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://vp.shxzskj.cn

PHP:  sort($arr);
来源：http://oo.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://su.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nd.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cc.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pv.shxzskj.cn

Ruby: arr.sort
来源：http://pi.bookmarksfly.cn

C#:   list.Sort();
来源：http://ic.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yi.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iq.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ko.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oi.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cl.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ky.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fa.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sj.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cg.muxihuayi.cn

[D11] 反转数组
来源：http://gs.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sf.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://hr.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://az.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://wz.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ah.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://pl.bookmarksfly.cn

Ruby: arr.reverse
来源：http://af.nicolike.cn

C#:   list.Reverse();
来源：http://mi.shxzukj.cn

[D12] 查找元素下标
来源：http://ad.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://zk.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uh.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hk.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ng.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wo.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://hk.9csxet.cn

Ruby: arr.index(x)
来源：http://dp.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://md.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ls.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qt.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jt.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://ov.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://vd.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cy.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ef.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://em.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ce.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://ws.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fs.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ki.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://dx.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://pg.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ce.lnxyls.cn

Go:   // 手写循环
来源：http://ca.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cg.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fk.bjjhwx.cn

[D15] 去重
来源：http://zd.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dz.nicolike.cn

PHP:  array_unique($arr);
来源：http://ml.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://gq.hahajie.cn

TS:   [...new Set(arr)]
来源：http://hl.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rz.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://aa.szsharing.cn

Ruby: arr.uniq
来源：http://kn.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://xv.shtwfgs.cn

[D16] 求和与平均值
来源：http://dq.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xo.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ww.9csxet.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zk.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uz.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cj.nszjky.cn

Go:   // 手写循环累加
来源：http://tm.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ek.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://iq.gzmigu.cn

[D17] 最大值与最小值
来源：http://nj.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ep.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://wg.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pf.gzmigu.cn

TS:   Math.max(...arr);
来源：http://bc.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://go.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ve.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://xf.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://ro.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://ij.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kg.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://rr.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ak.bookmarksfly.cn

TS:   nested.flat();
来源：http://dw.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gh.9csxet.cn

Go:   // 手写双层循环
来源：http://ln.szsharing.cn

Ruby: nested.flatten
来源：http://yg.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ix.jctech888.com.cn

[D19] 按字段分组
来源：http://xu.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cd.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yz.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://on.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hk.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zq.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://xi.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ar.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vl.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://fo.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://sg.colortex.cn

PHP:  array_count_values($arr);
来源：http://jb.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uq.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dj.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gk.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://oj.bjjhwx.cn

Ruby: arr.tally
来源：http://if.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fp.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://pi.szsharing.cn

Py:   x in arr
来源：http://vw.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://el.panjiajie.cn

JS:   arr.includes(x)
来源：http://ol.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://rp.lnxyls.cn

Java: list.contains(x)
来源：http://fu.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://cw.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://bs.asd995.cn

C#:   list.Contains(x)
来源：http://ua.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://gz.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fw.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qq.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iy.shxzukj.cn

TS:   [...arr];
来源：http://ou.szsharing.cn

Java: new ArrayList<>(list);
来源：http://ip.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qc.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://so.9csxet.cn

C#:   new List<int>(list);
来源：http://qv.bjjhwx.cn

[D23] reduce 累积计算
来源：http://qh.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bi.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tl.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fi.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://el.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sa.hahajie.cn

Go:   // 手写循环
来源：http://ee.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kl.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hj.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://wg.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sp.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ex.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xt.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://od.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kl.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vz.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tu.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yi.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://pi.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kz.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yz.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cg.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tj.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jk.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nj.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nt.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://so.521024.cn

[D26] 数组转字符串
来源：http://hi.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://nj.colortex.cn

PHP:  implode(", ", $arr);
来源：http://lw.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://or.9csxet.cn

TS:   arr.join(", ")
来源：http://dj.gzmigu.cn

Java: String.join(", ", list)
来源：http://dq.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://hz.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://te.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://in.yuntaijiaju.cn

================================================================================
来源：http://gn.gzmigu.cn

E. 字符串处理
来源：http://vz.newstarts.cn

================================================================================
来源：http://wz.nszjky.cn

[E01] 拼接字符串
来源：http://ny.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ui.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cn.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sk.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xu.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dy.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qh.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://na.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lf.huixiangedu.cn

[E02] 重复字符串
来源：http://yg.shtwfgs.cn

Py:   "ab" * 3
来源：http://ad.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://dl.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://rf.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://wq.colortex.cn

Java: "ab".repeat(3)
来源：http://kg.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://ci.newstarts.cn

Ruby: "ab" * 3
来源：http://ps.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vo.jctech888.com.cn

[E03] 截取子串
来源：http://fj.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bm.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tw.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qz.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://ik.szsharing.cn

Java: s.substring(1, 4)
来源：http://uq.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ie.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yd.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://lt.yuexingan06.cn

[E04] 查找子串位置
来源：http://qg.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://of.hahajie.cn

PHP:  strpos($s, "x");
来源：http://wy.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fx.nszjky.cn

TS:   s.indexOf("x")
来源：http://ak.colortex.cn

Java: s.indexOf("x")
来源：http://qv.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://zh.asd995.cn

Ruby: s.index("x")
来源：http://zt.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://qk.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fe.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pw.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wj.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ja.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://co.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hy.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ex.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rc.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fd.wgjwhj.cn

[E06] 替换子串
来源：http://mv.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iv.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://oi.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jt.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://tp.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://il.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yv.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cw.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://ub.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://fm.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lp.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://du.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pw.asd995.cn

TS:   s.split(",")
来源：http://wr.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dg.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lk.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://ol.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tg.asd995.cn

[E08] 数组按分隔符合并
来源：http://qa.shxzukj.cn

Py:   ",".join(items)
来源：http://nb.shxzskj.cn

PHP:  implode(",", $items);
来源：http://uz.gzmigu.cn

JS:   items.join(",")
来源：http://kq.bjjhwx.cn

TS:   items.join(",")
来源：http://hq.wgjwhj.cn

Java: String.join(",", items)
来源：http://ok.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://tn.asd995.cn

Ruby: items.join(",")
来源：http://hy.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://fj.521024.cn

[E09] 去除所有空白字符
来源：http://qa.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://za.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fa.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://bo.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://xl.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://jp.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wy.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vz.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vu.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://zl.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iw.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://se.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://rj.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://fx.newstarts.cn

Java: String.format("%03d", 7)
来源：http://rv.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tx.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hb.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rg.shtwfgs.cn

[E11] 反转字符串
来源：http://tx.wgjwhj.cn

Py:   s[::-1]
来源：http://jk.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://wl.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://fn.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://eg.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ew.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qp.asd995.cn

Ruby: s.reverse
来源：http://ch.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lk.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://cm.chemitech.net.cn

Py:   s.count("a")
来源：http://jr.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://wh.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://ks.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://rx.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ye.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://eo.gzmigu.cn

Ruby: s.count("a")
来源：http://ee.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://md.muxihuayi.cn

[E13] 逐字符遍历
来源：http://gb.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://kh.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xc.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rc.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lt.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ef.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ct.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://me.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pc.9csxet.cn


<!-- 参考信息 -->