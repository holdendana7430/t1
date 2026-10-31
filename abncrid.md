代发 wailian999

[D15] 去重
来源：http://nx.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ep.hnjuh.cn

PHP:  array_unique($arr);
来源：http://xx.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://xk.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://dr.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rp.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vg.shxzskj.cn

Ruby: arr.uniq
来源：http://mu.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://yj.wgjwhj.cn

[D16] 求和与平均值
来源：http://ch.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hi.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ru.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ov.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ld.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ji.hahajie.cn

Go:   // 手写循环累加
来源：http://gi.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://et.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://mv.yuexingan06.cn

[D17] 最大值与最小值
来源：http://za.asd995.cn

Py:   max(arr);  min(arr)
来源：http://ur.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://th.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lw.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://gz.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ky.huixinmuqiang.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://un.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://be.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://sn.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://ln.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mg.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://xa.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rf.hnjuh.cn

TS:   nested.flat();
来源：http://ei.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rn.gzmigu.cn

Go:   // 手写双层循环
来源：http://so.chemitech.net.cn

Ruby: nested.flatten
来源：http://hm.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gj.colortex.cn

[D19] 按字段分组
来源：http://sz.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://px.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pp.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zw.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uc.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bl.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://yw.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zz.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://en.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://wx.szsharing.cn

Py:   Counter(arr)
来源：http://dr.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://rr.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iv.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iy.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nl.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://dn.asd995.cn

Ruby: arr.tally
来源：http://gn.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nt.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://hf.bookmarksfly.cn

Py:   x in arr
来源：http://bp.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://ub.hahajie.cn

JS:   arr.includes(x)
来源：http://et.yuexingan06.cn

TS:   arr.includes(x)
来源：http://kp.asd995.cn

Java: list.contains(x)
来源：http://dn.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://wo.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://wl.shxzskj.cn

C#:   list.Contains(x)
来源：http://vq.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://pr.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://we.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gh.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fw.yuntaijiaju.cn

TS:   [...arr];
来源：http://mg.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://go.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pc.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://pq.colortex.cn

C#:   new List<int>(list);
来源：http://nb.szsharing.cn

[D23] reduce 累积计算
来源：http://mf.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rt.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wo.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mh.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mk.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rc.huixinmuqiang.cn

Go:   // 手写循环
来源：http://ck.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://au.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rm.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://rt.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ic.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wr.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fl.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ms.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nt.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://od.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ql.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ge.colortex.cn

[D25] Set 集合去重与交并差
来源：http://fi.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gl.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wf.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fx.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ac.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nc.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xg.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ye.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zj.nicolike.cn

[D26] 数组转字符串
来源：http://az.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://hw.colortex.cn

PHP:  implode(", ", $arr);
来源：http://gk.szxytkj.cn

JS:   arr.join(", ")
来源：http://re.wgjwhj.cn

TS:   arr.join(", ")
来源：http://ej.panjiajie.cn

Java: String.join(", ", list)
来源：http://up.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://gt.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://mg.huanxung.cn

C#:   string.Join(", ", list)
来源：http://pa.huixiangedu.cn

================================================================================
来源：http://ql.panjiajie.cn

E. 字符串处理
来源：http://tm.yuexingan06.cn

================================================================================
来源：http://qq.bjjhwx.cn

[E01] 拼接字符串
来源：http://jg.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yk.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ff.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tw.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ka.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ft.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ia.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vo.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uq.bjjhwx.cn

[E02] 重复字符串
来源：http://gh.asd995.cn

Py:   "ab" * 3
来源：http://mz.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://wf.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://mz.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://ed.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://cv.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://of.shxzukj.cn

Ruby: "ab" * 3
来源：http://ak.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zj.shxzukj.cn

[E03] 截取子串
来源：http://tj.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yf.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pn.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uh.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://ve.lnxyls.cn

Java: s.substring(1, 4)
来源：http://oh.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ej.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dr.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ue.bjjhwx.cn

[E04] 查找子串位置
来源：http://ql.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://rf.nszjky.cn

PHP:  strpos($s, "x");
来源：http://em.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yx.newstarts.cn

TS:   s.indexOf("x")
来源：http://dj.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://ds.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://nn.shtwfgs.cn

Ruby: s.index("x")
来源：http://ui.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://nd.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tv.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vi.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rc.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gn.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ml.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hw.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://af.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tg.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://af.bookmarksfly.cn

[E06] 替换子串
来源：http://tt.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rb.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://ve.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zm.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://yb.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oq.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tg.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gh.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://hq.shxzskj.cn

[E07] 按分隔符拆分
来源：http://kk.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sh.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cg.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wn.shxzskj.cn

TS:   s.split(",")
来源：http://cc.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ni.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eg.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://qu.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xg.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://wh.huixiangedu.cn

Py:   ",".join(items)
来源：http://qi.nicolike.cn

PHP:  implode(",", $items);
来源：http://ik.huixinmuqiang.cn

JS:   items.join(",")
来源：http://ot.muxihuayi.cn

TS:   items.join(",")
来源：http://ds.521024.cn

Java: String.join(",", items)
来源：http://hm.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://hh.szxytkj.cn

Ruby: items.join(",")
来源：http://kr.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://bd.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://rp.colortex.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lh.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://im.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://tw.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://gj.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://os.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ke.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lu.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bi.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://yu.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://we.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zk.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://jq.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://ec.asd995.cn

Java: String.format("%03d", 7)
来源：http://oh.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fp.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://po.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mm.asd995.cn

[E11] 反转字符串
来源：http://mu.haigaiapp.cn

Py:   s[::-1]
来源：http://pi.chemitech.net.cn

PHP:  strrev($s);
来源：http://oo.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://dk.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://uh.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ms.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kp.wgjwhj.cn

Ruby: s.reverse
来源：http://tn.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yn.szsharing.cn

[E12] 统计某字符出现次数
来源：http://xd.wgjwhj.cn

Py:   s.count("a")
来源：http://zi.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://ab.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://ht.9csxet.cn

TS:   s.split("a").length - 1
来源：http://xy.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dy.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://sm.asd995.cn

Ruby: s.count("a")
来源：http://ik.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://fz.hahajie.cn

[E13] 逐字符遍历
来源：http://ib.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://bq.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://on.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tl.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sk.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nz.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zu.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dm.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oq.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://ph.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://px.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gn.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://us.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wg.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dn.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vn.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cq.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gt.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://ji.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lw.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hk.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pb.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ga.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xg.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://te.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qa.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uz.wgjwhj.cn

[E16] 数字千分位
来源：http://cj.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://rp.shxzukj.cn

PHP:  number_format(1234567);
来源：http://cr.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ci.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tv.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jm.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ww.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hi.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://na.gzmigu.cn

[E17] 首字母大写
来源：http://it.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pb.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xo.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fi.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zs.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zw.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bp.huixiangedu.cn

Ruby: s.capitalize
来源：http://ww.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hy.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://ib.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ee.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mn.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xt.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lu.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jg.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kq.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vv.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vt.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://sy.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://xp.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bu.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://yz.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://wh.bjjhwx.cn

Java: s.lines().toList()
来源：http://lq.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://gj.yuntaijiaju.cn

Ruby: s.lines
来源：http://gu.hahajie.cn

C#:   s.Split('\n')
来源：http://io.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ur.haigaiapp.cn

Py:   if not s:
来源：http://ce.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hc.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ve.bjjhwx.cn

TS:   if (s === "") {}
来源：http://ut.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://nk.jctech888.com.cn

Go:   if s == "" {}
来源：http://al.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://sn.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ex.asd995.cn

[E21] 超长截断加省略号
来源：http://rk.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dg.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ic.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bn.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ej.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ly.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://fp.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vv.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dy.gzmigu.cn


<!-- 参考信息 -->