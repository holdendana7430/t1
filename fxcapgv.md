代发 wailian999

[D11] 反转数组
来源：http://wp.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zp.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://qa.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ex.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://ny.shxzskj.cn

Java: Collections.reverse(list);
来源：http://am.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://sy.gzmigu.cn

Ruby: arr.reverse
来源：http://nz.huanxung.cn

C#:   list.Reverse();
来源：http://ii.shxzskj.cn

[D12] 查找元素下标
来源：http://ob.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://pg.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://df.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ud.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uf.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ol.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ev.szsharing.cn

Ruby: arr.index(x)
来源：http://lw.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://ds.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://yt.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ad.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tv.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://py.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://ec.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://or.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vo.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://as.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qq.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://xh.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bf.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zt.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://hd.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://lp.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tv.szsharing.cn

Go:   // 手写循环
来源：http://ph.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vu.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gs.shxzskj.cn

[D15] 去重
来源：http://yb.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hm.521024.cn

PHP:  array_unique($arr);
来源：http://au.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://xj.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://ru.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ku.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cs.gzmigu.cn

Ruby: arr.uniq
来源：http://li.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://tl.huanxung.cn

[D16] 求和与平均值
来源：http://ly.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ya.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ep.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lk.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dm.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hu.521024.cn

Go:   // 手写循环累加
来源：http://rg.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://za.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://jf.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://kl.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ao.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://ya.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gz.nszjky.cn

TS:   Math.max(...arr);
来源：http://ew.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://no.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eu.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://qf.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://eo.colortex.cn

[D18] 扁平化嵌套数组
来源：http://ek.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vp.colortex.cn

PHP:  array_merge(...$nested);
来源：http://ti.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mo.newstarts.cn

TS:   nested.flat();
来源：http://le.newstarts.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://br.wgjwhj.cn

Go:   // 手写双层循环
来源：http://dg.bookmarksfly.cn

Ruby: nested.flatten
来源：http://jn.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sh.szsharing.cn

[D19] 按字段分组
来源：http://ov.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ti.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://du.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rt.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ic.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mp.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://ii.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ty.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pi.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://vm.huixiangedu.cn

Py:   Counter(arr)
来源：http://zy.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://bf.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kf.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://je.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qy.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://ai.yuntaijiaju.cn

Ruby: arr.tally
来源：http://nn.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yl.huanxung.cn

[D21] 判断是否包含某元素
来源：http://tl.szsharing.cn

Py:   x in arr
来源：http://oj.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://oy.wgjwhj.cn

JS:   arr.includes(x)
来源：http://qz.bjjhwx.cn

TS:   arr.includes(x)
来源：http://vp.shxzukj.cn

Java: list.contains(x)
来源：http://ak.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://ym.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://sk.muxihuayi.cn

C#:   list.Contains(x)
来源：http://ld.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://mj.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mp.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://we.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tf.asd995.cn

TS:   [...arr];
来源：http://et.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://gz.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://np.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://jd.shxzskj.cn

C#:   new List<int>(list);
来源：http://oq.bjjhwx.cn

[D23] reduce 累积计算
来源：http://em.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bo.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rn.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xt.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://je.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ra.colortex.cn

Go:   // 手写循环
来源：http://wy.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dc.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lo.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://qf.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ni.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://an.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sp.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zy.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mr.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ez.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yn.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oz.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://kg.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bt.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dk.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fp.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fx.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sv.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ct.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jb.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ph.haigaiapp.cn

[D26] 数组转字符串
来源：http://rt.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://pj.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://xu.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://df.gzmigu.cn

TS:   arr.join(", ")
来源：http://kl.bjjhwx.cn

Java: String.join(", ", list)
来源：http://bt.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://ps.nszjky.cn

Ruby: arr.join(", ")
来源：http://pj.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://pq.jianghongdianzi.cn

================================================================================
来源：http://bv.wgjwhj.cn

E. 字符串处理
来源：http://qj.hahajie.cn

================================================================================
来源：http://wr.nicolike.cn

[E01] 拼接字符串
来源：http://qi.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sv.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://em.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qj.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bi.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wx.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fr.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://my.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qv.hnjuh.cn

[E02] 重复字符串
来源：http://zk.shxzskj.cn

Py:   "ab" * 3
来源：http://zv.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://er.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://cf.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://zt.hnjuh.cn

Java: "ab".repeat(3)
来源：http://tn.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://so.lnxyls.cn

Ruby: "ab" * 3
来源：http://by.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ox.shxzukj.cn

[E03] 截取子串
来源：http://zq.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://we.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fu.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mo.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://wd.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://jr.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hk.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vf.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://rt.szsharing.cn

[E04] 查找子串位置
来源：http://am.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://sl.colortex.cn

PHP:  strpos($s, "x");
来源：http://il.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gh.panjiajie.cn

TS:   s.indexOf("x")
来源：http://nb.muxihuayi.cn

Java: s.indexOf("x")
来源：http://is.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://ve.wgjwhj.cn

Ruby: s.index("x")
来源：http://be.9csxet.cn

C#:   s.IndexOf("x")
来源：http://vn.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://me.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ht.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rb.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pt.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ez.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ib.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ip.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qm.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lm.wgjwhj.cn

[E06] 替换子串
来源：http://jd.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nm.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://nf.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tg.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://ma.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ae.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mf.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yw.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://fm.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://jc.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qm.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tf.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xl.chemitech.net.cn

TS:   s.split(",")
来源：http://nm.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pf.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://to.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://aa.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ij.nszjky.cn

[E08] 数组按分隔符合并
来源：http://oy.panjiajie.cn

Py:   ",".join(items)
来源：http://rx.asd995.cn

PHP:  implode(",", $items);
来源：http://la.jianghongdianzi.cn

JS:   items.join(",")
来源：http://vn.jianghongdianzi.cn

TS:   items.join(",")
来源：http://jt.huixiangedu.cn

Java: String.join(",", items)
来源：http://gu.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://zt.wgjwhj.cn

Ruby: items.join(",")
来源：http://tb.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://jp.hnjuh.cn

[E09] 去除所有空白字符
来源：http://fb.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kx.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dp.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://ec.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://cs.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://vv.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://va.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fm.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yt.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://lv.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hk.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rt.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://oz.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ih.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://vd.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yd.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qd.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lr.szxytkj.cn

[E11] 反转字符串
来源：http://af.haigaiapp.cn

Py:   s[::-1]
来源：http://mm.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://dy.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://vx.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://bq.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://by.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gp.nicolike.cn

Ruby: s.reverse
来源：http://hc.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gs.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://uh.shtwfgs.cn

Py:   s.count("a")
来源：http://mg.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://qc.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://so.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://db.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ws.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://wa.bjjhwx.cn

Ruby: s.count("a")
来源：http://hm.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://yo.hnjuh.cn

[E13] 逐字符遍历
来源：http://hw.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://mn.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xl.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jg.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lr.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lg.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wb.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sv.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cz.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://ra.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zr.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yj.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pt.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iz.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xd.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hk.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jk.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nk.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://bo.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xf.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vj.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hn.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qx.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qk.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ya.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ov.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wi.huixinmuqiang.cn

[E16] 数字千分位
来源：http://sc.colortex.cn

Py:   f"{1234567:,}"
来源：http://fk.szxytkj.cn

PHP:  number_format(1234567);
来源：http://fe.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ps.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qf.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wg.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yb.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vo.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://mb.huanxung.cn

[E17] 首字母大写
来源：http://hv.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pg.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kf.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sl.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ov.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yv.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ej.hahajie.cn

Ruby: s.capitalize
来源：http://xs.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gd.wgjwhj.cn


<!-- 参考信息 -->