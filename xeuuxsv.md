代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ks.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qm.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://oa.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://zy.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kf.szxytkj.cn

Go:   // 手写循环
来源：http://pv.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pq.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sw.muxihuayi.cn

[D15] 去重
来源：http://zk.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xc.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://cr.newstarts.cn

JS:   [...new Set(arr)]
来源：http://lg.newstarts.cn

TS:   [...new Set(arr)]
来源：http://tb.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ak.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lu.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://ld.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://fg.szxytkj.cn

[D16] 求和与平均值
来源：http://tr.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bb.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ei.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ml.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rr.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://db.jctech888.com.cn

Go:   // 手写循环累加
来源：http://ga.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dw.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://mg.colortex.cn

[D17] 最大值与最小值
来源：http://zm.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://fc.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://js.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://po.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://es.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hb.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rx.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://hx.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://wh.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://ip.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rq.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://ja.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kn.jianghongdianzi.cn

TS:   nested.flat();
来源：http://ey.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bs.szxytkj.cn

Go:   // 手写双层循环
来源：http://gf.shxzskj.cn

Ruby: nested.flatten
来源：http://il.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kt.jctech888.com.cn

[D19] 按字段分组
来源：http://rd.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://av.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qo.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nv.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fw.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jd.asd995.cn

Go:   // 手写 map[string][]T
来源：http://xo.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xt.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ep.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://xt.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://jk.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://at.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://td.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://np.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jm.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://hi.jctech888.com.cn

Ruby: arr.tally
来源：http://bh.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bu.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://az.huixiangedu.cn

Py:   x in arr
来源：http://tc.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://cn.bjjhwx.cn

JS:   arr.includes(x)
来源：http://nf.bjjhwx.cn

TS:   arr.includes(x)
来源：http://iy.huixinmuqiang.cn

Java: list.contains(x)
来源：http://cl.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://yd.lnxyls.cn

Ruby: arr.include?(x)
来源：http://dj.szxytkj.cn

C#:   list.Contains(x)
来源：http://wm.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://cb.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vy.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yo.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mr.hahajie.cn

TS:   [...arr];
来源：http://wa.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://kk.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dy.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://kr.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://lb.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://os.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hu.nicolike.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vc.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fg.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cq.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jy.bookmarksfly.cn

Go:   // 手写循环
来源：http://bd.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ym.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kl.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://um.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pw.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ko.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ac.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oc.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://us.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kd.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xu.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cj.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://to.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ln.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fq.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cx.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://be.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ax.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ro.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ay.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ka.gzmigu.cn

[D26] 数组转字符串
来源：http://tv.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://ps.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://sc.nicolike.cn

JS:   arr.join(", ")
来源：http://bl.jctech888.com.cn

TS:   arr.join(", ")
来源：http://ee.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://rf.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://wp.huanxung.cn

Ruby: arr.join(", ")
来源：http://yh.szsharing.cn

C#:   string.Join(", ", list)
来源：http://wq.muxihuayi.cn

================================================================================
来源：http://tq.9csxet.cn

E. 字符串处理
来源：http://sr.jctech888.com.cn

================================================================================
来源：http://ue.521024.cn

[E01] 拼接字符串
来源：http://lq.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hd.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hq.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xj.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ma.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ki.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cw.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xk.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nv.521024.cn

[E02] 重复字符串
来源：http://gw.muxihuayi.cn

Py:   "ab" * 3
来源：http://jw.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://dl.hahajie.cn

JS:   "ab".repeat(3)
来源：http://bw.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://ev.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://do.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://ae.newstarts.cn

Ruby: "ab" * 3
来源：http://xa.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vd.shtwfgs.cn

[E03] 截取子串
来源：http://nc.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://or.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cd.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ew.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://zt.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://pf.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wk.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hp.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ej.nicolike.cn

[E04] 查找子串位置
来源：http://ka.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://rz.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://cm.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ow.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://bm.lnxyls.cn

Java: s.indexOf("x")
来源：http://do.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://oi.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://me.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://ub.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://as.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hh.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ts.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mv.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vz.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ul.hahajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xr.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pd.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://up.wgjwhj.cn

[E06] 替换子串
来源：http://xg.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eo.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://bs.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tu.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://hm.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nd.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://us.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://or.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://nn.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://qs.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vl.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sd.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bd.colortex.cn

TS:   s.split(",")
来源：http://vh.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uz.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fw.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://tp.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kr.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://gt.nszjky.cn

Py:   ",".join(items)
来源：http://mj.newstarts.cn

PHP:  implode(",", $items);
来源：http://oo.huixiangedu.cn

JS:   items.join(",")
来源：http://ii.panjiajie.cn

TS:   items.join(",")
来源：http://zg.panjiajie.cn

Java: String.join(",", items)
来源：http://hp.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://df.yuexingan06.cn

Ruby: items.join(",")
来源：http://xg.huanxung.cn

C#:   string.Join(",", items)
来源：http://hi.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://jh.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pb.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gy.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://bb.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://qb.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://rf.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gr.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://af.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zb.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://dv.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ci.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cx.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://pl.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://qw.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://qe.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wf.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iq.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ie.newstarts.cn

[E11] 反转字符串
来源：http://qf.nszjky.cn

Py:   s[::-1]
来源：http://ix.haigaiapp.cn

PHP:  strrev($s);
来源：http://qu.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://af.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://ld.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yy.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://um.gzmigu.cn

Ruby: s.reverse
来源：http://vb.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sa.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://ok.szxytkj.cn

Py:   s.count("a")
来源：http://if.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://gw.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://ct.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://kf.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cz.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://hj.521024.cn

Ruby: s.count("a")
来源：http://fv.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://yn.nicolike.cn

[E13] 逐字符遍历
来源：http://il.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://cx.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kp.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jy.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uh.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ww.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kn.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rv.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cr.nszjky.cn

[E14] URL 编码与 Base64
来源：http://ga.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rt.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gu.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pk.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eb.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fz.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pa.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cr.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vu.521024.cn

[E15] HTML 转义 / 反转义
来源：http://cp.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://no.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ke.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cy.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://io.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ty.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yu.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://px.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xj.szsharing.cn

[E16] 数字千分位
来源：http://ry.asd995.cn

Py:   f"{1234567:,}"
来源：http://ao.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://tw.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uj.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wk.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tx.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yf.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bx.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://fe.shxzukj.cn

[E17] 首字母大写
来源：http://jn.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ds.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://da.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uj.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rt.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ns.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zc.haigaiapp.cn

Ruby: s.capitalize
来源：http://zs.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eo.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://op.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ae.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ft.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cu.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ke.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ew.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dp.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sm.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rh.nszjky.cn

[E19] 多行文本按行拆分
来源：http://cv.lnxyls.cn

Py:   s.splitlines()
来源：http://ra.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://um.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://pg.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://pn.szsharing.cn

Java: s.lines().toList()
来源：http://pe.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://ey.asd995.cn

Ruby: s.lines
来源：http://gf.9csxet.cn

C#:   s.Split('\n')
来源：http://ft.hahajie.cn

[E20] 判断字符串是否为空
来源：http://ny.shtwfgs.cn

Py:   if not s:
来源：http://js.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://td.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lu.chemitech.net.cn

TS:   if (s === "") {}
来源：http://qr.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://yg.hahajie.cn

Go:   if s == "" {}
来源：http://of.nszjky.cn

Ruby: if s.empty?
来源：http://tb.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zh.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://th.shtwfgs.cn


<!-- 参考信息 -->