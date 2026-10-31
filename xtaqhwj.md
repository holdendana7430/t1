代发 wailian999

[D11] 反转数组
来源：http://vm.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qe.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://uw.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uw.lnxyls.cn

TS:   [...arr].reverse();
来源：http://tk.shxzskj.cn

Java: Collections.reverse(list);
来源：http://wv.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://sq.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://hz.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://uz.chemitech.net.cn

[D12] 查找元素下标
来源：http://fu.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://nk.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kc.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bb.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tv.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rc.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://jv.nszjky.cn

Ruby: arr.index(x)
来源：http://uk.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://fr.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://oy.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fk.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mn.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://hn.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://di.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ro.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zw.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nx.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ks.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://wd.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ih.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eo.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://yd.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://hu.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nn.shxzskj.cn

Go:   // 手写循环
来源：http://id.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vp.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pl.colortex.cn

[D15] 去重
来源：http://bh.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nw.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://uu.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://kg.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://ic.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ii.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vu.asd995.cn

Ruby: arr.uniq
来源：http://jw.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://sl.lnxyls.cn

[D16] 求和与平均值
来源：http://wa.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bc.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oj.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://md.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://te.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kb.nicolike.cn

Go:   // 手写循环累加
来源：http://ox.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jt.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://ns.521024.cn

[D17] 最大值与最小值
来源：http://by.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://vm.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://ux.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ry.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://rs.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gk.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bm.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://tv.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ms.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://oq.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dg.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://nu.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kn.colortex.cn

TS:   nested.flat();
来源：http://ie.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xs.lnxyls.cn

Go:   // 手写双层循环
来源：http://vr.chemitech.net.cn

Ruby: nested.flatten
来源：http://nm.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hw.9csxet.cn

[D19] 按字段分组
来源：http://bd.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bt.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lo.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yr.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dt.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nr.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://te.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cy.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lc.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://xv.nicolike.cn

Py:   Counter(arr)
来源：http://fi.huanxung.cn

PHP:  array_count_values($arr);
来源：http://gr.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qb.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wb.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ps.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://rx.lnxyls.cn

Ruby: arr.tally
来源：http://ss.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oq.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://kx.shxzukj.cn

Py:   x in arr
来源：http://oi.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://un.9csxet.cn

JS:   arr.includes(x)
来源：http://vk.szxytkj.cn

TS:   arr.includes(x)
来源：http://ha.hahajie.cn

Java: list.contains(x)
来源：http://ad.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://ru.shxzukj.cn

Ruby: arr.include?(x)
来源：http://qf.nicolike.cn

C#:   list.Contains(x)
来源：http://ml.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ba.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xc.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kd.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ap.jctech888.com.cn

TS:   [...arr];
来源：http://vr.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://og.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lw.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://tn.wgjwhj.cn

C#:   new List<int>(list);
来源：http://or.521024.cn

[D23] reduce 累积计算
来源：http://lv.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xd.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uq.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ov.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xj.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rm.panjiajie.cn

Go:   // 手写循环
来源：http://ud.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wc.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kc.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://do.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cq.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xs.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ui.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ev.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oa.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xi.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rj.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zt.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://al.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hn.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xd.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wt.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dr.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jg.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ur.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mz.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qs.shxzukj.cn

[D26] 数组转字符串
来源：http://vy.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://cl.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://hz.gzmigu.cn

JS:   arr.join(", ")
来源：http://qd.panjiajie.cn

TS:   arr.join(", ")
来源：http://ip.bjjhwx.cn

Java: String.join(", ", list)
来源：http://fb.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://xc.gzmigu.cn

Ruby: arr.join(", ")
来源：http://yu.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://lo.jctech888.com.cn

================================================================================
来源：http://zb.colortex.cn

E. 字符串处理
来源：http://xr.huixiangedu.cn

================================================================================
来源：http://xz.hahajie.cn

[E01] 拼接字符串
来源：http://zp.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rn.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ud.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pw.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cb.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qz.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sx.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jo.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fz.nicolike.cn

[E02] 重复字符串
来源：http://ci.nszjky.cn

Py:   "ab" * 3
来源：http://nt.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://ha.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://vc.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://hi.9csxet.cn

Java: "ab".repeat(3)
来源：http://kj.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ce.jctech888.com.cn

Ruby: "ab" * 3
来源：http://mu.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://is.huixinmuqiang.cn

[E03] 截取子串
来源：http://yj.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ja.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zs.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ef.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://xj.521024.cn

Java: s.substring(1, 4)
来源：http://gc.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hq.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jc.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://vu.asd995.cn

[E04] 查找子串位置
来源：http://tx.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://pj.521024.cn

PHP:  strpos($s, "x");
来源：http://kr.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wy.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://en.newstarts.cn

Java: s.indexOf("x")
来源：http://ku.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://oy.huixiangedu.cn

Ruby: s.index("x")
来源：http://da.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://of.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xx.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ei.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pi.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wp.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ge.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zn.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://az.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://an.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ap.huixinmuqiang.cn

[E06] 替换子串
来源：http://gt.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yn.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://nn.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rh.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://fm.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jd.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qv.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mf.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://ja.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://ur.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kh.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cu.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://do.gzmigu.cn

TS:   s.split(",")
来源：http://cx.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vr.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tv.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://ka.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://la.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://cn.hahajie.cn

Py:   ",".join(items)
来源：http://rd.asd995.cn

PHP:  implode(",", $items);
来源：http://fs.shxzukj.cn

JS:   items.join(",")
来源：http://ih.hahajie.cn

TS:   items.join(",")
来源：http://kb.hnjuh.cn

Java: String.join(",", items)
来源：http://it.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://na.yuexingan06.cn

Ruby: items.join(",")
来源：http://ei.huanxung.cn

C#:   string.Join(",", items)
来源：http://as.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://rp.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://er.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wd.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://fw.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://tc.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://on.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://br.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qn.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gp.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://ue.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cd.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kd.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://ow.521024.cn

TS:   "7".padStart(3, "0")
来源：http://hz.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://ax.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cl.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gz.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nt.shtwfgs.cn

[E11] 反转字符串
来源：http://ph.muxihuayi.cn

Py:   s[::-1]
来源：http://ed.chemitech.net.cn

PHP:  strrev($s);
来源：http://lg.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://wn.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://pa.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ly.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eb.521024.cn

Ruby: s.reverse
来源：http://cl.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rq.9csxet.cn

[E12] 统计某字符出现次数
来源：http://lm.szxytkj.cn

Py:   s.count("a")
来源：http://xw.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://su.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://qp.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://gq.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ev.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://lg.521024.cn

Ruby: s.count("a")
来源：http://ym.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://bx.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://yl.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://ri.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ze.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yp.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kf.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vi.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ci.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://je.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qn.9csxet.cn

[E14] URL 编码与 Base64
来源：http://og.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://em.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ux.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bt.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nu.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kc.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nj.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vd.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ou.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://ro.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pk.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vo.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qg.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fo.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ft.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wa.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ha.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nz.hahajie.cn

[E16] 数字千分位
来源：http://pc.asd995.cn

Py:   f"{1234567:,}"
来源：http://hs.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://fl.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fy.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wq.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ia.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fi.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vf.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://xl.521024.cn

[E17] 首字母大写
来源：http://mx.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lz.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dy.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ss.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wb.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://af.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nd.yuexingan06.cn

Ruby: s.capitalize
来源：http://cg.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ag.szxytkj.cn


<!-- 参考信息 -->