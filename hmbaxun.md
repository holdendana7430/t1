代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://ro.huixiangedu.cn

Go:   // 手写循环
来源：http://dm.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vd.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jj.shtwfgs.cn

[D15] 去重
来源：http://jr.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fe.9csxet.cn

PHP:  array_unique($arr);
来源：http://dm.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://aq.nszjky.cn

TS:   [...new Set(arr)]
来源：http://lq.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sl.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oh.nszjky.cn

Ruby: arr.uniq
来源：http://ek.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://lr.hahajie.cn

[D16] 求和与平均值
来源：http://nm.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nk.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xx.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gy.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gd.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ep.colortex.cn

Go:   // 手写循环累加
来源：http://nn.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fm.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://pk.gzmigu.cn

[D17] 最大值与最小值
来源：http://qm.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ul.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://xa.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qa.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://pd.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lz.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fy.colortex.cn

Ruby: arr.max;  arr.min
来源：http://ch.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://gb.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://ta.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kr.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://rb.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tn.bookmarksfly.cn

TS:   nested.flat();
来源：http://nv.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kb.haigaiapp.cn

Go:   // 手写双层循环
来源：http://em.521024.cn

Ruby: nested.flatten
来源：http://hx.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eb.muxihuayi.cn

[D19] 按字段分组
来源：http://ff.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ov.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cf.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gj.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xp.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jp.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://md.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oy.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pz.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://xj.yuexingan06.cn

Py:   Counter(arr)
来源：http://gs.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://yj.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://du.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lt.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oi.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://uw.521024.cn

Ruby: arr.tally
来源：http://zo.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tg.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://cy.shxzskj.cn

Py:   x in arr
来源：http://ks.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://au.shxzskj.cn

JS:   arr.includes(x)
来源：http://kt.asd995.cn

TS:   arr.includes(x)
来源：http://qw.szxytkj.cn

Java: list.contains(x)
来源：http://rg.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://ov.asd995.cn

Ruby: arr.include?(x)
来源：http://vo.panjiajie.cn

C#:   list.Contains(x)
来源：http://qz.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://ft.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pm.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wy.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ph.nicolike.cn

TS:   [...arr];
来源：http://ns.9csxet.cn

Java: new ArrayList<>(list);
来源：http://bj.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ky.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://cr.yuexingan06.cn

C#:   new List<int>(list);
来源：http://yh.haigaiapp.cn

[D23] reduce 累积计算
来源：http://um.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jz.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ad.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hn.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fc.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hl.jctech888.com.cn

Go:   // 手写循环
来源：http://nn.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wa.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tq.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://qd.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pv.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cp.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gv.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nq.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pc.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vc.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ju.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fz.9csxet.cn

[D25] Set 集合去重与交并差
来源：http://hm.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hg.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tx.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dz.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hy.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uj.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bc.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sg.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mn.panjiajie.cn

[D26] 数组转字符串
来源：http://bo.nszjky.cn

Py:   ", ".join(map(str, arr))
来源：http://ty.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://yt.shxzukj.cn

JS:   arr.join(", ")
来源：http://hu.panjiajie.cn

TS:   arr.join(", ")
来源：http://st.gzmigu.cn

Java: String.join(", ", list)
来源：http://jj.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://fq.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://px.colortex.cn

C#:   string.Join(", ", list)
来源：http://gk.shxzukj.cn

================================================================================
来源：http://py.shtwfgs.cn

E. 字符串处理
来源：http://hd.shxzukj.cn

================================================================================
来源：http://wl.yuexingan06.cn

[E01] 拼接字符串
来源：http://hf.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oe.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xz.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kt.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ks.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ak.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dl.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wu.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sb.shtwfgs.cn

[E02] 重复字符串
来源：http://bm.lnxyls.cn

Py:   "ab" * 3
来源：http://ee.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://kt.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://yw.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://lp.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://lh.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://nb.gzmigu.cn

Ruby: "ab" * 3
来源：http://eh.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nc.newstarts.cn

[E03] 截取子串
来源：http://cr.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jk.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ti.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yh.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://jf.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://at.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zi.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jz.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://qo.panjiajie.cn

[E04] 查找子串位置
来源：http://lz.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://to.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://lz.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rt.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://uj.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://tu.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://uj.jctech888.com.cn

Ruby: s.index("x")
来源：http://hz.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://dk.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nm.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oe.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cg.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cn.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mo.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sm.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sp.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ny.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eb.jianghongdianzi.cn

[E06] 替换子串
来源：http://lr.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kf.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://ui.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wm.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://sy.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kk.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aa.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wo.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://pf.nicolike.cn

[E07] 按分隔符拆分
来源：http://io.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gv.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dz.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ye.newstarts.cn

TS:   s.split(",")
来源：http://xa.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gy.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ur.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://xm.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gr.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://ee.muxihuayi.cn

Py:   ",".join(items)
来源：http://kt.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://xc.szsharing.cn

JS:   items.join(",")
来源：http://yr.gzmigu.cn

TS:   items.join(",")
来源：http://hr.szxytkj.cn

Java: String.join(",", items)
来源：http://lf.521024.cn

Go:   strings.Join(items, ",")
来源：http://gn.huanxung.cn

Ruby: items.join(",")
来源：http://ro.shxzskj.cn

C#:   string.Join(",", items)
来源：http://ug.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://bq.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jv.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zr.shxzukj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ez.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://vq.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://oo.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sb.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ea.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ct.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://di.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ds.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uf.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://en.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://mr.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ov.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ha.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://un.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cw.muxihuayi.cn

[E11] 反转字符串
来源：http://dx.huixiangedu.cn

Py:   s[::-1]
来源：http://km.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://qy.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://qf.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://fg.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vn.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hm.yuntaijiaju.cn

Ruby: s.reverse
来源：http://ly.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vt.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://pc.szsharing.cn

Py:   s.count("a")
来源：http://gc.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://cx.szsharing.cn

JS:   s.split("a").length - 1
来源：http://ue.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://gb.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ac.521024.cn

Go:   strings.Count(s, "a")
来源：http://zy.haigaiapp.cn

Ruby: s.count("a")
来源：http://fv.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://an.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://an.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://om.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wy.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://np.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ja.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kh.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rl.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xc.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ir.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://mo.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sg.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rl.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ae.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hl.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tc.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qy.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vo.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ly.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://vy.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xh.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cx.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nc.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tl.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pd.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bs.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://on.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ed.lnxyls.cn

[E16] 数字千分位
来源：http://ja.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://th.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://jl.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vf.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lx.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bi.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bz.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cz.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://fg.gzmigu.cn

[E17] 首字母大写
来源：http://ct.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mn.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sn.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ue.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ld.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fm.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ob.bookmarksfly.cn

Ruby: s.capitalize
来源：http://ue.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qr.9csxet.cn

[E18] 模板占位符替换
来源：http://zw.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zx.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gw.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fz.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ky.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uw.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ll.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bl.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mk.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://go.chemitech.net.cn

Py:   s.splitlines()
来源：http://hl.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ju.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://np.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://ag.haigaiapp.cn

Java: s.lines().toList()
来源：http://au.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://tg.lnxyls.cn

Ruby: s.lines
来源：http://vb.shtwfgs.cn

C#:   s.Split('\n')
来源：http://st.nszjky.cn

[E20] 判断字符串是否为空
来源：http://tk.bjjhwx.cn

Py:   if not s:
来源：http://uo.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qs.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dt.shxzskj.cn

TS:   if (s === "") {}
来源：http://mb.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://cm.bookmarksfly.cn

Go:   if s == "" {}
来源：http://ui.lnxyls.cn

Ruby: if s.empty?
来源：http://nq.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oe.521024.cn

[E21] 超长截断加省略号
来源：http://sl.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kd.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rp.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kv.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://je.hahajie.cn


<!-- 参考信息 -->