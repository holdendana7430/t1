代发 wailian999

Ruby: arr.index(x)
来源：http://jd.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://nl.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://nv.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bf.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pz.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://ka.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://lj.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bs.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kt.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://du.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ax.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://yl.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jl.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://of.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://ny.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://yx.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fa.muxihuayi.cn

Go:   // 手写循环
来源：http://ac.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fa.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bi.nszjky.cn

[D15] 去重
来源：http://td.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kl.colortex.cn

PHP:  array_unique($arr);
来源：http://ct.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://lm.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://bz.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tb.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yk.wgjwhj.cn

Ruby: arr.uniq
来源：http://id.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://xo.bookmarksfly.cn

[D16] 求和与平均值
来源：http://ro.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vm.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nv.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xm.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vy.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wj.panjiajie.cn

Go:   // 手写循环累加
来源：http://zq.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yd.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://yc.asd995.cn

[D17] 最大值与最小值
来源：http://lw.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://bq.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://ec.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ey.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://xq.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://il.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ee.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ad.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://ty.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://mz.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://au.521024.cn

PHP:  array_merge(...$nested);
来源：http://nf.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rv.lnxyls.cn

TS:   nested.flat();
来源：http://hj.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lu.wgjwhj.cn

Go:   // 手写双层循环
来源：http://gi.colortex.cn

Ruby: nested.flatten
来源：http://da.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dr.nszjky.cn

[D19] 按字段分组
来源：http://by.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sn.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wu.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pi.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ie.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jt.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://bk.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gb.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ri.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://ca.521024.cn

Py:   Counter(arr)
来源：http://od.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://jv.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qg.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zp.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://me.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://ye.wgjwhj.cn

Ruby: arr.tally
来源：http://eb.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sz.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://xx.jianghongdianzi.cn

Py:   x in arr
来源：http://bw.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://by.shxzskj.cn

JS:   arr.includes(x)
来源：http://xg.wgjwhj.cn

TS:   arr.includes(x)
来源：http://qn.huixiangedu.cn

Java: list.contains(x)
来源：http://mp.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://kt.newstarts.cn

Ruby: arr.include?(x)
来源：http://fr.bjjhwx.cn

C#:   list.Contains(x)
来源：http://ky.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://qm.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cw.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dp.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ex.bjjhwx.cn

TS:   [...arr];
来源：http://nj.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://rt.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fv.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://qt.wgjwhj.cn

C#:   new List<int>(list);
来源：http://xc.newstarts.cn

[D23] reduce 累积计算
来源：http://si.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zi.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pm.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fc.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ge.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tc.shxzskj.cn

Go:   // 手写循环
来源：http://aw.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ku.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ya.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://pa.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rk.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ez.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dm.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zu.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bt.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hm.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ij.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mu.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ik.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lr.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ty.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ab.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gm.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ev.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ju.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uv.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jn.panjiajie.cn

[D26] 数组转字符串
来源：http://bv.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://bh.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://mn.lnxyls.cn

JS:   arr.join(", ")
来源：http://tm.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://mc.shxzukj.cn

Java: String.join(", ", list)
来源：http://dj.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://zv.lnxyls.cn

Ruby: arr.join(", ")
来源：http://rd.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://ho.panjiajie.cn

================================================================================
来源：http://tp.yuntaijiaju.cn

E. 字符串处理
来源：http://ye.panjiajie.cn

================================================================================
来源：http://yd.yuexingan06.cn

[E01] 拼接字符串
来源：http://ns.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cv.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xb.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tx.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pl.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cy.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dl.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://po.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xc.newstarts.cn

[E02] 重复字符串
来源：http://pt.lnxyls.cn

Py:   "ab" * 3
来源：http://sk.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://jn.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://ly.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://ne.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://fu.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://sg.shtwfgs.cn

Ruby: "ab" * 3
来源：http://rd.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kz.newstarts.cn

[E03] 截取子串
来源：http://ok.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fa.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wf.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wi.hahajie.cn

TS:   s.slice(1, 4)
来源：http://wm.panjiajie.cn

Java: s.substring(1, 4)
来源：http://fe.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pu.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nn.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://ct.huanxung.cn

[E04] 查找子串位置
来源：http://dx.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://fi.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://xr.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ig.9csxet.cn

TS:   s.indexOf("x")
来源：http://fa.huanxung.cn

Java: s.indexOf("x")
来源：http://hr.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://mg.hnjuh.cn

Ruby: s.index("x")
来源：http://ek.asd995.cn

C#:   s.IndexOf("x")
来源：http://wt.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zs.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fo.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zy.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bg.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://za.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zh.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uj.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lb.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xs.newstarts.cn

[E06] 替换子串
来源：http://fm.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gq.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://tj.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ux.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://wm.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hy.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vs.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xw.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://qh.colortex.cn

[E07] 按分隔符拆分
来源：http://ia.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xt.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pk.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dj.szsharing.cn

TS:   s.split(",")
来源：http://cx.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wp.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qr.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://rk.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oa.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://yq.haigaiapp.cn

Py:   ",".join(items)
来源：http://cc.colortex.cn

PHP:  implode(",", $items);
来源：http://gu.wgjwhj.cn

JS:   items.join(",")
来源：http://wg.521024.cn

TS:   items.join(",")
来源：http://mr.szxytkj.cn

Java: String.join(",", items)
来源：http://nj.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://uo.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://dl.9csxet.cn

C#:   string.Join(",", items)
来源：http://rj.szsharing.cn

[E09] 去除所有空白字符
来源：http://jc.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wo.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iz.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://eu.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://po.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://le.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ab.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uz.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ry.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://lh.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jm.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kh.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://yy.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://do.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ma.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hs.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fj.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://py.bjjhwx.cn

[E11] 反转字符串
来源：http://vb.szxytkj.cn

Py:   s[::-1]
来源：http://qg.bookmarksfly.cn

PHP:  strrev($s);
来源：http://lc.colortex.cn

JS:   [...s].reverse().join("")
来源：http://iz.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://zl.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qh.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gt.haigaiapp.cn

Ruby: s.reverse
来源：http://nd.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yo.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://za.muxihuayi.cn

Py:   s.count("a")
来源：http://ak.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://ir.colortex.cn

JS:   s.split("a").length - 1
来源：http://jn.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://yq.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pj.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://bb.521024.cn

Ruby: s.count("a")
来源：http://fy.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://ug.shxzukj.cn

[E13] 逐字符遍历
来源：http://bg.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://he.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lg.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ms.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uq.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ag.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wc.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qg.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ma.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ch.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lm.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zd.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gt.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qj.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tg.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vu.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bg.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pc.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://ec.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cq.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tt.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ep.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tu.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oo.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uq.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vf.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fs.yuntaijiaju.cn

[E16] 数字千分位
来源：http://li.szsharing.cn

Py:   f"{1234567:,}"
来源：http://rg.lnxyls.cn

PHP:  number_format(1234567);
来源：http://oh.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vu.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qn.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zu.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uh.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ah.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://pb.szsharing.cn

[E17] 首字母大写
来源：http://sw.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sp.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mz.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lo.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kv.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ch.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vh.9csxet.cn

Ruby: s.capitalize
来源：http://gw.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pt.bjjhwx.cn

[E18] 模板占位符替换
来源：http://dy.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mg.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uh.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wk.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zb.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dt.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ps.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dk.shxzukj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yf.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://jm.nicolike.cn

Py:   s.splitlines()
来源：http://qy.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zo.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://pt.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://zb.shtwfgs.cn

Java: s.lines().toList()
来源：http://bs.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://dh.yuexingan06.cn


<!-- 参考信息 -->