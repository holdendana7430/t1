代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://dr.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://oj.shxzskj.cn

[D09] 排序（升序）
来源：http://ie.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://az.9csxet.cn

PHP:  sort($arr);
来源：http://xa.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://py.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hb.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://st.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jf.yuexingan06.cn

Ruby: arr.sort
来源：http://qc.asd995.cn

C#:   list.Sort();
来源：http://hn.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://df.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sh.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ru.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ia.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dg.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gp.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lj.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://en.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sb.gzmigu.cn

[D11] 反转数组
来源：http://pf.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yo.asd995.cn

PHP:  array_reverse($arr);
来源：http://el.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mx.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://eo.shxzukj.cn

Java: Collections.reverse(list);
来源：http://wy.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://by.haigaiapp.cn

Ruby: arr.reverse
来源：http://pz.9csxet.cn

C#:   list.Reverse();
来源：http://ih.9csxet.cn

[D12] 查找元素下标
来源：http://dl.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ap.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bs.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ll.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jk.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fy.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://cq.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ff.nszjky.cn

C#:   list.IndexOf(x);
来源：http://lj.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ej.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cw.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sw.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://xq.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://pi.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bl.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xz.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ti.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://of.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://fc.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mr.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://td.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://fj.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://fh.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xu.yuexingan06.cn

Go:   // 手写循环
来源：http://pf.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cb.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://za.hnjuh.cn

[D15] 去重
来源：http://ys.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cs.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://fz.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ht.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://ig.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zk.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dr.asd995.cn

Ruby: arr.uniq
来源：http://mo.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://xn.newstarts.cn

[D16] 求和与平均值
来源：http://gj.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ne.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nc.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jm.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gd.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://og.huanxung.cn

Go:   // 手写循环累加
来源：http://ua.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://le.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://tu.jctech888.com.cn

[D17] 最大值与最小值
来源：http://sy.asd995.cn

Py:   max(arr);  min(arr)
来源：http://pl.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://fm.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uy.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://hr.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yq.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://en.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://fg.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://yp.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://bz.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aq.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://wp.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xt.lnxyls.cn

TS:   nested.flat();
来源：http://ru.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dd.nicolike.cn

Go:   // 手写双层循环
来源：http://cx.colortex.cn

Ruby: nested.flatten
来源：http://bn.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kr.bjjhwx.cn

[D19] 按字段分组
来源：http://ro.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tw.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ig.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vf.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://re.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wl.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ff.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xw.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tk.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://tz.bjjhwx.cn

Py:   Counter(arr)
来源：http://ag.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://qw.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ld.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rp.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://le.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://xy.shxzukj.cn

Ruby: arr.tally
来源：http://qp.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://no.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://cd.szxytkj.cn

Py:   x in arr
来源：http://ij.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://el.hahajie.cn

JS:   arr.includes(x)
来源：http://ax.colortex.cn

TS:   arr.includes(x)
来源：http://em.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ot.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://gh.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://yx.shxzskj.cn

C#:   list.Contains(x)
来源：http://ch.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://at.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ob.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://my.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cd.lnxyls.cn

TS:   [...arr];
来源：http://sa.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://mn.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cz.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://uq.huixiangedu.cn

C#:   new List<int>(list);
来源：http://sq.huixiangedu.cn

[D23] reduce 累积计算
来源：http://pz.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vj.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sm.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cv.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wg.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xg.lnxyls.cn

Go:   // 手写循环
来源：http://cz.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cj.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pe.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://ln.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zg.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fu.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lp.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://le.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://po.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://au.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ii.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ny.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://kq.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tl.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wf.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sy.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jf.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://av.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sz.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cx.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sy.asd995.cn

[D26] 数组转字符串
来源：http://tm.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://ds.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://be.yuexingan06.cn

JS:   arr.join(", ")
来源：http://gi.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://xm.shxzskj.cn

Java: String.join(", ", list)
来源：http://oa.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://tn.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://ih.hahajie.cn

C#:   string.Join(", ", list)
来源：http://el.hahajie.cn

================================================================================
来源：http://qh.colortex.cn

E. 字符串处理
来源：http://lz.yuexingan06.cn

================================================================================
来源：http://ir.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://hf.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hu.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wp.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://du.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ag.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kq.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ks.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ar.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uh.chemitech.net.cn

[E02] 重复字符串
来源：http://yh.bookmarksfly.cn

Py:   "ab" * 3
来源：http://pi.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://ie.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://qw.huanxung.cn

TS:   "ab".repeat(3)
来源：http://dh.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://nl.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ac.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://xr.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lf.gzmigu.cn

[E03] 截取子串
来源：http://ol.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xx.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kq.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pl.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://st.panjiajie.cn

Java: s.substring(1, 4)
来源：http://av.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eb.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://so.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://pw.shxzukj.cn

[E04] 查找子串位置
来源：http://ym.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://to.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://aj.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jz.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://ej.9csxet.cn

Java: s.indexOf("x")
来源：http://xw.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://co.szxytkj.cn

Ruby: s.index("x")
来源：http://lk.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://ww.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ok.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uo.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sy.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ah.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cj.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kc.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sq.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cs.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://io.9csxet.cn

[E06] 替换子串
来源：http://gc.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xp.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://uq.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jd.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://kx.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gx.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tf.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://am.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://np.szxytkj.cn

[E07] 按分隔符拆分
来源：http://wj.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ax.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://la.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://px.521024.cn

TS:   s.split(",")
来源：http://xz.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tg.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rh.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://bv.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ay.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://hm.szxytkj.cn

Py:   ",".join(items)
来源：http://ec.gzmigu.cn

PHP:  implode(",", $items);
来源：http://tb.huanxung.cn

JS:   items.join(",")
来源：http://fi.nszjky.cn

TS:   items.join(",")
来源：http://xu.huixiangedu.cn

Java: String.join(",", items)
来源：http://sk.colortex.cn

Go:   strings.Join(items, ",")
来源：http://xe.panjiajie.cn

Ruby: items.join(",")
来源：http://ek.gzmigu.cn

C#:   string.Join(",", items)
来源：http://ml.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://nu.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bh.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ds.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://nz.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://gv.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://qm.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tg.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wd.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yu.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://fm.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wz.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tz.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://gi.521024.cn

TS:   "7".padStart(3, "0")
来源：http://uw.szsharing.cn

Java: String.format("%03d", 7)
来源：http://pf.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hk.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pu.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://la.szsharing.cn

[E11] 反转字符串
来源：http://uy.yuntaijiaju.cn

Py:   s[::-1]
来源：http://se.huanxung.cn

PHP:  strrev($s);
来源：http://ud.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://sx.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://bc.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dg.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hf.huixiangedu.cn

Ruby: s.reverse
来源：http://ia.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vp.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://bx.shxzukj.cn

Py:   s.count("a")
来源：http://gr.colortex.cn

PHP:  substr_count($s, "a");
来源：http://nu.huanxung.cn

JS:   s.split("a").length - 1
来源：http://tr.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://xw.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xf.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://zj.newstarts.cn

Ruby: s.count("a")
来源：http://tl.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://xq.9csxet.cn

[E13] 逐字符遍历
来源：http://es.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://gw.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ht.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yx.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://at.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://he.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mv.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gl.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qu.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://mk.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qz.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mh.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vx.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rt.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zz.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://th.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bm.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sc.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://mj.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tj.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ie.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pa.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wi.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iy.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sv.shxzukj.cn


<!-- 参考信息 -->