代发 wailian999

Java: list.size();
来源：http://yn.hnjuh.cn

Go:   len(arr)
来源：http://bm.asd995.cn

Ruby: arr.length; arr.size
来源：http://ek.muxihuayi.cn

C#:   list.Count;
来源：http://yf.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://pj.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dh.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jw.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://bp.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://oq.newstarts.cn

Java: list.subList(1, 4);
来源：http://ar.szsharing.cn

Go:   arr[1:4]
来源：http://ab.9csxet.cn

Ruby: arr[1, 3]
来源：http://tt.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://et.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://qh.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://td.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://fk.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zr.chemitech.net.cn

TS:   [...a, ...b];
来源：http://mw.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rq.9csxet.cn

Go:   append(a, b...)
来源：http://td.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://ll.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://de.521024.cn

[D09] 排序（升序）
来源：http://ww.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://tr.huixiangedu.cn

PHP:  sort($arr);
来源：http://vf.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fw.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dt.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iy.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ab.newstarts.cn

Ruby: arr.sort
来源：http://pb.asd995.cn

C#:   list.Sort();
来源：http://iu.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uu.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qf.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://la.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tv.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mv.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ju.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ia.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gt.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oz.shxzukj.cn

[D11] 反转数组
来源：http://rg.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://da.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://nn.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tt.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://om.asd995.cn

Java: Collections.reverse(list);
来源：http://zg.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://pv.shtwfgs.cn

Ruby: arr.reverse
来源：http://zr.haigaiapp.cn

C#:   list.Reverse();
来源：http://gb.muxihuayi.cn

[D12] 查找元素下标
来源：http://xy.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://xs.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sj.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ik.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://de.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://av.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://gs.panjiajie.cn

Ruby: arr.index(x)
来源：http://ro.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://vm.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://cq.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vr.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wl.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://hz.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://xq.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ve.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gm.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ae.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xh.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://yb.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rr.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://te.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://oo.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://os.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yh.chemitech.net.cn

Go:   // 手写循环
来源：http://cb.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fq.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yu.yuexingan06.cn

[D15] 去重
来源：http://xd.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lo.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://lp.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://rt.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://gx.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bc.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ou.shxzskj.cn

Ruby: arr.uniq
来源：http://qn.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://cm.szsharing.cn

[D16] 求和与平均值
来源：http://zu.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sj.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ox.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://td.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://un.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ur.nszjky.cn

Go:   // 手写循环累加
来源：http://mz.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://pg.shtwfgs.cn

[D17] 最大值与最小值
来源：http://qu.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://pv.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://fu.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nv.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://bh.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fz.gzmigu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dx.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://pi.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://zh.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://fk.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nb.521024.cn

PHP:  array_merge(...$nested);
来源：http://dd.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aw.bookmarksfly.cn

TS:   nested.flat();
来源：http://ng.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pv.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://ee.shxzukj.cn

Ruby: nested.flatten
来源：http://ko.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nb.9csxet.cn

[D19] 按字段分组
来源：http://zy.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ee.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sa.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://at.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wz.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yv.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://fd.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wd.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ls.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://ln.bookmarksfly.cn

Py:   Counter(arr)
来源：http://nf.nicolike.cn

PHP:  array_count_values($arr);
来源：http://we.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://st.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ol.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qg.huanxung.cn

Go:   // 手写 map[T]int
来源：http://bj.shxzskj.cn

Ruby: arr.tally
来源：http://af.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nd.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://za.bjjhwx.cn

Py:   x in arr
来源：http://ui.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://yc.huanxung.cn

JS:   arr.includes(x)
来源：http://ep.9csxet.cn

TS:   arr.includes(x)
来源：http://jl.szsharing.cn

Java: list.contains(x)
来源：http://ot.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://vn.huanxung.cn

Ruby: arr.include?(x)
来源：http://ys.wgjwhj.cn

C#:   list.Contains(x)
来源：http://ru.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://ue.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ok.asd995.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ws.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tj.9csxet.cn

TS:   [...arr];
来源：http://lt.asd995.cn

Java: new ArrayList<>(list);
来源：http://tb.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qd.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ah.jctech888.com.cn

C#:   new List<int>(list);
来源：http://cb.bjjhwx.cn

[D23] reduce 累积计算
来源：http://nm.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rh.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dn.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pq.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hd.shxzskj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tz.huanxung.cn

Go:   // 手写循环
来源：http://iw.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cq.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zk.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://te.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dg.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kr.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://we.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gg.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aa.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mv.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qg.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oz.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://ix.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rm.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://az.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bz.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://do.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sw.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wx.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oo.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wu.asd995.cn

[D26] 数组转字符串
来源：http://de.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://dt.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://sj.chemitech.net.cn

JS:   arr.join(", ")
来源：http://lc.bjjhwx.cn

TS:   arr.join(", ")
来源：http://kj.colortex.cn

Java: String.join(", ", list)
来源：http://np.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://ik.hnjuh.cn

Ruby: arr.join(", ")
来源：http://dl.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://wc.jianghongdianzi.cn

================================================================================
来源：http://kh.newstarts.cn

E. 字符串处理
来源：http://mp.haigaiapp.cn

================================================================================
来源：http://mv.nszjky.cn

[E01] 拼接字符串
来源：http://lv.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sf.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wv.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zi.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tg.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yk.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qy.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qo.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gr.9csxet.cn

[E02] 重复字符串
来源：http://gv.wgjwhj.cn

Py:   "ab" * 3
来源：http://bg.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://qu.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://ii.hnjuh.cn

TS:   "ab".repeat(3)
来源：http://xb.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://vy.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://hs.szsharing.cn

Ruby: "ab" * 3
来源：http://my.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dj.bjjhwx.cn

[E03] 截取子串
来源：http://wz.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ha.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bz.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://za.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://xq.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://tm.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ip.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vk.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://kn.hahajie.cn

[E04] 查找子串位置
来源：http://ub.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://mu.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://ig.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ax.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://ku.szxytkj.cn

Java: s.indexOf("x")
来源：http://xy.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://lb.huanxung.cn

Ruby: s.index("x")
来源：http://mq.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://vd.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zx.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rr.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://om.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eo.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cz.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ai.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ci.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://at.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cz.colortex.cn

[E06] 替换子串
来源：http://ij.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://we.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://rt.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hg.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://su.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ei.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jq.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cq.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://rj.lnxyls.cn

[E07] 按分隔符拆分
来源：http://qb.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qv.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gh.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rj.nicolike.cn

TS:   s.split(",")
来源：http://rs.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ud.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rg.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://em.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jo.huanxung.cn

[E08] 数组按分隔符合并
来源：http://ma.nszjky.cn

Py:   ",".join(items)
来源：http://ms.hnjuh.cn

PHP:  implode(",", $items);
来源：http://ln.muxihuayi.cn

JS:   items.join(",")
来源：http://kv.jianghongdianzi.cn

TS:   items.join(",")
来源：http://sr.yuexingan06.cn

Java: String.join(",", items)
来源：http://yi.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://mo.shxzskj.cn

Ruby: items.join(",")
来源：http://ov.hnjuh.cn

C#:   string.Join(",", items)
来源：http://ys.asd995.cn

[E09] 去除所有空白字符
来源：http://bq.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ci.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ar.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://fj.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://sy.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://el.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vp.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xg.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fd.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://tr.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ca.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cw.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://fi.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://kx.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://zj.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yx.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cv.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cm.nszjky.cn

[E11] 反转字符串
来源：http://az.szsharing.cn

Py:   s[::-1]
来源：http://jm.jctech888.com.cn

PHP:  strrev($s);
来源：http://wp.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://sb.521024.cn

TS:   [...s].reverse().join("")
来源：http://go.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bv.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qm.huixiangedu.cn

Ruby: s.reverse
来源：http://yq.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vv.nszjky.cn

[E12] 统计某字符出现次数
来源：http://mo.shxzukj.cn

Py:   s.count("a")
来源：http://wh.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://eb.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://ob.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://vp.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ao.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://af.lnxyls.cn

Ruby: s.count("a")
来源：http://me.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://ma.newstarts.cn

[E13] 逐字符遍历
来源：http://vy.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://lm.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yw.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mi.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uy.asd995.cn


<!-- 参考信息 -->