代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://on.asd995.cn

Ruby: arr.sort
来源：http://bq.yuntaijiaju.cn

C#:   list.Sort();
来源：http://la.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yb.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://as.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pj.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ko.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ma.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kb.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pf.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vv.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mp.jctech888.com.cn

[D11] 反转数组
来源：http://un.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ca.huanxung.cn

PHP:  array_reverse($arr);
来源：http://hc.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wn.9csxet.cn

TS:   [...arr].reverse();
来源：http://ip.huanxung.cn

Java: Collections.reverse(list);
来源：http://qb.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://er.wgjwhj.cn

Ruby: arr.reverse
来源：http://ea.chemitech.net.cn

C#:   list.Reverse();
来源：http://jc.hahajie.cn

[D12] 查找元素下标
来源：http://dl.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://pn.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iy.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tc.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lj.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xu.colortex.cn

Go:   slices.Index(arr, x)
来源：http://co.wgjwhj.cn

Ruby: arr.index(x)
来源：http://zq.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://aa.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://tt.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wj.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ec.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://tk.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://tm.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vo.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ws.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ga.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wf.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://vf.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vd.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ub.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://tn.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://hw.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bz.bjjhwx.cn

Go:   // 手写循环
来源：http://cp.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nz.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bx.shxzukj.cn

[D15] 去重
来源：http://yq.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ca.colortex.cn

PHP:  array_unique($arr);
来源：http://kj.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ao.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://pp.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xk.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gl.shtwfgs.cn

Ruby: arr.uniq
来源：http://tt.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://mx.hahajie.cn

[D16] 求和与平均值
来源：http://og.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gb.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fu.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yy.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mt.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nm.newstarts.cn

Go:   // 手写循环累加
来源：http://rq.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fb.521024.cn

C#:   list.Sum();  list.Average()
来源：http://wx.yuexingan06.cn

[D17] 最大值与最小值
来源：http://sg.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://af.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://yi.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zp.521024.cn

TS:   Math.max(...arr);
来源：http://rh.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sv.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ke.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://tl.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://nw.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://uk.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yv.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://sp.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ec.yuntaijiaju.cn

TS:   nested.flat();
来源：http://vx.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bz.colortex.cn

Go:   // 手写双层循环
来源：http://ny.bookmarksfly.cn

Ruby: nested.flatten
来源：http://bi.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://od.bookmarksfly.cn

[D19] 按字段分组
来源：http://sc.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zl.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://te.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dc.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ux.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fm.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://zw.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dv.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mn.asd995.cn

[D20] 统计每个元素出现次数
来源：http://vx.szxytkj.cn

Py:   Counter(arr)
来源：http://yo.521024.cn

PHP:  array_count_values($arr);
来源：http://dv.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://po.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://he.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cz.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://wl.jctech888.com.cn

Ruby: arr.tally
来源：http://xm.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mw.huanxung.cn

[D21] 判断是否包含某元素
来源：http://iv.9csxet.cn

Py:   x in arr
来源：http://mc.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://hk.colortex.cn

JS:   arr.includes(x)
来源：http://if.gzmigu.cn

TS:   arr.includes(x)
来源：http://pw.shxzskj.cn

Java: list.contains(x)
来源：http://mo.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://wf.521024.cn

Ruby: arr.include?(x)
来源：http://ha.shxzukj.cn

C#:   list.Contains(x)
来源：http://vq.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://dc.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ib.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fx.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xc.shxzskj.cn

TS:   [...arr];
来源：http://zp.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://hm.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ss.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://rj.huixiangedu.cn

C#:   new List<int>(list);
来源：http://it.gzmigu.cn

[D23] reduce 累积计算
来源：http://bh.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rq.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qo.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vk.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tx.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ou.hahajie.cn

Go:   // 手写循环
来源：http://be.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://do.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lb.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://dr.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hw.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xo.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mf.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ia.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eg.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mg.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://va.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dt.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://sl.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kt.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ck.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://he.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nm.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qq.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sy.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eu.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jq.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://bu.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://bl.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://lx.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://lr.wgjwhj.cn

TS:   arr.join(", ")
来源：http://ap.nszjky.cn

Java: String.join(", ", list)
来源：http://as.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://jx.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://ua.huanxung.cn

C#:   string.Join(", ", list)
来源：http://vv.lnxyls.cn

================================================================================
来源：http://jd.yuntaijiaju.cn

E. 字符串处理
来源：http://rz.nicolike.cn

================================================================================
来源：http://zd.muxihuayi.cn

[E01] 拼接字符串
来源：http://kg.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sl.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tx.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nm.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://go.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gb.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wq.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qk.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sm.yuntaijiaju.cn

[E02] 重复字符串
来源：http://cv.shxzskj.cn

Py:   "ab" * 3
来源：http://xm.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://pe.huanxung.cn

JS:   "ab".repeat(3)
来源：http://dm.9csxet.cn

TS:   "ab".repeat(3)
来源：http://io.521024.cn

Java: "ab".repeat(3)
来源：http://bb.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://bc.lnxyls.cn

Ruby: "ab" * 3
来源：http://eg.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zw.bjjhwx.cn

[E03] 截取子串
来源：http://sa.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bn.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ce.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ei.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://my.hnjuh.cn

Java: s.substring(1, 4)
来源：http://hz.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zs.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xz.521024.cn

C#:   s.Substring(1, 3)
来源：http://iw.wgjwhj.cn

[E04] 查找子串位置
来源：http://bu.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://ti.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://pm.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jg.panjiajie.cn

TS:   s.indexOf("x")
来源：http://up.jianghongdianzi.cn

Java: s.indexOf("x")
来源：http://xa.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://hx.huixiangedu.cn

Ruby: s.index("x")
来源：http://eu.colortex.cn

C#:   s.IndexOf("x")
来源：http://my.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nq.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yr.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ik.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hy.huixinmuqiang.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gu.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vh.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ce.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tp.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://th.szsharing.cn

[E06] 替换子串
来源：http://kq.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://om.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://nd.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hg.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://gr.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wl.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vg.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://je.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://hj.lnxyls.cn

[E07] 按分隔符拆分
来源：http://gs.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lt.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://td.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ut.wgjwhj.cn

TS:   s.split(",")
来源：http://pd.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nw.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vv.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://yy.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oz.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://ca.lnxyls.cn

Py:   ",".join(items)
来源：http://il.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://kr.newstarts.cn

JS:   items.join(",")
来源：http://nd.lnxyls.cn

TS:   items.join(",")
来源：http://pt.yuexingan06.cn

Java: String.join(",", items)
来源：http://hm.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://jt.521024.cn

Ruby: items.join(",")
来源：http://fr.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://zh.hnjuh.cn

[E09] 去除所有空白字符
来源：http://hb.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pb.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iy.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://js.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://gu.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://ea.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://by.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://py.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kz.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://tu.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://av.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ze.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://sl.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://ch.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://zl.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oy.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://es.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bn.yuntaijiaju.cn

[E11] 反转字符串
来源：http://tm.jctech888.com.cn

Py:   s[::-1]
来源：http://ba.yuexingan06.cn

PHP:  strrev($s);
来源：http://jb.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://ao.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://xu.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rk.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gj.asd995.cn

Ruby: s.reverse
来源：http://pq.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wp.colortex.cn

[E12] 统计某字符出现次数
来源：http://vt.panjiajie.cn

Py:   s.count("a")
来源：http://vn.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://vm.nicolike.cn

JS:   s.split("a").length - 1
来源：http://wz.huanxung.cn

TS:   s.split("a").length - 1
来源：http://xe.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aa.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://pw.shxzskj.cn

Ruby: s.count("a")
来源：http://rm.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://ut.wgjwhj.cn

[E13] 逐字符遍历
来源：http://pa.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://zs.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wf.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bs.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vo.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ql.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tm.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hl.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://ie.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://se.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kn.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jd.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uv.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tv.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cj.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cq.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hw.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://wb.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rp.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pv.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wc.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oy.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bb.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://az.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bg.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oo.jctech888.com.cn

[E16] 数字千分位
来源：http://xw.szsharing.cn

Py:   f"{1234567:,}"
来源：http://iz.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://ik.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aa.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bk.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wj.colortex.cn


<!-- 参考信息 -->