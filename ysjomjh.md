代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://gh.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://yp.colortex.cn

[D09] 排序（升序）
来源：http://hl.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://la.asd995.cn

PHP:  sort($arr);
来源：http://zt.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pl.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wm.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ie.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ut.gzmigu.cn

Ruby: arr.sort
来源：http://rx.yuntaijiaju.cn

C#:   list.Sort();
来源：http://ch.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zl.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dh.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pc.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ih.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xd.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gn.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bw.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zl.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tg.shtwfgs.cn

[D11] 反转数组
来源：http://mu.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://om.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://ib.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nq.newstarts.cn

TS:   [...arr].reverse();
来源：http://le.asd995.cn

Java: Collections.reverse(list);
来源：http://xt.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://fr.nicolike.cn

Ruby: arr.reverse
来源：http://lt.colortex.cn

C#:   list.Reverse();
来源：http://pc.bjjhwx.cn

[D12] 查找元素下标
来源：http://fa.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://it.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qj.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ml.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rl.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ny.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://ek.gzmigu.cn

Ruby: arr.index(x)
来源：http://fg.szsharing.cn

C#:   list.IndexOf(x);
来源：http://jm.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://wt.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pn.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vw.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://ye.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://mc.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uq.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jk.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kp.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tw.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://oh.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gv.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://in.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://xl.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://cn.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tc.hnjuh.cn

Go:   // 手写循环
来源：http://fs.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fo.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wy.szxytkj.cn

[D15] 去重
来源：http://do.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jg.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://ty.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://ri.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://tk.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kk.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zn.panjiajie.cn

Ruby: arr.uniq
来源：http://cl.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://su.yuexingan06.cn

[D16] 求和与平均值
来源：http://gl.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hj.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ri.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bu.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hw.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ti.huanxung.cn

Go:   // 手写循环累加
来源：http://qd.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hs.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://ez.hahajie.cn

[D17] 最大值与最小值
来源：http://jl.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://fk.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://yt.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ea.colortex.cn

TS:   Math.max(...arr);
来源：http://zy.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xf.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fk.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://pt.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://dx.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://dt.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lj.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://bx.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://en.asd995.cn

TS:   nested.flat();
来源：http://bh.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zh.muxihuayi.cn

Go:   // 手写双层循环
来源：http://zw.nszjky.cn

Ruby: nested.flatten
来源：http://xj.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kb.szxytkj.cn

[D19] 按字段分组
来源：http://vb.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pw.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mu.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vm.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ts.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xx.asd995.cn

Go:   // 手写 map[string][]T
来源：http://ro.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xn.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qk.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://ip.hnjuh.cn

Py:   Counter(arr)
来源：http://fk.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://xw.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gf.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bn.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://db.asd995.cn

Go:   // 手写 map[T]int
来源：http://dl.huixinmuqiang.cn

Ruby: arr.tally
来源：http://ol.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ub.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://ir.bookmarksfly.cn

Py:   x in arr
来源：http://wy.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://yo.huixiangedu.cn

JS:   arr.includes(x)
来源：http://ay.chemitech.net.cn

TS:   arr.includes(x)
来源：http://bw.9csxet.cn

Java: list.contains(x)
来源：http://jt.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://ov.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://pm.asd995.cn

C#:   list.Contains(x)
来源：http://kw.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://se.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ji.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kp.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qu.9csxet.cn

TS:   [...arr];
来源：http://pr.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://oc.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pb.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://ic.colortex.cn

C#:   new List<int>(list);
来源：http://ci.asd995.cn

[D23] reduce 累积计算
来源：http://vu.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://th.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wp.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oi.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ah.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lj.yuexingan06.cn

Go:   // 手写循环
来源：http://qp.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vk.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cw.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://lq.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pi.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ze.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ie.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xt.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wc.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sa.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pp.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gy.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://fo.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xi.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nm.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kr.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kl.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xi.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kn.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jq.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://py.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://pj.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://pb.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://dt.shtwfgs.cn

JS:   arr.join(", ")
来源：http://yy.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://qd.521024.cn

Java: String.join(", ", list)
来源：http://rb.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://bq.huanxung.cn

Ruby: arr.join(", ")
来源：http://qz.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://kg.colortex.cn

================================================================================
来源：http://cj.panjiajie.cn

E. 字符串处理
来源：http://oc.szsharing.cn

================================================================================
来源：http://xe.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://sy.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tw.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yz.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vo.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ox.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nu.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ty.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wu.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sg.newstarts.cn

[E02] 重复字符串
来源：http://fk.huixiangedu.cn

Py:   "ab" * 3
来源：http://ee.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://wf.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://vg.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://pk.asd995.cn

Java: "ab".repeat(3)
来源：http://ne.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://vv.haigaiapp.cn

Ruby: "ab" * 3
来源：http://fh.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cx.wgjwhj.cn

[E03] 截取子串
来源：http://ad.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hc.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vp.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ru.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://pa.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://uz.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qk.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ci.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://wi.hnjuh.cn

[E04] 查找子串位置
来源：http://xd.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://vv.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://mf.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ci.asd995.cn

TS:   s.indexOf("x")
来源：http://of.shxzukj.cn

Java: s.indexOf("x")
来源：http://jg.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://xk.shxzskj.cn

Ruby: s.index("x")
来源：http://zo.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://lz.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://so.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://js.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rz.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hn.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://op.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uc.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vb.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fp.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lr.colortex.cn

[E06] 替换子串
来源：http://ys.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lm.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://zx.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sn.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://jk.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bp.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eq.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ji.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://dl.szxytkj.cn

[E07] 按分隔符拆分
来源：http://bd.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yf.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jc.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wx.szxytkj.cn

TS:   s.split(",")
来源：http://qh.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://np.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gc.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://za.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://um.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://wj.shtwfgs.cn

Py:   ",".join(items)
来源：http://xa.shxzukj.cn

PHP:  implode(",", $items);
来源：http://pd.hnjuh.cn

JS:   items.join(",")
来源：http://kk.muxihuayi.cn

TS:   items.join(",")
来源：http://el.newstarts.cn

Java: String.join(",", items)
来源：http://js.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://hs.jctech888.com.cn

Ruby: items.join(",")
来源：http://bf.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://li.nszjky.cn

[E09] 去除所有空白字符
来源：http://vb.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ur.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ht.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://yj.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://sm.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://tr.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cu.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vy.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oy.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://il.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hc.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ds.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://ce.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://ld.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://ke.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ci.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vx.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tt.nszjky.cn

[E11] 反转字符串
来源：http://ly.jianghongdianzi.cn

Py:   s[::-1]
来源：http://yu.lnxyls.cn

PHP:  strrev($s);
来源：http://uv.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://am.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://ai.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sa.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fw.panjiajie.cn

Ruby: s.reverse
来源：http://fo.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fn.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://eo.szsharing.cn

Py:   s.count("a")
来源：http://eu.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://zg.521024.cn

JS:   s.split("a").length - 1
来源：http://yv.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://is.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uy.colortex.cn

Go:   strings.Count(s, "a")
来源：http://bd.szxytkj.cn

Ruby: s.count("a")
来源：http://ho.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://ww.huanxung.cn

[E13] 逐字符遍历
来源：http://zb.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://ep.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dq.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cr.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uf.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ig.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bi.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ig.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://or.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://rc.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ee.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jd.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://me.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oq.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ev.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://se.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ic.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gb.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://jw.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sl.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hq.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zo.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cd.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ay.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rf.yuexingan06.cn


<!-- 参考信息 -->