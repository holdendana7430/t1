代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://en.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yi.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ig.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://lw.hnjuh.cn

Ruby: arr.index(x)
来源：http://mx.newstarts.cn

C#:   list.IndexOf(x);
来源：http://vq.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://us.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hu.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lp.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://ml.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://hy.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rm.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yp.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vs.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rf.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://cn.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lh.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xl.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://sr.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://zq.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ln.panjiajie.cn

Go:   // 手写循环
来源：http://ph.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kp.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tf.shtwfgs.cn

[D15] 去重
来源：http://bp.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tl.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://rf.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://eg.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://br.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://st.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://md.huixiangedu.cn

Ruby: arr.uniq
来源：http://sf.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://bm.szsharing.cn

[D16] 求和与平均值
来源：http://te.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gi.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://av.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hi.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hu.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://be.bookmarksfly.cn

Go:   // 手写循环累加
来源：http://pr.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pl.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://tm.asd995.cn

[D17] 最大值与最小值
来源：http://iq.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://yb.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://cj.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ly.szxytkj.cn

TS:   Math.max(...arr);
来源：http://oq.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ud.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gi.colortex.cn

Ruby: arr.max;  arr.min
来源：http://mt.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://jv.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://gf.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yo.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://nf.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gg.shxzukj.cn

TS:   nested.flat();
来源：http://ld.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://il.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://em.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://vh.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uv.yuexingan06.cn

[D19] 按字段分组
来源：http://sa.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sz.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zd.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tm.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lm.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ai.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://ah.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eo.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ud.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://fj.huanxung.cn

Py:   Counter(arr)
来源：http://oe.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://pw.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ai.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uc.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yz.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://eg.hnjuh.cn

Ruby: arr.tally
来源：http://xd.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://is.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://pk.9csxet.cn

Py:   x in arr
来源：http://oa.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://sg.huanxung.cn

JS:   arr.includes(x)
来源：http://fj.bjjhwx.cn

TS:   arr.includes(x)
来源：http://iq.huixiangedu.cn

Java: list.contains(x)
来源：http://re.shxzukj.cn

Go:   slices.Contains(arr, x)
来源：http://xd.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://hp.wgjwhj.cn

C#:   list.Contains(x)
来源：http://yj.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://nf.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yd.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ea.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yk.huanxung.cn

TS:   [...arr];
来源：http://fp.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://un.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jr.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://ot.9csxet.cn

C#:   new List<int>(list);
来源：http://nj.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://gd.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zs.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xb.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qg.jianghongdianzi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nw.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ko.521024.cn

Go:   // 手写循环
来源：http://xp.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lo.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kj.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://mw.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ro.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jt.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sb.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vr.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ro.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zk.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uh.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bv.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://ma.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xt.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hq.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nq.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jl.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lc.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ze.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ky.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kw.shxzukj.cn

[D26] 数组转字符串
来源：http://ua.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://lb.521024.cn

PHP:  implode(", ", $arr);
来源：http://uy.colortex.cn

JS:   arr.join(", ")
来源：http://qv.jctech888.com.cn

TS:   arr.join(", ")
来源：http://ao.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://xq.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://kq.9csxet.cn

Ruby: arr.join(", ")
来源：http://xk.newstarts.cn

C#:   string.Join(", ", list)
来源：http://wz.yuexingan06.cn

================================================================================
来源：http://ta.shxzukj.cn

E. 字符串处理
来源：http://kn.huixinmuqiang.cn

================================================================================
来源：http://jc.muxihuayi.cn

[E01] 拼接字符串
来源：http://an.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hc.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fj.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uh.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zj.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hp.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wo.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bh.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lr.bookmarksfly.cn

[E02] 重复字符串
来源：http://qv.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://lj.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://ei.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://uj.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ro.lnxyls.cn

Java: "ab".repeat(3)
来源：http://pu.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://sy.521024.cn

Ruby: "ab" * 3
来源：http://rq.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://md.yuntaijiaju.cn

[E03] 截取子串
来源：http://vr.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ea.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hl.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ym.szsharing.cn

TS:   s.slice(1, 4)
来源：http://bk.colortex.cn

Java: s.substring(1, 4)
来源：http://ft.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cm.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ov.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://hq.panjiajie.cn

[E04] 查找子串位置
来源：http://iu.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://gz.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://cq.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vg.szxytkj.cn

TS:   s.indexOf("x")
来源：http://le.nszjky.cn

Java: s.indexOf("x")
来源：http://jk.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://mf.hahajie.cn

Ruby: s.index("x")
来源：http://kq.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://rd.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gu.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zd.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://js.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://di.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qo.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fi.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ut.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pj.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://it.asd995.cn

[E06] 替换子串
来源：http://ca.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fs.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://gf.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bb.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://fi.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vi.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eq.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qq.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://wd.nicolike.cn

[E07] 按分隔符拆分
来源：http://qy.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pu.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yv.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ii.panjiajie.cn

TS:   s.split(",")
来源：http://ki.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bg.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ax.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://pd.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bh.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://nd.521024.cn

Py:   ",".join(items)
来源：http://if.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://tx.yuntaijiaju.cn

JS:   items.join(",")
来源：http://ba.szsharing.cn

TS:   items.join(",")
来源：http://sm.szxytkj.cn

Java: String.join(",", items)
来源：http://gf.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://xd.jctech888.com.cn

Ruby: items.join(",")
来源：http://md.hahajie.cn

C#:   string.Join(",", items)
来源：http://df.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://qi.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kj.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xo.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://we.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://xb.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://gx.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hv.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lb.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sm.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://hf.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fz.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ly.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://av.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://oe.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://yk.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lg.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ag.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tu.szxytkj.cn

[E11] 反转字符串
来源：http://xm.nicolike.cn

Py:   s[::-1]
来源：http://hf.hahajie.cn

PHP:  strrev($s);
来源：http://ad.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://fh.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://cg.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ee.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://is.bookmarksfly.cn

Ruby: s.reverse
来源：http://fx.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xu.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://kn.muxihuayi.cn

Py:   s.count("a")
来源：http://pf.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://gd.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://pv.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://vd.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bk.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://gn.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://pr.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://hv.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://kh.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ft.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wi.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://or.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://td.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://et.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://st.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hm.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ak.nicolike.cn

[E14] URL 编码与 Base64
来源：http://ri.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ae.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zk.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zw.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eh.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ik.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ie.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fy.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xu.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://qq.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nx.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cg.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mj.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://um.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hw.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ux.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://em.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ox.muxihuayi.cn

[E16] 数字千分位
来源：http://lb.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://cn.nszjky.cn

PHP:  number_format(1234567);
来源：http://wo.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ui.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tj.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ll.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sl.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nr.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://hr.szsharing.cn

[E17] 首字母大写
来源：http://jp.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eo.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hc.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cp.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qj.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sg.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qn.lnxyls.cn

Ruby: s.capitalize
来源：http://dr.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ie.huixiangedu.cn

[E18] 模板占位符替换
来源：http://zf.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://od.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://la.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vk.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qy.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xo.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gx.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pp.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fi.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://cj.hnjuh.cn

Py:   s.splitlines()
来源：http://eh.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hd.gzmigu.cn


<!-- 参考信息 -->