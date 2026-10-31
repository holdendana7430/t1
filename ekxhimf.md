代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://bh.shtwfgs.cn

TS:   [...a, ...b];
来源：http://ka.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wp.asd995.cn

Go:   append(a, b...)
来源：http://uk.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://mo.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://go.bjjhwx.cn

[D09] 排序（升序）
来源：http://lr.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://ux.521024.cn

PHP:  sort($arr);
来源：http://pj.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ky.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xs.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zu.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ai.huixiangedu.cn

Ruby: arr.sort
来源：http://gn.yuntaijiaju.cn

C#:   list.Sort();
来源：http://ik.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fu.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ex.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jn.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fz.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fg.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wh.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ua.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tt.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sr.lnxyls.cn

[D11] 反转数组
来源：http://nx.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ph.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://vv.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vs.newstarts.cn

TS:   [...arr].reverse();
来源：http://bk.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://ku.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://zu.wgjwhj.cn

Ruby: arr.reverse
来源：http://rz.panjiajie.cn

C#:   list.Reverse();
来源：http://gi.9csxet.cn

[D12] 查找元素下标
来源：http://fq.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://jo.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kg.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lj.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eq.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fm.521024.cn

Go:   slices.Index(arr, x)
来源：http://ns.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://qw.nicolike.cn

C#:   list.IndexOf(x);
来源：http://gg.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://dj.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oc.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nm.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://vq.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://vj.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ft.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xy.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qo.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://la.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://pz.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qb.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ea.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://ll.521024.cn

TS:   arr.map(x => x * 2)
来源：http://ta.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xa.hnjuh.cn

Go:   // 手写循环
来源：http://en.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rk.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fs.nicolike.cn

[D15] 去重
来源：http://sy.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vc.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://ln.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://zm.hahajie.cn

TS:   [...new Set(arr)]
来源：http://dl.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tv.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://px.colortex.cn

Ruby: arr.uniq
来源：http://po.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://br.huanxung.cn

[D16] 求和与平均值
来源：http://ov.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kt.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bp.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wu.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zl.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rc.szsharing.cn

Go:   // 手写循环累加
来源：http://eu.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://as.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://pp.chemitech.net.cn

[D17] 最大值与最小值
来源：http://yt.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://bq.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://og.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wj.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://as.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jp.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bb.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://vg.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://iz.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://lb.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hs.521024.cn

PHP:  array_merge(...$nested);
来源：http://iw.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ka.asd995.cn

TS:   nested.flat();
来源：http://mm.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cg.chemitech.net.cn

Go:   // 手写双层循环
来源：http://lz.colortex.cn

Ruby: nested.flatten
来源：http://sy.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kt.bookmarksfly.cn

[D19] 按字段分组
来源：http://cd.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vs.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ox.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ma.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ig.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://go.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://xu.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fc.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yi.521024.cn

[D20] 统计每个元素出现次数
来源：http://vu.yuexingan06.cn

Py:   Counter(arr)
来源：http://yc.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://pa.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kn.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lt.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qu.521024.cn

Go:   // 手写 map[T]int
来源：http://dj.nszjky.cn

Ruby: arr.tally
来源：http://ea.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nb.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://at.shtwfgs.cn

Py:   x in arr
来源：http://xa.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://cl.gzmigu.cn

JS:   arr.includes(x)
来源：http://gj.nszjky.cn

TS:   arr.includes(x)
来源：http://hi.lnxyls.cn

Java: list.contains(x)
来源：http://ib.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://nk.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://ov.lnxyls.cn

C#:   list.Contains(x)
来源：http://qo.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://rf.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nt.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://om.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dq.bjjhwx.cn

TS:   [...arr];
来源：http://tb.9csxet.cn

Java: new ArrayList<>(list);
来源：http://vq.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wm.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://lm.huanxung.cn

C#:   new List<int>(list);
来源：http://mo.bjjhwx.cn

[D23] reduce 累积计算
来源：http://nw.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ut.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ix.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mm.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ne.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eh.nszjky.cn

Go:   // 手写循环
来源：http://am.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ue.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qm.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://xu.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jd.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pk.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jj.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ws.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pk.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yl.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rc.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pi.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://kx.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nk.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oi.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tu.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://my.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gr.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kd.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lv.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wi.panjiajie.cn

[D26] 数组转字符串
来源：http://qh.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://uw.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://yp.asd995.cn

JS:   arr.join(", ")
来源：http://dl.shxzskj.cn

TS:   arr.join(", ")
来源：http://nd.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ug.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://it.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://du.huixiangedu.cn

C#:   string.Join(", ", list)
来源：http://nu.szxytkj.cn

================================================================================
来源：http://we.haigaiapp.cn

E. 字符串处理
来源：http://bs.jianghongdianzi.cn

================================================================================
来源：http://yo.newstarts.cn

[E01] 拼接字符串
来源：http://fd.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tg.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nw.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bk.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hh.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ws.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lt.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fv.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kr.nicolike.cn

[E02] 重复字符串
来源：http://lj.panjiajie.cn

Py:   "ab" * 3
来源：http://ue.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://sw.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://ps.hahajie.cn

TS:   "ab".repeat(3)
来源：http://gc.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://tq.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://vf.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://ja.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://me.nszjky.cn

[E03] 截取子串
来源：http://gp.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ed.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pp.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fd.newstarts.cn

TS:   s.slice(1, 4)
来源：http://nn.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://ak.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ul.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ld.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://cj.szxytkj.cn

[E04] 查找子串位置
来源：http://wm.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://ds.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://xm.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ci.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://bv.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ba.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://gt.yuexingan06.cn

Ruby: s.index("x")
来源：http://ab.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://gs.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://km.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xl.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xk.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hm.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xp.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zk.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ug.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cs.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ds.asd995.cn

[E06] 替换子串
来源：http://sv.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hq.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://lp.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vq.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://vm.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ro.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://le.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gx.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://rw.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://sd.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xd.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://co.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ho.newstarts.cn

TS:   s.split(",")
来源：http://qj.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lt.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eo.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://kh.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ex.521024.cn

[E08] 数组按分隔符合并
来源：http://ix.bjjhwx.cn

Py:   ",".join(items)
来源：http://fw.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://xl.521024.cn

JS:   items.join(",")
来源：http://yi.huanxung.cn

TS:   items.join(",")
来源：http://gs.haigaiapp.cn

Java: String.join(",", items)
来源：http://sd.asd995.cn

Go:   strings.Join(items, ",")
来源：http://xz.hnjuh.cn

Ruby: items.join(",")
来源：http://ps.panjiajie.cn

C#:   string.Join(",", items)
来源：http://nc.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://yh.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ty.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ay.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://bb.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://yk.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://wq.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://on.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wp.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mr.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://hw.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wq.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sy.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://jn.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://lc.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://bx.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://or.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tb.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mx.asd995.cn

[E11] 反转字符串
来源：http://vo.hnjuh.cn

Py:   s[::-1]
来源：http://xy.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://yy.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://xg.asd995.cn

TS:   [...s].reverse().join("")
来源：http://de.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dd.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ey.jctech888.com.cn

Ruby: s.reverse
来源：http://zo.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sv.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://zu.asd995.cn

Py:   s.count("a")
来源：http://db.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://rs.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://zs.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://gv.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yo.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://eu.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://qj.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://vr.yuexingan06.cn

[E13] 逐字符遍历
来源：http://tg.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://sa.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mz.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cb.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gn.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gj.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wm.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uz.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uw.9csxet.cn

[E14] URL 编码与 Base64
来源：http://zv.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://np.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tz.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fr.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uc.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qt.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qn.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pa.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tk.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://kv.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kh.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fc.chemitech.net.cn


<!-- 参考信息 -->