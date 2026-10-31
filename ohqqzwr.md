代发 wailian999

TS:   arr.slice(1, 4);
来源：http://za.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://ks.bookmarksfly.cn

Go:   arr[1:4]
来源：http://id.szxytkj.cn

Ruby: arr[1, 3]
来源：http://yi.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://oh.yuexingan06.cn

[D08] 合并两个数组
来源：http://pv.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://fq.asd995.cn

PHP:  array_merge($a, $b);
来源：http://hj.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nx.szxytkj.cn

TS:   [...a, ...b];
来源：http://nr.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xn.yuexingan06.cn

Go:   append(a, b...)
来源：http://vp.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://bc.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://wv.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://zg.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://wp.hahajie.cn

PHP:  sort($arr);
来源：http://ou.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vm.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tm.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jy.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ey.bjjhwx.cn

Ruby: arr.sort
来源：http://nl.shxzskj.cn

C#:   list.Sort();
来源：http://qb.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sz.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nn.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vz.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wb.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iw.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cq.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lp.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zq.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://la.yuexingan06.cn

[D11] 反转数组
来源：http://nu.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mx.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://bo.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yu.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://lx.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://tj.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://zy.muxihuayi.cn

Ruby: arr.reverse
来源：http://rq.huixiangedu.cn

C#:   list.Reverse();
来源：http://wh.jctech888.com.cn

[D12] 查找元素下标
来源：http://nv.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://uo.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ez.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ic.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zl.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ta.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://de.shxzukj.cn

Ruby: arr.index(x)
来源：http://up.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ge.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://vc.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sw.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fw.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://yp.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://fs.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uy.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pf.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qn.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gn.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://si.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eo.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tf.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://he.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://xt.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zu.nszjky.cn

Go:   // 手写循环
来源：http://ej.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bo.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jt.jianghongdianzi.cn

[D15] 去重
来源：http://bc.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hd.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://gp.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://ti.nszjky.cn

TS:   [...new Set(arr)]
来源：http://fc.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://td.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hn.asd995.cn

Ruby: arr.uniq
来源：http://jd.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://tp.yuexingan06.cn

[D16] 求和与平均值
来源：http://pf.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lh.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lu.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bu.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pp.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ag.hnjuh.cn

Go:   // 手写循环累加
来源：http://ka.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jg.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ty.wgjwhj.cn

[D17] 最大值与最小值
来源：http://nx.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://dd.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://zv.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uy.szxytkj.cn

TS:   Math.max(...arr);
来源：http://he.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kj.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gv.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://ew.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://zq.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://jg.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://co.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://ww.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gp.gzmigu.cn

TS:   nested.flat();
来源：http://bm.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://he.yuexingan06.cn

Go:   // 手写双层循环
来源：http://qr.gzmigu.cn

Ruby: nested.flatten
来源：http://jj.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wc.colortex.cn

[D19] 按字段分组
来源：http://yr.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vs.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ci.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zs.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uz.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tu.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://sp.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pe.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hr.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://do.yuexingan06.cn

Py:   Counter(arr)
来源：http://cu.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://zj.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://df.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qh.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xx.hahajie.cn

Go:   // 手写 map[T]int
来源：http://gx.muxihuayi.cn

Ruby: arr.tally
来源：http://gb.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nj.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://lq.asd995.cn

Py:   x in arr
来源：http://fd.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://ik.panjiajie.cn

JS:   arr.includes(x)
来源：http://bx.muxihuayi.cn

TS:   arr.includes(x)
来源：http://ty.haigaiapp.cn

Java: list.contains(x)
来源：http://zq.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://av.huanxung.cn

Ruby: arr.include?(x)
来源：http://li.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://os.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://xn.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ok.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://df.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xt.lnxyls.cn

TS:   [...arr];
来源：http://he.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://ay.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qx.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ii.hnjuh.cn

C#:   new List<int>(list);
来源：http://jb.9csxet.cn

[D23] reduce 累积计算
来源：http://ek.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nj.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hc.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://df.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rc.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zf.yuexingan06.cn

Go:   // 手写循环
来源：http://tt.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ji.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://af.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://fc.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zo.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://za.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tj.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jf.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jq.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ak.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://da.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ws.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://sk.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pa.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bs.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://li.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rg.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ub.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tx.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ro.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://af.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://jx.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://oo.colortex.cn

PHP:  implode(", ", $arr);
来源：http://at.haigaiapp.cn

JS:   arr.join(", ")
来源：http://xx.chemitech.net.cn

TS:   arr.join(", ")
来源：http://jk.haigaiapp.cn

Java: String.join(", ", list)
来源：http://pe.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://vq.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://fz.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://ys.huixiangedu.cn

================================================================================
来源：http://aq.szxytkj.cn

E. 字符串处理
来源：http://hp.huixiangedu.cn

================================================================================
来源：http://ac.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://oj.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ya.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ns.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fn.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yu.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://es.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vf.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xd.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ey.yuntaijiaju.cn

[E02] 重复字符串
来源：http://gv.asd995.cn

Py:   "ab" * 3
来源：http://sm.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://hd.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://st.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://pc.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://sw.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://mo.9csxet.cn

Ruby: "ab" * 3
来源：http://sl.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qf.szxytkj.cn

[E03] 截取子串
来源：http://fs.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ul.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fg.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ku.nszjky.cn

TS:   s.slice(1, 4)
来源：http://fx.gzmigu.cn

Java: s.substring(1, 4)
来源：http://ir.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ya.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xk.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://nj.colortex.cn

[E04] 查找子串位置
来源：http://lz.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://xm.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://fd.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nm.shxzskj.cn

TS:   s.indexOf("x")
来源：http://aa.szsharing.cn

Java: s.indexOf("x")
来源：http://ft.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://lr.muxihuayi.cn

Ruby: s.index("x")
来源：http://ac.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://ga.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://to.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ml.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wl.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qw.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wq.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xk.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://su.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ad.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://na.szxytkj.cn

[E06] 替换子串
来源：http://kq.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zs.bjjhwx.cn

PHP:  str_replace("a", "b", $s);
来源：http://mf.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tm.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://ek.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ik.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vn.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lh.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://bx.huanxung.cn

[E07] 按分隔符拆分
来源：http://vy.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oq.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ne.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ge.panjiajie.cn

TS:   s.split(",")
来源：http://ok.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yo.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fv.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://ut.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jw.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://mt.szsharing.cn

Py:   ",".join(items)
来源：http://mp.hnjuh.cn

PHP:  implode(",", $items);
来源：http://yb.yuexingan06.cn

JS:   items.join(",")
来源：http://mo.yuntaijiaju.cn

TS:   items.join(",")
来源：http://fp.hahajie.cn

Java: String.join(",", items)
来源：http://ke.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://yq.asd995.cn

Ruby: items.join(",")
来源：http://pp.szxytkj.cn

C#:   string.Join(",", items)
来源：http://wo.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://cc.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cz.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cd.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://ed.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://bq.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://st.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sk.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://il.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ks.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://sq.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fe.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ef.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://sv.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://gq.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://zu.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bg.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://by.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gs.9csxet.cn

[E11] 反转字符串
来源：http://mr.bjjhwx.cn

Py:   s[::-1]
来源：http://we.haigaiapp.cn

PHP:  strrev($s);
来源：http://jp.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://gq.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://su.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jh.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rs.colortex.cn

Ruby: s.reverse
来源：http://wj.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vx.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://ud.nicolike.cn

Py:   s.count("a")
来源：http://tp.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://pa.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://om.colortex.cn

TS:   s.split("a").length - 1
来源：http://qo.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mo.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://dj.521024.cn

Ruby: s.count("a")
来源：http://gs.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://nd.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://in.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://jf.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bu.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ru.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tk.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ii.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qk.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xy.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://us.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://yj.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hh.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uc.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wo.yuexingan06.cn


<!-- 参考信息 -->