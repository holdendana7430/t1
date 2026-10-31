代发 wailian999

Py:   len(arr)
来源：http://qn.shxzskj.cn

PHP:  count($arr);
来源：http://bk.gzmigu.cn

JS:   arr.length
来源：http://fm.szsharing.cn

TS:   arr.length
来源：http://us.haigaiapp.cn

Java: list.size();
来源：http://ef.muxihuayi.cn

Go:   len(arr)
来源：http://rh.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://cz.panjiajie.cn

C#:   list.Count;
来源：http://oz.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://dc.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://me.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zp.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://up.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://kf.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://zl.panjiajie.cn

Go:   arr[1:4]
来源：http://xs.nicolike.cn

Ruby: arr[1, 3]
来源：http://en.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://tv.hnjuh.cn

[D08] 合并两个数组
来源：http://op.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://yp.521024.cn

PHP:  array_merge($a, $b);
来源：http://ya.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ss.yuexingan06.cn

TS:   [...a, ...b];
来源：http://gr.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hx.chemitech.net.cn

Go:   append(a, b...)
来源：http://mf.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://fm.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://cn.gzmigu.cn

[D09] 排序（升序）
来源：http://ab.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://sd.szsharing.cn

PHP:  sort($arr);
来源：http://sk.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ym.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ho.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dp.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wk.shxzskj.cn

Ruby: arr.sort
来源：http://tc.szxytkj.cn

C#:   list.Sort();
来源：http://ki.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kg.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bg.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qd.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ts.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tf.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mb.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sw.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hc.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bn.yuexingan06.cn

[D11] 反转数组
来源：http://eg.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gu.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://hf.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zd.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ni.gzmigu.cn

Java: Collections.reverse(list);
来源：http://ai.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://zv.yuexingan06.cn

Ruby: arr.reverse
来源：http://ne.hahajie.cn

C#:   list.Reverse();
来源：http://ik.jctech888.com.cn

[D12] 查找元素下标
来源：http://sr.521024.cn

Py:   arr.index(x);  x in arr
来源：http://xg.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vb.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xc.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oa.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cs.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://fw.hnjuh.cn

Ruby: arr.index(x)
来源：http://ub.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://os.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://rf.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wu.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tw.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://nk.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://qk.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nn.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nh.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ar.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ip.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://ms.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cu.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ev.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://ic.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://th.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sg.muxihuayi.cn

Go:   // 手写循环
来源：http://fj.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xb.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vu.jianghongdianzi.cn

[D15] 去重
来源：http://ul.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hy.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://it.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://el.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://ur.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rx.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ps.bjjhwx.cn

Ruby: arr.uniq
来源：http://kz.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://kg.colortex.cn

[D16] 求和与平均值
来源：http://gt.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://in.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pf.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://os.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kj.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zd.nicolike.cn

Go:   // 手写循环累加
来源：http://ej.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mu.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://wt.gzmigu.cn

[D17] 最大值与最小值
来源：http://vj.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://xd.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://js.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tz.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://ls.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pr.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xc.asd995.cn

Ruby: arr.max;  arr.min
来源：http://lq.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://ef.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://md.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ht.521024.cn

PHP:  array_merge(...$nested);
来源：http://tj.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sy.newstarts.cn

TS:   nested.flat();
来源：http://ab.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://km.bjjhwx.cn

Go:   // 手写双层循环
来源：http://pj.521024.cn

Ruby: nested.flatten
来源：http://zd.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qx.huixiangedu.cn

[D19] 按字段分组
来源：http://zh.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zt.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qd.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nw.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://si.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mw.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://ti.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zy.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jy.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://so.lnxyls.cn

Py:   Counter(arr)
来源：http://yg.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://jm.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yx.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ux.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zn.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://tj.huixiangedu.cn

Ruby: arr.tally
来源：http://gm.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yh.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://bs.haigaiapp.cn

Py:   x in arr
来源：http://ms.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://pw.shtwfgs.cn

JS:   arr.includes(x)
来源：http://xt.chemitech.net.cn

TS:   arr.includes(x)
来源：http://id.muxihuayi.cn

Java: list.contains(x)
来源：http://th.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://tu.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://fi.panjiajie.cn

C#:   list.Contains(x)
来源：http://te.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://zu.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xi.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ux.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gy.lnxyls.cn

TS:   [...arr];
来源：http://gr.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://cq.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vy.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://sv.yuexingan06.cn

C#:   new List<int>(list);
来源：http://vc.wgjwhj.cn

[D23] reduce 累积计算
来源：http://td.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fg.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hn.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fw.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ar.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rg.lnxyls.cn

Go:   // 手写循环
来源：http://az.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://js.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wb.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://kw.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pa.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wi.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://js.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kh.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://em.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qy.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ae.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zk.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://vy.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yn.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ha.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dj.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://je.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hk.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zj.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wx.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cr.panjiajie.cn

[D26] 数组转字符串
来源：http://pq.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://he.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://wo.shxzukj.cn

JS:   arr.join(", ")
来源：http://rz.haigaiapp.cn

TS:   arr.join(", ")
来源：http://bh.asd995.cn

Java: String.join(", ", list)
来源：http://lj.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://en.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://la.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://qa.wgjwhj.cn

================================================================================
来源：http://zf.yuntaijiaju.cn

E. 字符串处理
来源：http://jg.szxytkj.cn

================================================================================
来源：http://yp.szsharing.cn

[E01] 拼接字符串
来源：http://kn.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vb.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mu.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ed.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://os.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ry.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yg.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ng.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xy.jctech888.com.cn

[E02] 重复字符串
来源：http://fi.bookmarksfly.cn

Py:   "ab" * 3
来源：http://yp.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://aj.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://fe.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://oa.521024.cn

Java: "ab".repeat(3)
来源：http://fw.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://tc.newstarts.cn

Ruby: "ab" * 3
来源：http://cd.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wb.gzmigu.cn

[E03] 截取子串
来源：http://yg.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ea.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ou.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hu.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://yo.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://xd.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ol.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nq.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://vb.yuexingan06.cn

[E04] 查找子串位置
来源：http://de.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://oh.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://hq.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://do.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://io.newstarts.cn

Java: s.indexOf("x")
来源：http://hj.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://sf.bjjhwx.cn

Ruby: s.index("x")
来源：http://mo.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://xl.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uk.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ke.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zx.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lw.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://er.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://in.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://od.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ij.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rh.bjjhwx.cn

[E06] 替换子串
来源：http://zu.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ef.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://ka.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sk.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://yp.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aa.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eg.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sm.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://xs.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://nd.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qc.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xi.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oa.huanxung.cn

TS:   s.split(",")
来源：http://wp.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tc.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ii.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://gf.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jr.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://hj.lnxyls.cn

Py:   ",".join(items)
来源：http://ge.panjiajie.cn

PHP:  implode(",", $items);
来源：http://bf.nszjky.cn

JS:   items.join(",")
来源：http://yo.szsharing.cn

TS:   items.join(",")
来源：http://em.jctech888.com.cn

Java: String.join(",", items)
来源：http://ep.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://hr.nicolike.cn

Ruby: items.join(",")
来源：http://uw.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://rw.hnjuh.cn

[E09] 去除所有空白字符
来源：http://bj.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wx.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yi.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://qr.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://fa.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://mg.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cp.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://by.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kg.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://ki.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lw.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tj.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://uh.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://ol.asd995.cn

Java: String.format("%03d", 7)
来源：http://nt.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lq.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kl.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gx.panjiajie.cn

[E11] 反转字符串
来源：http://iu.haigaiapp.cn

Py:   s[::-1]
来源：http://qd.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://bb.colortex.cn

JS:   [...s].reverse().join("")
来源：http://hi.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://hj.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mk.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ys.shtwfgs.cn

Ruby: s.reverse
来源：http://jm.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cn.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://hy.hnjuh.cn

Py:   s.count("a")
来源：http://nn.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://lk.asd995.cn

JS:   s.split("a").length - 1
来源：http://vj.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://qy.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dk.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://cb.nszjky.cn

Ruby: s.count("a")
来源：http://gk.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://mq.hnjuh.cn

[E13] 逐字符遍历
来源：http://ql.jctech888.com.cn


<!-- 参考信息 -->