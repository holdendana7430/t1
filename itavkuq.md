代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sp.haigaiapp.cn

Ruby: arr.sort
来源：http://ry.newstarts.cn

C#:   list.Sort();
来源：http://yw.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hf.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://po.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ep.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mg.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cg.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nh.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sc.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yd.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ie.9csxet.cn

[D11] 反转数组
来源：http://pj.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hx.huanxung.cn

PHP:  array_reverse($arr);
来源：http://lw.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bt.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://nj.huanxung.cn

Java: Collections.reverse(list);
来源：http://qi.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://by.9csxet.cn

Ruby: arr.reverse
来源：http://xv.yuexingan06.cn

C#:   list.Reverse();
来源：http://va.wgjwhj.cn

[D12] 查找元素下标
来源：http://ii.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://vv.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gb.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cw.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fy.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xf.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://ib.panjiajie.cn

Ruby: arr.index(x)
来源：http://cf.szsharing.cn

C#:   list.IndexOf(x);
来源：http://ka.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://hy.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yi.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ha.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://bw.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://ym.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dc.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bn.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xl.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pz.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://lj.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hr.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fw.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ch.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://gy.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hn.newstarts.cn

Go:   // 手写循环
来源：http://aa.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://id.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gk.haigaiapp.cn

[D15] 去重
来源：http://bm.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qb.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://ee.asd995.cn

JS:   [...new Set(arr)]
来源：http://mo.newstarts.cn

TS:   [...new Set(arr)]
来源：http://bn.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ck.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zf.huanxung.cn

Ruby: arr.uniq
来源：http://te.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://du.huixiangedu.cn

[D16] 求和与平均值
来源：http://ta.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iq.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wz.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fs.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jg.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jc.colortex.cn

Go:   // 手写循环累加
来源：http://me.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yg.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://fx.bjjhwx.cn

[D17] 最大值与最小值
来源：http://lv.colortex.cn

Py:   max(arr);  min(arr)
来源：http://eq.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://xb.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rb.nszjky.cn

TS:   Math.max(...arr);
来源：http://dh.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rb.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zh.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://sm.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://gn.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://qj.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ll.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://aw.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bw.huixiangedu.cn

TS:   nested.flat();
来源：http://zb.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yt.muxihuayi.cn

Go:   // 手写双层循环
来源：http://ut.szxytkj.cn

Ruby: nested.flatten
来源：http://mf.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yi.hnjuh.cn

[D19] 按字段分组
来源：http://hr.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bh.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xy.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sy.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lq.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ey.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://pr.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hf.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bv.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://lr.jctech888.com.cn

Py:   Counter(arr)
来源：http://pz.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://ld.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bo.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sx.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ck.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://nt.hnjuh.cn

Ruby: arr.tally
来源：http://rs.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cg.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://oe.huanxung.cn

Py:   x in arr
来源：http://nf.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://hj.9csxet.cn

JS:   arr.includes(x)
来源：http://ml.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://gs.bookmarksfly.cn

Java: list.contains(x)
来源：http://ny.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://sx.szxytkj.cn

Ruby: arr.include?(x)
来源：http://zl.szxytkj.cn

C#:   list.Contains(x)
来源：http://bm.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://eq.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ij.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oy.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jj.nicolike.cn

TS:   [...arr];
来源：http://yx.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://pq.szxytkj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sj.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://wn.521024.cn

C#:   new List<int>(list);
来源：http://mk.chemitech.net.cn

[D23] reduce 累积计算
来源：http://vc.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ox.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jt.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nt.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zx.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ib.colortex.cn

Go:   // 手写循环
来源：http://lx.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eq.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://it.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://xc.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cz.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vz.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ld.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fl.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fo.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lb.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tn.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rj.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://hx.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jw.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qm.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ij.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qm.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bb.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ie.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tg.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fn.gzmigu.cn

[D26] 数组转字符串
来源：http://xf.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://hw.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://hx.nszjky.cn

JS:   arr.join(", ")
来源：http://mm.shxzskj.cn

TS:   arr.join(", ")
来源：http://gl.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://qi.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://ep.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://dc.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://sb.nicolike.cn

================================================================================
来源：http://od.muxihuayi.cn

E. 字符串处理
来源：http://ww.chemitech.net.cn

================================================================================
来源：http://my.huixiangedu.cn

[E01] 拼接字符串
来源：http://ji.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ep.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dd.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iq.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ze.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dy.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jb.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kp.shtwfgs.cn

[E02] 重复字符串
来源：http://hz.colortex.cn

Py:   "ab" * 3
来源：http://gc.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://yf.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://cr.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://sh.shxzskj.cn

Java: "ab".repeat(3)
来源：http://wu.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://bj.shxzukj.cn

Ruby: "ab" * 3
来源：http://hx.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dr.szsharing.cn

[E03] 截取子串
来源：http://ud.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ge.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dx.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qi.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://es.gzmigu.cn

Java: s.substring(1, 4)
来源：http://hb.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nq.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nn.asd995.cn

C#:   s.Substring(1, 3)
来源：http://ex.jctech888.com.cn

[E04] 查找子串位置
来源：http://os.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://zz.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://hu.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gu.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://ej.szsharing.cn

Java: s.indexOf("x")
来源：http://ai.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://yy.bookmarksfly.cn

Ruby: s.index("x")
来源：http://si.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://bv.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oz.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://al.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gz.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://en.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sv.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zz.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xh.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hg.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qm.shxzskj.cn

[E06] 替换子串
来源：http://oc.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pr.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://mp.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mn.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://nw.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cz.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cq.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vs.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://tb.nszjky.cn

[E07] 按分隔符拆分
来源：http://ft.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yi.szsharing.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://od.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ob.hnjuh.cn

TS:   s.split(",")
来源：http://ae.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vq.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lv.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://pe.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qk.nszjky.cn

[E08] 数组按分隔符合并
来源：http://au.521024.cn

Py:   ",".join(items)
来源：http://qg.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://pb.szsharing.cn

JS:   items.join(",")
来源：http://yg.haigaiapp.cn

TS:   items.join(",")
来源：http://up.jctech888.com.cn

Java: String.join(",", items)
来源：http://pm.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://km.wgjwhj.cn

Ruby: items.join(",")
来源：http://ig.hnjuh.cn

C#:   string.Join(",", items)
来源：http://ih.hnjuh.cn

[E09] 去除所有空白字符
来源：http://fe.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lk.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nw.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://nd.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ic.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://nj.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cc.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jg.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://md.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://qk.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iw.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://og.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://uz.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://nl.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://vz.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hc.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dn.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qn.gzmigu.cn

[E11] 反转字符串
来源：http://ph.chemitech.net.cn

Py:   s[::-1]
来源：http://ex.haigaiapp.cn

PHP:  strrev($s);
来源：http://pg.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://wo.colortex.cn

TS:   [...s].reverse().join("")
来源：http://bq.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kn.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kv.shtwfgs.cn

Ruby: s.reverse
来源：http://bo.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://su.nicolike.cn

[E12] 统计某字符出现次数
来源：http://it.asd995.cn

Py:   s.count("a")
来源：http://oi.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://ih.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://sa.newstarts.cn

TS:   s.split("a").length - 1
来源：http://ec.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yd.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://mt.panjiajie.cn

Ruby: s.count("a")
来源：http://ys.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://it.muxihuayi.cn

[E13] 逐字符遍历
来源：http://zw.colortex.cn

Py:   for ch in s: print(ch)
来源：http://vm.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pi.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rw.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ih.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qr.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yk.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lb.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hi.hahajie.cn

[E14] URL 编码与 Base64
来源：http://ak.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sa.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cm.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tz.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rn.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kj.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gj.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uf.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sj.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://um.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vq.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bt.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kp.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yn.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xv.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yk.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yf.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ud.jianghongdianzi.cn

[E16] 数字千分位
来源：http://qm.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://ut.gzmigu.cn

PHP:  number_format(1234567);
来源：http://jj.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rh.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ky.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sb.huanxung.cn


<!-- 参考信息 -->