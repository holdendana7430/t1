代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jx.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lp.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hg.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://se.nszjky.cn

[D11] 反转数组
来源：http://ga.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dh.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://lb.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wh.nicolike.cn

TS:   [...arr].reverse();
来源：http://yl.szsharing.cn

Java: Collections.reverse(list);
来源：http://wn.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://cr.chemitech.net.cn

Ruby: arr.reverse
来源：http://hf.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://fs.huixiangedu.cn

[D12] 查找元素下标
来源：http://ef.521024.cn

Py:   arr.index(x);  x in arr
来源：http://re.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zy.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tp.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bp.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://os.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://la.shtwfgs.cn

Ruby: arr.index(x)
来源：http://yl.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://mp.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://ck.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dd.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vc.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://eo.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://vh.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nd.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gy.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dl.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ao.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://jc.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sa.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lu.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://fe.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://rl.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vy.gzmigu.cn

Go:   // 手写循环
来源：http://iy.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pu.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fp.panjiajie.cn

[D15] 去重
来源：http://zl.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oa.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://xk.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://li.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://sx.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nw.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zb.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://oz.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://sz.bookmarksfly.cn

[D16] 求和与平均值
来源：http://ln.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tk.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sf.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vb.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xe.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jb.szxytkj.cn

Go:   // 手写循环累加
来源：http://mo.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mc.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://pc.hahajie.cn

[D17] 最大值与最小值
来源：http://ke.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://ey.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://sf.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fv.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://aa.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ir.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gk.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://yh.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://aq.colortex.cn

[D18] 扁平化嵌套数组
来源：http://ee.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xl.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://sx.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zh.nicolike.cn

TS:   nested.flat();
来源：http://jk.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oi.huixiangedu.cn

Go:   // 手写双层循环
来源：http://lc.chemitech.net.cn

Ruby: nested.flatten
来源：http://ze.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sv.newstarts.cn

[D19] 按字段分组
来源：http://uf.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nv.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bs.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kl.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://td.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nh.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://wk.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ba.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fm.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://sk.huixiangedu.cn

Py:   Counter(arr)
来源：http://rk.9csxet.cn

PHP:  array_count_values($arr);
来源：http://gg.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hf.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cx.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://do.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://dn.jianghongdianzi.cn

Ruby: arr.tally
来源：http://sc.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xl.szsharing.cn

[D21] 判断是否包含某元素
来源：http://dj.huixiangedu.cn

Py:   x in arr
来源：http://up.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://bk.wgjwhj.cn

JS:   arr.includes(x)
来源：http://xr.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://pc.newstarts.cn

Java: list.contains(x)
来源：http://cj.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://ac.huanxung.cn

Ruby: arr.include?(x)
来源：http://vn.wgjwhj.cn

C#:   list.Contains(x)
来源：http://yz.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://xw.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pb.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wj.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yv.colortex.cn

TS:   [...arr];
来源：http://po.newstarts.cn

Java: new ArrayList<>(list);
来源：http://px.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jf.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ru.shtwfgs.cn

C#:   new List<int>(list);
来源：http://lq.shtwfgs.cn

[D23] reduce 累积计算
来源：http://ps.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ny.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mb.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pe.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lf.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bn.huixinmuqiang.cn

Go:   // 手写循环
来源：http://un.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yn.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mc.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://dg.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ow.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jb.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ko.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gb.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lh.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oq.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ob.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ls.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://tq.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fo.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ic.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://et.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tf.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hd.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gf.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://db.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ss.shtwfgs.cn

[D26] 数组转字符串
来源：http://yx.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://ba.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://rg.wgjwhj.cn

JS:   arr.join(", ")
来源：http://mm.hnjuh.cn

TS:   arr.join(", ")
来源：http://mu.newstarts.cn

Java: String.join(", ", list)
来源：http://ia.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://da.hahajie.cn

Ruby: arr.join(", ")
来源：http://kw.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://zn.yuexingan06.cn

================================================================================
来源：http://dr.shxzukj.cn

E. 字符串处理
来源：http://zb.haigaiapp.cn

================================================================================
来源：http://np.shtwfgs.cn

[E01] 拼接字符串
来源：http://ew.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mk.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mp.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://em.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pf.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ap.bookmarksfly.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ry.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kt.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nt.hahajie.cn

[E02] 重复字符串
来源：http://ry.nicolike.cn

Py:   "ab" * 3
来源：http://kz.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://me.nszjky.cn

JS:   "ab".repeat(3)
来源：http://fd.colortex.cn

TS:   "ab".repeat(3)
来源：http://lw.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://gm.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://vo.newstarts.cn

Ruby: "ab" * 3
来源：http://gz.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eg.muxihuayi.cn

[E03] 截取子串
来源：http://ag.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gv.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ua.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rx.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://yh.hahajie.cn

Java: s.substring(1, 4)
来源：http://ac.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ai.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fq.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://yg.shxzukj.cn

[E04] 查找子串位置
来源：http://xb.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://zg.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://oy.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hg.newstarts.cn

TS:   s.indexOf("x")
来源：http://sk.lnxyls.cn

Java: s.indexOf("x")
来源：http://is.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://ur.huixiangedu.cn

Ruby: s.index("x")
来源：http://aj.nicolike.cn

C#:   s.IndexOf("x")
来源：http://io.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uh.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://td.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ls.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mm.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wk.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://br.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://je.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qt.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wi.huanxung.cn

[E06] 替换子串
来源：http://wc.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ij.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://lt.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kw.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://ak.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wl.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mt.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aj.asd995.cn

C#:   s.Replace("a", "b")
来源：http://ux.hnjuh.cn

[E07] 按分隔符拆分
来源：http://hi.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rm.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mh.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ku.chemitech.net.cn

TS:   s.split(",")
来源：http://yq.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sb.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uz.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://ld.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ki.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://cy.hahajie.cn

Py:   ",".join(items)
来源：http://ff.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://tw.yuexingan06.cn

JS:   items.join(",")
来源：http://tk.newstarts.cn

TS:   items.join(",")
来源：http://nc.haigaiapp.cn

Java: String.join(",", items)
来源：http://in.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://ni.haigaiapp.cn

Ruby: items.join(",")
来源：http://yv.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://sl.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://ko.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://my.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cu.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://qz.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://du.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://kj.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mk.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://br.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ca.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://mq.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wr.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hu.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://jv.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://zu.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ey.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mo.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wa.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hk.shxzskj.cn

[E11] 反转字符串
来源：http://rn.nicolike.cn

Py:   s[::-1]
来源：http://co.bjjhwx.cn

PHP:  strrev($s);
来源：http://tw.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://pk.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://pp.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jn.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ps.yuntaijiaju.cn

Ruby: s.reverse
来源：http://rq.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sb.9csxet.cn

[E12] 统计某字符出现次数
来源：http://nq.bjjhwx.cn

Py:   s.count("a")
来源：http://na.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://ky.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://xo.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://lx.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hp.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://hs.bjjhwx.cn

Ruby: s.count("a")
来源：http://wl.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://mg.nszjky.cn

[E13] 逐字符遍历
来源：http://bu.jianghongdianzi.cn

Py:   for ch in s: print(ch)
来源：http://jd.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://or.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fk.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wk.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rq.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pe.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lx.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sf.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://zu.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cb.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yy.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://io.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vy.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://di.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hp.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vg.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hq.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://nl.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gj.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oz.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tw.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://od.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xl.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fx.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kt.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fv.asd995.cn

[E16] 数字千分位
来源：http://rv.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://md.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://pr.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gm.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mq.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wh.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ab.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://is.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://nq.jctech888.com.cn

[E17] 首字母大写
来源：http://fw.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ma.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ey.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fs.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yo.hahajie.cn


<!-- 参考信息 -->