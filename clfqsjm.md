代发 wailian999

[D07] 切片 / 取子数组
来源：http://om.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://td.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ry.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://wh.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://kr.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://ad.9csxet.cn

Go:   arr[1:4]
来源：http://oi.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://sr.521024.cn

C#:   list.GetRange(1, 3);
来源：http://ml.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://fx.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://sn.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://kx.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tp.hahajie.cn

TS:   [...a, ...b];
来源：http://tw.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://le.yuexingan06.cn

Go:   append(a, b...)
来源：http://jo.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://py.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://il.asd995.cn

[D09] 排序（升序）
来源：http://qj.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://ix.jctech888.com.cn

PHP:  sort($arr);
来源：http://sd.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://za.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ws.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wg.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kg.521024.cn

Ruby: arr.sort
来源：http://tz.lnxyls.cn

C#:   list.Sort();
来源：http://fw.jianghongdianzi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kj.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cu.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ge.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kv.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ay.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ug.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tq.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vr.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ve.jctech888.com.cn

[D11] 反转数组
来源：http://gt.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tm.hahajie.cn

PHP:  array_reverse($arr);
来源：http://ta.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wk.szsharing.cn

TS:   [...arr].reverse();
来源：http://da.colortex.cn

Java: Collections.reverse(list);
来源：http://zv.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://st.huixiangedu.cn

Ruby: arr.reverse
来源：http://lh.bookmarksfly.cn

C#:   list.Reverse();
来源：http://cr.chemitech.net.cn

[D12] 查找元素下标
来源：http://nw.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://yv.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nv.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hd.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wf.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zm.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://iy.asd995.cn

Ruby: arr.index(x)
来源：http://xj.asd995.cn

C#:   list.IndexOf(x);
来源：http://ns.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://sm.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://al.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iv.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://nw.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://gu.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ky.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nc.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wn.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lw.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://wd.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pu.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://es.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://my.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://fd.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://it.bjjhwx.cn

Go:   // 手写循环
来源：http://it.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ru.szsharing.cn

[D15] 去重
来源：http://zk.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://li.huanxung.cn

PHP:  array_unique($arr);
来源：http://qf.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://yt.hahajie.cn

TS:   [...new Set(arr)]
来源：http://nd.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kr.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cn.newstarts.cn

Ruby: arr.uniq
来源：http://zd.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://mk.chemitech.net.cn

[D16] 求和与平均值
来源：http://wv.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://py.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hv.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fy.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xx.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lm.shxzukj.cn

Go:   // 手写循环累加
来源：http://wc.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xh.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://ry.nicolike.cn

[D17] 最大值与最小值
来源：http://hy.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://if.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://bi.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oz.shxzukj.cn

TS:   Math.max(...arr);
来源：http://tp.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hg.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://up.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://bh.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://yt.colortex.cn

[D18] 扁平化嵌套数组
来源：http://kc.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vu.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://en.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oe.hnjuh.cn

TS:   nested.flat();
来源：http://vl.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bl.wgjwhj.cn

Go:   // 手写双层循环
来源：http://pl.haigaiapp.cn

Ruby: nested.flatten
来源：http://pq.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lv.hnjuh.cn

[D19] 按字段分组
来源：http://sj.shxzukj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ub.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fv.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ry.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oo.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ow.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://um.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tv.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jy.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://pc.szxytkj.cn

Py:   Counter(arr)
来源：http://my.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://jg.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gl.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qm.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://bj.huixiangedu.cn

Ruby: arr.tally
来源：http://wq.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yp.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://jt.jctech888.com.cn

Py:   x in arr
来源：http://qx.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://aq.bjjhwx.cn

JS:   arr.includes(x)
来源：http://yt.yuexingan06.cn

TS:   arr.includes(x)
来源：http://my.lnxyls.cn

Java: list.contains(x)
来源：http://tp.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://cu.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://xj.bjjhwx.cn

C#:   list.Contains(x)
来源：http://ll.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://ir.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lq.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ex.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://my.szxytkj.cn

TS:   [...arr];
来源：http://xz.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://zs.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kk.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://st.521024.cn

C#:   new List<int>(list);
来源：http://tq.muxihuayi.cn

[D23] reduce 累积计算
来源：http://en.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nc.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://js.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hr.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dp.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vw.yuntaijiaju.cn

Go:   // 手写循环
来源：http://iv.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fo.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xo.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://nf.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uc.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ye.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nr.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://il.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fi.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gq.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gx.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://le.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://cw.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://se.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://li.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ib.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gp.bjjhwx.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ez.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ff.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pt.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yq.muxihuayi.cn

[D26] 数组转字符串
来源：http://xq.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://cs.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://ap.muxihuayi.cn

JS:   arr.join(", ")
来源：http://oc.shxzskj.cn

TS:   arr.join(", ")
来源：http://ga.asd995.cn

Java: String.join(", ", list)
来源：http://xl.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://kl.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://yw.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://tq.huanxung.cn

================================================================================
来源：http://fs.jctech888.com.cn

E. 字符串处理
来源：http://pn.gzmigu.cn

================================================================================
来源：http://eo.wgjwhj.cn

[E01] 拼接字符串
来源：http://zf.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bg.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pe.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://er.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ga.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hy.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oc.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cx.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mp.shxzukj.cn

[E02] 重复字符串
来源：http://jt.jctech888.com.cn

Py:   "ab" * 3
来源：http://yc.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://mo.szsharing.cn

JS:   "ab".repeat(3)
来源：http://ew.hahajie.cn

TS:   "ab".repeat(3)
来源：http://mt.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://ee.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://hx.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://yt.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dd.huanxung.cn

[E03] 截取子串
来源：http://xn.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yu.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://id.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pu.szsharing.cn

TS:   s.slice(1, 4)
来源：http://jr.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://ks.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://md.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sb.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://op.muxihuayi.cn

[E04] 查找子串位置
来源：http://zo.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ke.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://du.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jj.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://az.yuexingan06.cn

Java: s.indexOf("x")
来源：http://nx.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://jw.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://dk.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://bc.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jq.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rb.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ta.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gf.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vm.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bd.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sg.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qq.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aa.lnxyls.cn

[E06] 替换子串
来源：http://ip.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zm.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://en.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nx.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://ri.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uw.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lx.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aq.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://pv.asd995.cn

[E07] 按分隔符拆分
来源：http://jh.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ql.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pz.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ai.huanxung.cn

TS:   s.split(",")
来源：http://yq.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zl.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bu.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://xo.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sr.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://lt.colortex.cn

Py:   ",".join(items)
来源：http://ln.szsharing.cn

PHP:  implode(",", $items);
来源：http://yd.szxytkj.cn

JS:   items.join(",")
来源：http://gh.nicolike.cn

TS:   items.join(",")
来源：http://df.huixiangedu.cn

Java: String.join(",", items)
来源：http://ds.asd995.cn

Go:   strings.Join(items, ",")
来源：http://wf.panjiajie.cn

Ruby: items.join(",")
来源：http://xl.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://ti.hahajie.cn

[E09] 去除所有空白字符
来源：http://nc.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fp.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yg.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://lw.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://fi.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://cp.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mq.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cc.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jq.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://in.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vd.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tl.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://ip.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://yp.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://xr.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vy.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fl.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mo.hnjuh.cn

[E11] 反转字符串
来源：http://hh.nszjky.cn

Py:   s[::-1]
来源：http://gu.lnxyls.cn

PHP:  strrev($s);
来源：http://cg.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://sg.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://or.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://os.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zn.nicolike.cn

Ruby: s.reverse
来源：http://al.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qb.huanxung.cn

[E12] 统计某字符出现次数
来源：http://kz.yuexingan06.cn

Py:   s.count("a")
来源：http://mz.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://dr.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://lo.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://eo.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gg.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://wh.shxzukj.cn

Ruby: s.count("a")
来源：http://nn.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://bl.gzmigu.cn

[E13] 逐字符遍历
来源：http://cx.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://vi.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nb.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nr.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fs.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://va.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wu.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lt.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://px.szxytkj.cn


<!-- 参考信息 -->