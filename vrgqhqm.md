代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bv.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hd.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bf.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vg.huixiangedu.cn

[D11] 反转数组
来源：http://sv.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qt.nszjky.cn

PHP:  array_reverse($arr);
来源：http://ld.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mx.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://am.panjiajie.cn

Java: Collections.reverse(list);
来源：http://gn.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://ne.bjjhwx.cn

Ruby: arr.reverse
来源：http://gx.panjiajie.cn

C#:   list.Reverse();
来源：http://hd.asd995.cn

[D12] 查找元素下标
来源：http://yb.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://gx.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zt.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mw.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fo.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sa.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://ms.shxzukj.cn

Ruby: arr.index(x)
来源：http://ni.hahajie.cn

C#:   list.IndexOf(x);
来源：http://oi.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://yl.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fs.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wf.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://qe.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://ij.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tu.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zb.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tv.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ax.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://pv.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ie.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lb.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://jx.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://lt.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://da.jianghongdianzi.cn

Go:   // 手写循环
来源：http://mk.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pw.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pr.yuntaijiaju.cn

[D15] 去重
来源：http://bb.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nx.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://uv.szsharing.cn

JS:   [...new Set(arr)]
来源：http://el.nszjky.cn

TS:   [...new Set(arr)]
来源：http://wk.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yy.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lk.hahajie.cn

Ruby: arr.uniq
来源：http://kl.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ok.bjjhwx.cn

[D16] 求和与平均值
来源：http://lw.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://go.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wh.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iu.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yo.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://us.nszjky.cn

Go:   // 手写循环累加
来源：http://tc.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tn.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://yr.panjiajie.cn

[D17] 最大值与最小值
来源：http://mz.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://sv.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://eh.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tj.shxzukj.cn

TS:   Math.max(...arr);
来源：http://fq.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fl.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fq.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://ji.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://gr.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://kk.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sc.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://cx.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qo.bjjhwx.cn

TS:   nested.flat();
来源：http://mt.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jh.wgjwhj.cn

Go:   // 手写双层循环
来源：http://eb.521024.cn

Ruby: nested.flatten
来源：http://hn.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xf.hahajie.cn

[D19] 按字段分组
来源：http://yz.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fm.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ow.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vo.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wm.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mg.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://di.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://az.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mm.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://ek.yuexingan06.cn

Py:   Counter(arr)
来源：http://st.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://er.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eh.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://se.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bw.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://vm.colortex.cn

Ruby: arr.tally
来源：http://id.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ly.asd995.cn

[D21] 判断是否包含某元素
来源：http://ny.9csxet.cn

Py:   x in arr
来源：http://vb.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://sn.muxihuayi.cn

JS:   arr.includes(x)
来源：http://wu.muxihuayi.cn

TS:   arr.includes(x)
来源：http://cd.huanxung.cn

Java: list.contains(x)
来源：http://zc.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://sk.jctech888.com.cn

Ruby: arr.include?(x)
来源：http://va.chemitech.net.cn

C#:   list.Contains(x)
来源：http://hk.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://mk.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ag.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oc.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vc.newstarts.cn

TS:   [...arr];
来源：http://ls.newstarts.cn

Java: new ArrayList<>(list);
来源：http://ku.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uo.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://yx.panjiajie.cn

C#:   new List<int>(list);
来源：http://de.shxzskj.cn

[D23] reduce 累积计算
来源：http://hv.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sx.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dh.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qh.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xx.shxzukj.cn

Go:   // 手写循环
来源：http://bn.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dw.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gw.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://bd.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hk.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://od.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vj.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zm.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tc.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vc.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kz.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tg.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://uw.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://le.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ke.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mr.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kg.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lk.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mp.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nl.jctech888.com.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bc.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ps.hnjuh.cn

Py:   ", ".join(map(str, arr))
来源：http://cy.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://dl.lnxyls.cn

JS:   arr.join(", ")
来源：http://jx.muxihuayi.cn

TS:   arr.join(", ")
来源：http://ot.521024.cn

Java: String.join(", ", list)
来源：http://eg.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://hs.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://na.szsharing.cn

C#:   string.Join(", ", list)
来源：http://dr.huixiangedu.cn

================================================================================
来源：http://oz.szxytkj.cn

E. 字符串处理
来源：http://ta.hahajie.cn

================================================================================
来源：http://pq.huanxung.cn

[E01] 拼接字符串
来源：http://ir.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hk.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cr.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qm.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eo.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mm.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bj.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jn.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rr.nicolike.cn

[E02] 重复字符串
来源：http://qn.huanxung.cn

Py:   "ab" * 3
来源：http://ye.huixiangedu.cn

PHP:  str_repeat("ab", 3);
来源：http://ca.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://an.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://qk.hahajie.cn

Java: "ab".repeat(3)
来源：http://yy.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://pb.gzmigu.cn

Ruby: "ab" * 3
来源：http://ix.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ha.shxzskj.cn

[E03] 截取子串
来源：http://km.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tt.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jr.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gw.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://zx.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://cy.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bj.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vx.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://gh.hahajie.cn

[E04] 查找子串位置
来源：http://qq.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://bg.colortex.cn

PHP:  strpos($s, "x");
来源：http://on.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kf.lnxyls.cn

TS:   s.indexOf("x")
来源：http://fy.bjjhwx.cn

Java: s.indexOf("x")
来源：http://do.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://ql.huanxung.cn

Ruby: s.index("x")
来源：http://fx.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://ml.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hy.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dg.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wm.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wg.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ss.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uu.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gq.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ef.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dj.jctech888.com.cn

[E06] 替换子串
来源：http://nv.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sp.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://cc.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yl.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://gy.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wa.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mt.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vk.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://cl.asd995.cn

[E07] 按分隔符拆分
来源：http://zx.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rs.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bh.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rn.wgjwhj.cn

TS:   s.split(",")
来源：http://bo.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tk.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nz.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://jb.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fv.hahajie.cn

[E08] 数组按分隔符合并
来源：http://cb.muxihuayi.cn

Py:   ",".join(items)
来源：http://yg.nszjky.cn

PHP:  implode(",", $items);
来源：http://we.szsharing.cn

JS:   items.join(",")
来源：http://mu.bjjhwx.cn

TS:   items.join(",")
来源：http://fl.huixiangedu.cn

Java: String.join(",", items)
来源：http://ff.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://yr.lnxyls.cn

Ruby: items.join(",")
来源：http://lf.hnjuh.cn

C#:   string.Join(",", items)
来源：http://vm.hnjuh.cn

[E09] 去除所有空白字符
来源：http://nm.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://su.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qu.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://rq.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://xp.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://zj.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://be.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ls.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kd.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://ys.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qo.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zp.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://vf.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://ja.asd995.cn

Java: String.format("%03d", 7)
来源：http://is.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bs.nicolike.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uk.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bk.wgjwhj.cn

[E11] 反转字符串
来源：http://oz.haigaiapp.cn

Py:   s[::-1]
来源：http://ai.yuexingan06.cn

PHP:  strrev($s);
来源：http://zw.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://ik.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://xn.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tk.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://if.chemitech.net.cn

Ruby: s.reverse
来源：http://ix.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ju.asd995.cn

[E12] 统计某字符出现次数
来源：http://pv.hnjuh.cn

Py:   s.count("a")
来源：http://ac.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://zi.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://dd.521024.cn

TS:   s.split("a").length - 1
来源：http://nt.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yc.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://hv.wgjwhj.cn

Ruby: s.count("a")
来源：http://om.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://xn.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://yv.colortex.cn

Py:   for ch in s: print(ch)
来源：http://lc.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wk.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nx.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mg.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ai.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tm.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ij.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ht.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://xk.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lq.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wv.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://as.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://br.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://te.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kd.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://no.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qa.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://og.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wn.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jc.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wy.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fp.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ew.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uw.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qk.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ml.newstarts.cn

[E16] 数字千分位
来源：http://bn.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://bk.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://sk.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fz.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yt.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yz.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ti.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ea.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://fu.bookmarksfly.cn

[E17] 首字母大写
来源：http://km.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bt.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nz.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bx.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.newstarts.cn


<!-- 参考信息 -->