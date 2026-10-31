代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://fx.shtwfgs.cn

TS:   [...a, ...b];
来源：http://ej.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zs.newstarts.cn

Go:   append(a, b...)
来源：http://tq.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://il.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://uv.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://mx.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ke.huixiangedu.cn

PHP:  sort($arr);
来源：http://dh.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vn.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zn.shxzskj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jp.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://db.shxzukj.cn

Ruby: arr.sort
来源：http://ug.hnjuh.cn

C#:   list.Sort();
来源：http://li.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cx.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ap.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qm.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yg.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sa.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gu.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rp.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gt.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://up.521024.cn

[D11] 反转数组
来源：http://ge.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rw.szsharing.cn

PHP:  array_reverse($arr);
来源：http://mt.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ft.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://jh.521024.cn

Java: Collections.reverse(list);
来源：http://zh.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://eb.bookmarksfly.cn

Ruby: arr.reverse
来源：http://mq.hahajie.cn

C#:   list.Reverse();
来源：http://rg.hahajie.cn

[D12] 查找元素下标
来源：http://et.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://vi.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ml.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://te.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fb.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cv.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://uz.jctech888.com.cn

Ruby: arr.index(x)
来源：http://rd.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://gg.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://al.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fk.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sv.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://hb.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://za.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gw.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vo.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wn.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eu.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://kr.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ix.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nv.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://ca.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://ip.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pf.shxzukj.cn

Go:   // 手写循环
来源：http://ip.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yc.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hg.huanxung.cn

[D15] 去重
来源：http://xc.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ar.nicolike.cn

PHP:  array_unique($arr);
来源：http://ci.hahajie.cn

JS:   [...new Set(arr)]
来源：http://kd.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://da.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://em.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bp.szxytkj.cn

Ruby: arr.uniq
来源：http://cc.asd995.cn

C#:   list.Distinct().ToList()
来源：http://ek.muxihuayi.cn

[D16] 求和与平均值
来源：http://jr.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ux.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://od.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nv.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uj.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hr.asd995.cn

Go:   // 手写循环累加
来源：http://kr.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://io.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://tj.nicolike.cn

[D17] 最大值与最小值
来源：http://qw.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://bz.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://xj.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gc.gzmigu.cn

TS:   Math.max(...arr);
来源：http://ea.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cf.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://si.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://zi.colortex.cn

C#:   list.Max();  list.Min()
来源：http://wl.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://ue.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lo.asd995.cn

PHP:  array_merge(...$nested);
来源：http://bz.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ml.newstarts.cn

TS:   nested.flat();
来源：http://vu.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mk.shxzukj.cn

Go:   // 手写双层循环
来源：http://bl.szxytkj.cn

Ruby: nested.flatten
来源：http://sk.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dr.haigaiapp.cn

[D19] 按字段分组
来源：http://uo.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ad.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dg.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bl.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nv.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rx.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://of.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gf.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ab.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://lq.szxytkj.cn

Py:   Counter(arr)
来源：http://dm.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://os.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pd.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sl.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xz.9csxet.cn

Go:   // 手写 map[T]int
来源：http://hl.jctech888.com.cn

Ruby: arr.tally
来源：http://ja.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zt.huanxung.cn

[D21] 判断是否包含某元素
来源：http://vh.521024.cn

Py:   x in arr
来源：http://jd.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://vn.szxytkj.cn

JS:   arr.includes(x)
来源：http://xo.asd995.cn

TS:   arr.includes(x)
来源：http://ia.huanxung.cn

Java: list.contains(x)
来源：http://vs.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://oc.9csxet.cn

Ruby: arr.include?(x)
来源：http://db.wgjwhj.cn

C#:   list.Contains(x)
来源：http://qu.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://et.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oy.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mc.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ud.shxzskj.cn

TS:   [...arr];
来源：http://ip.szsharing.cn

Java: new ArrayList<>(list);
来源：http://sc.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uy.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://ou.jctech888.com.cn

C#:   new List<int>(list);
来源：http://tw.hnjuh.cn

[D23] reduce 累积计算
来源：http://ky.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://md.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://or.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://io.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://un.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sk.bjjhwx.cn

Go:   // 手写循环
来源：http://bj.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wq.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rd.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://tt.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ww.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yp.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zk.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tg.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yk.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ms.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nl.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gf.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ak.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://za.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cy.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ko.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wi.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cf.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bh.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ow.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bq.gzmigu.cn

[D26] 数组转字符串
来源：http://tk.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://am.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://jr.szxytkj.cn

JS:   arr.join(", ")
来源：http://km.chemitech.net.cn

TS:   arr.join(", ")
来源：http://ua.shxzskj.cn

Java: String.join(", ", list)
来源：http://pe.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://ar.asd995.cn

Ruby: arr.join(", ")
来源：http://mb.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://xn.gzmigu.cn

================================================================================
来源：http://wk.huixinmuqiang.cn

E. 字符串处理
来源：http://zn.lnxyls.cn

================================================================================
来源：http://po.szsharing.cn

[E01] 拼接字符串
来源：http://fd.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://au.jctech888.com.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lf.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qn.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wp.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eg.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ie.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://td.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ct.muxihuayi.cn

[E02] 重复字符串
来源：http://va.shxzskj.cn

Py:   "ab" * 3
来源：http://mx.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://vv.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://ox.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://oc.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://rl.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://it.lnxyls.cn

Ruby: "ab" * 3
来源：http://lj.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://il.muxihuayi.cn

[E03] 截取子串
来源：http://qe.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ce.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ob.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vr.9csxet.cn

TS:   s.slice(1, 4)
来源：http://uo.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://ct.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ym.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://go.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://bx.muxihuayi.cn

[E04] 查找子串位置
来源：http://ni.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://jw.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://kb.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oq.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://yj.lnxyls.cn

Java: s.indexOf("x")
来源：http://hm.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://xm.9csxet.cn

Ruby: s.index("x")
来源：http://bs.szsharing.cn

C#:   s.IndexOf("x")
来源：http://xj.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ic.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tr.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dx.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ng.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wh.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ey.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hy.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dw.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jf.wgjwhj.cn

[E06] 替换子串
来源：http://sn.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ku.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://rh.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cx.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://oj.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bw.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lu.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://op.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://uo.huanxung.cn

[E07] 按分隔符拆分
来源：http://yj.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uh.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vt.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qz.jctech888.com.cn

TS:   s.split(",")
来源：http://qu.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tw.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gv.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://gs.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://va.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://yy.szsharing.cn

Py:   ",".join(items)
来源：http://hb.nszjky.cn

PHP:  implode(",", $items);
来源：http://sk.huixiangedu.cn

JS:   items.join(",")
来源：http://uh.9csxet.cn

TS:   items.join(",")
来源：http://dh.huanxung.cn

Java: String.join(",", items)
来源：http://mt.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://zp.muxihuayi.cn

Ruby: items.join(",")
来源：http://ub.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://vv.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://pn.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ik.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nl.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://gn.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://tg.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://ko.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bf.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ar.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ll.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://ns.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hq.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cw.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://eh.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://ru.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://ow.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kc.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ex.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vf.huanxung.cn

[E11] 反转字符串
来源：http://bl.newstarts.cn

Py:   s[::-1]
来源：http://uo.shtwfgs.cn

PHP:  strrev($s);
来源：http://rr.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://cw.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://fy.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nd.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pt.shxzukj.cn

Ruby: s.reverse
来源：http://gg.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uy.szsharing.cn

[E12] 统计某字符出现次数
来源：http://jd.lnxyls.cn

Py:   s.count("a")
来源：http://cf.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://oz.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://jm.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://fc.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cf.colortex.cn

Go:   strings.Count(s, "a")
来源：http://ld.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://pz.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://cc.bjjhwx.cn

[E13] 逐字符遍历
来源：http://fw.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://jk.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dt.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ht.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hy.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ny.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://le.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hi.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fz.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://fd.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://de.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uy.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://he.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qk.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dr.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oe.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xc.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://os.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://ve.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pq.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pv.shxzukj.cn


<!-- 参考信息 -->