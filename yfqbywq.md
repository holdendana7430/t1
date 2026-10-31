代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hq.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://py.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://ke.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qf.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sv.newstarts.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ps.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ad.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://tg.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vc.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ol.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://sy.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://ue.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sf.bookmarksfly.cn

Go:   // 手写循环
来源：http://zf.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vz.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sf.colortex.cn

[D15] 去重
来源：http://it.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mx.szxytkj.cn

PHP:  array_unique($arr);
来源：http://ek.newstarts.cn

JS:   [...new Set(arr)]
来源：http://pe.9csxet.cn

TS:   [...new Set(arr)]
来源：http://pa.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qf.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dh.szxytkj.cn

Ruby: arr.uniq
来源：http://rn.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://oz.nicolike.cn

[D16] 求和与平均值
来源：http://af.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wr.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gl.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aq.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vz.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uw.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://in.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ja.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://lr.jctech888.com.cn

[D17] 最大值与最小值
来源：http://qs.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://xx.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://ri.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bt.panjiajie.cn

TS:   Math.max(...arr);
来源：http://cy.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qb.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ny.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://ln.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://jl.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://do.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://px.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://zq.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pc.bjjhwx.cn

TS:   nested.flat();
来源：http://bg.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vc.haigaiapp.cn

Go:   // 手写双层循环
来源：http://zt.bjjhwx.cn

Ruby: nested.flatten
来源：http://vr.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hv.hahajie.cn

[D19] 按字段分组
来源：http://ey.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ho.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jn.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tn.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rc.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fp.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://xy.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tg.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mf.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://yh.szsharing.cn

Py:   Counter(arr)
来源：http://hj.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://ra.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ng.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ys.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tw.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://no.shxzskj.cn

Ruby: arr.tally
来源：http://du.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zm.hahajie.cn

[D21] 判断是否包含某元素
来源：http://jj.lnxyls.cn

Py:   x in arr
来源：http://kt.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://oj.newstarts.cn

JS:   arr.includes(x)
来源：http://lz.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://fa.521024.cn

Java: list.contains(x)
来源：http://wu.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://zb.hahajie.cn

Ruby: arr.include?(x)
来源：http://al.asd995.cn

C#:   list.Contains(x)
来源：http://cd.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://xd.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ye.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oh.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cw.huixiangedu.cn

TS:   [...arr];
来源：http://re.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://bd.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ap.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://qg.nicolike.cn

C#:   new List<int>(list);
来源：http://gp.hahajie.cn

[D23] reduce 累积计算
来源：http://tp.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gl.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dz.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xe.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lq.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dh.szxytkj.cn

Go:   // 手写循环
来源：http://ds.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ig.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zf.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://od.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ht.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vr.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kt.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://co.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gn.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://la.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sk.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qn.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://rf.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vi.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eh.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://at.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tv.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ep.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mw.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ch.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aq.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://gv.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://lp.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://ei.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://nn.yuexingan06.cn

TS:   arr.join(", ")
来源：http://qh.shxzukj.cn

Java: String.join(", ", list)
来源：http://mc.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://yp.asd995.cn

Ruby: arr.join(", ")
来源：http://lf.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://wu.szsharing.cn

================================================================================
来源：http://ki.panjiajie.cn

E. 字符串处理
来源：http://ju.jctech888.com.cn

================================================================================
来源：http://gy.huanxung.cn

[E01] 拼接字符串
来源：http://zj.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mo.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nk.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zi.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ev.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zm.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://in.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tx.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hy.gzmigu.cn

[E02] 重复字符串
来源：http://gn.shxzukj.cn

Py:   "ab" * 3
来源：http://vw.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://xv.szsharing.cn

JS:   "ab".repeat(3)
来源：http://zg.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://uz.colortex.cn

Java: "ab".repeat(3)
来源：http://qd.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://uc.hahajie.cn

Ruby: "ab" * 3
来源：http://ku.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xn.szsharing.cn

[E03] 截取子串
来源：http://cg.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tx.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oq.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oy.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://ix.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://mk.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sb.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://by.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://wr.bookmarksfly.cn

[E04] 查找子串位置
来源：http://su.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://zz.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://mb.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ys.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://zn.521024.cn

Java: s.indexOf("x")
来源：http://nq.521024.cn

Go:   strings.Index(s, "x")
来源：http://ao.colortex.cn

Ruby: s.index("x")
来源：http://jf.huanxung.cn

C#:   s.IndexOf("x")
来源：http://tq.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yb.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ps.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vt.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dy.bjjhwx.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ym.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jv.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bn.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yi.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qo.colortex.cn

[E06] 替换子串
来源：http://pm.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://be.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://qr.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qv.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://py.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lb.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kd.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xt.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://nj.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://ve.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xt.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pg.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ki.bookmarksfly.cn

TS:   s.split(",")
来源：http://jz.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ut.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cj.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://yj.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vn.huanxung.cn

[E08] 数组按分隔符合并
来源：http://sl.newstarts.cn

Py:   ",".join(items)
来源：http://vo.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://pp.asd995.cn

JS:   items.join(",")
来源：http://vb.muxihuayi.cn

TS:   items.join(",")
来源：http://vd.haigaiapp.cn

Java: String.join(",", items)
来源：http://eh.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://pm.asd995.cn

Ruby: items.join(",")
来源：http://qq.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://bt.9csxet.cn

[E09] 去除所有空白字符
来源：http://qf.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sy.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dw.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://ad.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ev.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://gc.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tb.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sj.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lw.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://xb.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fi.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uj.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://sy.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://jb.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://wx.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rz.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lq.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fc.yuntaijiaju.cn

[E11] 反转字符串
来源：http://pu.huixinmuqiang.cn

Py:   s[::-1]
来源：http://nv.newstarts.cn

PHP:  strrev($s);
来源：http://yl.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://or.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://fi.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sl.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nt.muxihuayi.cn

Ruby: s.reverse
来源：http://lc.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oa.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://hp.gzmigu.cn

Py:   s.count("a")
来源：http://ad.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://oh.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://nc.szsharing.cn

TS:   s.split("a").length - 1
来源：http://mi.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fg.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://hc.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://gw.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://cq.9csxet.cn

[E13] 逐字符遍历
来源：http://ht.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://hm.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://si.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ew.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ub.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xi.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xa.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ar.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ht.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://ae.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vj.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nq.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dq.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hf.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gi.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zu.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ny.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bp.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://eb.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vo.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tx.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://no.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://so.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oq.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ur.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xb.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zn.hnjuh.cn

[E16] 数字千分位
来源：http://qs.asd995.cn

Py:   f"{1234567:,}"
来源：http://ov.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://no.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nv.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yy.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jd.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gm.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ce.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://gl.bookmarksfly.cn

[E17] 首字母大写
来源：http://dm.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sj.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://du.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ak.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lq.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hv.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pe.huanxung.cn

Ruby: s.capitalize
来源：http://te.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wz.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://is.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jg.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ho.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ai.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ib.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://se.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rv.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vq.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gj.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://bd.newstarts.cn

Py:   s.splitlines()
来源：http://ra.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zf.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://xl.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://do.chemitech.net.cn

Java: s.lines().toList()
来源：http://lh.shtwfgs.cn

Go:   strings.Split(s, "\n")
来源：http://at.yuntaijiaju.cn

Ruby: s.lines
来源：http://dg.gzmigu.cn

C#:   s.Split('\n')
来源：http://te.huanxung.cn

[E20] 判断字符串是否为空
来源：http://gx.shxzukj.cn

Py:   if not s:
来源：http://rv.jctech888.com.cn


<!-- 参考信息 -->