代发 wailian999

TS:   arr.slice(1, 4);
来源：http://pv.newstarts.cn

Java: list.subList(1, 4);
来源：http://hj.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://hz.newstarts.cn

Ruby: arr[1, 3]
来源：http://xp.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://ko.yuexingan06.cn

[D08] 合并两个数组
来源：http://tl.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://zq.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://hy.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ii.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://oa.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://at.nicolike.cn

Go:   append(a, b...)
来源：http://tv.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://hy.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://mm.shxzukj.cn

[D09] 排序（升序）
来源：http://vl.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://jx.colortex.cn

PHP:  sort($arr);
来源：http://st.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://da.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xw.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rj.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://um.bjjhwx.cn

Ruby: arr.sort
来源：http://em.wgjwhj.cn

C#:   list.Sort();
来源：http://rq.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ws.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ni.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cr.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://am.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ia.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hf.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ix.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sv.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ex.jctech888.com.cn

[D11] 反转数组
来源：http://fd.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lu.9csxet.cn

PHP:  array_reverse($arr);
来源：http://ls.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://di.colortex.cn

TS:   [...arr].reverse();
来源：http://vt.shxzukj.cn

Java: Collections.reverse(list);
来源：http://ff.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://kr.haigaiapp.cn

Ruby: arr.reverse
来源：http://ba.newstarts.cn

C#:   list.Reverse();
来源：http://ax.asd995.cn

[D12] 查找元素下标
来源：http://qc.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://lt.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lv.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vp.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rd.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xx.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://wt.muxihuayi.cn

Ruby: arr.index(x)
来源：http://wz.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://si.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://ey.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sn.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gq.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://hg.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://yh.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qj.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qo.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sh.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cn.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://dm.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ep.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://am.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://ye.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://fd.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nm.521024.cn

Go:   // 手写循环
来源：http://ga.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xu.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://al.gzmigu.cn

[D15] 去重
来源：http://te.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tm.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://mt.huanxung.cn

JS:   [...new Set(arr)]
来源：http://fx.asd995.cn

TS:   [...new Set(arr)]
来源：http://bq.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ui.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wd.huixiangedu.cn

Ruby: arr.uniq
来源：http://ik.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://ml.asd995.cn

[D16] 求和与平均值
来源：http://xh.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ct.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wc.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ld.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kg.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yl.hahajie.cn

Go:   // 手写循环累加
来源：http://wh.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://az.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://dn.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://ot.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://wz.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://tj.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hp.asd995.cn

TS:   Math.max(...arr);
来源：http://bg.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zf.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ok.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://jc.521024.cn

C#:   list.Max();  list.Min()
来源：http://ek.asd995.cn

[D18] 扁平化嵌套数组
来源：http://ft.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hs.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://gy.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rc.muxihuayi.cn

TS:   nested.flat();
来源：http://md.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vf.521024.cn

Go:   // 手写双层循环
来源：http://qi.nicolike.cn

Ruby: nested.flatten
来源：http://oh.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xd.szsharing.cn

[D19] 按字段分组
来源：http://lh.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oe.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://do.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cz.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kc.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gx.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://bs.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gh.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rm.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://ct.colortex.cn

Py:   Counter(arr)
来源：http://zf.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://lu.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eg.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qs.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lp.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://jj.huixiangedu.cn

Ruby: arr.tally
来源：http://bx.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://re.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://lp.nszjky.cn

Py:   x in arr
来源：http://vr.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://sv.huanxung.cn

JS:   arr.includes(x)
来源：http://og.yuexingan06.cn

TS:   arr.includes(x)
来源：http://wl.hahajie.cn

Java: list.contains(x)
来源：http://gc.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://co.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://mf.yuntaijiaju.cn

C#:   list.Contains(x)
来源：http://sp.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://ju.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mj.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ly.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mq.shtwfgs.cn

TS:   [...arr];
来源：http://rq.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://cq.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uf.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://qj.wgjwhj.cn

C#:   new List<int>(list);
来源：http://xn.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://cr.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fs.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://se.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mz.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://io.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://al.lnxyls.cn

Go:   // 手写循环
来源：http://pi.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oq.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qr.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://hb.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fj.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ql.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://io.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ca.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cs.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ld.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yd.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fg.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://sq.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ri.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zq.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ed.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ar.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gp.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://to.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kx.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cy.hnjuh.cn

[D26] 数组转字符串
来源：http://lk.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://eb.jctech888.com.cn

PHP:  implode(", ", $arr);
来源：http://by.colortex.cn

JS:   arr.join(", ")
来源：http://le.nszjky.cn

TS:   arr.join(", ")
来源：http://hm.wgjwhj.cn

Java: String.join(", ", list)
来源：http://tu.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://ff.lnxyls.cn

Ruby: arr.join(", ")
来源：http://yw.asd995.cn

C#:   string.Join(", ", list)
来源：http://qe.lnxyls.cn

================================================================================
来源：http://gb.huixiangedu.cn

E. 字符串处理
来源：http://rq.colortex.cn

================================================================================
来源：http://cm.huixiangedu.cn

[E01] 拼接字符串
来源：http://gy.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ss.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nv.wgjwhj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vj.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rs.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qr.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fm.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gh.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eg.nicolike.cn

[E02] 重复字符串
来源：http://eg.wgjwhj.cn

Py:   "ab" * 3
来源：http://fg.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://lg.9csxet.cn

JS:   "ab".repeat(3)
来源：http://di.nszjky.cn

TS:   "ab".repeat(3)
来源：http://hp.gzmigu.cn

Java: "ab".repeat(3)
来源：http://ed.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://jj.nicolike.cn

Ruby: "ab" * 3
来源：http://qy.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uk.lnxyls.cn

[E03] 截取子串
来源：http://vv.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xr.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ck.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ok.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://fc.521024.cn

Java: s.substring(1, 4)
来源：http://qf.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fl.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jz.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://is.szxytkj.cn

[E04] 查找子串位置
来源：http://jm.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://dz.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://ye.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ir.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://an.colortex.cn

Java: s.indexOf("x")
来源：http://jd.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://tc.hahajie.cn

Ruby: s.index("x")
来源：http://su.asd995.cn

C#:   s.IndexOf("x")
来源：http://om.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ot.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fc.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kg.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ou.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xt.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kt.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ff.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tn.jianghongdianzi.cn

[E06] 替换子串
来源：http://ar.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oh.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://pl.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zs.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://lh.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://at.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ax.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nw.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://lr.gzmigu.cn

[E07] 按分隔符拆分
来源：http://vw.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ch.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yt.yuexingan06.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vy.wgjwhj.cn

TS:   s.split(",")
来源：http://ti.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xl.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kc.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://yt.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ye.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://fl.9csxet.cn

Py:   ",".join(items)
来源：http://bf.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://xu.hnjuh.cn

JS:   items.join(",")
来源：http://rl.hahajie.cn

TS:   items.join(",")
来源：http://wf.521024.cn

Java: String.join(",", items)
来源：http://tz.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://bt.yuexingan06.cn

Ruby: items.join(",")
来源：http://jk.colortex.cn

C#:   string.Join(",", items)
来源：http://ty.panjiajie.cn

[E09] 去除所有空白字符
来源：http://et.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://he.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zx.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://yk.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://xr.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ej.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://an.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zf.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wf.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://vi.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fa.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gf.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://uc.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://xv.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://tq.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://by.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bm.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fr.shxzskj.cn

[E11] 反转字符串
来源：http://cb.bookmarksfly.cn

Py:   s[::-1]
来源：http://mf.asd995.cn

PHP:  strrev($s);
来源：http://jw.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://nr.521024.cn

TS:   [...s].reverse().join("")
来源：http://xv.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fa.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nu.bookmarksfly.cn

Ruby: s.reverse
来源：http://ve.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ve.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://xl.huixiangedu.cn

Py:   s.count("a")
来源：http://ar.521024.cn

PHP:  substr_count($s, "a");
来源：http://kr.9csxet.cn

JS:   s.split("a").length - 1
来源：http://hi.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://ay.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gd.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://bt.newstarts.cn

Ruby: s.count("a")
来源：http://up.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://cg.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ce.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://ky.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://og.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yt.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yb.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qg.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dc.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xj.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rq.9csxet.cn

[E14] URL 编码与 Base64
来源：http://qa.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gj.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://na.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://st.521024.cn


<!-- 参考信息 -->