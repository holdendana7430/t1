代发 wailian999

C#:   list.Reverse();
来源：http://xa.shxzskj.cn

[D12] 查找元素下标
来源：http://wp.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ua.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://it.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tm.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ct.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vb.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://by.colortex.cn

Ruby: arr.index(x)
来源：http://ur.asd995.cn

C#:   list.IndexOf(x);
来源：http://zc.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://la.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://td.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://de.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://ub.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://mz.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zm.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fx.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mp.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zk.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://cj.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sl.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mo.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://kv.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://vp.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wz.jianghongdianzi.cn

Go:   // 手写循环
来源：http://ah.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fp.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yi.shxzskj.cn

[D15] 去重
来源：http://gr.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ub.huanxung.cn

PHP:  array_unique($arr);
来源：http://oj.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://in.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://rd.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lm.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qv.colortex.cn

Ruby: arr.uniq
来源：http://sh.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://cc.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://cc.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dn.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://az.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rz.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pr.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wb.lnxyls.cn

Go:   // 手写循环累加
来源：http://ir.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fj.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://uz.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://yd.521024.cn

Py:   max(arr);  min(arr)
来源：http://dh.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://vm.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://us.szsharing.cn

TS:   Math.max(...arr);
来源：http://sq.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wg.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pg.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://yw.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://xr.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://nd.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vo.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://cl.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ow.szsharing.cn

TS:   nested.flat();
来源：http://ic.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rt.colortex.cn

Go:   // 手写双层循环
来源：http://le.chemitech.net.cn

Ruby: nested.flatten
来源：http://xj.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://aq.hnjuh.cn

[D19] 按字段分组
来源：http://mt.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ts.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tk.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oe.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oy.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gx.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://fx.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://od.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zv.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://al.szsharing.cn

Py:   Counter(arr)
来源：http://nb.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://fx.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bh.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gi.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fq.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://sc.lnxyls.cn

Ruby: arr.tally
来源：http://af.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ss.nszjky.cn

[D21] 判断是否包含某元素
来源：http://pq.nicolike.cn

Py:   x in arr
来源：http://fh.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://wb.nszjky.cn

JS:   arr.includes(x)
来源：http://zo.colortex.cn

TS:   arr.includes(x)
来源：http://ox.newstarts.cn

Java: list.contains(x)
来源：http://bh.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://ja.hahajie.cn

Ruby: arr.include?(x)
来源：http://qi.nicolike.cn

C#:   list.Contains(x)
来源：http://ze.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://dn.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nn.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qj.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qu.lnxyls.cn

TS:   [...arr];
来源：http://gy.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://cm.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jd.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://dr.yuexingan06.cn

C#:   new List<int>(list);
来源：http://pj.hahajie.cn

[D23] reduce 累积计算
来源：http://tx.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rs.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nm.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dp.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ui.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ll.shxzskj.cn

Go:   // 手写循环
来源：http://vd.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ko.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ql.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://uh.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lj.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kt.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vf.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vt.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://li.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mf.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wt.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vi.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://fa.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ms.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zu.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pt.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cj.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://va.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uo.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://un.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xc.muxihuayi.cn

[D26] 数组转字符串
来源：http://hs.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://ms.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://lb.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://jo.shtwfgs.cn

TS:   arr.join(", ")
来源：http://qv.gzmigu.cn

Java: String.join(", ", list)
来源：http://hz.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://eq.gzmigu.cn

Ruby: arr.join(", ")
来源：http://kl.asd995.cn

C#:   string.Join(", ", list)
来源：http://qz.asd995.cn

================================================================================
来源：http://tk.bjjhwx.cn

E. 字符串处理
来源：http://eo.huixinmuqiang.cn

================================================================================
来源：http://sq.lnxyls.cn

[E01] 拼接字符串
来源：http://mo.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uq.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zq.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iu.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xv.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zd.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vu.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vz.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ay.yuexingan06.cn

[E02] 重复字符串
来源：http://ju.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://xf.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://mq.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://iz.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://wi.shxzskj.cn

Java: "ab".repeat(3)
来源：http://lr.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://sf.nicolike.cn

Ruby: "ab" * 3
来源：http://nt.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nt.yuexingan06.cn

[E03] 截取子串
来源：http://nm.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hc.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qb.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ft.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://xs.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://wa.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ss.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pl.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://ga.haigaiapp.cn

[E04] 查找子串位置
来源：http://qy.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://fq.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://kt.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ki.hahajie.cn

TS:   s.indexOf("x")
来源：http://np.chemitech.net.cn

Java: s.indexOf("x")
来源：http://vz.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://ob.lnxyls.cn

Ruby: s.index("x")
来源：http://xa.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://sk.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sd.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gl.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gf.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://er.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nm.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ob.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fi.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xa.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eg.panjiajie.cn

[E06] 替换子串
来源：http://de.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pz.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://zb.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qj.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://bz.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bw.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rv.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://da.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://ie.szxytkj.cn

[E07] 按分隔符拆分
来源：http://lq.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ck.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rl.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lz.szxytkj.cn

TS:   s.split(",")
来源：http://pv.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jd.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://en.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://zo.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hc.9csxet.cn

[E08] 数组按分隔符合并
来源：http://nz.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://yc.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://sg.huixinmuqiang.cn

JS:   items.join(",")
来源：http://qn.szsharing.cn

TS:   items.join(",")
来源：http://re.gzmigu.cn

Java: String.join(",", items)
来源：http://uc.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://wx.asd995.cn

Ruby: items.join(",")
来源：http://fd.gzmigu.cn

C#:   string.Join(",", items)
来源：http://iq.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://cq.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ui.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hv.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://ng.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://dc.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://pe.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qw.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sy.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://we.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://fv.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ie.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gg.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://ko.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://fo.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://cl.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mq.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tc.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wd.jctech888.com.cn

[E11] 反转字符串
来源：http://jq.jianghongdianzi.cn

Py:   s[::-1]
来源：http://hn.gzmigu.cn

PHP:  strrev($s);
来源：http://od.colortex.cn

JS:   [...s].reverse().join("")
来源：http://uw.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://wf.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zp.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ak.haigaiapp.cn

Ruby: s.reverse
来源：http://us.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vg.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://pj.shtwfgs.cn

Py:   s.count("a")
来源：http://rf.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://ap.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://zq.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://id.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vo.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://fr.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://gr.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://vg.9csxet.cn

[E13] 逐字符遍历
来源：http://gc.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://ps.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ik.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://po.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xd.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ne.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fp.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://op.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ot.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://hk.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cf.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://me.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://os.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pi.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qs.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://le.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rp.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qz.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://kn.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ps.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ra.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wb.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lm.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zd.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hl.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ij.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zk.huixiangedu.cn

[E16] 数字千分位
来源：http://ub.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://es.szxytkj.cn

PHP:  number_format(1234567);
来源：http://se.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bi.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bc.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wm.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qu.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jp.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://it.szsharing.cn

[E17] 首字母大写
来源：http://yd.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rg.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nr.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nc.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xp.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nd.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bf.haigaiapp.cn

Ruby: s.capitalize
来源：http://pe.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xw.huanxung.cn

[E18] 模板占位符替换
来源：http://nr.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rk.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pq.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bo.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kx.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://he.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ya.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bl.bookmarksfly.cn


<!-- 参考信息 -->