代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qh.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vx.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jg.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xd.muxihuayi.cn

[D11] 反转数组
来源：http://kv.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ei.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://wa.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ih.hnjuh.cn

TS:   [...arr].reverse();
来源：http://to.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://jy.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://en.nicolike.cn

Ruby: arr.reverse
来源：http://wl.hnjuh.cn

C#:   list.Reverse();
来源：http://ht.nszjky.cn

[D12] 查找元素下标
来源：http://sf.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://it.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hk.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://md.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yt.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jp.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://jp.chemitech.net.cn

Ruby: arr.index(x)
来源：http://kg.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://fj.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://rx.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yd.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vn.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://aw.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://pl.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fk.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://on.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gu.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lw.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://uk.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xn.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xx.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://jc.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://yw.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nu.hahajie.cn

Go:   // 手写循环
来源：http://th.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uf.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xw.hahajie.cn

[D15] 去重
来源：http://wf.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hs.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://fw.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://ez.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://bh.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://or.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lw.nszjky.cn

Ruby: arr.uniq
来源：http://vr.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://ri.lnxyls.cn

[D16] 求和与平均值
来源：http://sw.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rw.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bo.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xm.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sv.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ql.chemitech.net.cn

Go:   // 手写循环累加
来源：http://ay.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rp.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://hn.huixiangedu.cn

[D17] 最大值与最小值
来源：http://uz.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://kd.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://xf.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gw.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://xg.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wv.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jc.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://xs.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://eq.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://qe.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uu.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://vg.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://no.huixinmuqiang.cn

TS:   nested.flat();
来源：http://dy.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lh.shtwfgs.cn

Go:   // 手写双层循环
来源：http://ai.newstarts.cn

Ruby: nested.flatten
来源：http://qq.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cp.chemitech.net.cn

[D19] 按字段分组
来源：http://sy.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ph.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qe.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dx.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hu.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zi.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://xv.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fz.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mb.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://fv.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://pu.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://sr.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dt.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zh.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mi.nszjky.cn

Go:   // 手写 map[T]int
来源：http://pz.muxihuayi.cn

Ruby: arr.tally
来源：http://qy.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ac.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://jm.chemitech.net.cn

Py:   x in arr
来源：http://wk.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://qm.shtwfgs.cn

JS:   arr.includes(x)
来源：http://fj.jctech888.com.cn

TS:   arr.includes(x)
来源：http://br.panjiajie.cn

Java: list.contains(x)
来源：http://qr.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://sw.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://ue.muxihuayi.cn

C#:   list.Contains(x)
来源：http://vq.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://et.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kk.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bi.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kj.yuntaijiaju.cn

TS:   [...arr];
来源：http://eh.newstarts.cn

Java: new ArrayList<>(list);
来源：http://mm.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wn.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://cy.nicolike.cn

C#:   new List<int>(list);
来源：http://nr.521024.cn

[D23] reduce 累积计算
来源：http://pk.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sq.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://id.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ss.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vw.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lf.yuexingan06.cn

Go:   // 手写循环
来源：http://gs.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pm.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qc.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://as.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zo.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lz.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ca.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ea.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ee.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gv.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qz.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://do.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ux.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sm.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wm.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ly.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gf.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dw.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jd.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://za.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pr.colortex.cn

[D26] 数组转字符串
来源：http://te.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://bg.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://wv.chemitech.net.cn

JS:   arr.join(", ")
来源：http://al.shtwfgs.cn

TS:   arr.join(", ")
来源：http://ld.gzmigu.cn

Java: String.join(", ", list)
来源：http://xc.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://hi.szsharing.cn

Ruby: arr.join(", ")
来源：http://gz.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://tb.gzmigu.cn

================================================================================
来源：http://wz.hnjuh.cn

E. 字符串处理
来源：http://db.panjiajie.cn

================================================================================
来源：http://bb.szxytkj.cn

[E01] 拼接字符串
来源：http://wc.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vh.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vk.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lj.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ys.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jx.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ws.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gd.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gs.newstarts.cn

[E02] 重复字符串
来源：http://kr.jctech888.com.cn

Py:   "ab" * 3
来源：http://yh.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://kn.521024.cn

JS:   "ab".repeat(3)
来源：http://dn.hahajie.cn

TS:   "ab".repeat(3)
来源：http://za.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://zb.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://ep.shxzskj.cn

Ruby: "ab" * 3
来源：http://dq.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://my.newstarts.cn

[E03] 截取子串
来源：http://da.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gd.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xu.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mu.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://bp.shtwfgs.cn

Java: s.substring(1, 4)
来源：http://ul.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kq.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xx.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://lp.shxzskj.cn

[E04] 查找子串位置
来源：http://ox.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://lt.hahajie.cn

PHP:  strpos($s, "x");
来源：http://bp.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wu.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://ye.521024.cn

Java: s.indexOf("x")
来源：http://pp.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://zt.shtwfgs.cn

Ruby: s.index("x")
来源：http://sr.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://co.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pc.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ph.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://og.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xt.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jh.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fl.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lj.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jl.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bc.yuexingan06.cn

[E06] 替换子串
来源：http://fv.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lb.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://qp.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://no.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://cx.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vp.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wt.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ih.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://tx.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://lv.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wr.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gs.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yh.hnjuh.cn

TS:   s.split(",")
来源：http://hy.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rx.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lr.asd995.cn

Ruby: s.split(",");  s.split
来源：http://bw.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yw.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://dt.yuexingan06.cn

Py:   ",".join(items)
来源：http://jo.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://ts.jianghongdianzi.cn

JS:   items.join(",")
来源：http://we.nicolike.cn

TS:   items.join(",")
来源：http://tf.yuexingan06.cn

Java: String.join(",", items)
来源：http://oz.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://ej.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://eo.hnjuh.cn

C#:   string.Join(",", items)
来源：http://ee.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://kk.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cy.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qe.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://hr.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ni.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://hn.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kq.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bx.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fs.wgjwhj.cn

[E10] 左侧补零 / 定长填充
来源：http://sg.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zs.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://go.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://rq.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://ew.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://of.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://is.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zo.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sm.shtwfgs.cn

[E11] 反转字符串
来源：http://qc.huixinmuqiang.cn

Py:   s[::-1]
来源：http://ya.yuexingan06.cn

PHP:  strrev($s);
来源：http://pz.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://fn.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://qb.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pr.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://te.yuntaijiaju.cn

Ruby: s.reverse
来源：http://em.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ks.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://pm.9csxet.cn

Py:   s.count("a")
来源：http://wp.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://cz.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://ni.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://jt.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pw.colortex.cn

Go:   strings.Count(s, "a")
来源：http://eb.panjiajie.cn

Ruby: s.count("a")
来源：http://tg.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://ij.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://qe.521024.cn

Py:   for ch in s: print(ch)
来源：http://vw.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xb.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xh.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nh.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zi.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://un.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cw.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mc.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://xp.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cs.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lh.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wt.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zq.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wy.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fi.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gq.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://io.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://aw.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rn.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://we.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yo.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://my.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vz.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lz.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kh.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rr.huixinmuqiang.cn

[E16] 数字千分位
来源：http://cr.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://vt.shxzukj.cn

PHP:  number_format(1234567);
来源：http://ud.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hc.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tj.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://br.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://th.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ot.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://di.yuexingan06.cn

[E17] 首字母大写
来源：http://sd.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jf.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dx.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xx.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ap.jianghongdianzi.cn


<!-- 参考信息 -->