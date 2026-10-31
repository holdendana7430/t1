代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hg.nicolike.cn

TS:   [...a, ...b];
来源：http://ue.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ef.lnxyls.cn

Go:   append(a, b...)
来源：http://vv.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://td.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://jq.jctech888.com.cn

[D09] 排序（升序）
来源：http://nj.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://hz.nszjky.cn

PHP:  sort($arr);
来源：http://ya.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xt.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tm.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oa.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ci.shxzskj.cn

Ruby: arr.sort
来源：http://tn.hnjuh.cn

C#:   list.Sort();
来源：http://nc.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xh.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ux.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ur.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://is.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ch.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wr.bookmarksfly.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ug.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nj.hnjuh.cn

[D11] 反转数组
来源：http://yb.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rl.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://ot.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sh.shxzskj.cn

TS:   [...arr].reverse();
来源：http://pd.nicolike.cn

Java: Collections.reverse(list);
来源：http://cp.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://rm.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://fg.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://zr.asd995.cn

[D12] 查找元素下标
来源：http://tn.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://ie.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://og.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rj.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uj.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://su.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://se.hahajie.cn

Ruby: arr.index(x)
来源：http://if.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ez.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://rd.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jy.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ta.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://ed.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://vs.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://et.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vn.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ae.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ff.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://of.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xw.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zj.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://if.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://gy.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nk.colortex.cn

Go:   // 手写循环
来源：http://rl.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://my.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qq.szxytkj.cn

[D15] 去重
来源：http://vk.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oy.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://pl.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://rx.newstarts.cn

TS:   [...new Set(arr)]
来源：http://be.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ut.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fx.jctech888.com.cn

Ruby: arr.uniq
来源：http://hh.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://sb.newstarts.cn

[D16] 求和与平均值
来源：http://lq.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xi.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://en.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mt.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aj.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cr.asd995.cn

Go:   // 手写循环累加
来源：http://qn.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aa.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://ju.nszjky.cn

[D17] 最大值与最小值
来源：http://dl.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://gp.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://od.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ug.panjiajie.cn

TS:   Math.max(...arr);
来源：http://uv.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ia.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xk.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://rr.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://gf.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://ti.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pm.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://ht.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wa.huixinmuqiang.cn

TS:   nested.flat();
来源：http://jf.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yz.shxzskj.cn

Go:   // 手写双层循环
来源：http://gh.shtwfgs.cn

Ruby: nested.flatten
来源：http://ac.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xc.jctech888.com.cn

[D19] 按字段分组
来源：http://kr.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zz.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bw.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mg.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fm.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kw.521024.cn

Go:   // 手写 map[string][]T
来源：http://kw.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dk.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ld.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://xn.jctech888.com.cn

Py:   Counter(arr)
来源：http://sg.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ho.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wz.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yd.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xs.colortex.cn

Go:   // 手写 map[T]int
来源：http://uq.nicolike.cn

Ruby: arr.tally
来源：http://uk.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gs.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://ds.9csxet.cn

Py:   x in arr
来源：http://uq.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://eb.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://fd.yuexingan06.cn

TS:   arr.includes(x)
来源：http://mi.newstarts.cn

Java: list.contains(x)
来源：http://ws.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://yv.shxzukj.cn

Ruby: arr.include?(x)
来源：http://rd.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://yd.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://fs.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bb.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qq.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nn.yuexingan06.cn

TS:   [...arr];
来源：http://wh.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://jc.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dr.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://zh.gzmigu.cn

C#:   new List<int>(list);
来源：http://ji.hahajie.cn

[D23] reduce 累积计算
来源：http://gy.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lf.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yw.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nv.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://el.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ik.szxytkj.cn

Go:   // 手写循环
来源：http://yy.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://je.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lk.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://it.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dy.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rx.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mt.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bk.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oh.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gl.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nj.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ec.asd995.cn

[D25] Set 集合去重与交并差
来源：http://hp.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zd.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cb.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jq.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://et.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zs.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dk.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mz.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fy.shxzukj.cn

[D26] 数组转字符串
来源：http://rc.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://if.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://jc.yuexingan06.cn

JS:   arr.join(", ")
来源：http://rl.huixiangedu.cn

TS:   arr.join(", ")
来源：http://zd.shxzskj.cn

Java: String.join(", ", list)
来源：http://ju.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://ux.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://db.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://hh.huixiangedu.cn

================================================================================
来源：http://lh.gzmigu.cn

E. 字符串处理
来源：http://ae.muxihuayi.cn

================================================================================
来源：http://tj.9csxet.cn

[E01] 拼接字符串
来源：http://qn.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nq.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ny.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fc.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nv.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qj.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yd.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eg.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hp.hahajie.cn

[E02] 重复字符串
来源：http://cx.huanxung.cn

Py:   "ab" * 3
来源：http://pq.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ks.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://pn.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://le.9csxet.cn

Java: "ab".repeat(3)
来源：http://vm.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://fe.jctech888.com.cn

Ruby: "ab" * 3
来源：http://xx.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mn.szxytkj.cn

[E03] 截取子串
来源：http://uz.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://go.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pv.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://md.huanxung.cn

TS:   s.slice(1, 4)
来源：http://ut.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://zw.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jj.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vo.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://fp.colortex.cn

[E04] 查找子串位置
来源：http://jj.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://cx.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://ue.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cn.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://uz.nicolike.cn

Java: s.indexOf("x")
来源：http://zb.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://na.muxihuayi.cn

Ruby: s.index("x")
来源：http://uk.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://cf.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dj.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://su.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dj.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wu.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xr.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vk.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://az.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jc.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ta.shxzukj.cn

[E06] 替换子串
来源：http://ct.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://td.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://xk.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yw.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://yn.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cw.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xt.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://us.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://za.nszjky.cn

[E07] 按分隔符拆分
来源：http://cg.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tm.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ai.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rv.gzmigu.cn

TS:   s.split(",")
来源：http://in.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qh.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nn.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://dh.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vp.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://yf.lnxyls.cn

Py:   ",".join(items)
来源：http://si.szsharing.cn

PHP:  implode(",", $items);
来源：http://ov.shtwfgs.cn

JS:   items.join(",")
来源：http://ew.szsharing.cn

TS:   items.join(",")
来源：http://ho.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://xc.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://zc.muxihuayi.cn

Ruby: items.join(",")
来源：http://dd.nszjky.cn

C#:   string.Join(",", items)
来源：http://ie.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://iz.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ez.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hy.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://qs.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://vx.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://gk.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dv.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nf.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ii.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://zg.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ii.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jn.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://op.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://ax.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://ae.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yh.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xp.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xu.colortex.cn

[E11] 反转字符串
来源：http://nv.panjiajie.cn

Py:   s[::-1]
来源：http://dh.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://mo.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://tg.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://vb.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mc.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vl.bjjhwx.cn

Ruby: s.reverse
来源：http://jl.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wl.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://mq.chemitech.net.cn

Py:   s.count("a")
来源：http://dt.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://bh.521024.cn

JS:   s.split("a").length - 1
来源：http://mr.asd995.cn

TS:   s.split("a").length - 1
来源：http://ob.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://br.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://iv.szxytkj.cn

Ruby: s.count("a")
来源：http://ts.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://bi.nicolike.cn

[E13] 逐字符遍历
来源：http://zj.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ih.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xd.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nc.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rj.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://je.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vb.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rz.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://ym.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://if.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ht.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yi.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mu.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xu.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xl.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dl.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bg.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://rv.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nu.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dk.jctech888.com.cn


<!-- 参考信息 -->