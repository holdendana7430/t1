代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sf.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://mn.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tu.newstarts.cn

TS:   nested.flat();
来源：http://pt.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kk.nicolike.cn

Go:   // 手写双层循环
来源：http://vz.nicolike.cn

Ruby: nested.flatten
来源：http://dq.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://me.szsharing.cn

[D19] 按字段分组
来源：http://qy.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cd.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cn.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://od.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zz.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cd.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://dn.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mz.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ql.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://qw.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://ay.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://xz.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ix.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rv.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://di.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://zs.gzmigu.cn

Ruby: arr.tally
来源：http://dq.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hh.huanxung.cn

[D21] 判断是否包含某元素
来源：http://jj.lnxyls.cn

Py:   x in arr
来源：http://sx.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://nj.shtwfgs.cn

JS:   arr.includes(x)
来源：http://dz.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://vp.bookmarksfly.cn

Java: list.contains(x)
来源：http://so.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://lo.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://al.newstarts.cn

C#:   list.Contains(x)
来源：http://si.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://el.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zg.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zk.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ak.newstarts.cn

TS:   [...arr];
来源：http://dh.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://wj.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zm.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://on.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://oc.shxzskj.cn

[D23] reduce 累积计算
来源：http://yt.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pd.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ug.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://la.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gh.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nd.huanxung.cn

Go:   // 手写循环
来源：http://lb.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wf.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xs.521024.cn

[D24] 字典 / Map 基本操作
来源：http://lg.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://va.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pu.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ms.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zb.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qs.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eo.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ao.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://id.colortex.cn

[D25] Set 集合去重与交并差
来源：http://ki.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://is.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xl.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sm.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vd.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nj.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ui.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sf.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ac.wgjwhj.cn

[D26] 数组转字符串
来源：http://oq.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://uk.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://eq.shxzukj.cn

JS:   arr.join(", ")
来源：http://lg.9csxet.cn

TS:   arr.join(", ")
来源：http://ia.shxzukj.cn

Java: String.join(", ", list)
来源：http://ym.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://gs.asd995.cn

Ruby: arr.join(", ")
来源：http://tw.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://ye.asd995.cn

================================================================================
来源：http://wa.shxzskj.cn

E. 字符串处理
来源：http://lj.jianghongdianzi.cn

================================================================================
来源：http://kw.hahajie.cn

[E01] 拼接字符串
来源：http://ha.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uj.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pe.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vi.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hn.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bv.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uh.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kl.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ut.lnxyls.cn

[E02] 重复字符串
来源：http://tb.gzmigu.cn

Py:   "ab" * 3
来源：http://qs.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://xy.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://me.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://jv.hnjuh.cn

Java: "ab".repeat(3)
来源：http://dc.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://qn.panjiajie.cn

Ruby: "ab" * 3
来源：http://oz.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ha.szxytkj.cn

[E03] 截取子串
来源：http://bj.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ix.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vu.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lo.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://kd.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://io.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tp.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ng.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://hn.szsharing.cn

[E04] 查找子串位置
来源：http://qf.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://xa.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://yh.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fq.panjiajie.cn

TS:   s.indexOf("x")
来源：http://ku.szsharing.cn

Java: s.indexOf("x")
来源：http://kq.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://xo.huixiangedu.cn

Ruby: s.index("x")
来源：http://vy.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://et.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://od.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ud.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://is.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://or.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hb.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ih.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jc.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wq.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ky.chemitech.net.cn

[E06] 替换子串
来源：http://uw.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://di.huanxung.cn

PHP:  str_replace("a", "b", $s);
来源：http://av.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://th.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://th.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lg.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xi.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mg.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://to.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://nw.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oa.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://me.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hq.wgjwhj.cn

TS:   s.split(",")
来源：http://oy.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vv.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gp.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://vp.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ly.colortex.cn

[E08] 数组按分隔符合并
来源：http://nm.hahajie.cn

Py:   ",".join(items)
来源：http://mc.lnxyls.cn

PHP:  implode(",", $items);
来源：http://ba.asd995.cn

JS:   items.join(",")
来源：http://ro.hnjuh.cn

TS:   items.join(",")
来源：http://fg.panjiajie.cn

Java: String.join(",", items)
来源：http://jw.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://gj.bjjhwx.cn

Ruby: items.join(",")
来源：http://hb.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://hk.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://zm.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ic.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tw.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://kn.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://fu.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://jx.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qr.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ei.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wl.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://gc.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ty.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kq.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://or.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://ge.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://an.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ax.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tl.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ca.yuexingan06.cn

[E11] 反转字符串
来源：http://uj.nicolike.cn

Py:   s[::-1]
来源：http://bd.lnxyls.cn

PHP:  strrev($s);
来源：http://ij.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://pb.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://ma.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hp.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qv.521024.cn

Ruby: s.reverse
来源：http://yd.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ex.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://tk.szsharing.cn

Py:   s.count("a")
来源：http://if.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://os.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://uz.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://qu.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xz.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://bs.gzmigu.cn

Ruby: s.count("a")
来源：http://rk.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://bf.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://yv.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://wj.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cj.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hs.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tt.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://in.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ac.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pk.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iq.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://gx.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cz.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qm.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yu.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kl.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ka.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sv.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kk.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pq.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://ju.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zy.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sv.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://er.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ck.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kl.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kz.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://to.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gq.panjiajie.cn

[E16] 数字千分位
来源：http://ga.hahajie.cn

Py:   f"{1234567:,}"
来源：http://hj.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://ad.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jq.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nj.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qe.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hk.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://df.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://pu.9csxet.cn

[E17] 首字母大写
来源：http://lv.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gj.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ny.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ux.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pt.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rb.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cc.shxzskj.cn

Ruby: s.capitalize
来源：http://vt.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ju.colortex.cn

[E18] 模板占位符替换
来源：http://wr.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bn.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qf.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zx.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qq.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dr.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://en.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fb.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tf.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://ps.asd995.cn

Py:   s.splitlines()
来源：http://ga.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dq.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://wx.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://qt.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://fx.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://oh.haigaiapp.cn

Ruby: s.lines
来源：http://wv.muxihuayi.cn

C#:   s.Split('\n')
来源：http://mp.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://io.wgjwhj.cn

Py:   if not s:
来源：http://fx.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ry.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uu.szxytkj.cn

TS:   if (s === "") {}
来源：http://pp.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://ki.muxihuayi.cn

Go:   if s == "" {}
来源：http://cf.yuexingan06.cn

Ruby: if s.empty?
来源：http://ii.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fh.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://fm.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xf.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ov.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bw.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yc.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kr.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://bv.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://au.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ml.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://tv.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yy.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cl.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vx.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kh.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://we.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uk.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://xo.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rm.huanxung.cn

================================================================================
来源：http://qo.shtwfgs.cn

F. 文件与目录
来源：http://ux.huanxung.cn

================================================================================
来源：http://nq.asd995.cn

[F01] 读取整个文件
来源：http://vg.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ke.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://fy.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ww.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://af.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ge.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://co.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://bt.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://dd.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://rz.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hr.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://er.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ig.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cq.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ea.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://af.shxzukj.cn


<!-- 参考信息 -->