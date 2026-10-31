代发 wailian999

Py:   len(arr)
来源：http://cg.yuntaijiaju.cn

PHP:  count($arr);
来源：http://go.muxihuayi.cn

JS:   arr.length
来源：http://eb.haigaiapp.cn

TS:   arr.length
来源：http://zl.521024.cn

Java: list.size();
来源：http://ay.colortex.cn

Go:   len(arr)
来源：http://pi.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://ic.9csxet.cn

C#:   list.Count;
来源：http://bq.colortex.cn

[D07] 切片 / 取子数组
来源：http://zd.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dq.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ui.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://cn.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://qh.huanxung.cn

Java: list.subList(1, 4);
来源：http://wu.huanxung.cn

Go:   arr[1:4]
来源：http://pv.huanxung.cn

Ruby: arr[1, 3]
来源：http://fx.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://sr.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://dq.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://aw.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://dd.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hy.yuexingan06.cn

TS:   [...a, ...b];
来源：http://cx.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vw.huixiangedu.cn

Go:   append(a, b...)
来源：http://rh.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://fa.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ct.hnjuh.cn

[D09] 排序（升序）
来源：http://lq.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://od.szsharing.cn

PHP:  sort($arr);
来源：http://qe.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qm.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qo.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tg.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ut.wgjwhj.cn

Ruby: arr.sort
来源：http://ep.jctech888.com.cn

C#:   list.Sort();
来源：http://za.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ka.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ad.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fu.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qc.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ml.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kn.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://im.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ka.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://an.muxihuayi.cn

[D11] 反转数组
来源：http://vk.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ym.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://jo.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bs.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://bf.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ao.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://yd.hnjuh.cn

Ruby: arr.reverse
来源：http://ws.newstarts.cn

C#:   list.Reverse();
来源：http://ct.yuexingan06.cn

[D12] 查找元素下标
来源：http://at.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://us.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qu.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pk.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://df.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yl.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://ad.chemitech.net.cn

Ruby: arr.index(x)
来源：http://st.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://lz.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://bh.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gg.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cl.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://xy.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ra.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://li.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qu.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nf.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uq.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://gy.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ya.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://zk.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://wl.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fg.nicolike.cn

Go:   // 手写循环
来源：http://ti.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ic.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qk.gzmigu.cn

[D15] 去重
来源：http://sp.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fr.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ei.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://ea.nicolike.cn

TS:   [...new Set(arr)]
来源：http://id.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fd.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ev.9csxet.cn

Ruby: arr.uniq
来源：http://sd.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://yk.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://tv.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ql.9csxet.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gx.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cg.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pi.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://al.521024.cn

Go:   // 手写循环累加
来源：http://cw.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yf.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://mo.colortex.cn

[D17] 最大值与最小值
来源：http://ie.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://ej.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://ec.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hf.9csxet.cn

TS:   Math.max(...arr);
来源：http://rf.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hx.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://us.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://xr.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://he.asd995.cn

[D18] 扁平化嵌套数组
来源：http://tq.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eu.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ou.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://py.shxzukj.cn

TS:   nested.flat();
来源：http://oi.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://og.colortex.cn

Go:   // 手写双层循环
来源：http://wq.muxihuayi.cn

Ruby: nested.flatten
来源：http://gn.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pm.huixiangedu.cn

[D19] 按字段分组
来源：http://vk.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hc.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rq.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ln.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yn.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zp.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://rp.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tw.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gj.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://dc.szxytkj.cn

Py:   Counter(arr)
来源：http://we.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://ps.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ml.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fc.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pv.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://go.muxihuayi.cn

Ruby: arr.tally
来源：http://yl.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nq.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://yy.muxihuayi.cn

Py:   x in arr
来源：http://gy.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://kc.huanxung.cn

JS:   arr.includes(x)
来源：http://cl.9csxet.cn

TS:   arr.includes(x)
来源：http://ui.jctech888.com.cn

Java: list.contains(x)
来源：http://rp.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://qp.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://gx.colortex.cn

C#:   list.Contains(x)
来源：http://gx.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://rt.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://in.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://si.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://po.hnjuh.cn

TS:   [...arr];
来源：http://sd.huanxung.cn

Java: new ArrayList<>(list);
来源：http://nd.bjjhwx.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mt.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://ef.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://qc.shxzukj.cn

[D23] reduce 累积计算
来源：http://ix.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tw.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://db.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wt.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ce.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cw.panjiajie.cn

Go:   // 手写循环
来源：http://bg.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gw.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fs.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://ox.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://li.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gj.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zx.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://no.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ln.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xr.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bh.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ku.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://yo.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://me.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wa.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gb.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pi.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cu.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cs.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://re.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yd.newstarts.cn

[D26] 数组转字符串
来源：http://wi.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://qr.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://zm.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://vt.shxzskj.cn

TS:   arr.join(", ")
来源：http://ef.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://li.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://jc.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://fo.nicolike.cn

C#:   string.Join(", ", list)
来源：http://se.hahajie.cn

================================================================================
来源：http://lm.chemitech.net.cn

E. 字符串处理
来源：http://gf.panjiajie.cn

================================================================================
来源：http://hf.shxzskj.cn

[E01] 拼接字符串
来源：http://il.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wl.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ja.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xd.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ag.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qo.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yk.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bk.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vg.nszjky.cn

[E02] 重复字符串
来源：http://vi.newstarts.cn

Py:   "ab" * 3
来源：http://zs.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://zv.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://zh.szsharing.cn

TS:   "ab".repeat(3)
来源：http://ci.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://zx.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://ca.haigaiapp.cn

Ruby: "ab" * 3
来源：http://te.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vu.nicolike.cn

[E03] 截取子串
来源：http://he.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xx.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ie.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sa.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://lb.nicolike.cn

Java: s.substring(1, 4)
来源：http://lu.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ql.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qe.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://uw.lnxyls.cn

[E04] 查找子串位置
来源：http://iy.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://hf.nicolike.cn

PHP:  strpos($s, "x");
来源：http://au.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tu.panjiajie.cn

TS:   s.indexOf("x")
来源：http://dl.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ya.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://os.newstarts.cn

Ruby: s.index("x")
来源：http://rd.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ul.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ny.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fc.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vm.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cy.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ll.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zt.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sx.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oo.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ja.haigaiapp.cn

[E06] 替换子串
来源：http://tp.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://db.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://zf.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gx.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://qg.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zo.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zu.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://za.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://mx.9csxet.cn

[E07] 按分隔符拆分
来源：http://cb.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://as.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mt.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uh.bjjhwx.cn

TS:   s.split(",")
来源：http://en.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://np.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ji.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://ry.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hd.colortex.cn

[E08] 数组按分隔符合并
来源：http://oq.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://uf.gzmigu.cn

PHP:  implode(",", $items);
来源：http://sh.newstarts.cn

JS:   items.join(",")
来源：http://wa.muxihuayi.cn

TS:   items.join(",")
来源：http://dh.nszjky.cn

Java: String.join(",", items)
来源：http://en.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://cw.9csxet.cn

Ruby: items.join(",")
来源：http://qg.asd995.cn

C#:   string.Join(",", items)
来源：http://rm.shxzskj.cn

[E09] 去除所有空白字符
来源：http://tl.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://il.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ai.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://jn.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://os.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://eg.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wq.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gf.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ba.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://lz.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hv.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dh.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://bx.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://qd.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://pu.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wx.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sr.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ea.jctech888.com.cn

[E11] 反转字符串
来源：http://vz.shxzskj.cn

Py:   s[::-1]
来源：http://sn.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://zv.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://gt.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://cy.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jt.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://je.szsharing.cn

Ruby: s.reverse
来源：http://la.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ot.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://fo.newstarts.cn

Py:   s.count("a")
来源：http://oa.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://vj.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://lc.521024.cn

TS:   s.split("a").length - 1
来源：http://ln.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ip.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://vb.lnxyls.cn

Ruby: s.count("a")
来源：http://yk.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://ez.huixiangedu.cn

[E13] 逐字符遍历
来源：http://gh.nicolike.cn


<!-- 参考信息 -->