代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://xh.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://fe.jctech888.com.cn

[D09] 排序（升序）
来源：http://gt.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://xi.shxzskj.cn

PHP:  sort($arr);
来源：http://cs.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://va.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yk.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://be.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yw.lnxyls.cn

Ruby: arr.sort
来源：http://ac.bookmarksfly.cn

C#:   list.Sort();
来源：http://zf.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fa.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jy.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ck.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qr.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hp.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lc.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hp.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vj.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tk.panjiajie.cn

[D11] 反转数组
来源：http://bp.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yx.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://wj.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eu.9csxet.cn

TS:   [...arr].reverse();
来源：http://tg.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://gn.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://gp.shxzskj.cn

Ruby: arr.reverse
来源：http://ya.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://qx.shxzukj.cn

[D12] 查找元素下标
来源：http://qv.521024.cn

Py:   arr.index(x);  x in arr
来源：http://ke.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jc.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mz.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ai.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://in.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://xa.nicolike.cn

Ruby: arr.index(x)
来源：http://wo.521024.cn

C#:   list.IndexOf(x);
来源：http://xi.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://oi.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qc.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rw.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://zm.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://gt.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fl.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yx.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://md.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xz.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://iv.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dd.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qp.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://vf.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://rl.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ci.asd995.cn

Go:   // 手写循环
来源：http://zr.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fa.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hx.gzmigu.cn

[D15] 去重
来源：http://xp.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sm.szsharing.cn

PHP:  array_unique($arr);
来源：http://ij.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://xe.szsharing.cn

TS:   [...new Set(arr)]
来源：http://bf.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sl.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yl.bookmarksfly.cn

Ruby: arr.uniq
来源：http://mc.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://zc.wgjwhj.cn

[D16] 求和与平均值
来源：http://fi.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wl.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ap.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lu.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://py.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zy.9csxet.cn

Go:   // 手写循环累加
来源：http://pf.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jb.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://oe.hahajie.cn

[D17] 最大值与最小值
来源：http://ak.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://qt.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://ik.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fy.asd995.cn

TS:   Math.max(...arr);
来源：http://wm.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ku.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qa.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://er.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://ns.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://xr.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ep.colortex.cn

PHP:  array_merge(...$nested);
来源：http://pc.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oo.shtwfgs.cn

TS:   nested.flat();
来源：http://tm.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mx.huanxung.cn

Go:   // 手写双层循环
来源：http://zp.bookmarksfly.cn

Ruby: nested.flatten
来源：http://cz.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://af.9csxet.cn

[D19] 按字段分组
来源：http://cc.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gh.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ha.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wo.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lk.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ro.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://oj.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lr.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mj.colortex.cn

[D20] 统计每个元素出现次数
来源：http://us.shtwfgs.cn

Py:   Counter(arr)
来源：http://da.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://uv.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hr.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ug.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ly.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://il.asd995.cn

Ruby: arr.tally
来源：http://rn.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qk.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://vp.9csxet.cn

Py:   x in arr
来源：http://wc.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://yo.asd995.cn

JS:   arr.includes(x)
来源：http://ub.nszjky.cn

TS:   arr.includes(x)
来源：http://dv.szsharing.cn

Java: list.contains(x)
来源：http://nn.hahajie.cn

Go:   slices.Contains(arr, x)
来源：http://ox.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://pu.yuexingan06.cn

C#:   list.Contains(x)
来源：http://it.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://sv.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dd.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ye.colortex.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lk.nicolike.cn

TS:   [...arr];
来源：http://am.9csxet.cn

Java: new ArrayList<>(list);
来源：http://wj.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ai.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://po.szsharing.cn

C#:   new List<int>(list);
来源：http://oi.hahajie.cn

[D23] reduce 累积计算
来源：http://pv.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://th.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qe.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vo.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rm.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ib.yuexingan06.cn

Go:   // 手写循环
来源：http://mz.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qa.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://en.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://cd.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hs.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ff.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fq.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dc.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vj.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cr.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wa.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://df.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://kp.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hq.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fd.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cs.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gw.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zg.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vk.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oj.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lx.asd995.cn

[D26] 数组转字符串
来源：http://eh.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://op.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://tg.521024.cn

JS:   arr.join(", ")
来源：http://vb.521024.cn

TS:   arr.join(", ")
来源：http://pt.hahajie.cn

Java: String.join(", ", list)
来源：http://qj.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://dd.hahajie.cn

Ruby: arr.join(", ")
来源：http://xl.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://ky.jianghongdianzi.cn

================================================================================
来源：http://by.9csxet.cn

E. 字符串处理
来源：http://ha.haigaiapp.cn

================================================================================
来源：http://jy.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://pc.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nu.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ko.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mm.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kr.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://es.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rb.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hl.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kz.panjiajie.cn

[E02] 重复字符串
来源：http://wb.nicolike.cn

Py:   "ab" * 3
来源：http://ws.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://rk.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://sr.szsharing.cn

TS:   "ab".repeat(3)
来源：http://lj.nszjky.cn

Java: "ab".repeat(3)
来源：http://ju.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://ov.wgjwhj.cn

Ruby: "ab" * 3
来源：http://dq.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dc.muxihuayi.cn

[E03] 截取子串
来源：http://dw.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mp.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yu.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yx.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://xs.gzmigu.cn

Java: s.substring(1, 4)
来源：http://hh.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nk.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vg.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://ry.szxytkj.cn

[E04] 查找子串位置
来源：http://wc.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://jt.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://sv.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ad.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://vj.hahajie.cn

Java: s.indexOf("x")
来源：http://yt.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://kf.bjjhwx.cn

Ruby: s.index("x")
来源：http://gh.colortex.cn

C#:   s.IndexOf("x")
来源：http://bm.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kk.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cn.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lp.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rt.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ze.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://br.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yz.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ce.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ja.colortex.cn

[E06] 替换子串
来源：http://kw.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tj.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://zs.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wh.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://li.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oe.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dj.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rf.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://hm.lnxyls.cn

[E07] 按分隔符拆分
来源：http://pg.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uh.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wz.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gf.521024.cn

TS:   s.split(",")
来源：http://yo.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ty.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kt.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://um.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cc.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://ti.nszjky.cn

Py:   ",".join(items)
来源：http://kj.huanxung.cn

PHP:  implode(",", $items);
来源：http://bb.bookmarksfly.cn

JS:   items.join(",")
来源：http://lh.hnjuh.cn

TS:   items.join(",")
来源：http://xg.bjjhwx.cn

Java: String.join(",", items)
来源：http://ot.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://df.gzmigu.cn

Ruby: items.join(",")
来源：http://yn.nicolike.cn

C#:   string.Join(",", items)
来源：http://ef.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://rz.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hu.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mr.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://ob.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://lo.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://xp.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wz.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xu.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://st.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://pc.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://em.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://il.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://yv.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://xz.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://kx.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xc.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fq.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bf.gzmigu.cn

[E11] 反转字符串
来源：http://fw.nszjky.cn

Py:   s[::-1]
来源：http://xn.colortex.cn

PHP:  strrev($s);
来源：http://ku.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://pt.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://id.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ia.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rk.nszjky.cn

Ruby: s.reverse
来源：http://ln.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ke.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://hu.huanxung.cn

Py:   s.count("a")
来源：http://ix.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://wu.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://ya.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://bl.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ga.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://cq.shxzukj.cn

Ruby: s.count("a")
来源：http://ef.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://vv.jctech888.com.cn

[E13] 逐字符遍历
来源：http://qv.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://ra.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sy.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fo.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lm.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iz.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pk.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rn.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dm.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://mr.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vn.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pv.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dh.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vo.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hi.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gv.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rz.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ps.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://yy.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://su.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ib.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zg.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ke.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://am.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vu.newstarts.cn


<!-- 参考信息 -->