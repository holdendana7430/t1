代发 wailian999

TS:   arr.slice(1, 4);
来源：http://pa.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://sk.shtwfgs.cn

Go:   arr[1:4]
来源：http://se.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://fo.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://vk.haigaiapp.cn

[D08] 合并两个数组
来源：http://sz.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://bc.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://it.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vz.asd995.cn

TS:   [...a, ...b];
来源：http://rb.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vc.asd995.cn

Go:   append(a, b...)
来源：http://mx.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://gh.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://ke.hahajie.cn

[D09] 排序（升序）
来源：http://fa.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ss.jctech888.com.cn

PHP:  sort($arr);
来源：http://nr.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hf.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jd.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mn.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ow.huixinmuqiang.cn

Ruby: arr.sort
来源：http://fq.huixiangedu.cn

C#:   list.Sort();
来源：http://on.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://no.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fd.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ag.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ka.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lj.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ei.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wj.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vq.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nq.jianghongdianzi.cn

[D11] 反转数组
来源：http://am.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nw.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://xq.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vq.9csxet.cn

TS:   [...arr].reverse();
来源：http://mc.shxzskj.cn

Java: Collections.reverse(list);
来源：http://ct.521024.cn

Go:   slices.Reverse(arr)
来源：http://ku.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://jy.hahajie.cn

C#:   list.Reverse();
来源：http://zr.lnxyls.cn

[D12] 查找元素下标
来源：http://gg.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://qn.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kf.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nd.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ad.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ax.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://ox.muxihuayi.cn

Ruby: arr.index(x)
来源：http://va.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://ha.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://lv.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://al.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hj.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://oa.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://kd.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hg.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yr.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://we.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fv.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://tl.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ak.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fo.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://cx.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://rs.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gs.asd995.cn

Go:   // 手写循环
来源：http://wd.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://em.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vz.521024.cn

[D15] 去重
来源：http://tr.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fx.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://df.hahajie.cn

JS:   [...new Set(arr)]
来源：http://dk.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://nl.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cc.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hf.asd995.cn

Ruby: arr.uniq
来源：http://rp.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://ee.chemitech.net.cn

[D16] 求和与平均值
来源：http://az.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pe.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://in.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://me.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://me.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://et.wgjwhj.cn

Go:   // 手写循环累加
来源：http://wa.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://at.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://lf.shxzukj.cn

[D17] 最大值与最小值
来源：http://ax.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://am.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://qg.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://va.shxzskj.cn

TS:   Math.max(...arr);
来源：http://yw.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pb.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://av.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://ls.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://wp.colortex.cn

[D18] 扁平化嵌套数组
来源：http://oj.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jo.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://wc.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dq.hahajie.cn

TS:   nested.flat();
来源：http://ef.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ud.hahajie.cn

Go:   // 手写双层循环
来源：http://fb.wgjwhj.cn

Ruby: nested.flatten
来源：http://ux.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ej.szsharing.cn

[D19] 按字段分组
来源：http://rt.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bg.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ql.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ra.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://em.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xs.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://ul.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://on.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mw.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://ms.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://el.colortex.cn

PHP:  array_count_values($arr);
来源：http://vd.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://if.bookmarksfly.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pl.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ax.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://gp.shxzukj.cn

Ruby: arr.tally
来源：http://da.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nv.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://jc.gzmigu.cn

Py:   x in arr
来源：http://fr.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://gc.colortex.cn

JS:   arr.includes(x)
来源：http://be.szsharing.cn

TS:   arr.includes(x)
来源：http://qq.szxytkj.cn

Java: list.contains(x)
来源：http://gk.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://le.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://rq.shxzskj.cn

C#:   list.Contains(x)
来源：http://oi.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://gq.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ro.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wp.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sp.bookmarksfly.cn

TS:   [...arr];
来源：http://wj.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://kk.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ok.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://cw.jctech888.com.cn

C#:   new List<int>(list);
来源：http://we.yuexingan06.cn

[D23] reduce 累积计算
来源：http://iz.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ot.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fy.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://df.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xg.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nq.bjjhwx.cn

Go:   // 手写循环
来源：http://ob.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rs.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hp.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://aq.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cl.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lj.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wm.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rb.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fo.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ze.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bw.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vf.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://kz.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bz.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qv.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://np.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://df.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wu.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kv.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://an.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oz.shxzskj.cn

[D26] 数组转字符串
来源：http://lr.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://bd.asd995.cn

PHP:  implode(", ", $arr);
来源：http://qo.newstarts.cn

JS:   arr.join(", ")
来源：http://iv.chemitech.net.cn

TS:   arr.join(", ")
来源：http://nn.szsharing.cn

Java: String.join(", ", list)
来源：http://rz.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://dq.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://qz.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://dc.hnjuh.cn

================================================================================
来源：http://aj.szsharing.cn

E. 字符串处理
来源：http://fi.jianghongdianzi.cn

================================================================================
来源：http://rg.nszjky.cn

[E01] 拼接字符串
来源：http://mc.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sr.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ju.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fx.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tj.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hb.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tj.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ko.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pk.bjjhwx.cn

[E02] 重复字符串
来源：http://dl.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://nz.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://av.huanxung.cn

JS:   "ab".repeat(3)
来源：http://yj.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://uz.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://rb.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://yt.jctech888.com.cn

Ruby: "ab" * 3
来源：http://gj.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ki.wgjwhj.cn

[E03] 截取子串
来源：http://vn.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://md.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vf.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pj.newstarts.cn

TS:   s.slice(1, 4)
来源：http://xw.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://bv.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cl.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cm.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://ro.huixiangedu.cn

[E04] 查找子串位置
来源：http://hf.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://jh.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://bi.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ei.lnxyls.cn

TS:   s.indexOf("x")
来源：http://kv.szsharing.cn

Java: s.indexOf("x")
来源：http://ji.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://lc.huixiangedu.cn

Ruby: s.index("x")
来源：http://ga.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://kj.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ut.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yq.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bn.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ta.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cd.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zu.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tj.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lt.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yq.wgjwhj.cn

[E06] 替换子串
来源：http://pk.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wc.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://yl.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hx.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://vd.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aw.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gq.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wd.colortex.cn

C#:   s.Replace("a", "b")
来源：http://em.shxzskj.cn

[E07] 按分隔符拆分
来源：http://mo.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://io.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://od.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uw.asd995.cn

TS:   s.split(",")
来源：http://bp.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vn.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xx.colortex.cn

Ruby: s.split(",");  s.split
来源：http://mc.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wy.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://zg.muxihuayi.cn

Py:   ",".join(items)
来源：http://pv.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://dw.hnjuh.cn

JS:   items.join(",")
来源：http://wr.colortex.cn

TS:   items.join(",")
来源：http://hf.hahajie.cn

Java: String.join(",", items)
来源：http://jo.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://hr.huixiangedu.cn

Ruby: items.join(",")
来源：http://eo.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://vo.nszjky.cn

[E09] 去除所有空白字符
来源：http://pl.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zx.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tg.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://we.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://pc.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://sb.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pm.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cr.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ca.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://nd.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ue.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fe.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://st.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://jj.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://qa.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://at.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wc.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://au.shxzskj.cn

[E11] 反转字符串
来源：http://hy.shtwfgs.cn

Py:   s[::-1]
来源：http://fp.bjjhwx.cn

PHP:  strrev($s);
来源：http://oz.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://yg.asd995.cn

TS:   [...s].reverse().join("")
来源：http://dq.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fb.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tc.szsharing.cn

Ruby: s.reverse
来源：http://zm.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://po.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://vd.muxihuayi.cn

Py:   s.count("a")
来源：http://gt.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://yz.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://og.asd995.cn

TS:   s.split("a").length - 1
来源：http://rx.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jx.asd995.cn

Go:   strings.Count(s, "a")
来源：http://ez.huixiangedu.cn

Ruby: s.count("a")
来源：http://qb.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://ub.haigaiapp.cn

[E13] 逐字符遍历
来源：http://jd.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://hw.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ql.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jv.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kl.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ks.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bk.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://io.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qx.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://re.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rq.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wt.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dy.shtwfgs.cn


<!-- 参考信息 -->