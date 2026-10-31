代发 wailian999

TS:   [...arr].reverse();
来源：http://rr.szxytkj.cn

Java: Collections.reverse(list);
来源：http://wo.521024.cn

Go:   slices.Reverse(arr)
来源：http://aq.521024.cn

Ruby: arr.reverse
来源：http://lz.shtwfgs.cn

C#:   list.Reverse();
来源：http://mm.bjjhwx.cn

[D12] 查找元素下标
来源：http://bk.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://ml.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jc.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://er.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dw.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://ss.bjjhwx.cn

Ruby: arr.index(x)
来源：http://is.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://di.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://fg.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ix.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fy.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://wo.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://ud.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yw.haigaiapp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kj.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gz.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tu.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://fn.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dv.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gr.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://qm.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://yp.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yq.jianghongdianzi.cn

Go:   // 手写循环
来源：http://xd.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xi.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mx.szsharing.cn

[D15] 去重
来源：http://qh.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mw.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://sc.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://cl.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://qb.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ut.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tn.colortex.cn

Ruby: arr.uniq
来源：http://zi.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://rr.shxzukj.cn

[D16] 求和与平均值
来源：http://ei.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ov.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qs.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nu.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://po.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tu.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://qr.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://av.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://ed.haigaiapp.cn

[D17] 最大值与最小值
来源：http://or.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://fv.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://wc.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gi.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://uc.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tf.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mj.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://kb.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://io.colortex.cn

[D18] 扁平化嵌套数组
来源：http://rf.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lt.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://ff.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oh.lnxyls.cn

TS:   nested.flat();
来源：http://om.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ek.hnjuh.cn

Go:   // 手写双层循环
来源：http://kc.nicolike.cn

Ruby: nested.flatten
来源：http://hb.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zh.bookmarksfly.cn

[D19] 按字段分组
来源：http://fs.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eu.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cd.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cs.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vu.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qm.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://zl.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ir.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nl.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://re.jctech888.com.cn

Py:   Counter(arr)
来源：http://vf.szsharing.cn

PHP:  array_count_values($arr);
来源：http://dy.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ru.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rs.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fz.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://uv.chemitech.net.cn

Ruby: arr.tally
来源：http://wn.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ar.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://uv.shxzukj.cn

Py:   x in arr
来源：http://tf.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://ys.9csxet.cn

JS:   arr.includes(x)
来源：http://ju.bjjhwx.cn

TS:   arr.includes(x)
来源：http://ea.lnxyls.cn

Java: list.contains(x)
来源：http://un.521024.cn

Go:   slices.Contains(arr, x)
来源：http://cp.shxzskj.cn

Ruby: arr.include?(x)
来源：http://nt.panjiajie.cn

C#:   list.Contains(x)
来源：http://za.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://br.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://si.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tx.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oz.colortex.cn

TS:   [...arr];
来源：http://wy.nicolike.cn

Java: new ArrayList<>(list);
来源：http://us.521024.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ls.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://ql.9csxet.cn

C#:   new List<int>(list);
来源：http://el.9csxet.cn

[D23] reduce 累积计算
来源：http://nh.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ar.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ix.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zr.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hh.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yy.colortex.cn

Go:   // 手写循环
来源：http://jl.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pd.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gx.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://se.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ta.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tt.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fw.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yx.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ko.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mx.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://di.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wt.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://ir.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://td.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wl.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jj.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mn.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ne.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://js.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nt.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://up.huanxung.cn

[D26] 数组转字符串
来源：http://pe.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://dg.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://xw.panjiajie.cn

JS:   arr.join(", ")
来源：http://sh.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://ra.nicolike.cn

Java: String.join(", ", list)
来源：http://ga.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://dt.panjiajie.cn

Ruby: arr.join(", ")
来源：http://op.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://dn.haigaiapp.cn

================================================================================
来源：http://ku.jctech888.com.cn

E. 字符串处理
来源：http://sm.muxihuayi.cn

================================================================================
来源：http://wp.nszjky.cn

[E01] 拼接字符串
来源：http://nn.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yi.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rh.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://op.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zh.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ce.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ok.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jx.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pu.szxytkj.cn

[E02] 重复字符串
来源：http://mq.panjiajie.cn

Py:   "ab" * 3
来源：http://qo.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://ol.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://mw.newstarts.cn

TS:   "ab".repeat(3)
来源：http://cn.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://ev.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://vf.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://nh.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qr.521024.cn

[E03] 截取子串
来源：http://kt.gzmigu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ub.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jt.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iq.asd995.cn

TS:   s.slice(1, 4)
来源：http://sh.hnjuh.cn

Java: s.substring(1, 4)
来源：http://vt.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jx.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pf.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://oh.lnxyls.cn

[E04] 查找子串位置
来源：http://mn.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://fm.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://zf.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gx.9csxet.cn

TS:   s.indexOf("x")
来源：http://gh.shxzukj.cn

Java: s.indexOf("x")
来源：http://pc.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://ul.chemitech.net.cn

Ruby: s.index("x")
来源：http://gq.newstarts.cn

C#:   s.IndexOf("x")
来源：http://lb.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ur.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bs.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ln.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oe.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tl.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ox.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jy.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wl.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eh.gzmigu.cn

[E06] 替换子串
来源：http://li.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ur.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://wo.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://us.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://dx.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zp.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ah.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lm.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://nc.gzmigu.cn

[E07] 按分隔符拆分
来源：http://je.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vv.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ea.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://im.yuexingan06.cn

TS:   s.split(",")
来源：http://qd.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mn.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vn.hahajie.cn

Ruby: s.split(",");  s.split
来源：http://sf.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ps.huanxung.cn

[E08] 数组按分隔符合并
来源：http://eu.muxihuayi.cn

Py:   ",".join(items)
来源：http://kt.lnxyls.cn

PHP:  implode(",", $items);
来源：http://bz.szxytkj.cn

JS:   items.join(",")
来源：http://zw.yuexingan06.cn

TS:   items.join(",")
来源：http://ud.gzmigu.cn

Java: String.join(",", items)
来源：http://cz.asd995.cn

Go:   strings.Join(items, ",")
来源：http://kk.nszjky.cn

Ruby: items.join(",")
来源：http://nu.lnxyls.cn

C#:   string.Join(",", items)
来源：http://wc.shxzukj.cn

[E09] 去除所有空白字符
来源：http://cs.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sd.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pc.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://bw.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://rv.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ln.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sa.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oo.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qi.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://lo.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cg.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cr.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://tt.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://am.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://oj.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fa.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gp.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jr.lnxyls.cn

[E11] 反转字符串
来源：http://ex.bookmarksfly.cn

Py:   s[::-1]
来源：http://kv.huixiangedu.cn

PHP:  strrev($s);
来源：http://ms.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://tc.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://xf.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ho.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qy.gzmigu.cn

Ruby: s.reverse
来源：http://zw.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jy.nicolike.cn

[E12] 统计某字符出现次数
来源：http://cp.yuntaijiaju.cn

Py:   s.count("a")
来源：http://gt.asd995.cn

PHP:  substr_count($s, "a");
来源：http://bd.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://kx.nicolike.cn

TS:   s.split("a").length - 1
来源：http://lg.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zj.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://so.gzmigu.cn

Ruby: s.count("a")
来源：http://ce.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://qs.9csxet.cn

[E13] 逐字符遍历
来源：http://hi.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://ts.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gh.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ik.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bq.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kr.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ss.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rb.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aj.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://pg.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yt.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mh.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ht.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ap.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://in.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dq.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wl.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fz.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://yr.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bm.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oi.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mo.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yj.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ps.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xi.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dr.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fa.colortex.cn

[E16] 数字千分位
来源：http://sy.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://mo.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://kn.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://et.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tb.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sb.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xc.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://if.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://ab.hnjuh.cn

[E17] 首字母大写
来源：http://gu.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gx.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lb.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://la.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uh.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ni.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lq.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://af.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bd.huanxung.cn

[E18] 模板占位符替换
来源：http://gw.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bx.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pr.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ra.wgjwhj.cn


<!-- 参考信息 -->