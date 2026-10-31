代发 wailian999

[D11] 反转数组
来源：http://mw.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dy.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://os.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wu.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://lo.huanxung.cn

Java: Collections.reverse(list);
来源：http://nv.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://cz.521024.cn

Ruby: arr.reverse
来源：http://ga.bookmarksfly.cn

C#:   list.Reverse();
来源：http://gd.panjiajie.cn

[D12] 查找元素下标
来源：http://we.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://pg.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://et.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sx.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://id.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ev.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://ga.newstarts.cn

Ruby: arr.index(x)
来源：http://gy.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://ba.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://bf.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yr.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ha.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://vc.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://md.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nt.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zu.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vz.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zc.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://hw.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jp.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zs.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://mj.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://yu.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://do.szsharing.cn

Go:   // 手写循环
来源：http://ph.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xe.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kn.muxihuayi.cn

[D15] 去重
来源：http://zd.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zf.nszjky.cn

PHP:  array_unique($arr);
来源：http://ch.newstarts.cn

JS:   [...new Set(arr)]
来源：http://gf.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://xo.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nv.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ch.bjjhwx.cn

Ruby: arr.uniq
来源：http://aq.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://mi.szsharing.cn

[D16] 求和与平均值
来源：http://kv.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hp.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qz.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://by.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sb.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qe.521024.cn

Go:   // 手写循环累加
来源：http://xp.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sp.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://vd.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://bz.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://wf.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://av.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ed.colortex.cn

TS:   Math.max(...arr);
来源：http://rr.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nu.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ro.521024.cn

Ruby: arr.max;  arr.min
来源：http://tk.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://bb.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://uy.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zq.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://hu.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ee.shtwfgs.cn

TS:   nested.flat();
来源：http://ge.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wt.yuexingan06.cn

Go:   // 手写双层循环
来源：http://fc.yuexingan06.cn

Ruby: nested.flatten
来源：http://wm.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oz.newstarts.cn

[D19] 按字段分组
来源：http://ei.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dk.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hp.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xq.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cx.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://np.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://tz.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gb.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uj.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://cr.haigaiapp.cn

Py:   Counter(arr)
来源：http://ii.huanxung.cn

PHP:  array_count_values($arr);
来源：http://zs.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sh.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kv.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qq.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://er.jianghongdianzi.cn

Ruby: arr.tally
来源：http://zw.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mq.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://gu.521024.cn

Py:   x in arr
来源：http://rz.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://eg.newstarts.cn

JS:   arr.includes(x)
来源：http://um.shtwfgs.cn

TS:   arr.includes(x)
来源：http://gb.colortex.cn

Java: list.contains(x)
来源：http://mt.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://dy.gzmigu.cn

Ruby: arr.include?(x)
来源：http://jp.jctech888.com.cn

C#:   list.Contains(x)
来源：http://yk.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://zt.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lt.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nw.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qq.huixiangedu.cn

TS:   [...arr];
来源：http://nn.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://ou.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yv.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://bg.nszjky.cn

C#:   new List<int>(list);
来源：http://ol.521024.cn

[D23] reduce 累积计算
来源：http://xy.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hv.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xd.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nc.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mn.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mg.521024.cn

Go:   // 手写循环
来源：http://cb.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kv.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hv.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://tu.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jw.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://me.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vu.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rg.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nx.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ks.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ju.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zj.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://po.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qp.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dq.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ay.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gh.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kg.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vw.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://by.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uh.huanxung.cn

[D26] 数组转字符串
来源：http://og.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://as.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://ex.9csxet.cn

JS:   arr.join(", ")
来源：http://wd.shxzukj.cn

TS:   arr.join(", ")
来源：http://oo.szsharing.cn

Java: String.join(", ", list)
来源：http://id.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://xh.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://sp.nszjky.cn

C#:   string.Join(", ", list)
来源：http://do.gzmigu.cn

================================================================================
来源：http://tu.521024.cn

E. 字符串处理
来源：http://ti.nicolike.cn

================================================================================
来源：http://mz.bjjhwx.cn

[E01] 拼接字符串
来源：http://pr.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ws.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yx.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lt.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vv.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rm.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kk.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dp.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bj.nszjky.cn

[E02] 重复字符串
来源：http://gy.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://cg.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://ix.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://lm.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://sr.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://rf.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://tt.newstarts.cn

Ruby: "ab" * 3
来源：http://ny.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ac.chemitech.net.cn

[E03] 截取子串
来源：http://qm.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wh.huanxung.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ve.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wa.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://il.hnjuh.cn

Java: s.substring(1, 4)
来源：http://fj.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://im.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mp.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://nd.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://yd.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://ml.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://at.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ej.colortex.cn

TS:   s.indexOf("x")
来源：http://gm.521024.cn

Java: s.indexOf("x")
来源：http://dp.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://hl.hahajie.cn

Ruby: s.index("x")
来源：http://ji.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://ty.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yl.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hd.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ob.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tn.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mc.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://st.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jj.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pf.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lh.newstarts.cn

[E06] 替换子串
来源：http://mz.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fy.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://tk.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ec.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://ec.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ff.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ak.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mb.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://mr.gzmigu.cn

[E07] 按分隔符拆分
来源：http://qu.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://se.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://et.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ro.nszjky.cn

TS:   s.split(",")
来源：http://il.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qe.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lf.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://hb.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qi.huanxung.cn

[E08] 数组按分隔符合并
来源：http://dt.chemitech.net.cn

Py:   ",".join(items)
来源：http://hf.9csxet.cn

PHP:  implode(",", $items);
来源：http://ki.jctech888.com.cn

JS:   items.join(",")
来源：http://vo.colortex.cn

TS:   items.join(",")
来源：http://ug.nszjky.cn

Java: String.join(",", items)
来源：http://cy.colortex.cn

Go:   strings.Join(items, ",")
来源：http://nz.nszjky.cn

Ruby: items.join(",")
来源：http://gh.nicolike.cn

C#:   string.Join(",", items)
来源：http://is.asd995.cn

[E09] 去除所有空白字符
来源：http://bn.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lx.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pj.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://wo.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://lb.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://ms.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vo.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gs.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tx.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://pg.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tl.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lb.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://vw.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://sq.newstarts.cn

Java: String.format("%03d", 7)
来源：http://rg.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sk.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ok.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://de.shtwfgs.cn

[E11] 反转字符串
来源：http://bc.chemitech.net.cn

Py:   s[::-1]
来源：http://rd.panjiajie.cn

PHP:  strrev($s);
来源：http://al.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://vz.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://mr.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cm.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jf.hnjuh.cn

Ruby: s.reverse
来源：http://vg.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ib.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://cy.haigaiapp.cn

Py:   s.count("a")
来源：http://ue.521024.cn

PHP:  substr_count($s, "a");
来源：http://be.9csxet.cn

JS:   s.split("a").length - 1
来源：http://og.szsharing.cn

TS:   s.split("a").length - 1
来源：http://rz.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rl.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://md.newstarts.cn

Ruby: s.count("a")
来源：http://po.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://le.nicolike.cn

[E13] 逐字符遍历
来源：http://kp.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://yj.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zr.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://il.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eh.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cy.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bg.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ny.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ic.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ip.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hy.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gf.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vy.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lb.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kz.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gb.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jb.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://py.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://mx.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kk.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bp.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mv.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eh.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xp.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ju.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eu.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vw.shtwfgs.cn

[E16] 数字千分位
来源：http://wy.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://py.gzmigu.cn

PHP:  number_format(1234567);
来源：http://vp.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pw.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dk.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dc.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ua.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yn.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://zo.shtwfgs.cn

[E17] 首字母大写
来源：http://gf.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ng.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ci.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wd.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qz.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://va.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dl.newstarts.cn

Ruby: s.capitalize
来源：http://ui.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vi.colortex.cn


<!-- 参考信息 -->