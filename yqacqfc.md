代发 wailian999

TS:   [...new Set(arr)]
来源：http://dy.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ec.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vw.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://xb.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://sy.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://vo.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vm.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pf.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qy.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bz.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sh.lnxyls.cn

Go:   // 手写循环累加
来源：http://sz.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://od.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://gw.bjjhwx.cn

[D17] 最大值与最小值
来源：http://du.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ol.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://us.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uj.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://sg.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zn.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yq.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://kp.asd995.cn

C#:   list.Max();  list.Min()
来源：http://po.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://nr.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ho.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://dr.shtwfgs.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rr.szsharing.cn

TS:   nested.flat();
来源：http://mr.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lf.muxihuayi.cn

Go:   // 手写双层循环
来源：http://me.hnjuh.cn

Ruby: nested.flatten
来源：http://ev.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mo.nszjky.cn

[D19] 按字段分组
来源：http://hk.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jf.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vj.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mh.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gw.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://up.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://py.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cy.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dt.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://ay.jctech888.com.cn

Py:   Counter(arr)
来源：http://gw.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://jp.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vs.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gh.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://br.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://bu.shxzukj.cn

Ruby: arr.tally
来源：http://fh.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cj.szsharing.cn

[D21] 判断是否包含某元素
来源：http://xm.panjiajie.cn

Py:   x in arr
来源：http://qw.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://og.asd995.cn

JS:   arr.includes(x)
来源：http://ev.wgjwhj.cn

TS:   arr.includes(x)
来源：http://qw.9csxet.cn

Java: list.contains(x)
来源：http://pj.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://ae.gzmigu.cn

Ruby: arr.include?(x)
来源：http://jc.lnxyls.cn

C#:   list.Contains(x)
来源：http://sz.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://mg.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bg.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fq.panjiajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ex.muxihuayi.cn

TS:   [...arr];
来源：http://xu.9csxet.cn

Java: new ArrayList<>(list);
来源：http://gi.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cj.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://jq.colortex.cn

C#:   new List<int>(list);
来源：http://fp.hahajie.cn

[D23] reduce 累积计算
来源：http://iz.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nr.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yu.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ki.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rs.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sv.bjjhwx.cn

Go:   // 手写循环
来源：http://kd.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jk.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://og.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://so.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://px.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xe.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vc.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ax.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sl.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ot.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gt.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nb.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://po.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vp.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tq.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zv.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zv.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fd.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ro.jctech888.com.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tt.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bj.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://lz.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://nw.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://ji.panjiajie.cn

JS:   arr.join(", ")
来源：http://gm.bookmarksfly.cn

TS:   arr.join(", ")
来源：http://rd.yuexingan06.cn

Java: String.join(", ", list)
来源：http://xo.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://nu.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://ze.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://sn.bookmarksfly.cn

================================================================================
来源：http://cj.bjjhwx.cn

E. 字符串处理
来源：http://uh.9csxet.cn

================================================================================
来源：http://zf.yuexingan06.cn

[E01] 拼接字符串
来源：http://uw.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zy.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nq.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dj.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eg.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://of.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pf.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vd.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xq.bjjhwx.cn

[E02] 重复字符串
来源：http://tp.huanxung.cn

Py:   "ab" * 3
来源：http://fo.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://yp.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://of.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://md.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://eo.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://jc.wgjwhj.cn

Ruby: "ab" * 3
来源：http://ot.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ec.chemitech.net.cn

[E03] 截取子串
来源：http://zf.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://if.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xm.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ic.hahajie.cn

TS:   s.slice(1, 4)
来源：http://ej.huanxung.cn

Java: s.substring(1, 4)
来源：http://db.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wk.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pv.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://vk.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://ci.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://co.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://lw.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pz.9csxet.cn

TS:   s.indexOf("x")
来源：http://hv.huanxung.cn

Java: s.indexOf("x")
来源：http://lg.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://rc.chemitech.net.cn

Ruby: s.index("x")
来源：http://kh.nicolike.cn

C#:   s.IndexOf("x")
来源：http://dd.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zh.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ub.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jd.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xj.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qr.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zb.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gz.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mf.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eu.newstarts.cn

[E06] 替换子串
来源：http://tj.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kr.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://cy.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bo.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://nn.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pd.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fn.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fk.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://hp.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://qq.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ib.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fr.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rn.9csxet.cn

TS:   s.split(",")
来源：http://va.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ft.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pd.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://wm.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jx.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://rw.colortex.cn

Py:   ",".join(items)
来源：http://tw.shxzukj.cn

PHP:  implode(",", $items);
来源：http://si.bjjhwx.cn

JS:   items.join(",")
来源：http://nv.gzmigu.cn

TS:   items.join(",")
来源：http://hh.asd995.cn

Java: String.join(",", items)
来源：http://is.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://af.bjjhwx.cn

Ruby: items.join(",")
来源：http://cd.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://vq.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://jd.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kj.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gv.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://jw.shxzukj.cn

TS:   s.replace(/\s+/g, "")
来源：http://dg.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://pu.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rg.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xz.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rp.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://zy.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qm.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iq.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://xl.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://tz.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://ax.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qs.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tr.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rw.lnxyls.cn

[E11] 反转字符串
来源：http://qe.9csxet.cn

Py:   s[::-1]
来源：http://rj.hnjuh.cn

PHP:  strrev($s);
来源：http://oi.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://aj.521024.cn

TS:   [...s].reverse().join("")
来源：http://dq.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rj.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vx.haigaiapp.cn

Ruby: s.reverse
来源：http://fs.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sf.newstarts.cn

[E12] 统计某字符出现次数
来源：http://nw.newstarts.cn

Py:   s.count("a")
来源：http://mo.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://ix.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://xn.asd995.cn

TS:   s.split("a").length - 1
来源：http://go.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rl.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://zh.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://wz.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://qx.9csxet.cn

[E13] 逐字符遍历
来源：http://ch.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ju.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://re.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yp.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bg.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://va.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zg.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://va.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://be.huanxung.cn

[E14] URL 编码与 Base64
来源：http://ef.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cf.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xz.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dv.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wu.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pt.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pl.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gv.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lt.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://ou.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rb.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ia.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xv.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://to.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://va.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jk.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bf.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://op.newstarts.cn

[E16] 数字千分位
来源：http://dq.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://hk.szxytkj.cn

PHP:  number_format(1234567);
来源：http://gc.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fq.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://en.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tm.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nw.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wa.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://tj.yuexingan06.cn

[E17] 首字母大写
来源：http://zk.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bi.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vf.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hi.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ob.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bw.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wq.shxzskj.cn

Ruby: s.capitalize
来源：http://pq.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hh.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://oi.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xj.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tm.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ux.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mm.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cy.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lp.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ki.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://of.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://dt.gzmigu.cn

Py:   s.splitlines()
来源：http://xl.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nw.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://ms.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://pt.shtwfgs.cn

Java: s.lines().toList()
来源：http://yc.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://ee.521024.cn

Ruby: s.lines
来源：http://kg.nicolike.cn

C#:   s.Split('\n')
来源：http://ez.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://of.huixiangedu.cn

Py:   if not s:
来源：http://af.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mg.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cz.9csxet.cn

TS:   if (s === "") {}
来源：http://bg.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://kw.haigaiapp.cn

Go:   if s == "" {}
来源：http://vd.haigaiapp.cn

Ruby: if s.empty?
来源：http://lv.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://et.nicolike.cn

[E21] 超长截断加省略号
来源：http://vh.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nj.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iu.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oq.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zo.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qy.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://xn.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jd.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fp.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://or.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ke.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lj.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aw.huixiangedu.cn


<!-- 参考信息 -->