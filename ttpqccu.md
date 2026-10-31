代发 wailian999

PHP:  sort($arr);
来源：http://iu.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ns.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://co.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wr.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xg.nicolike.cn

Ruby: arr.sort
来源：http://wp.szxytkj.cn

C#:   list.Sort();
来源：http://no.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nz.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://we.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://un.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bh.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kf.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oz.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iu.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qs.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sn.jianghongdianzi.cn

[D11] 反转数组
来源：http://cy.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xa.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://sd.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ok.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://yb.colortex.cn

Java: Collections.reverse(list);
来源：http://zh.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://ol.shxzskj.cn

Ruby: arr.reverse
来源：http://ar.muxihuayi.cn

C#:   list.Reverse();
来源：http://gw.szxytkj.cn

[D12] 查找元素下标
来源：http://qb.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://tb.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zv.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pz.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jl.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jk.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://bm.yuexingan06.cn

Ruby: arr.index(x)
来源：http://vn.hahajie.cn

C#:   list.IndexOf(x);
来源：http://kn.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://gc.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lh.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sh.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://jh.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://wp.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://do.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://da.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qm.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xc.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://vg.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wk.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ll.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://cq.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://jp.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zr.huixinmuqiang.cn

Go:   // 手写循环
来源：http://dm.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fo.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lm.huixinmuqiang.cn

[D15] 去重
来源：http://rw.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ps.9csxet.cn

PHP:  array_unique($arr);
来源：http://nh.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://mn.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://cd.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fz.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ej.shxzskj.cn

Ruby: arr.uniq
来源：http://bs.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://wi.newstarts.cn

[D16] 求和与平均值
来源：http://cy.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aq.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nz.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rj.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jy.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rf.muxihuayi.cn

Go:   // 手写循环累加
来源：http://ul.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yl.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://bz.muxihuayi.cn

[D17] 最大值与最小值
来源：http://hs.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://qf.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://cw.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gj.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://bv.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qf.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jo.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://pt.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://eh.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://ze.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pv.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://tx.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dw.asd995.cn

TS:   nested.flat();
来源：http://vq.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qp.9csxet.cn

Go:   // 手写双层循环
来源：http://qg.shxzskj.cn

Ruby: nested.flatten
来源：http://md.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zb.huixinmuqiang.cn

[D19] 按字段分组
来源：http://qd.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ql.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ua.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sl.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nx.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dt.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://rt.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nd.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gb.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://sh.huixiangedu.cn

Py:   Counter(arr)
来源：http://jt.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://iu.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sk.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ck.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bt.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://vb.nicolike.cn

Ruby: arr.tally
来源：http://xk.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mu.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://pd.shxzskj.cn

Py:   x in arr
来源：http://vu.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://rf.asd995.cn

JS:   arr.includes(x)
来源：http://ls.huixiangedu.cn

TS:   arr.includes(x)
来源：http://ha.huanxung.cn

Java: list.contains(x)
来源：http://qt.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://in.panjiajie.cn

Ruby: arr.include?(x)
来源：http://yt.hnjuh.cn

C#:   list.Contains(x)
来源：http://ut.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://vr.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fx.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ro.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fc.chemitech.net.cn

TS:   [...arr];
来源：http://pt.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://xi.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://in.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://dx.nszjky.cn

C#:   new List<int>(list);
来源：http://zg.shtwfgs.cn

[D23] reduce 累积计算
来源：http://dk.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ki.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dh.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wj.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://im.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sb.szxytkj.cn

Go:   // 手写循环
来源：http://ej.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ra.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xf.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://yz.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yw.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nh.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pg.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rh.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qw.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mg.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ro.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kq.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://vr.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wk.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pu.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lx.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ly.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sf.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yn.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rx.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ha.shtwfgs.cn

[D26] 数组转字符串
来源：http://es.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://bn.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://ik.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://fa.bjjhwx.cn

TS:   arr.join(", ")
来源：http://bq.wgjwhj.cn

Java: String.join(", ", list)
来源：http://aq.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://ft.newstarts.cn

Ruby: arr.join(", ")
来源：http://fh.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://yh.shxzskj.cn

================================================================================
来源：http://pw.yuexingan06.cn

E. 字符串处理
来源：http://kz.huixiangedu.cn

================================================================================
来源：http://tk.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://vv.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://up.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ss.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yc.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ru.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tb.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ty.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vk.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lm.huixiangedu.cn

[E02] 重复字符串
来源：http://uv.hnjuh.cn

Py:   "ab" * 3
来源：http://lc.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://bi.hahajie.cn

JS:   "ab".repeat(3)
来源：http://md.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://cw.shxzskj.cn

Java: "ab".repeat(3)
来源：http://ta.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://pz.521024.cn

Ruby: "ab" * 3
来源：http://vf.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vx.521024.cn

[E03] 截取子串
来源：http://cw.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qf.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://no.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dq.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://ra.panjiajie.cn

Java: s.substring(1, 4)
来源：http://fq.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eh.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zg.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://kv.newstarts.cn

[E04] 查找子串位置
来源：http://jc.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://bp.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://to.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bu.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://ej.lnxyls.cn

Java: s.indexOf("x")
来源：http://zg.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://pp.nicolike.cn

Ruby: s.index("x")
来源：http://or.hahajie.cn

C#:   s.IndexOf("x")
来源：http://id.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zg.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zq.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dg.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vd.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fn.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zq.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qz.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pb.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ns.gzmigu.cn

[E06] 替换子串
来源：http://hn.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cu.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://vt.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iy.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://cu.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cb.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fp.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ab.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://qv.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://lp.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tc.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fj.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://by.jctech888.com.cn

TS:   s.split(",")
来源：http://wh.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kf.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rj.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://mh.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cj.nicolike.cn

[E08] 数组按分隔符合并
来源：http://dp.haigaiapp.cn

Py:   ",".join(items)
来源：http://tc.nszjky.cn

PHP:  implode(",", $items);
来源：http://hm.521024.cn

JS:   items.join(",")
来源：http://ba.gzmigu.cn

TS:   items.join(",")
来源：http://mx.shxzskj.cn

Java: String.join(",", items)
来源：http://ze.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://tj.yuexingan06.cn

Ruby: items.join(",")
来源：http://op.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://kr.panjiajie.cn

[E09] 去除所有空白字符
来源：http://cj.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ga.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wy.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://zg.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://pq.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://dj.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ed.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gk.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ya.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://ot.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ru.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mu.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://wl.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://bw.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://jd.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ce.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pe.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qo.huixiangedu.cn

[E11] 反转字符串
来源：http://th.hahajie.cn

Py:   s[::-1]
来源：http://co.521024.cn

PHP:  strrev($s);
来源：http://ok.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://vc.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://kn.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cs.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jr.newstarts.cn

Ruby: s.reverse
来源：http://qi.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cq.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://ss.yuntaijiaju.cn

Py:   s.count("a")
来源：http://kd.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://xg.nszjky.cn

JS:   s.split("a").length - 1
来源：http://os.asd995.cn

TS:   s.split("a").length - 1
来源：http://ag.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yq.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://om.asd995.cn

Ruby: s.count("a")
来源：http://wh.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://pv.lnxyls.cn

[E13] 逐字符遍历
来源：http://ip.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://tn.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ls.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lw.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sl.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jh.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nk.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eq.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rk.huanxung.cn

[E14] URL 编码与 Base64
来源：http://rk.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ky.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tr.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ho.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wq.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vq.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jw.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vb.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xf.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://hc.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://db.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hi.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://re.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uw.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tc.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uk.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://en.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ch.szsharing.cn

[E16] 数字千分位
来源：http://uc.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://hn.hnjuh.cn


<!-- 参考信息 -->