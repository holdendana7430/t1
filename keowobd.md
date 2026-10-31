代发 wailian999

TS:   arr.slice(1, 4);
来源：http://aq.hahajie.cn

Java: list.subList(1, 4);
来源：http://sd.wgjwhj.cn

Go:   arr[1:4]
来源：http://ct.gzmigu.cn

Ruby: arr[1, 3]
来源：http://zj.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://wg.yuexingan06.cn

[D08] 合并两个数组
来源：http://pq.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://dz.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://za.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xe.nszjky.cn

TS:   [...a, ...b];
来源：http://fg.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xx.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://vu.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://fw.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://rg.shxzskj.cn

[D09] 排序（升序）
来源：http://il.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.yuexingan06.cn

PHP:  sort($arr);
来源：http://bt.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ha.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nb.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://og.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cz.9csxet.cn

Ruby: arr.sort
来源：http://qj.shxzukj.cn

C#:   list.Sort();
来源：http://pu.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ek.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dx.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wh.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rm.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ek.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ta.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://te.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pf.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ua.yuexingan06.cn

[D11] 反转数组
来源：http://zc.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iq.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://gw.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zv.nicolike.cn

TS:   [...arr].reverse();
来源：http://vn.newstarts.cn

Java: Collections.reverse(list);
来源：http://vk.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://fj.9csxet.cn

Ruby: arr.reverse
来源：http://hu.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://zr.nszjky.cn

[D12] 查找元素下标
来源：http://uv.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://kb.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gq.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ue.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tz.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://th.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://xo.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://sk.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://gq.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ey.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vy.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bk.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://fr.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://zi.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yl.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yq.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pe.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vl.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://mf.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yo.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iv.521024.cn

JS:   arr.map(x => x * 2)
来源：http://db.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://qy.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hv.bookmarksfly.cn

Go:   // 手写循环
来源：http://mz.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gf.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ph.jianghongdianzi.cn

[D15] 去重
来源：http://de.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fw.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://ul.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://jt.gzmigu.cn

TS:   [...new Set(arr)]
来源：http://eq.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gr.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lx.wgjwhj.cn

Ruby: arr.uniq
来源：http://cj.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://gh.nicolike.cn

[D16] 求和与平均值
来源：http://am.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ro.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zg.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tw.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fv.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://og.nicolike.cn

Go:   // 手写循环累加
来源：http://mz.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cl.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://kt.muxihuayi.cn

[D17] 最大值与最小值
来源：http://gm.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://me.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://vi.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ee.hnjuh.cn

TS:   Math.max(...arr);
来源：http://nh.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bu.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bs.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://zj.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://wz.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://zn.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uq.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://do.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nj.yuntaijiaju.cn

TS:   nested.flat();
来源：http://eb.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ne.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://sc.colortex.cn

Ruby: nested.flatten
来源：http://bu.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rw.huanxung.cn

[D19] 按字段分组
来源：http://lx.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mb.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zb.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ez.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gb.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jj.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://io.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rx.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eo.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://lw.szsharing.cn

Py:   Counter(arr)
来源：http://ld.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://qc.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://my.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mo.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wv.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://nn.nszjky.cn

Ruby: arr.tally
来源：http://xv.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qh.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://pb.newstarts.cn

Py:   x in arr
来源：http://wy.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://ox.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://ir.jctech888.com.cn

TS:   arr.includes(x)
来源：http://gy.huanxung.cn

Java: list.contains(x)
来源：http://ts.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://sj.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://db.szxytkj.cn

C#:   list.Contains(x)
来源：http://gh.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://dv.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://np.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yp.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eu.jianghongdianzi.cn

TS:   [...arr];
来源：http://ae.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://eh.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://co.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://ay.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ze.hnjuh.cn

[D23] reduce 累积计算
来源：http://xi.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kv.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://up.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://um.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ix.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bg.jctech888.com.cn

Go:   // 手写循环
来源：http://vk.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mw.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qq.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://wx.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sk.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fq.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rs.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ao.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kl.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qg.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tn.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jx.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://bf.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rj.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bu.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kl.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lk.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zv.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jv.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vd.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qz.bookmarksfly.cn

[D26] 数组转字符串
来源：http://kg.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://xq.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://pu.szxytkj.cn

JS:   arr.join(", ")
来源：http://bj.521024.cn

TS:   arr.join(", ")
来源：http://gm.shxzskj.cn

Java: String.join(", ", list)
来源：http://ay.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://yy.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://nn.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://aq.shxzukj.cn

================================================================================
来源：http://cn.lnxyls.cn

E. 字符串处理
来源：http://pj.jctech888.com.cn

================================================================================
来源：http://cr.yuexingan06.cn

[E01] 拼接字符串
来源：http://vq.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rm.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cd.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dn.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vq.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://js.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lx.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zr.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lq.wgjwhj.cn

[E02] 重复字符串
来源：http://vo.chemitech.net.cn

Py:   "ab" * 3
来源：http://pp.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://lh.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://vr.newstarts.cn

TS:   "ab".repeat(3)
来源：http://dz.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://ix.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://kp.huanxung.cn

Ruby: "ab" * 3
来源：http://hc.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ur.shxzukj.cn

[E03] 截取子串
来源：http://bg.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ff.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ih.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gu.huanxung.cn

TS:   s.slice(1, 4)
来源：http://jb.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://to.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ty.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wg.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://zz.newstarts.cn

[E04] 查找子串位置
来源：http://qy.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://lu.hahajie.cn

PHP:  strpos($s, "x");
来源：http://oq.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wq.lnxyls.cn

TS:   s.indexOf("x")
来源：http://zr.wgjwhj.cn

Java: s.indexOf("x")
来源：http://qb.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://xr.newstarts.cn

Ruby: s.index("x")
来源：http://gb.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://do.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pt.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lx.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pu.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lj.shxzskj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://un.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mv.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cp.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ea.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qa.hahajie.cn

[E06] 替换子串
来源：http://kr.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ao.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://lg.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ab.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://aj.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gz.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://za.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sj.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://rd.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://sx.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ba.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rm.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://es.shtwfgs.cn

TS:   s.split(",")
来源：http://qd.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ru.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ql.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://tt.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sl.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://ni.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://cw.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://cq.huanxung.cn

JS:   items.join(",")
来源：http://sn.szxytkj.cn

TS:   items.join(",")
来源：http://ru.shxzskj.cn

Java: String.join(",", items)
来源：http://rk.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://bi.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://yc.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://oe.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://ke.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dk.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lv.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://kw.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://zf.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://zt.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oa.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bc.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gx.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://rl.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fr.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yv.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://ac.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://di.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://xl.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mn.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lm.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gr.bookmarksfly.cn

[E11] 反转字符串
来源：http://xi.szxytkj.cn

Py:   s[::-1]
来源：http://wn.nicolike.cn

PHP:  strrev($s);
来源：http://kc.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://yw.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://en.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dh.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gr.shxzukj.cn

Ruby: s.reverse
来源：http://lx.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zz.521024.cn

[E12] 统计某字符出现次数
来源：http://qf.szsharing.cn

Py:   s.count("a")
来源：http://sg.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://ja.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://ry.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ry.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kh.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://ht.wgjwhj.cn

Ruby: s.count("a")
来源：http://xg.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://ko.nszjky.cn

[E13] 逐字符遍历
来源：http://ug.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://ts.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yi.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xr.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tz.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qn.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sr.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hk.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ed.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://ac.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xn.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dl.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://df.bookmarksfly.cn


<!-- 参考信息 -->