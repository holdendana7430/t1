代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://co.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zn.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://es.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://fn.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://us.colortex.cn

Go:   // 手写循环
来源：http://mt.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tf.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zd.nszjky.cn

[D15] 去重
来源：http://dz.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vq.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://ry.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://nc.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://yh.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xx.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gg.newstarts.cn

Ruby: arr.uniq
来源：http://rw.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://kd.haigaiapp.cn

[D16] 求和与平均值
来源：http://ho.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yc.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vp.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ch.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ii.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qz.chemitech.net.cn

Go:   // 手写循环累加
来源：http://qc.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fk.521024.cn

C#:   list.Sum();  list.Average()
来源：http://zl.huanxung.cn

[D17] 最大值与最小值
来源：http://fu.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://xa.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://vz.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dv.szxytkj.cn

TS:   Math.max(...arr);
来源：http://iz.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ur.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dx.asd995.cn

Ruby: arr.max;  arr.min
来源：http://za.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://gz.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://bd.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eg.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://qk.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lq.shxzukj.cn

TS:   nested.flat();
来源：http://wz.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kx.colortex.cn

Go:   // 手写双层循环
来源：http://hi.wgjwhj.cn

Ruby: nested.flatten
来源：http://qz.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bj.colortex.cn

[D19] 按字段分组
来源：http://sh.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gm.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://me.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eh.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cd.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rc.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://nk.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://me.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cn.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://ba.asd995.cn

Py:   Counter(arr)
来源：http://tl.huanxung.cn

PHP:  array_count_values($arr);
来源：http://ko.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dz.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://an.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uw.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://jl.wgjwhj.cn

Ruby: arr.tally
来源：http://pw.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mg.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://no.9csxet.cn

Py:   x in arr
来源：http://sp.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://pj.szsharing.cn

JS:   arr.includes(x)
来源：http://bc.colortex.cn

TS:   arr.includes(x)
来源：http://bv.shxzskj.cn

Java: list.contains(x)
来源：http://af.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://ul.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://go.huixiangedu.cn

C#:   list.Contains(x)
来源：http://aw.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://vn.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ij.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zy.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ym.nicolike.cn

TS:   [...arr];
来源：http://mg.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://as.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://st.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://eq.shxzskj.cn

C#:   new List<int>(list);
来源：http://uw.nszjky.cn

[D23] reduce 累积计算
来源：http://lk.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zu.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bp.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://et.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mo.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ks.huanxung.cn

Go:   // 手写循环
来源：http://lx.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ez.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ne.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://zj.newstarts.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yk.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fu.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jp.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wc.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cy.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lo.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hl.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ef.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://lw.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jw.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kr.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fk.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ug.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oo.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mg.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ph.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fb.muxihuayi.cn

[D26] 数组转字符串
来源：http://qr.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://kz.colortex.cn

PHP:  implode(", ", $arr);
来源：http://bb.9csxet.cn

JS:   arr.join(", ")
来源：http://gw.asd995.cn

TS:   arr.join(", ")
来源：http://ms.shxzskj.cn

Java: String.join(", ", list)
来源：http://wj.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://cf.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://bx.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://op.muxihuayi.cn

================================================================================
来源：http://pd.yuntaijiaju.cn

E. 字符串处理
来源：http://bm.wgjwhj.cn

================================================================================
来源：http://fd.gzmigu.cn

[E01] 拼接字符串
来源：http://ya.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tm.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rx.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nk.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lu.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dl.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nu.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qe.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ff.panjiajie.cn

[E02] 重复字符串
来源：http://qo.shtwfgs.cn

Py:   "ab" * 3
来源：http://dt.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://qq.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://jr.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://xs.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://tk.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://lk.jctech888.com.cn

Ruby: "ab" * 3
来源：http://vu.huanxung.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jk.yuntaijiaju.cn

[E03] 截取子串
来源：http://dl.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ie.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xk.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oo.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://yn.hahajie.cn

Java: s.substring(1, 4)
来源：http://ec.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rf.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rq.colortex.cn

C#:   s.Substring(1, 3)
来源：http://cl.hahajie.cn

[E04] 查找子串位置
来源：http://zc.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://nd.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://pp.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hq.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://bx.yuexingan06.cn

Java: s.indexOf("x")
来源：http://bd.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://hs.chemitech.net.cn

Ruby: s.index("x")
来源：http://jw.huanxung.cn

C#:   s.IndexOf("x")
来源：http://fg.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hs.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://re.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dc.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://od.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zv.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vj.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wb.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gu.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ci.wgjwhj.cn

[E06] 替换子串
来源：http://dn.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mh.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://qg.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kb.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://dk.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ws.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zg.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zr.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://mw.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://ls.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xi.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vz.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bn.huanxung.cn

TS:   s.split(",")
来源：http://xl.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fc.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rh.colortex.cn

Ruby: s.split(",");  s.split
来源：http://ey.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sl.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://mt.szxytkj.cn

Py:   ",".join(items)
来源：http://pj.521024.cn

PHP:  implode(",", $items);
来源：http://yh.panjiajie.cn

JS:   items.join(",")
来源：http://tz.newstarts.cn

TS:   items.join(",")
来源：http://oz.nszjky.cn

Java: String.join(",", items)
来源：http://sc.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://pl.newstarts.cn

Ruby: items.join(",")
来源：http://zs.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://in.9csxet.cn

[E09] 去除所有空白字符
来源：http://pm.panjiajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hu.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qm.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://hx.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://pk.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://uy.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oz.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rm.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ov.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://pa.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cl.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gj.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://qx.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://ch.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://rj.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nc.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kb.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fn.shxzskj.cn

[E11] 反转字符串
来源：http://ts.huanxung.cn

Py:   s[::-1]
来源：http://st.jianghongdianzi.cn

PHP:  strrev($s);
来源：http://lc.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://jm.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://cf.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ah.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uu.nicolike.cn

Ruby: s.reverse
来源：http://pp.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vo.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://qt.shxzukj.cn

Py:   s.count("a")
来源：http://mm.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://it.asd995.cn

JS:   s.split("a").length - 1
来源：http://yy.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://rd.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://on.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://pn.wgjwhj.cn

Ruby: s.count("a")
来源：http://vw.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://yy.hahajie.cn

[E13] 逐字符遍历
来源：http://uh.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://li.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vq.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qj.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wm.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ut.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ck.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iz.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://so.nicolike.cn

[E14] URL 编码与 Base64
来源：http://tk.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tz.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ul.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fd.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vs.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gu.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://of.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qn.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uq.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://re.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mq.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ui.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xr.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wo.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ep.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zc.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yl.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://th.huixiangedu.cn

[E16] 数字千分位
来源：http://kr.nszjky.cn

Py:   f"{1234567:,}"
来源：http://an.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://lq.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gx.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vl.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sg.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ma.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yb.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://wq.jianghongdianzi.cn

[E17] 首字母大写
来源：http://dd.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cx.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zr.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xf.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dl.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://on.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ry.bjjhwx.cn

Ruby: s.capitalize
来源：http://vc.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fj.shxzukj.cn

[E18] 模板占位符替换
来源：http://ia.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wo.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ys.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sg.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ks.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kl.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hm.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dn.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nh.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://ri.panjiajie.cn

Py:   s.splitlines()
来源：http://lr.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cl.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://zn.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://dt.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://wk.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://fk.bookmarksfly.cn

Ruby: s.lines
来源：http://ls.wgjwhj.cn

C#:   s.Split('\n')
来源：http://le.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://ir.panjiajie.cn

Py:   if not s:
来源：http://zl.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zm.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vw.muxihuayi.cn

TS:   if (s === "") {}
来源：http://cr.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://on.asd995.cn

Go:   if s == "" {}
来源：http://rh.huanxung.cn

Ruby: if s.empty?
来源：http://fw.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://df.szxytkj.cn

[E21] 超长截断加省略号
来源：http://qi.huixinmuqiang.cn


<!-- 参考信息 -->