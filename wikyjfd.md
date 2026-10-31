代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://cg.huixiangedu.cn

Go:   // 手写循环
来源：http://us.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hs.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dc.huanxung.cn

[D15] 去重
来源：http://mz.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gr.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://ii.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://cn.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://cy.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fb.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ru.yuexingan06.cn

Ruby: arr.uniq
来源：http://dp.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://lu.haigaiapp.cn

[D16] 求和与平均值
来源：http://mb.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zp.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ei.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pj.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ql.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zv.szxytkj.cn

Go:   // 手写循环累加
来源：http://mb.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xr.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://za.colortex.cn

[D17] 最大值与最小值
来源：http://cw.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://tf.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://ec.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jx.shxzukj.cn

TS:   Math.max(...arr);
来源：http://uq.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fz.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://od.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ei.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://ik.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://cr.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://al.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://ny.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vc.jctech888.com.cn

TS:   nested.flat();
来源：http://sh.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hm.szxytkj.cn

Go:   // 手写双层循环
来源：http://da.hnjuh.cn

Ruby: nested.flatten
来源：http://ua.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bg.haigaiapp.cn

[D19] 按字段分组
来源：http://jo.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wp.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mm.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nm.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zc.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://as.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://lr.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rc.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cr.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://ru.szxytkj.cn

Py:   Counter(arr)
来源：http://yx.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://ld.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jd.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://au.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nv.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://ks.shxzskj.cn

Ruby: arr.tally
来源：http://bt.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yt.nszjky.cn

[D21] 判断是否包含某元素
来源：http://ol.shxzukj.cn

Py:   x in arr
来源：http://xx.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://zm.huanxung.cn

JS:   arr.includes(x)
来源：http://si.szsharing.cn

TS:   arr.includes(x)
来源：http://vk.nszjky.cn

Java: list.contains(x)
来源：http://mi.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://zj.nicolike.cn

Ruby: arr.include?(x)
来源：http://rc.hahajie.cn

C#:   list.Contains(x)
来源：http://cq.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://ev.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pr.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://px.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ej.szsharing.cn

TS:   [...arr];
来源：http://qy.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://ao.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cr.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://tt.yuexingan06.cn

C#:   new List<int>(list);
来源：http://wg.haigaiapp.cn

[D23] reduce 累积计算
来源：http://os.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sm.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dj.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ox.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hu.huanxung.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gl.chemitech.net.cn

Go:   // 手写循环
来源：http://gd.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oz.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dl.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://xs.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ll.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hl.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ma.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nl.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uh.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xa.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ro.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fe.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://pp.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tf.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jl.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sk.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jf.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fx.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vm.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://er.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zd.yuexingan06.cn

[D26] 数组转字符串
来源：http://jw.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://sv.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://kc.jctech888.com.cn

JS:   arr.join(", ")
来源：http://fd.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://ot.wgjwhj.cn

Java: String.join(", ", list)
来源：http://lc.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://jn.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://sr.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://pt.yuntaijiaju.cn

================================================================================
来源：http://gt.szsharing.cn

E. 字符串处理
来源：http://qt.521024.cn

================================================================================
来源：http://wx.gzmigu.cn

[E01] 拼接字符串
来源：http://vs.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rx.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://au.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mb.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ge.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xv.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qm.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qa.hahajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hu.9csxet.cn

[E02] 重复字符串
来源：http://hz.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://kz.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://dt.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://us.colortex.cn

TS:   "ab".repeat(3)
来源：http://dx.hahajie.cn

Java: "ab".repeat(3)
来源：http://nx.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://ie.shxzskj.cn

Ruby: "ab" * 3
来源：http://xm.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xz.muxihuayi.cn

[E03] 截取子串
来源：http://nv.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ip.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pa.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://si.asd995.cn

TS:   s.slice(1, 4)
来源：http://qb.szsharing.cn

Java: s.substring(1, 4)
来源：http://xg.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zn.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gn.colortex.cn

C#:   s.Substring(1, 3)
来源：http://ck.9csxet.cn

[E04] 查找子串位置
来源：http://fu.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://je.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://um.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hy.nszjky.cn

TS:   s.indexOf("x")
来源：http://yw.hahajie.cn

Java: s.indexOf("x")
来源：http://vy.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://gh.521024.cn

Ruby: s.index("x")
来源：http://og.newstarts.cn

C#:   s.IndexOf("x")
来源：http://rt.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pa.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ai.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fi.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tj.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jq.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sy.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://up.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rj.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://js.shxzskj.cn

[E06] 替换子串
来源：http://lm.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nj.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://kq.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fo.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://xj.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hd.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vw.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jr.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://hk.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://qn.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://en.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kg.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pc.bookmarksfly.cn

TS:   s.split(",")
来源：http://ni.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kg.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tl.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://hk.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lk.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://ai.muxihuayi.cn

Py:   ",".join(items)
来源：http://di.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://tp.newstarts.cn

JS:   items.join(",")
来源：http://ca.yuexingan06.cn

TS:   items.join(",")
来源：http://ow.hnjuh.cn

Java: String.join(",", items)
来源：http://mx.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://fi.yuexingan06.cn

Ruby: items.join(",")
来源：http://bl.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://ro.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://rn.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://be.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bw.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://gd.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://zx.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://zq.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fr.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gl.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ig.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://oc.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://it.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ec.521024.cn

JS:   "7".padStart(3, "0")
来源：http://mx.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://wj.szsharing.cn

Java: String.format("%03d", 7)
来源：http://ku.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uy.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tr.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ew.lnxyls.cn

[E11] 反转字符串
来源：http://qn.shxzskj.cn

Py:   s[::-1]
来源：http://mk.haigaiapp.cn

PHP:  strrev($s);
来源：http://bo.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://kw.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://rg.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lo.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zd.nszjky.cn

Ruby: s.reverse
来源：http://ep.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zc.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://kp.panjiajie.cn

Py:   s.count("a")
来源：http://vi.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://mp.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://fz.hahajie.cn

TS:   s.split("a").length - 1
来源：http://fd.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kx.521024.cn

Go:   strings.Count(s, "a")
来源：http://zr.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://re.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://ps.shxzukj.cn

[E13] 逐字符遍历
来源：http://gf.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://xq.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ss.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gn.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oh.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ft.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aw.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://te.521024.cn

[E14] URL 编码与 Base64
来源：http://nx.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lk.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vn.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xs.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://do.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://as.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qd.wgjwhj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pr.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://li.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://cf.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://du.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uk.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hk.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://or.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ro.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bs.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yu.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nb.hahajie.cn

[E16] 数字千分位
来源：http://vo.asd995.cn

Py:   f"{1234567:,}"
来源：http://qd.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://wt.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cc.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://us.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ba.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fh.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fd.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://xp.panjiajie.cn

[E17] 首字母大写
来源：http://iw.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qm.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fi.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ya.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cr.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bc.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ip.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://lb.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zo.yuexingan06.cn

[E18] 模板占位符替换
来源：http://td.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nq.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xo.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xf.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ym.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mn.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ls.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://el.colortex.cn

[E19] 多行文本按行拆分
来源：http://tu.newstarts.cn

Py:   s.splitlines()
来源：http://wo.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://to.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://qp.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://bv.wgjwhj.cn

Java: s.lines().toList()
来源：http://jg.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://hg.lnxyls.cn

Ruby: s.lines
来源：http://lh.9csxet.cn

C#:   s.Split('\n')
来源：http://li.nszjky.cn

[E20] 判断字符串是否为空
来源：http://uf.521024.cn

Py:   if not s:
来源：http://ah.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vv.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ui.shxzukj.cn

TS:   if (s === "") {}
来源：http://dg.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://ur.huanxung.cn

Go:   if s == "" {}
来源：http://ck.szsharing.cn

Ruby: if s.empty?
来源：http://ou.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gm.gzmigu.cn

[E21] 超长截断加省略号
来源：http://fi.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://co.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hh.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://py.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ao.muxihuayi.cn


<!-- 参考信息 -->