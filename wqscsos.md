代发 wailian999

[D07] 切片 / 取子数组
来源：http://bg.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ae.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mt.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://qg.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://gt.lnxyls.cn

Java: list.subList(1, 4);
来源：http://lb.szxytkj.cn

Go:   arr[1:4]
来源：http://ne.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://ag.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ru.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://oe.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://nv.521024.cn

PHP:  array_merge($a, $b);
来源：http://rz.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yh.9csxet.cn

TS:   [...a, ...b];
来源：http://gv.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zp.lnxyls.cn

Go:   append(a, b...)
来源：http://es.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://bq.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://ln.hahajie.cn

[D09] 排序（升序）
来源：http://ha.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://dq.hahajie.cn

PHP:  sort($arr);
来源：http://zo.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jw.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tf.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://el.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pp.9csxet.cn

Ruby: arr.sort
来源：http://js.asd995.cn

C#:   list.Sort();
来源：http://zu.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://um.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kf.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fm.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://an.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gz.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nx.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ox.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oy.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tx.lnxyls.cn

[D11] 反转数组
来源：http://xb.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fb.hahajie.cn

PHP:  array_reverse($arr);
来源：http://ne.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tz.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://hv.shxzskj.cn

Java: Collections.reverse(list);
来源：http://fg.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://jj.yuexingan06.cn

Ruby: arr.reverse
来源：http://qj.szsharing.cn

C#:   list.Reverse();
来源：http://ye.521024.cn

[D12] 查找元素下标
来源：http://hg.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://uz.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gu.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rs.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hf.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qi.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://fv.haigaiapp.cn

Ruby: arr.index(x)
来源：http://wx.newstarts.cn

C#:   list.IndexOf(x);
来源：http://kx.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://hk.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wl.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jn.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://md.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://fl.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xn.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ll.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xk.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gf.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://fm.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ax.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rp.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://tq.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://je.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ke.gzmigu.cn

Go:   // 手写循环
来源：http://sj.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fi.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rb.hahajie.cn

[D15] 去重
来源：http://ox.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ec.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://gk.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://le.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://uh.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bi.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ru.szxytkj.cn

Ruby: arr.uniq
来源：http://er.colortex.cn

C#:   list.Distinct().ToList()
来源：http://uk.yuexingan06.cn

[D16] 求和与平均值
来源：http://gz.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tx.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sm.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nh.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lb.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lb.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://bz.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zs.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://gn.nicolike.cn

[D17] 最大值与最小值
来源：http://le.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://zz.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://md.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fd.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://hw.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cb.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zh.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://vf.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://ay.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://la.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fv.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://jj.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ep.shxzskj.cn

TS:   nested.flat();
来源：http://za.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jw.jctech888.com.cn

Go:   // 手写双层循环
来源：http://gm.lnxyls.cn

Ruby: nested.flatten
来源：http://rf.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vr.yuntaijiaju.cn

[D19] 按字段分组
来源：http://wf.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cj.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://au.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sf.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://af.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sa.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://ja.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qp.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xb.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://eu.jctech888.com.cn

Py:   Counter(arr)
来源：http://gt.hahajie.cn

PHP:  array_count_values($arr);
来源：http://iw.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ef.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ph.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ts.colortex.cn

Go:   // 手写 map[T]int
来源：http://pp.shtwfgs.cn

Ruby: arr.tally
来源：http://vr.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bg.asd995.cn

[D21] 判断是否包含某元素
来源：http://bk.szsharing.cn

Py:   x in arr
来源：http://zv.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://vb.shtwfgs.cn

JS:   arr.includes(x)
来源：http://wj.huanxung.cn

TS:   arr.includes(x)
来源：http://qz.huixiangedu.cn

Java: list.contains(x)
来源：http://lu.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://sl.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://gh.jctech888.com.cn

C#:   list.Contains(x)
来源：http://hs.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://vj.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ws.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mi.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oh.shxzukj.cn

TS:   [...arr];
来源：http://hu.asd995.cn

Java: new ArrayList<>(list);
来源：http://xq.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ys.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://rt.nicolike.cn

C#:   new List<int>(list);
来源：http://ck.colortex.cn

[D23] reduce 累积计算
来源：http://pb.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zt.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fc.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nf.shxzukj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zw.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qr.huanxung.cn

Go:   // 手写循环
来源：http://ma.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kh.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cu.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://ys.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cs.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ie.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yn.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wr.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nc.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zu.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ib.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ig.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://cl.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ft.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zh.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iu.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cb.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lc.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zj.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uz.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lo.521024.cn

[D26] 数组转字符串
来源：http://vc.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ya.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://hz.bjjhwx.cn

JS:   arr.join(", ")
来源：http://fa.shxzskj.cn

TS:   arr.join(", ")
来源：http://wc.bjjhwx.cn

Java: String.join(", ", list)
来源：http://pa.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://hr.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://ti.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://yx.bjjhwx.cn

================================================================================
来源：http://ir.jianghongdianzi.cn

E. 字符串处理
来源：http://sb.panjiajie.cn

================================================================================
来源：http://aw.nicolike.cn

[E01] 拼接字符串
来源：http://cz.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nu.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rm.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rh.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ib.newstarts.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mc.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wq.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yg.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://td.chemitech.net.cn

[E02] 重复字符串
来源：http://on.lnxyls.cn

Py:   "ab" * 3
来源：http://ew.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://ha.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://me.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://va.nszjky.cn

Java: "ab".repeat(3)
来源：http://ug.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://dl.muxihuayi.cn

Ruby: "ab" * 3
来源：http://ij.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yh.lnxyls.cn

[E03] 截取子串
来源：http://ej.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vt.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zc.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bg.521024.cn

TS:   s.slice(1, 4)
来源：http://qp.shxzukj.cn

Java: s.substring(1, 4)
来源：http://zu.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oi.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ug.colortex.cn

C#:   s.Substring(1, 3)
来源：http://mx.nszjky.cn

[E04] 查找子串位置
来源：http://hg.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://uo.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://yp.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ob.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://dr.nszjky.cn

Java: s.indexOf("x")
来源：http://xl.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://be.yuexingan06.cn

Ruby: s.index("x")
来源：http://lc.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://zq.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://up.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nd.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sa.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ut.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ep.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oi.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iw.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iz.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fu.colortex.cn

[E06] 替换子串
来源：http://uc.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://df.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://od.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rx.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://nu.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gp.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ro.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dw.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://cy.nszjky.cn

[E07] 按分隔符拆分
来源：http://lo.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wo.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fh.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zy.huixiangedu.cn

TS:   s.split(",")
来源：http://bg.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vu.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nw.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://sv.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jb.521024.cn

[E08] 数组按分隔符合并
来源：http://ev.colortex.cn

Py:   ",".join(items)
来源：http://kt.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://hc.szxytkj.cn

JS:   items.join(",")
来源：http://tg.huixinmuqiang.cn

TS:   items.join(",")
来源：http://ii.521024.cn

Java: String.join(",", items)
来源：http://en.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://no.shxzukj.cn

Ruby: items.join(",")
来源：http://jc.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://xh.colortex.cn

[E09] 去除所有空白字符
来源：http://zy.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ye.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ve.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://jg.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://pq.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://bb.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vm.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ll.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tz.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://iw.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ql.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dl.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://zd.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://eh.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://kg.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yz.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ee.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fr.muxihuayi.cn

[E11] 反转字符串
来源：http://zy.huixiangedu.cn

Py:   s[::-1]
来源：http://fc.jctech888.com.cn

PHP:  strrev($s);
来源：http://na.asd995.cn

JS:   [...s].reverse().join("")
来源：http://qw.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://sm.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rj.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zm.hnjuh.cn

Ruby: s.reverse
来源：http://fx.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vd.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://cn.newstarts.cn

Py:   s.count("a")
来源：http://cq.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://lm.asd995.cn

JS:   s.split("a").length - 1
来源：http://px.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://qk.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uv.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://mb.panjiajie.cn

Ruby: s.count("a")
来源：http://hg.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://iy.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://xa.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://cw.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qq.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pp.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xv.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pf.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dk.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mp.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ku.shxzukj.cn


<!-- 参考信息 -->