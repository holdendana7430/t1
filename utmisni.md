代发 wailian999

TS:   [...arr].reverse();
来源：http://xx.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://vr.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://io.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://xn.nszjky.cn

C#:   list.Reverse();
来源：http://sh.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://zt.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://rh.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://td.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hm.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qa.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kg.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://ys.lnxyls.cn

Ruby: arr.index(x)
来源：http://ux.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://te.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://qc.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tz.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vw.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://io.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://ui.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ta.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ml.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ht.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lw.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://yx.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sg.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ht.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://kk.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://ir.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://df.szxytkj.cn

Go:   // 手写循环
来源：http://so.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aq.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kz.huixinmuqiang.cn

[D15] 去重
来源：http://fd.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gq.gzmigu.cn

PHP:  array_unique($arr);
来源：http://fy.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://sy.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://mb.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://br.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ii.colortex.cn

Ruby: arr.uniq
来源：http://mc.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://te.shxzukj.cn

[D16] 求和与平均值
来源：http://og.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xx.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dr.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ad.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bl.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://al.chemitech.net.cn

Go:   // 手写循环累加
来源：http://yk.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ej.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://ak.nszjky.cn

[D17] 最大值与最小值
来源：http://av.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://ta.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://ie.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rv.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://ug.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://md.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ka.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://hy.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://lc.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://ps.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ny.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://sf.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ja.panjiajie.cn

TS:   nested.flat();
来源：http://cy.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cq.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://ji.muxihuayi.cn

Ruby: nested.flatten
来源：http://ez.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sp.panjiajie.cn

[D19] 按字段分组
来源：http://ld.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ft.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tn.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vm.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jh.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ql.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://qy.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ow.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nw.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://fv.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://bx.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://jz.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ql.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ox.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yt.asd995.cn

Go:   // 手写 map[T]int
来源：http://ax.9csxet.cn

Ruby: arr.tally
来源：http://kb.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wm.nicolike.cn

[D21] 判断是否包含某元素
来源：http://vk.panjiajie.cn

Py:   x in arr
来源：http://ym.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://by.colortex.cn

JS:   arr.includes(x)
来源：http://th.asd995.cn

TS:   arr.includes(x)
来源：http://fw.shxzukj.cn

Java: list.contains(x)
来源：http://ir.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://wy.panjiajie.cn

Ruby: arr.include?(x)
来源：http://an.hahajie.cn

C#:   list.Contains(x)
来源：http://qs.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://bd.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qq.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pb.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lw.hahajie.cn

TS:   [...arr];
来源：http://of.hahajie.cn

Java: new ArrayList<>(list);
来源：http://nd.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ln.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://ti.lnxyls.cn

C#:   new List<int>(list);
来源：http://ol.hahajie.cn

[D23] reduce 累积计算
来源：http://rz.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qj.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ok.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bl.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bt.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vx.chemitech.net.cn

Go:   // 手写循环
来源：http://jx.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oq.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hb.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://vh.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ek.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qa.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kt.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://we.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ad.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eo.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zw.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nj.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://zs.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nj.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ie.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xs.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ce.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aj.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qq.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ve.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sa.szsharing.cn

[D26] 数组转字符串
来源：http://rg.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://mz.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://if.gzmigu.cn

JS:   arr.join(", ")
来源：http://wt.asd995.cn

TS:   arr.join(", ")
来源：http://ni.bjjhwx.cn

Java: String.join(", ", list)
来源：http://hz.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://ma.huanxung.cn

Ruby: arr.join(", ")
来源：http://wf.szsharing.cn

C#:   string.Join(", ", list)
来源：http://zh.shxzskj.cn

================================================================================
来源：http://xz.muxihuayi.cn

E. 字符串处理
来源：http://tn.haigaiapp.cn

================================================================================
来源：http://yi.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://we.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sx.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fz.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oj.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ob.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hf.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ep.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rh.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qr.huixiangedu.cn

[E02] 重复字符串
来源：http://qp.521024.cn

Py:   "ab" * 3
来源：http://jm.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://bg.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://zh.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://yh.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://zf.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ab.lnxyls.cn

Ruby: "ab" * 3
来源：http://ld.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hj.newstarts.cn

[E03] 截取子串
来源：http://ww.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gz.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rg.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oy.nszjky.cn

TS:   s.slice(1, 4)
来源：http://ba.shxzukj.cn

Java: s.substring(1, 4)
来源：http://li.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sa.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nm.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://jq.wgjwhj.cn

[E04] 查找子串位置
来源：http://pu.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://pe.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://rp.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kl.huanxung.cn

TS:   s.indexOf("x")
来源：http://hi.shxzskj.cn

Java: s.indexOf("x")
来源：http://mz.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://wh.panjiajie.cn

Ruby: s.index("x")
来源：http://du.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://wy.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tn.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mj.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zp.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nq.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ij.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hr.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qu.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qj.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ga.yuntaijiaju.cn

[E06] 替换子串
来源：http://xm.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://na.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://gr.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xq.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://uz.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kn.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wt.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yz.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://tz.521024.cn

[E07] 按分隔符拆分
来源：http://bd.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pa.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bl.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fr.wgjwhj.cn

TS:   s.split(",")
来源：http://wp.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ko.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zb.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://au.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gk.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://io.huixiangedu.cn

Py:   ",".join(items)
来源：http://jo.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://am.hnjuh.cn

JS:   items.join(",")
来源：http://hl.szxytkj.cn

TS:   items.join(",")
来源：http://yk.lnxyls.cn

Java: String.join(",", items)
来源：http://nt.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://gn.hahajie.cn

Ruby: items.join(",")
来源：http://eo.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://sl.nszjky.cn

[E09] 去除所有空白字符
来源：http://dq.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vf.huixinmuqiang.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ea.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://ou.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://os.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://dk.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yh.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ey.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://im.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://sv.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uo.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gn.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://av.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://db.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ln.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yx.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vb.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qn.shxzskj.cn

[E11] 反转字符串
来源：http://lw.huanxung.cn

Py:   s[::-1]
来源：http://mu.huanxung.cn

PHP:  strrev($s);
来源：http://qf.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://cs.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://qh.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ft.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bx.9csxet.cn

Ruby: s.reverse
来源：http://xk.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vi.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://qs.haigaiapp.cn

Py:   s.count("a")
来源：http://cm.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://rs.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://ut.nicolike.cn

TS:   s.split("a").length - 1
来源：http://tg.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ay.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://gw.newstarts.cn

Ruby: s.count("a")
来源：http://fw.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://wn.szxytkj.cn

[E13] 逐字符遍历
来源：http://zj.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://hf.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ob.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://so.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ce.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xk.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uj.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fm.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gt.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://xu.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pg.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ht.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vx.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qs.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jp.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vw.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bn.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wy.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://vk.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zy.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ee.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ol.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xl.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sd.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rw.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yd.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vk.colortex.cn

[E16] 数字千分位
来源：http://mh.szsharing.cn

Py:   f"{1234567:,}"
来源：http://ua.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://wp.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iu.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cq.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ap.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lr.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ky.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://ju.muxihuayi.cn

[E17] 首字母大写
来源：http://id.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wm.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xd.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uo.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jp.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fb.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eb.chemitech.net.cn

Ruby: s.capitalize
来源：http://yn.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mh.wgjwhj.cn

[E18] 模板占位符替换
来源：http://lv.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lh.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fy.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fc.lnxyls.cn


<!-- 参考信息 -->