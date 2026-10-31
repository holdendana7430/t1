代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://ew.yuntaijiaju.cn

Go:   // 手写循环
来源：http://mv.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dc.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nr.gzmigu.cn

[D15] 去重
来源：http://kq.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oq.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://ae.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://tt.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ty.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cu.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kn.huixiangedu.cn

Ruby: arr.uniq
来源：http://ea.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://qi.colortex.cn

[D16] 求和与平均值
来源：http://jb.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uv.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pc.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yb.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nz.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yr.newstarts.cn

Go:   // 手写循环累加
来源：http://zu.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vl.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://rw.muxihuayi.cn

[D17] 最大值与最小值
来源：http://pj.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://hh.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://sc.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vj.nszjky.cn

TS:   Math.max(...arr);
来源：http://jq.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ni.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://la.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://qs.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://it.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://zs.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zf.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://wr.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fu.nszjky.cn

TS:   nested.flat();
来源：http://ts.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jl.huanxung.cn

Go:   // 手写双层循环
来源：http://mw.newstarts.cn

Ruby: nested.flatten
来源：http://ho.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fy.shtwfgs.cn

[D19] 按字段分组
来源：http://nn.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wx.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tv.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aj.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ot.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yf.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://zi.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gi.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://md.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://fr.shxzukj.cn

Py:   Counter(arr)
来源：http://lg.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://th.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lv.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://us.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sq.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://js.panjiajie.cn

Ruby: arr.tally
来源：http://uq.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vw.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://sl.jctech888.com.cn

Py:   x in arr
来源：http://td.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://op.nicolike.cn

JS:   arr.includes(x)
来源：http://az.shxzskj.cn

TS:   arr.includes(x)
来源：http://za.521024.cn

Java: list.contains(x)
来源：http://db.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://vr.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://be.shxzskj.cn

C#:   list.Contains(x)
来源：http://gr.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://pv.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://id.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fc.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ss.shtwfgs.cn

TS:   [...arr];
来源：http://hb.newstarts.cn

Java: new ArrayList<>(list);
来源：http://pc.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xg.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://px.bjjhwx.cn

C#:   new List<int>(list);
来源：http://dz.shtwfgs.cn

[D23] reduce 累积计算
来源：http://xb.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zq.newstarts.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://at.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://za.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wq.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hg.gzmigu.cn

Go:   // 手写循环
来源：http://xv.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bn.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ju.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://ad.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mu.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uh.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bs.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bw.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eo.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ju.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ul.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ub.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://dx.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://en.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://js.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jt.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ni.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://to.shxzskj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wr.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://av.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tl.szxytkj.cn

[D26] 数组转字符串
来源：http://zk.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://kk.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://lt.521024.cn

JS:   arr.join(", ")
来源：http://ld.colortex.cn

TS:   arr.join(", ")
来源：http://kq.shxzskj.cn

Java: String.join(", ", list)
来源：http://gz.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://yd.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://bu.hnjuh.cn

C#:   string.Join(", ", list)
来源：http://tn.jianghongdianzi.cn

================================================================================
来源：http://ky.shxzukj.cn

E. 字符串处理
来源：http://op.huixiangedu.cn

================================================================================
来源：http://ni.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://bx.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dl.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cj.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tn.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ch.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://av.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://em.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ss.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lc.wgjwhj.cn

[E02] 重复字符串
来源：http://nb.panjiajie.cn

Py:   "ab" * 3
来源：http://bf.gzmigu.cn

PHP:  str_repeat("ab", 3);
来源：http://gt.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://zv.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://gc.shxzukj.cn

Java: "ab".repeat(3)
来源：http://yz.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://gf.lnxyls.cn

Ruby: "ab" * 3
来源：http://ie.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bi.jctech888.com.cn

[E03] 截取子串
来源：http://xc.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mv.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bo.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uy.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://lo.nszjky.cn

Java: s.substring(1, 4)
来源：http://js.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tw.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bf.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://op.huixiangedu.cn

[E04] 查找子串位置
来源：http://gf.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://xu.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://pa.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jl.gzmigu.cn

TS:   s.indexOf("x")
来源：http://ul.lnxyls.cn

Java: s.indexOf("x")
来源：http://ap.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://qu.521024.cn

Ruby: s.index("x")
来源：http://sh.szsharing.cn

C#:   s.IndexOf("x")
来源：http://cr.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kb.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rj.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ox.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rx.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ac.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lh.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ha.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pz.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ef.colortex.cn

[E06] 替换子串
来源：http://aq.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kk.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://bn.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xi.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://iq.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zm.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pj.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kw.colortex.cn

C#:   s.Replace("a", "b")
来源：http://jz.asd995.cn

[E07] 按分隔符拆分
来源：http://aa.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xp.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://og.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sz.muxihuayi.cn

TS:   s.split(",")
来源：http://eb.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yk.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nu.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://bt.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://az.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://bu.bookmarksfly.cn

Py:   ",".join(items)
来源：http://bl.yuexingan06.cn

PHP:  implode(",", $items);
来源：http://mj.jianghongdianzi.cn

JS:   items.join(",")
来源：http://ti.panjiajie.cn

TS:   items.join(",")
来源：http://hi.nszjky.cn

Java: String.join(",", items)
来源：http://mo.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://cq.9csxet.cn

Ruby: items.join(",")
来源：http://zr.lnxyls.cn

C#:   string.Join(",", items)
来源：http://il.shxzskj.cn

[E09] 去除所有空白字符
来源：http://bt.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://re.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fl.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://by.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ak.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://rc.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nr.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://th.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oy.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://sp.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kv.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ev.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://ru.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://kw.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://aa.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qt.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ml.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dp.asd995.cn

[E11] 反转字符串
来源：http://vp.huixiangedu.cn

Py:   s[::-1]
来源：http://gp.nicolike.cn

PHP:  strrev($s);
来源：http://rr.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://pw.colortex.cn

TS:   [...s].reverse().join("")
来源：http://pd.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://md.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rn.hahajie.cn

Ruby: s.reverse
来源：http://il.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ol.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://bv.gzmigu.cn

Py:   s.count("a")
来源：http://av.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://kx.nszjky.cn

JS:   s.split("a").length - 1
来源：http://zh.huanxung.cn

TS:   s.split("a").length - 1
来源：http://wb.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pu.colortex.cn

Go:   strings.Count(s, "a")
来源：http://fc.newstarts.cn

Ruby: s.count("a")
来源：http://sf.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://ms.yuexingan06.cn

[E13] 逐字符遍历
来源：http://fz.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://xv.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ou.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://np.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ic.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dm.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://il.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tm.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ta.521024.cn

[E14] URL 编码与 Base64
来源：http://me.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ao.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qp.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mb.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://na.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ep.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ss.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ov.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xt.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://mn.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://on.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xc.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://de.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yu.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uc.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zs.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oo.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qq.hahajie.cn

[E16] 数字千分位
来源：http://ae.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://ns.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://xj.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ju.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zi.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pu.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bj.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cz.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://sh.szxytkj.cn

[E17] 首字母大写
来源：http://fb.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ff.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wi.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qi.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tk.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://io.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qa.bookmarksfly.cn

Ruby: s.capitalize
来源：http://qi.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vd.szsharing.cn

[E18] 模板占位符替换
来源：http://dw.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xz.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vh.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zb.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mz.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rm.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://al.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gl.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wo.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://tn.haigaiapp.cn

Py:   s.splitlines()
来源：http://tp.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xw.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ny.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://fm.hnjuh.cn

Java: s.lines().toList()
来源：http://pz.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://uo.lnxyls.cn

Ruby: s.lines
来源：http://yo.huanxung.cn

C#:   s.Split('\n')
来源：http://fw.nicolike.cn

[E20] 判断字符串是否为空
来源：http://za.haigaiapp.cn

Py:   if not s:
来源：http://yq.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kx.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dv.huixiangedu.cn

TS:   if (s === "") {}
来源：http://ub.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://mu.panjiajie.cn

Go:   if s == "" {}
来源：http://uy.yuexingan06.cn

Ruby: if s.empty?
来源：http://oo.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qo.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://ka.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://or.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zg.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xk.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mt.nszjky.cn


<!-- 参考信息 -->