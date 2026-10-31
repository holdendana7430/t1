代发 wailian999

Ruby: arr.index(x)
来源：http://ak.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://qk.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://ms.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://an.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qg.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://bg.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://nt.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dn.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fm.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hh.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mj.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://iw.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zf.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xc.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://kl.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://lk.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yy.newstarts.cn

Go:   // 手写循环
来源：http://nt.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qr.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zs.gzmigu.cn

[D15] 去重
来源：http://pr.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://br.521024.cn

PHP:  array_unique($arr);
来源：http://wa.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://mi.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://ln.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bp.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://or.shtwfgs.cn

Ruby: arr.uniq
来源：http://ku.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://ze.nszjky.cn

[D16] 求和与平均值
来源：http://gn.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vi.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dj.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bw.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kz.9csxet.cn

Go:   // 手写循环累加
来源：http://qh.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ag.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://rn.szxytkj.cn

[D17] 最大值与最小值
来源：http://in.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://pg.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://wq.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ij.521024.cn

TS:   Math.max(...arr);
来源：http://ar.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ji.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xi.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://qb.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://ds.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://kk.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://to.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://or.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wm.bjjhwx.cn

TS:   nested.flat();
来源：http://rm.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pm.nszjky.cn

Go:   // 手写双层循环
来源：http://bu.hahajie.cn

Ruby: nested.flatten
来源：http://fq.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cd.chemitech.net.cn

[D19] 按字段分组
来源：http://wv.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yg.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pa.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fo.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yq.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jt.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://xh.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dz.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fq.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://lj.hnjuh.cn

Py:   Counter(arr)
来源：http://hu.nszjky.cn

PHP:  array_count_values($arr);
来源：http://xt.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ju.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qq.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tn.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://xl.asd995.cn

Ruby: arr.tally
来源：http://cy.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kb.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://uo.shtwfgs.cn

Py:   x in arr
来源：http://yy.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://om.bjjhwx.cn

JS:   arr.includes(x)
来源：http://se.hnjuh.cn

TS:   arr.includes(x)
来源：http://qt.wgjwhj.cn

Java: list.contains(x)
来源：http://bl.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://yx.szsharing.cn

Ruby: arr.include?(x)
来源：http://pb.bjjhwx.cn

C#:   list.Contains(x)
来源：http://wq.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://bz.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jc.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ze.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ei.colortex.cn

TS:   [...arr];
来源：http://ab.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://qc.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rh.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://hq.yuexingan06.cn

C#:   new List<int>(list);
来源：http://tp.huixiangedu.cn

[D23] reduce 累积计算
来源：http://yx.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://iq.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vr.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ts.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ms.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kt.asd995.cn

Go:   // 手写循环
来源：http://ru.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://da.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qi.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://nx.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vi.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://th.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kk.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oc.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ap.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ir.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yk.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rr.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://cy.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hv.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tj.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wq.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jz.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ui.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jl.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zu.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://du.huixiangedu.cn

[D26] 数组转字符串
来源：http://kt.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://ik.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://ox.panjiajie.cn

JS:   arr.join(", ")
来源：http://pg.yuexingan06.cn

TS:   arr.join(", ")
来源：http://uy.shxzskj.cn

Java: String.join(", ", list)
来源：http://fj.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://sh.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://or.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://hf.colortex.cn

================================================================================
来源：http://om.jianghongdianzi.cn

E. 字符串处理
来源：http://qb.jianghongdianzi.cn

================================================================================
来源：http://ga.huanxung.cn

[E01] 拼接字符串
来源：http://qy.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://df.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qo.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ex.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tn.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ds.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zu.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cm.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ke.newstarts.cn

[E02] 重复字符串
来源：http://kw.newstarts.cn

Py:   "ab" * 3
来源：http://wj.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://zj.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://yv.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://og.shxzukj.cn

Java: "ab".repeat(3)
来源：http://gy.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ea.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://mj.shxzukj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jf.szxytkj.cn

[E03] 截取子串
来源：http://if.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oq.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sd.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ep.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://jo.szsharing.cn

Java: s.substring(1, 4)
来源：http://bp.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://de.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ve.newstarts.cn

C#:   s.Substring(1, 3)
来源：http://dg.haigaiapp.cn

[E04] 查找子串位置
来源：http://ks.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://qq.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://kk.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://so.nicolike.cn

TS:   s.indexOf("x")
来源：http://ka.nicolike.cn

Java: s.indexOf("x")
来源：http://zy.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://jm.panjiajie.cn

Ruby: s.index("x")
来源：http://gz.9csxet.cn

C#:   s.IndexOf("x")
来源：http://sm.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ur.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wp.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ud.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eq.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oo.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rx.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hw.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fr.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://go.hahajie.cn

[E06] 替换子串
来源：http://ek.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ul.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://ky.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vd.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://op.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eq.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sw.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yo.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://ay.hnjuh.cn

[E07] 按分隔符拆分
来源：http://wy.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jm.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ng.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ol.newstarts.cn

TS:   s.split(",")
来源：http://qp.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lp.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fw.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://tz.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://le.asd995.cn

[E08] 数组按分隔符合并
来源：http://kz.hahajie.cn

Py:   ",".join(items)
来源：http://pr.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://ii.shxzukj.cn

JS:   items.join(",")
来源：http://po.nicolike.cn

TS:   items.join(",")
来源：http://us.nicolike.cn

Java: String.join(",", items)
来源：http://uk.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://hr.nszjky.cn

Ruby: items.join(",")
来源：http://zk.hnjuh.cn

C#:   string.Join(",", items)
来源：http://fj.hnjuh.cn

[E09] 去除所有空白字符
来源：http://ii.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ni.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lf.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://cy.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://dk.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://eq.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://af.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ex.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ob.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://gk.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tl.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bz.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://tm.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://dp.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://dl.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hx.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ql.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sm.muxihuayi.cn

[E11] 反转字符串
来源：http://qq.asd995.cn

Py:   s[::-1]
来源：http://yd.panjiajie.cn

PHP:  strrev($s);
来源：http://ns.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://mg.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://tx.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dw.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fe.huanxung.cn

Ruby: s.reverse
来源：http://lw.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qv.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://mn.lnxyls.cn

Py:   s.count("a")
来源：http://zf.asd995.cn

PHP:  substr_count($s, "a");
来源：http://kw.szsharing.cn

JS:   s.split("a").length - 1
来源：http://pf.asd995.cn

TS:   s.split("a").length - 1
来源：http://kc.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ju.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://np.yuexingan06.cn

Ruby: s.count("a")
来源：http://lr.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://iv.hnjuh.cn

[E13] 逐字符遍历
来源：http://qh.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://jy.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pn.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eq.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ke.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://or.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nj.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ug.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jf.asd995.cn

[E14] URL 编码与 Base64
来源：http://xk.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fn.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uj.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rh.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cn.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bw.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://am.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yk.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://go.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://hp.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yt.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yl.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kj.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wr.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://io.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nw.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://im.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hc.huanxung.cn

[E16] 数字千分位
来源：http://ss.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://ok.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://yt.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gj.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://af.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yx.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jn.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tv.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://yq.chemitech.net.cn

[E17] 首字母大写
来源：http://wp.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tk.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://po.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gv.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ct.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kv.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://du.nszjky.cn

Ruby: s.capitalize
来源：http://do.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uq.nszjky.cn

[E18] 模板占位符替换
来源：http://ji.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fg.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lw.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mn.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rd.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mo.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uu.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kf.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yb.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://jh.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://my.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://he.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://vw.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://jc.shxzskj.cn

Java: s.lines().toList()
来源：http://eq.521024.cn

Go:   strings.Split(s, "\n")
来源：http://kx.lnxyls.cn


<!-- 参考信息 -->