代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bl.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cy.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ib.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://od.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tb.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://et.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://cs.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://jl.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fk.521024.cn

Go:   // 手写循环
来源：http://fg.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qy.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nd.szxytkj.cn

[D15] 去重
来源：http://gg.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cq.szxytkj.cn

PHP:  array_unique($arr);
来源：http://sz.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://jg.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://zm.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pv.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ng.chemitech.net.cn

Ruby: arr.uniq
来源：http://tp.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://ok.newstarts.cn

[D16] 求和与平均值
来源：http://dn.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://do.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rg.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dt.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zt.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ey.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://ga.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ml.521024.cn

C#:   list.Sum();  list.Average()
来源：http://eb.haigaiapp.cn

[D17] 最大值与最小值
来源：http://tm.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://ge.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://bm.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ih.panjiajie.cn

TS:   Math.max(...arr);
来源：http://jh.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ya.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mp.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://ou.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://yq.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://cw.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bx.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://yf.shxzskj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zr.shxzukj.cn

TS:   nested.flat();
来源：http://ew.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wl.hnjuh.cn

Go:   // 手写双层循环
来源：http://gc.shxzukj.cn

Ruby: nested.flatten
来源：http://od.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rt.shxzukj.cn

[D19] 按字段分组
来源：http://ls.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kj.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://on.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nf.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sd.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zg.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://lm.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ne.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iz.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://cv.szxytkj.cn

Py:   Counter(arr)
来源：http://wr.asd995.cn

PHP:  array_count_values($arr);
来源：http://ci.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sp.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fa.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ua.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://gi.yuexingan06.cn

Ruby: arr.tally
来源：http://gh.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uc.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://oy.521024.cn

Py:   x in arr
来源：http://tu.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://wg.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://fv.shtwfgs.cn

TS:   arr.includes(x)
来源：http://zn.9csxet.cn

Java: list.contains(x)
来源：http://jr.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://en.szxytkj.cn

Ruby: arr.include?(x)
来源：http://if.muxihuayi.cn

C#:   list.Contains(x)
来源：http://nj.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://ur.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qi.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ld.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mo.szsharing.cn

TS:   [...arr];
来源：http://xj.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://rt.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uf.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://ix.szsharing.cn

C#:   new List<int>(list);
来源：http://dj.panjiajie.cn

[D23] reduce 累积计算
来源：http://yh.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cx.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ne.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yy.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ab.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zu.jctech888.com.cn

Go:   // 手写循环
来源：http://hj.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ni.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ut.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ai.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ib.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yw.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zb.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mv.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nh.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qh.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mv.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qu.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://ie.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ea.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dk.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cc.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fq.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zb.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tw.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jb.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://il.newstarts.cn

[D26] 数组转字符串
来源：http://aw.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://jn.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://hn.gzmigu.cn

JS:   arr.join(", ")
来源：http://xq.wgjwhj.cn

TS:   arr.join(", ")
来源：http://oq.nicolike.cn

Java: String.join(", ", list)
来源：http://in.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://ie.asd995.cn

Ruby: arr.join(", ")
来源：http://xz.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://hv.newstarts.cn

================================================================================
来源：http://db.szsharing.cn

E. 字符串处理
来源：http://wu.hahajie.cn

================================================================================
来源：http://yd.gzmigu.cn

[E01] 拼接字符串
来源：http://wp.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ox.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://it.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zj.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bz.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hf.panjiajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pz.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://te.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eo.newstarts.cn

[E02] 重复字符串
来源：http://ks.hnjuh.cn

Py:   "ab" * 3
来源：http://bm.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://be.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://gq.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://hg.shxzukj.cn

Java: "ab".repeat(3)
来源：http://pk.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://ea.bjjhwx.cn

Ruby: "ab" * 3
来源：http://nb.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kb.hahajie.cn

[E03] 截取子串
来源：http://nd.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yr.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iw.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rf.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://vo.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://sh.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cp.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sq.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://cy.szsharing.cn

[E04] 查找子串位置
来源：http://wx.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://gh.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://ia.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wb.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://bu.szsharing.cn

Java: s.indexOf("x")
来源：http://ah.521024.cn

Go:   strings.Index(s, "x")
来源：http://gw.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://cv.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://sa.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ux.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rb.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ho.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yx.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hf.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ut.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ym.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://as.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nh.yuntaijiaju.cn

[E06] 替换子串
来源：http://ot.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ee.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://xx.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ns.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://ag.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fd.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fi.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vd.521024.cn

C#:   s.Replace("a", "b")
来源：http://mx.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://du.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qp.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sm.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hh.szxytkj.cn

TS:   s.split(",")
来源：http://mn.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ga.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://og.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://fc.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gz.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://wp.hnjuh.cn

Py:   ",".join(items)
来源：http://xj.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://na.newstarts.cn

JS:   items.join(",")
来源：http://dy.9csxet.cn

TS:   items.join(",")
来源：http://wb.wgjwhj.cn

Java: String.join(",", items)
来源：http://xo.asd995.cn

Go:   strings.Join(items, ",")
来源：http://gj.huixiangedu.cn

Ruby: items.join(",")
来源：http://xm.shxzskj.cn

C#:   string.Join(",", items)
来源：http://dp.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://nl.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bj.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dq.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://vy.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://ot.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://aa.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rr.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mk.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vk.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://uv.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://da.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sd.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://ch.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://wb.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://uf.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ry.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ri.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ew.hahajie.cn

[E11] 反转字符串
来源：http://mb.jctech888.com.cn

Py:   s[::-1]
来源：http://zm.shtwfgs.cn

PHP:  strrev($s);
来源：http://mj.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://wx.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://sr.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eb.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vx.huixiangedu.cn

Ruby: s.reverse
来源：http://yw.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yz.szsharing.cn

[E12] 统计某字符出现次数
来源：http://uv.shtwfgs.cn

Py:   s.count("a")
来源：http://fa.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://lq.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://bg.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://ei.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ib.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://ma.lnxyls.cn

Ruby: s.count("a")
来源：http://or.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://tw.asd995.cn

[E13] 逐字符遍历
来源：http://uh.colortex.cn

Py:   for ch in s: print(ch)
来源：http://gz.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xw.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rp.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rc.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gm.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ns.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lg.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wm.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://ir.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ya.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vw.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xj.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dp.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lo.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ur.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ux.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sx.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://ws.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bc.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rq.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pt.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lw.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xt.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rs.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oj.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://im.muxihuayi.cn

[E16] 数字千分位
来源：http://zh.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://zl.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://be.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sf.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ve.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oo.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://en.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ax.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://jo.yuntaijiaju.cn

[E17] 首字母大写
来源：http://on.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fp.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cj.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kl.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ze.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rf.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://im.bookmarksfly.cn

Ruby: s.capitalize
来源：http://fk.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://me.newstarts.cn

[E18] 模板占位符替换
来源：http://qb.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zq.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ai.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tm.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qm.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bd.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ke.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aa.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wf.9csxet.cn

[E19] 多行文本按行拆分
来源：http://jx.muxihuayi.cn

Py:   s.splitlines()
来源：http://sn.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://og.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://cz.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://cu.shxzskj.cn

Java: s.lines().toList()
来源：http://il.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://hy.yuntaijiaju.cn

Ruby: s.lines
来源：http://qz.jctech888.com.cn

C#:   s.Split('\n')
来源：http://cr.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://io.asd995.cn

Py:   if not s:
来源：http://iy.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rk.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fu.huanxung.cn

TS:   if (s === "") {}
来源：http://pp.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://bc.hahajie.cn


<!-- 参考信息 -->