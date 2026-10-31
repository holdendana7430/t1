代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://jf.wgjwhj.cn

[D08] 合并两个数组
来源：http://xp.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://jg.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://dc.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lo.bjjhwx.cn

TS:   [...a, ...b];
来源：http://wu.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gx.nszjky.cn

Go:   append(a, b...)
来源：http://co.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://dc.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://ss.gzmigu.cn

[D09] 排序（升序）
来源：http://am.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://cq.szxytkj.cn

PHP:  sort($arr);
来源：http://bs.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rd.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://re.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://av.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xh.szsharing.cn

Ruby: arr.sort
来源：http://ju.9csxet.cn

C#:   list.Sort();
来源：http://rm.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tb.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wo.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wa.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yh.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gp.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://it.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ql.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://py.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uc.gzmigu.cn

[D11] 反转数组
来源：http://is.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dl.colortex.cn

PHP:  array_reverse($arr);
来源：http://ol.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://im.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://gj.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://dh.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://ux.bookmarksfly.cn

Ruby: arr.reverse
来源：http://xo.muxihuayi.cn

C#:   list.Reverse();
来源：http://zl.muxihuayi.cn

[D12] 查找元素下标
来源：http://mu.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://kw.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nd.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nd.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gh.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://am.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://vl.chemitech.net.cn

Ruby: arr.index(x)
来源：http://wg.nicolike.cn

C#:   list.IndexOf(x);
来源：http://go.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://vx.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mr.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qj.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://jr.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://hs.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zd.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ye.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cs.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ev.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://zp.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yi.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rq.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://kk.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://cf.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lq.shxzukj.cn

Go:   // 手写循环
来源：http://zb.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://et.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vo.huixinmuqiang.cn

[D15] 去重
来源：http://cx.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lj.shxzskj.cn

PHP:  array_unique($arr);
来源：http://aq.colortex.cn

JS:   [...new Set(arr)]
来源：http://mf.9csxet.cn

TS:   [...new Set(arr)]
来源：http://tc.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://py.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cr.hahajie.cn

Ruby: arr.uniq
来源：http://ir.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://cd.szsharing.cn

[D16] 求和与平均值
来源：http://ry.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ld.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sb.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aq.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vv.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jh.newstarts.cn

Go:   // 手写循环累加
来源：http://dq.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://id.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://hn.gzmigu.cn

[D17] 最大值与最小值
来源：http://lb.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://yl.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://gd.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sl.lnxyls.cn

TS:   Math.max(...arr);
来源：http://lt.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vw.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pi.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://si.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://ro.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://cs.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kd.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://ze.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://as.huanxung.cn

TS:   nested.flat();
来源：http://xv.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nz.shxzukj.cn

Go:   // 手写双层循环
来源：http://pd.bjjhwx.cn

Ruby: nested.flatten
来源：http://jc.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lc.bjjhwx.cn

[D19] 按字段分组
来源：http://ee.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tl.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vc.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://le.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://do.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jk.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://hh.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ah.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://df.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://wb.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://dr.hahajie.cn

PHP:  array_count_values($arr);
来源：http://wi.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ne.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lp.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yv.hahajie.cn

Go:   // 手写 map[T]int
来源：http://mx.shxzukj.cn

Ruby: arr.tally
来源：http://ip.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jt.hahajie.cn

[D21] 判断是否包含某元素
来源：http://ym.jctech888.com.cn

Py:   x in arr
来源：http://ln.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://bg.hnjuh.cn

JS:   arr.includes(x)
来源：http://qx.9csxet.cn

TS:   arr.includes(x)
来源：http://bw.nicolike.cn

Java: list.contains(x)
来源：http://kf.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://py.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://er.huixiangedu.cn

C#:   list.Contains(x)
来源：http://um.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://tl.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ww.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lf.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uq.huanxung.cn

TS:   [...arr];
来源：http://wy.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://wy.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qf.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://jq.newstarts.cn

C#:   new List<int>(list);
来源：http://ty.jctech888.com.cn

[D23] reduce 累积计算
来源：http://id.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yn.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dx.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ac.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sw.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zd.huixiangedu.cn

Go:   // 手写循环
来源：http://jb.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eb.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oo.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://rs.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jo.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vp.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ec.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kn.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://it.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ov.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ip.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uy.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://pg.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rc.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pe.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://io.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zd.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gd.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yk.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xd.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ey.shxzukj.cn

[D26] 数组转字符串
来源：http://nd.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://iq.521024.cn

PHP:  implode(", ", $arr);
来源：http://eh.muxihuayi.cn

JS:   arr.join(", ")
来源：http://el.lnxyls.cn

TS:   arr.join(", ")
来源：http://hl.szsharing.cn

Java: String.join(", ", list)
来源：http://xh.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://dy.hnjuh.cn

Ruby: arr.join(", ")
来源：http://ru.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://vz.521024.cn

================================================================================
来源：http://fr.muxihuayi.cn

E. 字符串处理
来源：http://yd.haigaiapp.cn

================================================================================
来源：http://df.jctech888.com.cn

[E01] 拼接字符串
来源：http://tx.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://as.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gp.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pa.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sw.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://we.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://la.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ol.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wa.9csxet.cn

[E02] 重复字符串
来源：http://sb.hnjuh.cn

Py:   "ab" * 3
来源：http://cj.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://jx.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://om.newstarts.cn

TS:   "ab".repeat(3)
来源：http://zu.asd995.cn

Java: "ab".repeat(3)
来源：http://bu.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://zq.521024.cn

Ruby: "ab" * 3
来源：http://za.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pt.jctech888.com.cn

[E03] 截取子串
来源：http://sp.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://on.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://if.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://at.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://fj.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://ce.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xa.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gg.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://xv.colortex.cn

[E04] 查找子串位置
来源：http://lb.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://kr.szsharing.cn

PHP:  strpos($s, "x");
来源：http://vg.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ye.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://hq.hnjuh.cn

Java: s.indexOf("x")
来源：http://vk.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://cu.colortex.cn

Ruby: s.index("x")
来源：http://ln.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://vz.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ue.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://je.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tn.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ql.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xi.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://it.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jo.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yw.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ao.shxzskj.cn

[E06] 替换子串
来源：http://ym.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tk.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://jg.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ma.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://dz.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ka.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qr.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dv.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://kn.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://gj.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vq.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aw.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nr.shxzukj.cn

TS:   s.split(",")
来源：http://yr.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ss.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kf.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://jg.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qn.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ae.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://gh.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://yk.hnjuh.cn

JS:   items.join(",")
来源：http://fc.haigaiapp.cn

TS:   items.join(",")
来源：http://ni.chemitech.net.cn

Java: String.join(",", items)
来源：http://kj.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://pr.lnxyls.cn

Ruby: items.join(",")
来源：http://ty.huanxung.cn

C#:   string.Join(",", items)
来源：http://br.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ar.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xm.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mz.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://an.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ii.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://uh.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ac.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hs.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cg.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://ju.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jt.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ui.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://bv.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://wk.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://dt.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lf.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://is.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cc.nicolike.cn

[E11] 反转字符串
来源：http://ky.yuntaijiaju.cn

Py:   s[::-1]
来源：http://ha.nszjky.cn

PHP:  strrev($s);
来源：http://qp.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://zf.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://zj.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eh.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gk.yuexingan06.cn

Ruby: s.reverse
来源：http://zj.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oj.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://lg.shxzukj.cn

Py:   s.count("a")
来源：http://vv.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://fx.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://kt.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://ic.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mh.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://ab.shtwfgs.cn

Ruby: s.count("a")
来源：http://fx.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://bo.9csxet.cn

[E13] 逐字符遍历
来源：http://al.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://cl.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nd.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xt.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zr.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wf.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oi.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uk.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yt.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://dj.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ua.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qr.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sj.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xh.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://av.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dq.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gg.szsharing.cn


<!-- 参考信息 -->