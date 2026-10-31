代发 wailian999

[D15] 去重
来源：http://hc.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cv.szxytkj.cn

PHP:  array_unique($arr);
来源：http://wk.colortex.cn

JS:   [...new Set(arr)]
来源：http://px.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://qm.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uz.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://um.lnxyls.cn

Ruby: arr.uniq
来源：http://mh.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://qy.lnxyls.cn

[D16] 求和与平均值
来源：http://du.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dw.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qe.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ar.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bm.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ir.nicolike.cn

Go:   // 手写循环累加
来源：http://ot.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fu.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://au.yuexingan06.cn

[D17] 最大值与最小值
来源：http://cq.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://kh.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://vs.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jx.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://uc.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lk.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://go.521024.cn

Ruby: arr.max;  arr.min
来源：http://wd.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://gs.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://bl.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://az.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://em.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mk.huixiangedu.cn

TS:   nested.flat();
来源：http://pu.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hx.jctech888.com.cn

Go:   // 手写双层循环
来源：http://hv.9csxet.cn

Ruby: nested.flatten
来源：http://ue.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ed.yuexingan06.cn

[D19] 按字段分组
来源：http://vg.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iv.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bn.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ow.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ia.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xm.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://gp.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://co.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://is.gzmigu.cn

[D20] 统计每个元素出现次数
来源：http://ak.asd995.cn

Py:   Counter(arr)
来源：http://zg.521024.cn

PHP:  array_count_values($arr);
来源：http://mx.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bj.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gb.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://of.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://kn.9csxet.cn

Ruby: arr.tally
来源：http://vk.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://co.newstarts.cn

[D21] 判断是否包含某元素
来源：http://ne.newstarts.cn

Py:   x in arr
来源：http://nz.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ue.9csxet.cn

JS:   arr.includes(x)
来源：http://re.lnxyls.cn

TS:   arr.includes(x)
来源：http://ur.bookmarksfly.cn

Java: list.contains(x)
来源：http://fm.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://gu.nicolike.cn

Ruby: arr.include?(x)
来源：http://vq.hnjuh.cn

C#:   list.Contains(x)
来源：http://sy.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://hh.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gb.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pu.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vz.colortex.cn

TS:   [...arr];
来源：http://ts.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://jv.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://co.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://kj.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://mz.521024.cn

[D23] reduce 累积计算
来源：http://rp.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xn.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wa.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qp.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qe.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xg.bookmarksfly.cn

Go:   // 手写循环
来源：http://rc.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ny.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jl.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://ub.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sz.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ix.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pw.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://os.huanxung.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kv.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zc.huixiangedu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jt.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dt.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://fy.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lx.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xo.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pa.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bv.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kb.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wl.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ir.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bo.shtwfgs.cn

[D26] 数组转字符串
来源：http://fx.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://pz.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://uy.wgjwhj.cn

JS:   arr.join(", ")
来源：http://xi.szxytkj.cn

TS:   arr.join(", ")
来源：http://ne.hahajie.cn

Java: String.join(", ", list)
来源：http://ty.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://ri.9csxet.cn

Ruby: arr.join(", ")
来源：http://iy.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://xr.colortex.cn

================================================================================
来源：http://gu.colortex.cn

E. 字符串处理
来源：http://du.bookmarksfly.cn

================================================================================
来源：http://ec.jctech888.com.cn

[E01] 拼接字符串
来源：http://ie.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pv.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fm.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dl.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://za.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ez.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fx.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fy.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dh.hnjuh.cn

[E02] 重复字符串
来源：http://oj.newstarts.cn

Py:   "ab" * 3
来源：http://xb.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://lt.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://am.asd995.cn

TS:   "ab".repeat(3)
来源：http://bs.huanxung.cn

Java: "ab".repeat(3)
来源：http://jm.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://th.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://ig.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mw.wgjwhj.cn

[E03] 截取子串
来源：http://hf.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://re.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pe.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zz.colortex.cn

TS:   s.slice(1, 4)
来源：http://zc.nicolike.cn

Java: s.substring(1, 4)
来源：http://hx.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xd.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vx.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://pu.shxzukj.cn

[E04] 查找子串位置
来源：http://go.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://ph.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://hg.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qw.shxzukj.cn

TS:   s.indexOf("x")
来源：http://uc.nszjky.cn

Java: s.indexOf("x")
来源：http://ls.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://dr.nicolike.cn

Ruby: s.index("x")
来源：http://ax.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://id.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kp.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://df.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nx.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vi.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bw.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yg.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rg.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jw.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lj.lnxyls.cn

[E06] 替换子串
来源：http://tj.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://by.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://ps.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rx.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://zm.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jw.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ai.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qh.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://vh.shxzskj.cn

[E07] 按分隔符拆分
来源：http://kl.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ya.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mz.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jp.panjiajie.cn

TS:   s.split(",")
来源：http://ls.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uw.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qa.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://yj.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iu.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://zk.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://oq.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://dn.hnjuh.cn

JS:   items.join(",")
来源：http://uz.jianghongdianzi.cn

TS:   items.join(",")
来源：http://yl.jctech888.com.cn

Java: String.join(",", items)
来源：http://om.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://bq.lnxyls.cn

Ruby: items.join(",")
来源：http://qw.shxzukj.cn

C#:   string.Join(",", items)
来源：http://jl.huanxung.cn

[E09] 去除所有空白字符
来源：http://cv.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://st.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fe.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://dp.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://ca.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://mq.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qn.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vg.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wt.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://wn.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kv.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fd.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://js.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://kp.9csxet.cn

Java: String.format("%03d", 7)
来源：http://cg.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://up.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gn.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dh.chemitech.net.cn

[E11] 反转字符串
来源：http://vm.haigaiapp.cn

Py:   s[::-1]
来源：http://tx.haigaiapp.cn

PHP:  strrev($s);
来源：http://qu.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://vp.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://hj.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oc.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dq.wgjwhj.cn

Ruby: s.reverse
来源：http://mo.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kb.szsharing.cn

[E12] 统计某字符出现次数
来源：http://ja.szxytkj.cn

Py:   s.count("a")
来源：http://gp.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://wf.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://iq.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://ue.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vj.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://ig.521024.cn

Ruby: s.count("a")
来源：http://pf.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://jx.haigaiapp.cn

[E13] 逐字符遍历
来源：http://zw.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://pb.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bt.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sq.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fm.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nc.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://te.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kz.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gd.9csxet.cn

[E14] URL 编码与 Base64
来源：http://en.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fa.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jh.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lo.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jb.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ky.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wd.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mc.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xy.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://sf.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://of.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xq.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ko.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ns.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wo.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zo.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qy.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xl.nszjky.cn

[E16] 数字千分位
来源：http://if.asd995.cn

Py:   f"{1234567:,}"
来源：http://vc.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://gy.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://am.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xl.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cb.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tu.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ve.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://wg.hahajie.cn

[E17] 首字母大写
来源：http://og.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ll.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pw.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vk.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ul.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jn.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zt.colortex.cn

Ruby: s.capitalize
来源：http://wf.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cw.colortex.cn

[E18] 模板占位符替换
来源：http://tf.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://po.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tk.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ke.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gp.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://of.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ct.szxytkj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wx.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ej.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://ub.panjiajie.cn

Py:   s.splitlines()
来源：http://hu.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zj.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://bv.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://an.bjjhwx.cn

Java: s.lines().toList()
来源：http://jv.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://gz.huixiangedu.cn

Ruby: s.lines
来源：http://zl.nszjky.cn

C#:   s.Split('\n')
来源：http://ja.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://rh.9csxet.cn

Py:   if not s:
来源：http://kx.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uo.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rt.bjjhwx.cn

TS:   if (s === "") {}
来源：http://xu.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://lr.bookmarksfly.cn

Go:   if s == "" {}
来源：http://xa.huanxung.cn

Ruby: if s.empty?
来源：http://vd.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ag.nicolike.cn

[E21] 超长截断加省略号
来源：http://xd.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dx.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ee.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ow.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hg.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fa.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://gq.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zf.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://id.yuexingan06.cn


<!-- 参考信息 -->