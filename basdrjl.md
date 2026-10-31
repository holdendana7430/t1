代发 wailian999

Ruby: arr.index(x)
来源：http://dz.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://cs.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://dw.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kx.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bm.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://ma.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://ss.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tm.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ix.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lm.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rj.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://wn.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fg.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ki.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://ke.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://gg.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jo.szxytkj.cn

Go:   // 手写循环
来源：http://ji.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bc.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mm.szsharing.cn

[D15] 去重
来源：http://ee.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://re.hahajie.cn

PHP:  array_unique($arr);
来源：http://bm.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://ww.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://nh.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ra.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sk.szxytkj.cn

Ruby: arr.uniq
来源：http://dn.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://dn.panjiajie.cn

[D16] 求和与平均值
来源：http://of.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://md.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mb.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://au.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pw.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hk.lnxyls.cn

Go:   // 手写循环累加
来源：http://ps.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xy.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://ui.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://gu.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://ft.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://zi.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pu.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://bs.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qp.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ba.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://od.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://rb.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://ok.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wu.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://xt.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yq.lnxyls.cn

TS:   nested.flat();
来源：http://sy.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rv.huixiangedu.cn

Go:   // 手写双层循环
来源：http://bl.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://dn.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sw.muxihuayi.cn

[D19] 按字段分组
来源：http://kt.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yx.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ty.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ao.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vz.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ng.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://jb.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dt.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nw.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://ve.huanxung.cn

Py:   Counter(arr)
来源：http://yp.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://tj.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jy.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dd.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://lk.szxytkj.cn

Ruby: arr.tally
来源：http://gg.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ro.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://ge.yuntaijiaju.cn

Py:   x in arr
来源：http://nu.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://gk.panjiajie.cn

JS:   arr.includes(x)
来源：http://dp.szxytkj.cn

TS:   arr.includes(x)
来源：http://yb.bookmarksfly.cn

Java: list.contains(x)
来源：http://oc.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://gm.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://zz.nszjky.cn

C#:   list.Contains(x)
来源：http://lj.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://gw.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mb.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hp.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sw.panjiajie.cn

TS:   [...arr];
来源：http://aw.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://fp.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yz.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://pu.9csxet.cn

C#:   new List<int>(list);
来源：http://fo.hnjuh.cn

[D23] reduce 累积计算
来源：http://lr.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ty.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kq.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ks.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://al.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ar.hahajie.cn

Go:   // 手写循环
来源：http://pz.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ug.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ft.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://iu.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sj.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iq.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://js.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zt.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tl.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ox.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ps.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tb.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://za.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ez.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rs.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oi.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ik.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ml.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pv.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lg.colortex.cn

[D26] 数组转字符串
来源：http://jv.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://br.asd995.cn

PHP:  implode(", ", $arr);
来源：http://mc.521024.cn

JS:   arr.join(", ")
来源：http://iz.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://ld.521024.cn

Java: String.join(", ", list)
来源：http://mb.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://qa.szxytkj.cn

Ruby: arr.join(", ")
来源：http://xi.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://so.huanxung.cn

================================================================================
来源：http://fb.jianghongdianzi.cn

E. 字符串处理
来源：http://li.521024.cn

================================================================================
来源：http://go.bookmarksfly.cn

[E01] 拼接字符串
来源：http://vm.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sk.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ma.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hp.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jt.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zh.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lg.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://df.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vz.9csxet.cn

[E02] 重复字符串
来源：http://ph.shxzukj.cn

Py:   "ab" * 3
来源：http://np.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://wc.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://ms.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://sh.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://ng.panjiajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://gm.newstarts.cn

Ruby: "ab" * 3
来源：http://eh.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qj.bjjhwx.cn

[E03] 截取子串
来源：http://xc.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nq.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wu.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yv.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://ki.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://bi.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eo.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pn.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://lp.colortex.cn

[E04] 查找子串位置
来源：http://mo.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://xv.szsharing.cn

PHP:  strpos($s, "x");
来源：http://wx.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ij.521024.cn

TS:   s.indexOf("x")
来源：http://ru.wgjwhj.cn

Java: s.indexOf("x")
来源：http://sv.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://xs.muxihuayi.cn

Ruby: s.index("x")
来源：http://nk.9csxet.cn

C#:   s.IndexOf("x")
来源：http://gt.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lg.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://of.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xt.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ya.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zn.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kc.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://an.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cc.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gg.szsharing.cn

[E06] 替换子串
来源：http://ba.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zv.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://ag.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://is.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://uc.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yn.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://em.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ln.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://fq.hahajie.cn

[E07] 按分隔符拆分
来源：http://gg.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lo.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xu.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://he.9csxet.cn

TS:   s.split(",")
来源：http://jn.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hd.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xo.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://lj.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://te.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://un.bjjhwx.cn

Py:   ",".join(items)
来源：http://jh.lnxyls.cn

PHP:  implode(",", $items);
来源：http://hv.wgjwhj.cn

JS:   items.join(",")
来源：http://zc.haigaiapp.cn

TS:   items.join(",")
来源：http://uj.szxytkj.cn

Java: String.join(",", items)
来源：http://sb.colortex.cn

Go:   strings.Join(items, ",")
来源：http://yn.9csxet.cn

Ruby: items.join(",")
来源：http://zl.colortex.cn

C#:   string.Join(",", items)
来源：http://oh.huanxung.cn

[E09] 去除所有空白字符
来源：http://sr.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yv.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wt.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://pf.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://em.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://lb.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bg.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ew.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wn.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://ld.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yo.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sa.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://gb.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://aw.huanxung.cn

Java: String.format("%03d", 7)
来源：http://sp.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vt.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qu.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xa.jianghongdianzi.cn

[E11] 反转字符串
来源：http://et.nicolike.cn

Py:   s[::-1]
来源：http://ji.colortex.cn

PHP:  strrev($s);
来源：http://cu.colortex.cn

JS:   [...s].reverse().join("")
来源：http://nn.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://hy.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ll.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nn.nszjky.cn

Ruby: s.reverse
来源：http://mg.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://of.huanxung.cn

[E12] 统计某字符出现次数
来源：http://ns.shtwfgs.cn

Py:   s.count("a")
来源：http://gb.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://ha.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://qz.szsharing.cn

TS:   s.split("a").length - 1
来源：http://pk.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vo.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://md.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://sb.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://wj.521024.cn

[E13] 逐字符遍历
来源：http://gb.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://kv.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rz.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zg.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kc.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lu.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bj.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jn.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://om.hahajie.cn

[E14] URL 编码与 Base64
来源：http://zu.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vi.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ic.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aj.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ab.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wz.bookmarksfly.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ob.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yf.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://vt.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ci.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pr.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xc.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ux.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lp.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oo.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cj.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iv.shtwfgs.cn

[E16] 数字千分位
来源：http://ha.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://mf.hahajie.cn

PHP:  number_format(1234567);
来源：http://kb.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mr.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fb.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vy.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nb.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qb.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://px.hnjuh.cn

[E17] 首字母大写
来源：http://vf.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cs.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vu.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uj.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nf.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ew.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yv.jctech888.com.cn

Ruby: s.capitalize
来源：http://wl.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nm.shxzukj.cn

[E18] 模板占位符替换
来源：http://dx.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ar.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://le.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tg.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vs.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lk.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://td.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wr.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vj.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://pv.jctech888.com.cn

Py:   s.splitlines()
来源：http://jg.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qx.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://ob.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ib.newstarts.cn

Java: s.lines().toList()
来源：http://qj.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://su.jianghongdianzi.cn


<!-- 参考信息 -->