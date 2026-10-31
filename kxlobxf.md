代发 wailian999

TS:   arr.slice(1, 4);
来源：http://yc.hahajie.cn

Java: list.subList(1, 4);
来源：http://ho.bjjhwx.cn

Go:   arr[1:4]
来源：http://hq.colortex.cn

Ruby: arr[1, 3]
来源：http://iv.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://jn.yuexingan06.cn

[D08] 合并两个数组
来源：http://dx.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://jb.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://qh.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xm.lnxyls.cn

TS:   [...a, ...b];
来源：http://nt.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fm.shxzskj.cn

Go:   append(a, b...)
来源：http://wb.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://va.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://yv.wgjwhj.cn

[D09] 排序（升序）
来源：http://fe.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://si.szsharing.cn

PHP:  sort($arr);
来源：http://rp.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jd.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mu.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sx.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ol.colortex.cn

Ruby: arr.sort
来源：http://we.huixiangedu.cn

C#:   list.Sort();
来源：http://ia.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://at.jctech888.com.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qm.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yq.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rd.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tz.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pa.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ks.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qq.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mz.lnxyls.cn

[D11] 反转数组
来源：http://mx.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ec.hahajie.cn

PHP:  array_reverse($arr);
来源：http://be.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qo.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://lh.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://wg.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://va.huanxung.cn

Ruby: arr.reverse
来源：http://rb.colortex.cn

C#:   list.Reverse();
来源：http://nv.nszjky.cn

[D12] 查找元素下标
来源：http://vb.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://go.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rr.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://th.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wz.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://be.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://rs.huixiangedu.cn

Ruby: arr.index(x)
来源：http://nx.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://my.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://rz.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nd.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ba.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://je.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://nh.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hy.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bo.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xx.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ur.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://mg.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ac.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lk.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://cs.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://dx.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qh.lnxyls.cn

Go:   // 手写循环
来源：http://fm.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ae.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tu.newstarts.cn

[D15] 去重
来源：http://ur.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fg.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://jo.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://il.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://mq.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bq.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fc.gzmigu.cn

Ruby: arr.uniq
来源：http://pz.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://zp.hnjuh.cn

[D16] 求和与平均值
来源：http://wu.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yc.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fw.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lx.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lk.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jl.haigaiapp.cn

Go:   // 手写循环累加
来源：http://cs.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sq.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://nd.hnjuh.cn

[D17] 最大值与最小值
来源：http://gt.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://zx.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://dc.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wx.asd995.cn

TS:   Math.max(...arr);
来源：http://lh.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ry.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ex.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://um.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://ab.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://va.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gj.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://os.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tx.yuexingan06.cn

TS:   nested.flat();
来源：http://yy.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mc.gzmigu.cn

Go:   // 手写双层循环
来源：http://ga.gzmigu.cn

Ruby: nested.flatten
来源：http://pt.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hw.shxzukj.cn

[D19] 按字段分组
来源：http://tk.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yu.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cl.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xt.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vh.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qw.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://tx.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tj.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ak.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://jf.shxzskj.cn

Py:   Counter(arr)
来源：http://zw.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://fp.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ct.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qa.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zs.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://yg.gzmigu.cn

Ruby: arr.tally
来源：http://rl.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cj.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://np.yuntaijiaju.cn

Py:   x in arr
来源：http://hd.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://qf.9csxet.cn

JS:   arr.includes(x)
来源：http://aw.hahajie.cn

TS:   arr.includes(x)
来源：http://cm.huanxung.cn

Java: list.contains(x)
来源：http://cv.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://lz.9csxet.cn

Ruby: arr.include?(x)
来源：http://nc.9csxet.cn

C#:   list.Contains(x)
来源：http://tb.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://mv.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nz.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iy.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jh.hahajie.cn

TS:   [...arr];
来源：http://xd.asd995.cn

Java: new ArrayList<>(list);
来源：http://nv.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ed.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://zh.asd995.cn

C#:   new List<int>(list);
来源：http://ln.huixiangedu.cn

[D23] reduce 累积计算
来源：http://lu.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sl.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://il.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nm.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uy.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kd.hahajie.cn

Go:   // 手写循环
来源：http://rx.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wa.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vv.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://rb.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pf.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fw.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zc.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wx.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sc.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ug.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pa.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://te.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://kw.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wb.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zy.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qi.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ia.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dt.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ac.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tk.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tg.jctech888.com.cn

[D26] 数组转字符串
来源：http://ll.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://gf.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://gl.panjiajie.cn

JS:   arr.join(", ")
来源：http://jo.521024.cn

TS:   arr.join(", ")
来源：http://dl.nszjky.cn

Java: String.join(", ", list)
来源：http://ri.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://lr.shxzskj.cn

Ruby: arr.join(", ")
来源：http://uj.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://vg.bookmarksfly.cn

================================================================================
来源：http://dp.huixiangedu.cn

E. 字符串处理
来源：http://uz.nicolike.cn

================================================================================
来源：http://xj.huixiangedu.cn

[E01] 拼接字符串
来源：http://va.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tc.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jp.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ip.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://me.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gw.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mx.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dj.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gt.hahajie.cn

[E02] 重复字符串
来源：http://ag.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://zm.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://ba.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://vg.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://io.szsharing.cn

Java: "ab".repeat(3)
来源：http://nz.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://ul.wgjwhj.cn

Ruby: "ab" * 3
来源：http://lf.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iz.shxzukj.cn

[E03] 截取子串
来源：http://ij.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kg.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wb.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fp.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://iy.asd995.cn

Java: s.substring(1, 4)
来源：http://mr.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mg.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://va.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://jy.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://gb.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://pp.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://hn.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zo.szxytkj.cn

TS:   s.indexOf("x")
来源：http://wv.nszjky.cn

Java: s.indexOf("x")
来源：http://ui.521024.cn

Go:   strings.Index(s, "x")
来源：http://ok.shxzukj.cn

Ruby: s.index("x")
来源：http://ln.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://za.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vk.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ut.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pn.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://da.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qr.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gz.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wq.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bm.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jz.szxytkj.cn

[E06] 替换子串
来源：http://xd.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hv.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://go.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cb.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://zc.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qu.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zg.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://za.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://in.nszjky.cn

[E07] 按分隔符拆分
来源：http://yu.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yg.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aq.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hm.bjjhwx.cn

TS:   s.split(",")
来源：http://te.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ld.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jo.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://vs.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pw.hahajie.cn

[E08] 数组按分隔符合并
来源：http://eh.bjjhwx.cn

Py:   ",".join(items)
来源：http://ct.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://px.9csxet.cn

JS:   items.join(",")
来源：http://ao.yuntaijiaju.cn

TS:   items.join(",")
来源：http://dd.muxihuayi.cn

Java: String.join(",", items)
来源：http://ug.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://zz.9csxet.cn

Ruby: items.join(",")
来源：http://jf.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://si.521024.cn

[E09] 去除所有空白字符
来源：http://av.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uw.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rp.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://us.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://ko.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://re.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ca.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uv.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ua.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://rc.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dq.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ax.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://nw.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://cq.hahajie.cn

Java: String.format("%03d", 7)
来源：http://sr.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sn.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pp.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vq.yuntaijiaju.cn

[E11] 反转字符串
来源：http://hf.lnxyls.cn

Py:   s[::-1]
来源：http://jp.shxzukj.cn

PHP:  strrev($s);
来源：http://am.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://co.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://ag.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sq.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://am.lnxyls.cn

Ruby: s.reverse
来源：http://fo.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wj.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://ti.newstarts.cn

Py:   s.count("a")
来源：http://dw.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://py.asd995.cn

JS:   s.split("a").length - 1
来源：http://wk.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ly.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cr.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://sq.gzmigu.cn

Ruby: s.count("a")
来源：http://tt.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://zp.panjiajie.cn

[E13] 逐字符遍历
来源：http://he.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://ju.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sw.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zd.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mm.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zc.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mw.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nf.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sj.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://bg.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xe.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mk.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uy.bookmarksfly.cn


<!-- 参考信息 -->