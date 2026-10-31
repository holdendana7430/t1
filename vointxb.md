代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gq.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ti.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://wf.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://fb.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nh.colortex.cn

Go:   // 手写循环
来源：http://pd.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ul.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://av.szxytkj.cn

[D15] 去重
来源：http://or.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ld.shxzskj.cn

PHP:  array_unique($arr);
来源：http://ue.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://op.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://tm.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gg.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sp.huanxung.cn

Ruby: arr.uniq
来源：http://dv.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://il.newstarts.cn

[D16] 求和与平均值
来源：http://sk.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gk.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://am.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hf.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qa.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qu.yuexingan06.cn

Go:   // 手写循环累加
来源：http://zd.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jp.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://al.521024.cn

[D17] 最大值与最小值
来源：http://mr.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://zz.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://tq.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ix.newstarts.cn

TS:   Math.max(...arr);
来源：http://zr.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fu.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pn.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://fv.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://zp.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://vh.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qt.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://mi.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kn.jctech888.com.cn

TS:   nested.flat();
来源：http://mu.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jy.colortex.cn

Go:   // 手写双层循环
来源：http://dd.shxzukj.cn

Ruby: nested.flatten
来源：http://lj.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mj.szxytkj.cn

[D19] 按字段分组
来源：http://ci.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cf.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://km.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://km.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qy.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xs.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://dj.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ll.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xq.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://qn.shxzukj.cn

Py:   Counter(arr)
来源：http://fb.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://tk.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xh.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lw.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ym.nszjky.cn

Go:   // 手写 map[T]int
来源：http://ue.521024.cn

Ruby: arr.tally
来源：http://xq.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bg.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://xt.shxzskj.cn

Py:   x in arr
来源：http://wz.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ae.colortex.cn

JS:   arr.includes(x)
来源：http://vr.haigaiapp.cn

TS:   arr.includes(x)
来源：http://ap.newstarts.cn

Java: list.contains(x)
来源：http://tb.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://zb.huanxung.cn

Ruby: arr.include?(x)
来源：http://qd.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://ni.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://ey.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cq.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zr.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ho.szsharing.cn

TS:   [...arr];
来源：http://ay.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ya.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xb.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://ek.colortex.cn

C#:   new List<int>(list);
来源：http://ni.hahajie.cn

[D23] reduce 累积计算
来源：http://ig.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zb.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ko.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://co.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vk.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://iz.panjiajie.cn

Go:   // 手写循环
来源：http://pz.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yl.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ub.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://um.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hd.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xa.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fk.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nl.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nr.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://na.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cw.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nh.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://em.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dk.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pq.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mm.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fg.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ti.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qg.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vn.521024.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jx.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ga.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://yj.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://ul.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://ex.nicolike.cn

TS:   arr.join(", ")
来源：http://wl.gzmigu.cn

Java: String.join(", ", list)
来源：http://et.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://xi.shxzskj.cn

Ruby: arr.join(", ")
来源：http://sn.huanxung.cn

C#:   string.Join(", ", list)
来源：http://lm.shxzukj.cn

================================================================================
来源：http://mz.asd995.cn

E. 字符串处理
来源：http://vl.9csxet.cn

================================================================================
来源：http://tq.colortex.cn

[E01] 拼接字符串
来源：http://up.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dd.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bx.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hm.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ex.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uk.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sy.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xs.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gp.wgjwhj.cn

[E02] 重复字符串
来源：http://lq.asd995.cn

Py:   "ab" * 3
来源：http://iw.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://mm.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://or.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://wq.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://kt.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://yc.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://bz.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://be.szsharing.cn

[E03] 截取子串
来源：http://cj.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vi.szxytkj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jt.haigaiapp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://su.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://dx.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://tu.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kh.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bo.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://ty.hahajie.cn

[E04] 查找子串位置
来源：http://vq.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://zk.huanxung.cn

PHP:  strpos($s, "x");
来源：http://nh.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mn.9csxet.cn

TS:   s.indexOf("x")
来源：http://ui.huanxung.cn

Java: s.indexOf("x")
来源：http://dp.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://ky.hahajie.cn

Ruby: s.index("x")
来源：http://go.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://dj.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qm.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oh.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qk.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qo.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dh.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ii.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tc.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://su.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yk.huixinmuqiang.cn

[E06] 替换子串
来源：http://pe.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nk.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://qp.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cr.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://ya.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gk.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jd.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bx.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://ck.asd995.cn

[E07] 按分隔符拆分
来源：http://dp.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bb.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wv.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ld.muxihuayi.cn

TS:   s.split(",")
来源：http://co.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gk.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://da.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://rv.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://em.9csxet.cn

[E08] 数组按分隔符合并
来源：http://tg.lnxyls.cn

Py:   ",".join(items)
来源：http://qk.panjiajie.cn

PHP:  implode(",", $items);
来源：http://lg.szsharing.cn

JS:   items.join(",")
来源：http://lg.colortex.cn

TS:   items.join(",")
来源：http://zu.shxzukj.cn

Java: String.join(",", items)
来源：http://vh.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://ql.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://wk.huanxung.cn

C#:   string.Join(",", items)
来源：http://em.521024.cn

[E09] 去除所有空白字符
来源：http://jr.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lj.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vm.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://jt.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://zl.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://ky.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gr.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sh.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://te.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://mc.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tq.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zk.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://vu.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://wv.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://fh.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://my.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lu.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dq.521024.cn

[E11] 反转字符串
来源：http://gl.nicolike.cn

Py:   s[::-1]
来源：http://kp.wgjwhj.cn

PHP:  strrev($s);
来源：http://ji.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://ty.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://pe.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ph.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://du.huanxung.cn

Ruby: s.reverse
来源：http://sq.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xx.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://kz.szxytkj.cn

Py:   s.count("a")
来源：http://qo.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://hc.newstarts.cn

JS:   s.split("a").length - 1
来源：http://id.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://qu.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nh.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://bc.shxzskj.cn

Ruby: s.count("a")
来源：http://ej.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://hv.gzmigu.cn

[E13] 逐字符遍历
来源：http://hm.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://wg.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cf.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qs.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ws.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qu.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xa.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://er.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gy.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://yj.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nk.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kq.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tj.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tj.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ww.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ns.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bi.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qd.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://br.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ix.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wj.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zq.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gc.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kv.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yl.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zd.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wh.bookmarksfly.cn

[E16] 数字千分位
来源：http://dd.szsharing.cn

Py:   f"{1234567:,}"
来源：http://aa.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://pf.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vs.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sl.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wl.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ne.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uo.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://wo.panjiajie.cn

[E17] 首字母大写
来源：http://zq.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uc.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dp.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hm.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mo.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cc.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xr.szxytkj.cn

Ruby: s.capitalize
来源：http://vb.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mn.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://yt.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mm.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wz.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ab.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qh.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://es.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jw.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dy.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yn.asd995.cn

[E19] 多行文本按行拆分
来源：http://bl.wgjwhj.cn

Py:   s.splitlines()
来源：http://gy.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wg.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://rr.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://tk.521024.cn

Java: s.lines().toList()
来源：http://ji.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://wg.521024.cn

Ruby: s.lines
来源：http://tn.shtwfgs.cn

C#:   s.Split('\n')
来源：http://ey.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://qy.huixinmuqiang.cn

Py:   if not s:
来源：http://zc.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bu.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aq.huanxung.cn

TS:   if (s === "") {}
来源：http://sh.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://im.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://hg.shxzukj.cn

Ruby: if s.empty?
来源：http://gd.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vi.9csxet.cn

[E21] 超长截断加省略号
来源：http://kt.haigaiapp.cn


<!-- 参考信息 -->