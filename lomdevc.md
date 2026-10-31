代发 wailian999

Py:   len(arr)
来源：http://yb.muxihuayi.cn

PHP:  count($arr);
来源：http://ew.jianghongdianzi.cn

JS:   arr.length
来源：http://hm.szsharing.cn

TS:   arr.length
来源：http://ot.szsharing.cn

Java: list.size();
来源：http://cq.szxytkj.cn

Go:   len(arr)
来源：http://no.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://fw.huixiangedu.cn

C#:   list.Count;
来源：http://ha.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://dl.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zm.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qw.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://zg.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://fn.9csxet.cn

Java: list.subList(1, 4);
来源：http://ej.shxzskj.cn

Go:   arr[1:4]
来源：http://gy.521024.cn

Ruby: arr[1, 3]
来源：http://vi.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://mc.shtwfgs.cn

[D08] 合并两个数组
来源：http://xy.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://zx.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://uj.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hc.bjjhwx.cn

TS:   [...a, ...b];
来源：http://bt.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ca.huixiangedu.cn

Go:   append(a, b...)
来源：http://oa.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://jh.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://qf.chemitech.net.cn

[D09] 排序（升序）
来源：http://hq.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://xx.shtwfgs.cn

PHP:  sort($arr);
来源：http://tj.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wo.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nq.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qf.hnjuh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://an.nszjky.cn

Ruby: arr.sort
来源：http://md.shtwfgs.cn

C#:   list.Sort();
来源：http://oq.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xd.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://os.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ft.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ul.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mz.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pg.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gs.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://by.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fg.nszjky.cn

[D11] 反转数组
来源：http://lm.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kz.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://zg.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xx.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://kb.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://gg.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://yt.muxihuayi.cn

Ruby: arr.reverse
来源：http://bz.9csxet.cn

C#:   list.Reverse();
来源：http://zv.szsharing.cn

[D12] 查找元素下标
来源：http://ei.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://hi.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bx.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nh.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oc.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jb.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://zh.lnxyls.cn

Ruby: arr.index(x)
来源：http://lg.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://ml.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://cx.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://be.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zs.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://qf.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://aa.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bz.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://na.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iy.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gh.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://ce.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rc.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ia.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://sw.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://ak.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aa.huixiangedu.cn

Go:   // 手写循环
来源：http://um.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zi.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bw.szsharing.cn

[D15] 去重
来源：http://wc.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rj.asd995.cn

PHP:  array_unique($arr);
来源：http://zj.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://lb.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ty.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ng.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zg.nszjky.cn

Ruby: arr.uniq
来源：http://za.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://jj.nicolike.cn

[D16] 求和与平均值
来源：http://iv.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vy.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://am.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xx.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xe.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ev.wgjwhj.cn

Go:   // 手写循环累加
来源：http://gy.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jx.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://xp.hahajie.cn

[D17] 最大值与最小值
来源：http://ku.colortex.cn

Py:   max(arr);  min(arr)
来源：http://tb.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://vb.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vn.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://cj.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rd.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ta.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ha.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://wn.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://oo.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qy.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://ql.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uk.asd995.cn

TS:   nested.flat();
来源：http://xb.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://th.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://ht.wgjwhj.cn

Ruby: nested.flatten
来源：http://gj.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bw.chemitech.net.cn

[D19] 按字段分组
来源：http://hp.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://me.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gl.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bm.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dd.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yb.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://ro.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nc.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hl.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://jx.newstarts.cn

Py:   Counter(arr)
来源：http://nh.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://jr.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vy.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xa.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cr.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://vi.huanxung.cn

Ruby: arr.tally
来源：http://mx.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tf.szsharing.cn

[D21] 判断是否包含某元素
来源：http://dd.huanxung.cn

Py:   x in arr
来源：http://he.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://vq.nszjky.cn

JS:   arr.includes(x)
来源：http://hy.szsharing.cn

TS:   arr.includes(x)
来源：http://fb.nicolike.cn

Java: list.contains(x)
来源：http://lw.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://pi.hahajie.cn

Ruby: arr.include?(x)
来源：http://li.9csxet.cn

C#:   list.Contains(x)
来源：http://xp.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://ze.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lc.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aq.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vj.haigaiapp.cn

TS:   [...arr];
来源：http://wc.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://nf.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ti.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://gk.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://un.szsharing.cn

[D23] reduce 累积计算
来源：http://ud.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ek.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rr.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gy.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nw.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dh.szxytkj.cn

Go:   // 手写循环
来源：http://ie.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yk.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ac.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://gt.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://za.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lu.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uz.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gz.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xn.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ho.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bg.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ym.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://cz.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zq.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qm.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nd.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jq.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sj.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dg.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lc.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mf.nszjky.cn

[D26] 数组转字符串
来源：http://zj.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://ck.521024.cn

PHP:  implode(", ", $arr);
来源：http://pg.jctech888.com.cn

JS:   arr.join(", ")
来源：http://xg.huixiangedu.cn

TS:   arr.join(", ")
来源：http://hn.521024.cn

Java: String.join(", ", list)
来源：http://zk.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://cf.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://sm.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://nl.gzmigu.cn

================================================================================
来源：http://sz.gzmigu.cn

E. 字符串处理
来源：http://hx.shxzukj.cn

================================================================================
来源：http://pk.lnxyls.cn

[E01] 拼接字符串
来源：http://ti.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tf.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ug.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bb.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://st.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rr.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://af.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://is.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mu.haigaiapp.cn

[E02] 重复字符串
来源：http://fk.hnjuh.cn

Py:   "ab" * 3
来源：http://uq.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://dp.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://tq.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://rn.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://as.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://xm.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://bh.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ks.haigaiapp.cn

[E03] 截取子串
来源：http://jc.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fv.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cx.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yk.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://hy.nszjky.cn

Java: s.substring(1, 4)
来源：http://iz.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wx.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zl.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://jy.asd995.cn

[E04] 查找子串位置
来源：http://pa.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://wc.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://af.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xo.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://dz.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ru.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://ry.gzmigu.cn

Ruby: s.index("x")
来源：http://wm.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://sc.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://om.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nv.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jj.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rt.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xd.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ui.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yt.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pj.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qc.newstarts.cn

[E06] 替换子串
来源：http://qo.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wp.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://iy.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ot.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://vu.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ux.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eo.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gd.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://do.521024.cn

[E07] 按分隔符拆分
来源：http://ls.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ot.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ce.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lm.yuntaijiaju.cn

TS:   s.split(",")
来源：http://nm.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hj.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gh.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://el.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bq.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://vv.hnjuh.cn

Py:   ",".join(items)
来源：http://yb.szsharing.cn

PHP:  implode(",", $items);
来源：http://xb.szsharing.cn

JS:   items.join(",")
来源：http://jr.huixinmuqiang.cn

TS:   items.join(",")
来源：http://bn.huixiangedu.cn

Java: String.join(",", items)
来源：http://bi.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://ig.shxzukj.cn

Ruby: items.join(",")
来源：http://fv.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://rh.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://lh.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vu.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ao.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://sm.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://en.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://zl.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hm.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zr.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xj.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://aq.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hq.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://es.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://du.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://hy.newstarts.cn

Java: String.format("%03d", 7)
来源：http://fh.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ld.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://an.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://la.lnxyls.cn

[E11] 反转字符串
来源：http://kv.lnxyls.cn

Py:   s[::-1]
来源：http://py.muxihuayi.cn

PHP:  strrev($s);
来源：http://pi.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://xq.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://pz.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ez.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jb.szxytkj.cn

Ruby: s.reverse
来源：http://nw.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yo.hahajie.cn

[E12] 统计某字符出现次数
来源：http://ef.wgjwhj.cn

Py:   s.count("a")
来源：http://zv.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://ew.nicolike.cn

JS:   s.split("a").length - 1
来源：http://rl.521024.cn

TS:   s.split("a").length - 1
来源：http://oz.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bh.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://ut.nszjky.cn

Ruby: s.count("a")
来源：http://ch.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://qc.panjiajie.cn

[E13] 逐字符遍历
来源：http://zn.muxihuayi.cn


<!-- 参考信息 -->