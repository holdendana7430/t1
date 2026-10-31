代发 wailian999

TS:   arr.slice(1, 4);
来源：http://kh.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://sx.chemitech.net.cn

Go:   arr[1:4]
来源：http://cd.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://gt.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://hd.huixiangedu.cn

[D08] 合并两个数组
来源：http://re.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://gk.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://yx.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bj.jctech888.com.cn

TS:   [...a, ...b];
来源：http://cb.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yo.shxzskj.cn

Go:   append(a, b...)
来源：http://ma.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://po.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://hm.colortex.cn

[D09] 排序（升序）
来源：http://nt.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://sf.nicolike.cn

PHP:  sort($arr);
来源：http://fj.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rd.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gc.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rs.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://no.muxihuayi.cn

Ruby: arr.sort
来源：http://mg.9csxet.cn

C#:   list.Sort();
来源：http://qk.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hw.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nh.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cr.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gj.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ag.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jm.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ei.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pb.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vq.colortex.cn

[D11] 反转数组
来源：http://ba.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zz.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://px.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ec.nszjky.cn

TS:   [...arr].reverse();
来源：http://lm.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ib.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://iz.shtwfgs.cn

Ruby: arr.reverse
来源：http://zu.colortex.cn

C#:   list.Reverse();
来源：http://qp.521024.cn

[D12] 查找元素下标
来源：http://kd.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://oj.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nb.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uf.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yv.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jp.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://kz.nicolike.cn

Ruby: arr.index(x)
来源：http://rx.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://du.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://yf.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mo.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kv.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://mo.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://ld.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mu.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vl.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gl.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zs.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://pl.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eg.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nf.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://bm.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://zo.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lx.9csxet.cn

Go:   // 手写循环
来源：http://mj.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hq.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ap.hahajie.cn

[D15] 去重
来源：http://ie.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ep.szxytkj.cn

PHP:  array_unique($arr);
来源：http://qb.nszjky.cn

JS:   [...new Set(arr)]
来源：http://xx.colortex.cn

TS:   [...new Set(arr)]
来源：http://nz.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nr.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bt.jctech888.com.cn

Ruby: arr.uniq
来源：http://xd.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://cp.panjiajie.cn

[D16] 求和与平均值
来源：http://ym.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vw.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://we.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kf.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qj.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xk.521024.cn

Go:   // 手写循环累加
来源：http://vv.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qs.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://aw.hnjuh.cn

[D17] 最大值与最小值
来源：http://xz.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://eo.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://fk.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vu.9csxet.cn

TS:   Math.max(...arr);
来源：http://gh.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fr.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sd.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://mo.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ew.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://nd.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jr.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://yr.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bx.hahajie.cn

TS:   nested.flat();
来源：http://yn.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xb.asd995.cn

Go:   // 手写双层循环
来源：http://gs.lnxyls.cn

Ruby: nested.flatten
来源：http://yl.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xu.szxytkj.cn

[D19] 按字段分组
来源：http://ld.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rx.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jh.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vu.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kp.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://lt.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hb.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dy.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://tf.9csxet.cn

Py:   Counter(arr)
来源：http://zi.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://tx.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ex.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://av.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tj.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://uh.jctech888.com.cn

Ruby: arr.tally
来源：http://nv.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yl.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://xe.nicolike.cn

Py:   x in arr
来源：http://gg.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://af.haigaiapp.cn

JS:   arr.includes(x)
来源：http://qm.colortex.cn

TS:   arr.includes(x)
来源：http://kf.bookmarksfly.cn

Java: list.contains(x)
来源：http://cl.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://mx.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://rz.9csxet.cn

C#:   list.Contains(x)
来源：http://ca.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://gn.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rw.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ls.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tr.huanxung.cn

TS:   [...arr];
来源：http://lw.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://wp.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://or.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://xf.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://fz.nszjky.cn

[D23] reduce 累积计算
来源：http://uk.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mk.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zu.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ms.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fo.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://op.hnjuh.cn

Go:   // 手写循环
来源：http://ay.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zm.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://go.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://ei.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ij.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uj.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wf.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fh.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ul.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lk.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ik.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dm.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://dj.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xy.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jb.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://na.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hx.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://du.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tn.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ug.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qk.huanxung.cn

[D26] 数组转字符串
来源：http://bt.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://pt.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://vp.jctech888.com.cn

JS:   arr.join(", ")
来源：http://lp.shxzukj.cn

TS:   arr.join(", ")
来源：http://pk.shxzukj.cn

Java: String.join(", ", list)
来源：http://gd.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://jl.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://iy.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://xf.jianghongdianzi.cn

================================================================================
来源：http://fi.lnxyls.cn

E. 字符串处理
来源：http://ot.shxzukj.cn

================================================================================
来源：http://qh.yuexingan06.cn

[E01] 拼接字符串
来源：http://px.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rl.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://af.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://id.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ur.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://so.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ln.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tl.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uz.nicolike.cn

[E02] 重复字符串
来源：http://qf.521024.cn

Py:   "ab" * 3
来源：http://ql.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://no.nszjky.cn

JS:   "ab".repeat(3)
来源：http://ir.newstarts.cn

TS:   "ab".repeat(3)
来源：http://fy.newstarts.cn

Java: "ab".repeat(3)
来源：http://nm.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://eq.colortex.cn

Ruby: "ab" * 3
来源：http://jw.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ia.huanxung.cn

[E03] 截取子串
来源：http://ta.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dv.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bm.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vq.nszjky.cn

TS:   s.slice(1, 4)
来源：http://di.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://xz.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://st.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cx.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://nw.lnxyls.cn

[E04] 查找子串位置
来源：http://ji.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://uo.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://tj.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pv.shxzukj.cn

TS:   s.indexOf("x")
来源：http://zp.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://mk.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://qu.newstarts.cn

Ruby: s.index("x")
来源：http://bj.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://mq.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wm.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nh.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tz.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kn.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nd.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yd.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://al.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pw.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://po.shtwfgs.cn

[E06] 替换子串
来源：http://hr.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://af.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://id.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cu.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://io.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dl.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cg.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ir.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://oh.colortex.cn

[E07] 按分隔符拆分
来源：http://vk.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eo.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nr.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gi.nszjky.cn

TS:   s.split(",")
来源：http://ls.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://no.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mo.521024.cn

Ruby: s.split(",");  s.split
来源：http://hm.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ry.colortex.cn

[E08] 数组按分隔符合并
来源：http://mp.shxzskj.cn

Py:   ",".join(items)
来源：http://gx.hnjuh.cn

PHP:  implode(",", $items);
来源：http://zu.chemitech.net.cn

JS:   items.join(",")
来源：http://uq.muxihuayi.cn

TS:   items.join(",")
来源：http://oh.muxihuayi.cn

Java: String.join(",", items)
来源：http://gw.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://fj.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://rp.huanxung.cn

C#:   string.Join(",", items)
来源：http://tl.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://tj.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://js.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lx.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://dz.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://dv.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ol.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mc.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ef.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oi.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://bd.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gl.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lm.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://mo.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://ig.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://rp.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vu.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ph.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wx.huixiangedu.cn

[E11] 反转字符串
来源：http://op.nszjky.cn

Py:   s[::-1]
来源：http://wm.colortex.cn

PHP:  strrev($s);
来源：http://dj.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://wy.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://wu.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zi.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://we.chemitech.net.cn

Ruby: s.reverse
来源：http://tl.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sp.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://ka.bookmarksfly.cn

Py:   s.count("a")
来源：http://kw.521024.cn

PHP:  substr_count($s, "a");
来源：http://dj.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://fm.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://xh.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zo.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://vh.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://ko.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://pd.huanxung.cn

[E13] 逐字符遍历
来源：http://uc.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://ow.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ay.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bs.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ts.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://im.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sd.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ca.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fg.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://na.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ls.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pu.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dg.asd995.cn


<!-- 参考信息 -->