代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://py.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yb.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xw.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://wj.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bi.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ox.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://xk.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://cm.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ae.szsharing.cn

Go:   // 手写循环
来源：http://le.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nj.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ns.asd995.cn

[D15] 去重
来源：http://oi.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://us.nicolike.cn

PHP:  array_unique($arr);
来源：http://if.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://zp.nicolike.cn

TS:   [...new Set(arr)]
来源：http://it.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oj.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sf.huixiangedu.cn

Ruby: arr.uniq
来源：http://sz.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://jx.wgjwhj.cn

[D16] 求和与平均值
来源：http://ju.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ck.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mn.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gl.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://je.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wm.shxzskj.cn

Go:   // 手写循环累加
来源：http://ca.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ui.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://xa.gzmigu.cn

[D17] 最大值与最小值
来源：http://cf.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://np.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://gn.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dw.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://uo.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sn.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oo.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://jc.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://dg.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://iz.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ui.521024.cn

PHP:  array_merge(...$nested);
来源：http://of.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dg.colortex.cn

TS:   nested.flat();
来源：http://mo.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xp.chemitech.net.cn

Go:   // 手写双层循环
来源：http://tl.yuexingan06.cn

Ruby: nested.flatten
来源：http://rr.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qi.szxytkj.cn

[D19] 按字段分组
来源：http://vw.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jq.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wn.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tq.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://am.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wd.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://pg.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jf.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sf.asd995.cn

[D20] 统计每个元素出现次数
来源：http://vq.521024.cn

Py:   Counter(arr)
来源：http://vx.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://ck.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fr.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nj.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ex.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://si.gzmigu.cn

Ruby: arr.tally
来源：http://qq.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ia.nicolike.cn

[D21] 判断是否包含某元素
来源：http://my.huixiangedu.cn

Py:   x in arr
来源：http://zr.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://zs.asd995.cn

JS:   arr.includes(x)
来源：http://qx.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://ej.szsharing.cn

Java: list.contains(x)
来源：http://cn.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://lm.9csxet.cn

Ruby: arr.include?(x)
来源：http://lg.newstarts.cn

C#:   list.Contains(x)
来源：http://qd.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://nn.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ba.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lb.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qn.chemitech.net.cn

TS:   [...arr];
来源：http://ha.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://pd.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zv.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://sv.bjjhwx.cn

C#:   new List<int>(list);
来源：http://mt.szxytkj.cn

[D23] reduce 累积计算
来源：http://yu.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rh.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aw.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wd.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://no.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cg.lnxyls.cn

Go:   // 手写循环
来源：http://sk.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ha.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ip.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://hi.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tj.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vx.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bh.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kb.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yu.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gd.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lq.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kx.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://dv.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fn.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mi.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pr.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://em.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xn.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xn.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nx.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sf.colortex.cn

[D26] 数组转字符串
来源：http://vp.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://ky.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://sb.521024.cn

JS:   arr.join(", ")
来源：http://wm.hahajie.cn

TS:   arr.join(", ")
来源：http://pi.nicolike.cn

Java: String.join(", ", list)
来源：http://bh.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://vg.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://ld.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://ho.huixinmuqiang.cn

================================================================================
来源：http://uy.gzmigu.cn

E. 字符串处理
来源：http://hs.yuexingan06.cn

================================================================================
来源：http://sx.muxihuayi.cn

[E01] 拼接字符串
来源：http://en.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ja.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://un.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tc.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://np.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jn.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lw.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ee.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tj.gzmigu.cn

[E02] 重复字符串
来源：http://ua.shtwfgs.cn

Py:   "ab" * 3
来源：http://jr.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://sy.521024.cn

JS:   "ab".repeat(3)
来源：http://js.9csxet.cn

TS:   "ab".repeat(3)
来源：http://ot.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://ty.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://re.lnxyls.cn

Ruby: "ab" * 3
来源：http://yr.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pt.yuexingan06.cn

[E03] 截取子串
来源：http://ck.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sr.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ux.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://un.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://sy.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://fj.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iy.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sa.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://xz.nszjky.cn

[E04] 查找子串位置
来源：http://wd.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://mf.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://jr.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://um.szsharing.cn

TS:   s.indexOf("x")
来源：http://qt.wgjwhj.cn

Java: s.indexOf("x")
来源：http://au.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://qz.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://kv.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://rw.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yj.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ii.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fq.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://om.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tp.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pu.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ge.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tq.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rc.521024.cn

[E06] 替换子串
来源：http://mh.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kk.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://gn.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zr.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://bt.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aa.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mt.asd995.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wj.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://mf.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://re.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ax.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://da.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iu.huanxung.cn

TS:   s.split(",")
来源：http://vu.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iq.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fs.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://je.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://di.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://ph.bjjhwx.cn

Py:   ",".join(items)
来源：http://og.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://df.9csxet.cn

JS:   items.join(",")
来源：http://ee.nicolike.cn

TS:   items.join(",")
来源：http://fo.shxzukj.cn

Java: String.join(",", items)
来源：http://ub.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://ri.szsharing.cn

Ruby: items.join(",")
来源：http://iz.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://hy.huanxung.cn

[E09] 去除所有空白字符
来源：http://vd.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kn.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uu.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://xb.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://rf.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://iz.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ko.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ui.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://am.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://bt.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://it.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cg.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://vg.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://yk.asd995.cn

Java: String.format("%03d", 7)
来源：http://ri.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lm.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mb.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cc.szxytkj.cn

[E11] 反转字符串
来源：http://rx.newstarts.cn

Py:   s[::-1]
来源：http://od.szxytkj.cn

PHP:  strrev($s);
来源：http://gp.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://af.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://tl.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uj.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wb.szsharing.cn

Ruby: s.reverse
来源：http://vs.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dv.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://na.huixiangedu.cn

Py:   s.count("a")
来源：http://zp.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://jp.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://zd.521024.cn

TS:   s.split("a").length - 1
来源：http://wz.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vm.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://bl.huanxung.cn

Ruby: s.count("a")
来源：http://ua.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://lu.nszjky.cn

[E13] 逐字符遍历
来源：http://ij.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://bh.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://om.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lr.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://og.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wi.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://co.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ru.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yc.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://zu.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qk.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qy.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pg.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gf.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://es.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bo.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vf.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ig.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://dq.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cj.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bl.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nr.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ow.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qi.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nv.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://by.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dk.jianghongdianzi.cn

[E16] 数字千分位
来源：http://yx.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://is.colortex.cn

PHP:  number_format(1234567);
来源：http://fz.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ie.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dl.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://za.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xy.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://va.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://gc.shtwfgs.cn

[E17] 首字母大写
来源：http://ms.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://km.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tf.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dl.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gq.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jh.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yr.shtwfgs.cn

Ruby: s.capitalize
来源：http://gj.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lg.colortex.cn

[E18] 模板占位符替换
来源：http://sg.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hp.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://le.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eh.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nh.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bq.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zu.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tm.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gm.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://wj.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://ix.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jg.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://fa.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://oo.hnjuh.cn

Java: s.lines().toList()
来源：http://sw.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://hd.asd995.cn

Ruby: s.lines
来源：http://id.gzmigu.cn

C#:   s.Split('\n')
来源：http://pc.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://jb.szxytkj.cn

Py:   if not s:
来源：http://dp.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vu.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ut.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://is.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://in.gzmigu.cn


<!-- 参考信息 -->