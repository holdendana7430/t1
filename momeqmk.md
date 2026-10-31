代发 wailian999

[D11] 反转数组
来源：http://fu.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gl.lnxyls.cn

PHP:  array_reverse($arr);
来源：http://nz.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kd.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://jp.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://mf.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://tp.panjiajie.cn

Ruby: arr.reverse
来源：http://hb.hahajie.cn

C#:   list.Reverse();
来源：http://tv.lnxyls.cn

[D12] 查找元素下标
来源：http://ex.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://oe.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gt.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wo.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mg.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dm.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://zw.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://mb.huanxung.cn

C#:   list.IndexOf(x);
来源：http://fr.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://te.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://on.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nj.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://yw.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://vb.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fh.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qv.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pw.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oe.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://ip.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ux.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vd.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://xw.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://xn.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xk.chemitech.net.cn

Go:   // 手写循环
来源：http://fa.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lj.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ep.wgjwhj.cn

[D15] 去重
来源：http://gv.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cq.panjiajie.cn

PHP:  array_unique($arr);
来源：http://by.hahajie.cn

JS:   [...new Set(arr)]
来源：http://xd.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://aa.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jn.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://my.lnxyls.cn

Ruby: arr.uniq
来源：http://zl.521024.cn

C#:   list.Distinct().ToList()
来源：http://ps.huanxung.cn

[D16] 求和与平均值
来源：http://uh.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ba.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xr.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://su.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jp.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xc.asd995.cn

Go:   // 手写循环累加
来源：http://bz.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kj.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://tk.haigaiapp.cn

[D17] 最大值与最小值
来源：http://ap.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://fk.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ka.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://db.szsharing.cn

TS:   Math.max(...arr);
来源：http://xc.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bd.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lf.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://os.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://uj.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://ni.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fx.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://ns.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jx.panjiajie.cn

TS:   nested.flat();
来源：http://tx.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jk.colortex.cn

Go:   // 手写双层循环
来源：http://vw.nicolike.cn

Ruby: nested.flatten
来源：http://tu.shtwfgs.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://su.nicolike.cn

[D19] 按字段分组
来源：http://sx.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sx.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ub.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jd.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qe.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pv.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://qh.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ya.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ms.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://lo.colortex.cn

Py:   Counter(arr)
来源：http://vi.nszjky.cn

PHP:  array_count_values($arr);
来源：http://yw.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yl.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yh.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lk.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://lx.jianghongdianzi.cn

Ruby: arr.tally
来源：http://gj.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vf.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://rs.9csxet.cn

Py:   x in arr
来源：http://ka.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://bi.szsharing.cn

JS:   arr.includes(x)
来源：http://gh.nszjky.cn

TS:   arr.includes(x)
来源：http://fn.lnxyls.cn

Java: list.contains(x)
来源：http://qf.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://sb.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://fk.asd995.cn

C#:   list.Contains(x)
来源：http://cw.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://aa.lnxyls.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qd.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://md.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dt.gzmigu.cn

TS:   [...arr];
来源：http://ib.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ey.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nn.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://vk.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://ts.gzmigu.cn

[D23] reduce 累积计算
来源：http://ri.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ny.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lj.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jb.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pv.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://es.colortex.cn

Go:   // 手写循环
来源：http://hc.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mz.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cx.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://my.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sk.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vv.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lc.bookmarksfly.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cp.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zy.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gs.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vz.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jr.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://me.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gg.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://so.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qf.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zv.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rw.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gm.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ye.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vq.asd995.cn

[D26] 数组转字符串
来源：http://ja.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://hk.asd995.cn

PHP:  implode(", ", $arr);
来源：http://vl.asd995.cn

JS:   arr.join(", ")
来源：http://bl.haigaiapp.cn

TS:   arr.join(", ")
来源：http://qi.shxzukj.cn

Java: String.join(", ", list)
来源：http://ag.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://zs.521024.cn

Ruby: arr.join(", ")
来源：http://id.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://iz.shxzskj.cn

================================================================================
来源：http://vp.bjjhwx.cn

E. 字符串处理
来源：http://eu.lnxyls.cn

================================================================================
来源：http://ns.huanxung.cn

[E01] 拼接字符串
来源：http://hy.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ar.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nb.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oq.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ap.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cl.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cv.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tw.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bf.szsharing.cn

[E02] 重复字符串
来源：http://qw.muxihuayi.cn

Py:   "ab" * 3
来源：http://gt.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://lg.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://yr.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://ll.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://bd.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://xc.huixiangedu.cn

Ruby: "ab" * 3
来源：http://kh.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://si.hahajie.cn

[E03] 截取子串
来源：http://xg.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xp.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gm.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fe.nszjky.cn

TS:   s.slice(1, 4)
来源：http://xy.9csxet.cn

Java: s.substring(1, 4)
来源：http://ka.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jr.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vx.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://bm.colortex.cn

[E04] 查找子串位置
来源：http://iq.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://wi.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://et.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yb.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://mj.hnjuh.cn

Java: s.indexOf("x")
来源：http://vd.colortex.cn

Go:   strings.Index(s, "x")
来源：http://ci.hnjuh.cn

Ruby: s.index("x")
来源：http://dk.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://nc.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yz.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wv.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ch.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kj.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zo.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hr.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uy.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qg.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ph.colortex.cn

[E06] 替换子串
来源：http://jh.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://po.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://mh.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mp.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://fe.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uy.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fl.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sv.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://qf.nicolike.cn

[E07] 按分隔符拆分
来源：http://ey.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ac.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://la.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pr.huixinmuqiang.cn

TS:   s.split(",")
来源：http://tf.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ra.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aa.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://vr.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kb.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://fe.gzmigu.cn

Py:   ",".join(items)
来源：http://vj.szsharing.cn

PHP:  implode(",", $items);
来源：http://kz.shxzskj.cn

JS:   items.join(",")
来源：http://bq.chemitech.net.cn

TS:   items.join(",")
来源：http://dy.521024.cn

Java: String.join(",", items)
来源：http://ta.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://jx.huixiangedu.cn

Ruby: items.join(",")
来源：http://np.asd995.cn

C#:   string.Join(",", items)
来源：http://ni.szsharing.cn

[E09] 去除所有空白字符
来源：http://zy.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qj.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://df.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://dt.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://oa.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://by.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nw.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iu.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kq.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://ct.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sn.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wl.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://gb.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://mm.9csxet.cn

Java: String.format("%03d", 7)
来源：http://dr.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qh.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xt.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://za.huixiangedu.cn

[E11] 反转字符串
来源：http://dr.yuexingan06.cn

Py:   s[::-1]
来源：http://ty.jctech888.com.cn

PHP:  strrev($s);
来源：http://qc.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://ss.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://cb.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hi.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bn.huixinmuqiang.cn

Ruby: s.reverse
来源：http://gr.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sq.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://zm.panjiajie.cn

Py:   s.count("a")
来源：http://gg.colortex.cn

PHP:  substr_count($s, "a");
来源：http://sm.hahajie.cn

JS:   s.split("a").length - 1
来源：http://vt.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://ml.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rm.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://tf.asd995.cn

Ruby: s.count("a")
来源：http://jn.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://rl.hnjuh.cn

[E13] 逐字符遍历
来源：http://hv.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://ub.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://le.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://it.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qc.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ks.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yt.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ox.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mv.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://qq.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bm.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cg.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fu.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://je.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qe.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ib.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gq.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://fs.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bz.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ee.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wl.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pg.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rg.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qt.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hq.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cz.hahajie.cn

[E16] 数字千分位
来源：http://ta.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://gu.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://kr.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yy.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ya.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jf.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xm.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mx.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://lc.nicolike.cn

[E17] 首字母大写
来源：http://nh.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qn.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zh.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lq.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hg.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tq.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cr.shxzskj.cn

Ruby: s.capitalize
来源：http://ej.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://de.chemitech.net.cn


<!-- 参考信息 -->