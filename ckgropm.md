代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qn.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eo.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://wh.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://lv.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sh.huanxung.cn

Go:   // 手写循环
来源：http://xm.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pq.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mt.wgjwhj.cn

[D15] 去重
来源：http://kf.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rz.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://yk.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://jy.nicolike.cn

TS:   [...new Set(arr)]
来源：http://vs.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hi.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ke.yuntaijiaju.cn

Ruby: arr.uniq
来源：http://xg.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://ce.wgjwhj.cn

[D16] 求和与平均值
来源：http://eb.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xz.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qo.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mz.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jn.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lm.shtwfgs.cn

Go:   // 手写循环累加
来源：http://zi.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wk.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://zr.9csxet.cn

[D17] 最大值与最小值
来源：http://zj.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://nd.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://bp.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sy.huanxung.cn

TS:   Math.max(...arr);
来源：http://fy.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://it.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://am.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://yv.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://vi.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://iy.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xi.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://gi.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dt.gzmigu.cn

TS:   nested.flat();
来源：http://wq.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sc.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://ss.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://hg.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hw.shxzskj.cn

[D19] 按字段分组
来源：http://gc.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dj.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://so.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xa.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hp.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tj.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://vf.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fk.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ah.521024.cn

[D20] 统计每个元素出现次数
来源：http://xg.shxzskj.cn

Py:   Counter(arr)
来源：http://dl.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://bu.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ay.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ka.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tp.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://mh.hahajie.cn

Ruby: arr.tally
来源：http://sr.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://me.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://vy.yuexingan06.cn

Py:   x in arr
来源：http://lf.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://yc.haigaiapp.cn

JS:   arr.includes(x)
来源：http://fh.colortex.cn

TS:   arr.includes(x)
来源：http://gw.lnxyls.cn

Java: list.contains(x)
来源：http://rm.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://if.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://tc.jctech888.com.cn

C#:   list.Contains(x)
来源：http://di.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://sr.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hr.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zx.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dx.huixiangedu.cn

TS:   [...arr];
来源：http://su.nszjky.cn

Java: new ArrayList<>(list);
来源：http://jn.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kk.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://wa.chemitech.net.cn

C#:   new List<int>(list);
来源：http://zt.hahajie.cn

[D23] reduce 累积计算
来源：http://qy.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xd.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xq.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iy.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vz.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hi.colortex.cn

Go:   // 手写循环
来源：http://jk.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hq.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sz.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://xv.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qf.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fc.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vr.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wp.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xu.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nw.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tu.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xw.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://tz.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rz.jctech888.com.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ek.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ts.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://co.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rw.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dl.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wg.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xe.hnjuh.cn

[D26] 数组转字符串
来源：http://yb.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://mn.521024.cn

PHP:  implode(", ", $arr);
来源：http://tg.huixiangedu.cn

JS:   arr.join(", ")
来源：http://ji.jctech888.com.cn

TS:   arr.join(", ")
来源：http://uw.yuexingan06.cn

Java: String.join(", ", list)
来源：http://ei.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://ts.521024.cn

Ruby: arr.join(", ")
来源：http://sb.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://pf.huixiangedu.cn

================================================================================
来源：http://fs.szxytkj.cn

E. 字符串处理
来源：http://ui.asd995.cn

================================================================================
来源：http://sp.wgjwhj.cn

[E01] 拼接字符串
来源：http://sq.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fd.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hk.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dt.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bs.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ie.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oz.jctech888.com.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xf.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qg.9csxet.cn

[E02] 重复字符串
来源：http://zt.shxzukj.cn

Py:   "ab" * 3
来源：http://kw.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://dr.521024.cn

JS:   "ab".repeat(3)
来源：http://qs.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://eo.szsharing.cn

Java: "ab".repeat(3)
来源：http://kf.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://ss.nszjky.cn

Ruby: "ab" * 3
来源：http://pq.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yy.szxytkj.cn

[E03] 截取子串
来源：http://gn.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rz.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ww.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hb.newstarts.cn

TS:   s.slice(1, 4)
来源：http://rz.nicolike.cn

Java: s.substring(1, 4)
来源：http://zp.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jk.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://az.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://dd.huanxung.cn

[E04] 查找子串位置
来源：http://wk.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://we.521024.cn

PHP:  strpos($s, "x");
来源：http://ds.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xf.szsharing.cn

TS:   s.indexOf("x")
来源：http://nx.szxytkj.cn

Java: s.indexOf("x")
来源：http://tw.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://el.szsharing.cn

Ruby: s.index("x")
来源：http://xn.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://ti.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ni.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bs.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lj.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ys.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fi.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ny.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fh.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fq.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fu.shxzskj.cn

[E06] 替换子串
来源：http://om.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zl.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ie.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rm.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://wm.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://if.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ns.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lo.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://bh.lnxyls.cn

[E07] 按分隔符拆分
来源：http://xo.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kj.gzmigu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fz.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cu.huanxung.cn

TS:   s.split(",")
来源：http://fe.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pw.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jr.colortex.cn

Ruby: s.split(",");  s.split
来源：http://nu.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cw.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://sa.shxzukj.cn

Py:   ",".join(items)
来源：http://hb.shxzukj.cn

PHP:  implode(",", $items);
来源：http://gq.nicolike.cn

JS:   items.join(",")
来源：http://kp.jctech888.com.cn

TS:   items.join(",")
来源：http://ko.jctech888.com.cn

Java: String.join(",", items)
来源：http://wo.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://gi.lnxyls.cn

Ruby: items.join(",")
来源：http://py.hnjuh.cn

C#:   string.Join(",", items)
来源：http://vy.9csxet.cn

[E09] 去除所有空白字符
来源：http://mk.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kd.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ha.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://en.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://et.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://eo.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bd.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vg.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zu.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://me.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://re.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://la.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://yk.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://tb.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://nc.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wv.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mn.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qu.muxihuayi.cn

[E11] 反转字符串
来源：http://nx.yuntaijiaju.cn

Py:   s[::-1]
来源：http://wm.jctech888.com.cn

PHP:  strrev($s);
来源：http://sb.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://ft.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://bm.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yz.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jw.huanxung.cn

Ruby: s.reverse
来源：http://ae.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tv.szsharing.cn

[E12] 统计某字符出现次数
来源：http://oy.huanxung.cn

Py:   s.count("a")
来源：http://po.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://pu.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://gd.huanxung.cn

TS:   s.split("a").length - 1
来源：http://qu.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lk.asd995.cn

Go:   strings.Count(s, "a")
来源：http://cp.nszjky.cn

Ruby: s.count("a")
来源：http://zc.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://da.asd995.cn

[E13] 逐字符遍历
来源：http://vx.panjiajie.cn

Py:   for ch in s: print(ch)
来源：http://tb.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uq.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iy.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rl.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wy.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fe.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eb.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gd.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://vb.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ta.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wx.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dq.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wp.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kl.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xo.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ip.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oh.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://wo.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gx.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lk.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://te.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://er.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wq.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://og.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ub.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cd.huixinmuqiang.cn

[E16] 数字千分位
来源：http://ld.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://go.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://hn.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cx.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rr.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kz.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yx.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nn.asd995.cn

C#:   1234567.ToString("N0")
来源：http://wv.nicolike.cn

[E17] 首字母大写
来源：http://dp.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xv.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ss.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jc.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ib.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vd.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vo.huixiangedu.cn

Ruby: s.capitalize
来源：http://lj.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://th.521024.cn

[E18] 模板占位符替换
来源：http://yh.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gv.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xr.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yd.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ul.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ps.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jx.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rj.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wb.521024.cn

[E19] 多行文本按行拆分
来源：http://fy.bjjhwx.cn

Py:   s.splitlines()
来源：http://zz.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vp.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://lw.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://vb.asd995.cn

Java: s.lines().toList()
来源：http://ku.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://uu.shtwfgs.cn

Ruby: s.lines
来源：http://hy.panjiajie.cn

C#:   s.Split('\n')
来源：http://ul.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://nk.huixiangedu.cn

Py:   if not s:
来源：http://tz.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ru.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vp.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://km.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://ck.bookmarksfly.cn

Go:   if s == "" {}
来源：http://sy.wgjwhj.cn

Ruby: if s.empty?
来源：http://lj.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cq.newstarts.cn

[E21] 超长截断加省略号
来源：http://nw.chemitech.net.cn


<!-- 参考信息 -->