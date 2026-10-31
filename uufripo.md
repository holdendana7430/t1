代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://ai.huanxung.cn

Go:   // 手写循环
来源：http://mh.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qb.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hx.yuexingan06.cn

[D15] 去重
来源：http://wm.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mn.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://xq.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://yn.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://sg.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ay.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vc.shxzukj.cn

Ruby: arr.uniq
来源：http://ps.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://co.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ww.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ck.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xs.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wh.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://px.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hw.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ub.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://al.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://oy.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://iy.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://bh.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://hc.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tv.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://vf.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dt.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://he.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://nz.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://bu.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://yy.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yb.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://zm.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yu.nszjky.cn

TS:   nested.flat();
来源：http://vr.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qp.asd995.cn

Go:   // 手写双层循环
来源：http://uk.huixiangedu.cn

Ruby: nested.flatten
来源：http://el.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ew.jctech888.com.cn

[D19] 按字段分组
来源：http://pp.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mj.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://id.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bg.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cb.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cm.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://ih.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rr.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gx.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://xn.huanxung.cn

Py:   Counter(arr)
来源：http://pp.huanxung.cn

PHP:  array_count_values($arr);
来源：http://oz.nszjky.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xl.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://is.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://is.shxzukj.cn

Go:   // 手写 map[T]int
来源：http://ky.yuntaijiaju.cn

Ruby: arr.tally
来源：http://cx.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jl.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://ho.nszjky.cn

Py:   x in arr
来源：http://yg.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://hh.shxzukj.cn

JS:   arr.includes(x)
来源：http://qb.muxihuayi.cn

TS:   arr.includes(x)
来源：http://en.nszjky.cn

Java: list.contains(x)
来源：http://fu.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://kw.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://hd.9csxet.cn

C#:   list.Contains(x)
来源：http://fd.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://zk.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vj.yuntaijiaju.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yd.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qm.chemitech.net.cn

TS:   [...arr];
来源：http://aq.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://hl.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tn.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://ub.shtwfgs.cn

C#:   new List<int>(list);
来源：http://jh.panjiajie.cn

[D23] reduce 累积计算
来源：http://is.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gu.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://io.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xo.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nc.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xr.huixinmuqiang.cn

Go:   // 手写循环
来源：http://va.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ze.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sg.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://sf.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sp.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iu.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rk.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pq.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mh.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ep.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yj.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dl.521024.cn

[D25] Set 集合去重与交并差
来源：http://wv.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fu.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eg.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wq.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hk.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tn.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ez.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vy.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ms.szxytkj.cn

[D26] 数组转字符串
来源：http://vo.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://dg.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://lq.yuexingan06.cn

JS:   arr.join(", ")
来源：http://ge.huixiangedu.cn

TS:   arr.join(", ")
来源：http://xj.muxihuayi.cn

Java: String.join(", ", list)
来源：http://qb.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://fk.bjjhwx.cn

Ruby: arr.join(", ")
来源：http://rz.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://vm.bjjhwx.cn

================================================================================
来源：http://hw.yuexingan06.cn

E. 字符串处理
来源：http://nr.nszjky.cn

================================================================================
来源：http://zi.nszjky.cn

[E01] 拼接字符串
来源：http://sj.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pm.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qt.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ej.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bk.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mf.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://av.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lv.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vr.muxihuayi.cn

[E02] 重复字符串
来源：http://ty.hnjuh.cn

Py:   "ab" * 3
来源：http://xx.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://do.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://qr.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://mg.shxzukj.cn

Java: "ab".repeat(3)
来源：http://kc.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://tl.huanxung.cn

Ruby: "ab" * 3
来源：http://jp.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ui.jctech888.com.cn

[E03] 截取子串
来源：http://tj.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vh.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ey.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ud.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://dm.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://xz.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ge.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://je.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://lg.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://to.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://nn.nicolike.cn

PHP:  strpos($s, "x");
来源：http://qr.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mr.gzmigu.cn

TS:   s.indexOf("x")
来源：http://ty.9csxet.cn

Java: s.indexOf("x")
来源：http://wp.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://wa.gzmigu.cn

Ruby: s.index("x")
来源：http://uo.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://du.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rg.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ew.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jf.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://od.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ca.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yc.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gq.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xe.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bu.shxzukj.cn

[E06] 替换子串
来源：http://iy.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jo.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://kk.panjiajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ca.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://no.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qx.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yk.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hf.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://lj.szsharing.cn

[E07] 按分隔符拆分
来源：http://iu.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ud.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nx.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gz.nszjky.cn

TS:   s.split(",")
来源：http://hy.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xx.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://om.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://pj.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wf.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://os.shxzskj.cn

Py:   ",".join(items)
来源：http://an.hahajie.cn

PHP:  implode(",", $items);
来源：http://bf.bjjhwx.cn

JS:   items.join(",")
来源：http://hg.huanxung.cn

TS:   items.join(",")
来源：http://ed.huixiangedu.cn

Java: String.join(",", items)
来源：http://cr.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://au.nicolike.cn

Ruby: items.join(",")
来源：http://cm.yuntaijiaju.cn

C#:   string.Join(",", items)
来源：http://fa.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://os.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oa.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gt.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://sy.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://ed.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://dw.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ka.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pz.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bu.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://aa.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xz.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bh.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://im.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://kb.huanxung.cn

Java: String.format("%03d", 7)
来源：http://tz.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cd.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cr.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vu.yuexingan06.cn

[E11] 反转字符串
来源：http://rl.bjjhwx.cn

Py:   s[::-1]
来源：http://uv.shxzskj.cn

PHP:  strrev($s);
来源：http://cj.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://qn.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://cu.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://to.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yp.chemitech.net.cn

Ruby: s.reverse
来源：http://rn.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cv.nicolike.cn

[E12] 统计某字符出现次数
来源：http://jy.hahajie.cn

Py:   s.count("a")
来源：http://se.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://yf.newstarts.cn

JS:   s.split("a").length - 1
来源：http://fs.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://gu.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vz.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://yr.szxytkj.cn

Ruby: s.count("a")
来源：http://dz.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://yh.chemitech.net.cn

[E13] 逐字符遍历
来源：http://mm.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://hk.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ww.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://io.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nb.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vz.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tc.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jg.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bg.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://vj.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://py.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uy.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mv.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sa.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ag.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ji.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cf.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lc.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://lj.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mo.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bw.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lh.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://np.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bw.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ly.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ja.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ke.521024.cn

[E16] 数字千分位
来源：http://it.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://ey.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://eh.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vm.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pu.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cc.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gq.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uw.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://sj.lnxyls.cn

[E17] 首字母大写
来源：http://gb.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sd.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://en.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gm.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mv.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sc.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ub.huanxung.cn

Ruby: s.capitalize
来源：http://fz.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xm.wgjwhj.cn

[E18] 模板占位符替换
来源：http://lb.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ip.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://at.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yv.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uq.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xl.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ev.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wr.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ed.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://xq.chemitech.net.cn

Py:   s.splitlines()
来源：http://pp.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dx.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://jt.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://vr.shxzskj.cn

Java: s.lines().toList()
来源：http://km.521024.cn

Go:   strings.Split(s, "\n")
来源：http://rg.wgjwhj.cn

Ruby: s.lines
来源：http://he.hahajie.cn

C#:   s.Split('\n')
来源：http://vf.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://jm.jctech888.com.cn

Py:   if not s:
来源：http://oo.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wp.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ew.shxzukj.cn

TS:   if (s === "") {}
来源：http://bm.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://uh.shxzskj.cn

Go:   if s == "" {}
来源：http://ty.panjiajie.cn

Ruby: if s.empty?
来源：http://bh.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gt.shxzukj.cn

[E21] 超长截断加省略号
来源：http://lo.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sf.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iu.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pc.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://im.shxzskj.cn


<!-- 参考信息 -->