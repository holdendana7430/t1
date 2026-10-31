代发 wailian999

[D15] 去重
来源：http://hn.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sl.nszjky.cn

PHP:  array_unique($arr);
来源：http://lx.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://hs.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://aq.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sb.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vd.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://os.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://xt.szxytkj.cn

[D16] 求和与平均值
来源：http://jo.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ru.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cr.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gm.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gz.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eh.bjjhwx.cn

Go:   // 手写循环累加
来源：http://jm.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wx.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://dt.yuexingan06.cn

[D17] 最大值与最小值
来源：http://bw.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://ue.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://uj.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rp.nicolike.cn

TS:   Math.max(...arr);
来源：http://fe.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vr.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yr.asd995.cn

Ruby: arr.max;  arr.min
来源：http://qe.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://wp.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://bf.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lc.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://mu.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hq.wgjwhj.cn

TS:   nested.flat();
来源：http://nz.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tl.asd995.cn

Go:   // 手写双层循环
来源：http://cw.panjiajie.cn

Ruby: nested.flatten
来源：http://fm.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wf.huanxung.cn

[D19] 按字段分组
来源：http://xg.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yi.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cv.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kb.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ot.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uc.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://jd.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sg.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tl.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://sc.lnxyls.cn

Py:   Counter(arr)
来源：http://fb.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://rl.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qi.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sr.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ou.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://da.jctech888.com.cn

Ruby: arr.tally
来源：http://hs.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ce.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://ca.shxzskj.cn

Py:   x in arr
来源：http://lt.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://ec.shxzskj.cn

JS:   arr.includes(x)
来源：http://rq.newstarts.cn

TS:   arr.includes(x)
来源：http://ou.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ey.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://wi.asd995.cn

Ruby: arr.include?(x)
来源：http://qq.haigaiapp.cn

C#:   list.Contains(x)
来源：http://ku.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://qv.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://up.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xr.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zd.521024.cn

TS:   [...arr];
来源：http://st.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://ve.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ty.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://ou.chemitech.net.cn

C#:   new List<int>(list);
来源：http://ro.nicolike.cn

[D23] reduce 累积计算
来源：http://kg.huanxung.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zz.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dt.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tl.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fh.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wk.gzmigu.cn

Go:   // 手写循环
来源：http://dt.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ml.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ug.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://sl.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vr.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vj.colortex.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sp.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mv.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yy.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tb.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yq.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ap.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://eu.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vx.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zu.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ah.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ia.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qf.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hj.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sm.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xo.szsharing.cn

[D26] 数组转字符串
来源：http://pm.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://ih.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://cc.asd995.cn

JS:   arr.join(", ")
来源：http://zd.9csxet.cn

TS:   arr.join(", ")
来源：http://bn.nszjky.cn

Java: String.join(", ", list)
来源：http://ns.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://lq.9csxet.cn

Ruby: arr.join(", ")
来源：http://sr.szsharing.cn

C#:   string.Join(", ", list)
来源：http://qh.yuntaijiaju.cn

================================================================================
来源：http://qq.lnxyls.cn

E. 字符串处理
来源：http://uq.hahajie.cn

================================================================================
来源：http://we.9csxet.cn

[E01] 拼接字符串
来源：http://nk.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ik.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yr.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ie.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zr.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lv.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ya.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xb.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gd.shxzskj.cn

[E02] 重复字符串
来源：http://um.jctech888.com.cn

Py:   "ab" * 3
来源：http://qy.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://mr.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://oc.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://cm.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://ni.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://os.521024.cn

Ruby: "ab" * 3
来源：http://ci.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fg.gzmigu.cn

[E03] 截取子串
来源：http://uc.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nz.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lp.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vo.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://dr.lnxyls.cn

Java: s.substring(1, 4)
来源：http://qz.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xp.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qf.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://ek.newstarts.cn

[E04] 查找子串位置
来源：http://xf.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://yx.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://lt.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zh.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://qg.huanxung.cn

Java: s.indexOf("x")
来源：http://ju.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://zi.nszjky.cn

Ruby: s.index("x")
来源：http://gj.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://dh.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iw.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lv.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dp.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mi.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dm.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vz.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cj.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://po.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dp.9csxet.cn

[E06] 替换子串
来源：http://rw.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://au.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://mj.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ix.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://ge.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ih.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zc.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://it.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://co.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://fp.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hc.nicolike.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wd.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sn.yuexingan06.cn

TS:   s.split(",")
来源：http://ky.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ll.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mi.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://dd.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ux.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://jl.colortex.cn

Py:   ",".join(items)
来源：http://af.huanxung.cn

PHP:  implode(",", $items);
来源：http://uy.huanxung.cn

JS:   items.join(",")
来源：http://vy.hahajie.cn

TS:   items.join(",")
来源：http://jf.asd995.cn

Java: String.join(",", items)
来源：http://gl.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://yt.panjiajie.cn

Ruby: items.join(",")
来源：http://xd.hnjuh.cn

C#:   string.Join(",", items)
来源：http://rc.szxytkj.cn

[E09] 去除所有空白字符
来源：http://fi.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wi.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kf.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://kq.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://rm.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://yp.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bs.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://em.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qf.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://fm.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://im.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bj.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://oi.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://nr.colortex.cn

Java: String.format("%03d", 7)
来源：http://eh.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rz.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yg.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wt.haigaiapp.cn

[E11] 反转字符串
来源：http://dt.shtwfgs.cn

Py:   s[::-1]
来源：http://bd.colortex.cn

PHP:  strrev($s);
来源：http://cd.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://ib.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://cj.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ss.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zk.hahajie.cn

Ruby: s.reverse
来源：http://ex.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://si.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://ag.wgjwhj.cn

Py:   s.count("a")
来源：http://eb.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://zx.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://wg.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://ug.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qk.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://bd.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://wy.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://km.hnjuh.cn

[E13] 逐字符遍历
来源：http://no.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://ra.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cv.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hv.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gg.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hi.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sg.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fk.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jq.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://hp.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sz.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cw.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gj.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yt.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://im.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tr.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bj.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xq.521024.cn

[E15] HTML 转义 / 反转义
来源：http://uo.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hk.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jb.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kf.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rt.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yt.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ah.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://en.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mt.lnxyls.cn

[E16] 数字千分位
来源：http://fa.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://nn.szsharing.cn

PHP:  number_format(1234567);
来源：http://pu.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://he.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mo.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://or.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uf.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fg.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://ii.szxytkj.cn

[E17] 首字母大写
来源：http://mo.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dy.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ym.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sa.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pa.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://je.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://se.lnxyls.cn

Ruby: s.capitalize
来源：http://sz.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mq.huixiangedu.cn

[E18] 模板占位符替换
来源：http://bc.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vc.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sj.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://or.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hb.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://of.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://da.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rb.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pw.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://fi.nszjky.cn

Py:   s.splitlines()
来源：http://xo.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lz.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://bn.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ur.lnxyls.cn

Java: s.lines().toList()
来源：http://hh.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://rs.huixinmuqiang.cn

Ruby: s.lines
来源：http://ek.hahajie.cn

C#:   s.Split('\n')
来源：http://ny.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://bw.asd995.cn

Py:   if not s:
来源：http://up.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mt.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jv.szsharing.cn

TS:   if (s === "") {}
来源：http://zo.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://wf.521024.cn

Go:   if s == "" {}
来源：http://co.jctech888.com.cn

Ruby: if s.empty?
来源：http://qt.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ui.szxytkj.cn

[E21] 超长截断加省略号
来源：http://ya.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zi.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rw.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mg.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fs.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sz.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://st.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zk.huixinmuqiang.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iz.newstarts.cn


<!-- 参考信息 -->