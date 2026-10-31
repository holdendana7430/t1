代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hj.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sl.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://il.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://ga.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://an.wgjwhj.cn

Go:   // 手写循环
来源：http://bw.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://po.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yx.yuexingan06.cn

[D15] 去重
来源：http://kq.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gw.hnjuh.cn

PHP:  array_unique($arr);
来源：http://xy.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://rf.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://oj.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tu.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rg.szsharing.cn

Ruby: arr.uniq
来源：http://wq.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://ux.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://zd.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eb.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://be.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ko.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uw.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lv.huixiangedu.cn

Go:   // 手写循环累加
来源：http://fn.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wd.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://st.panjiajie.cn

[D17] 最大值与最小值
来源：http://bq.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://no.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://ch.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ph.colortex.cn

TS:   Math.max(...arr);
来源：http://wq.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://eh.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vc.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://al.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://zw.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://ob.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cw.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://xj.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pf.bjjhwx.cn

TS:   nested.flat();
来源：http://zx.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ws.hnjuh.cn

Go:   // 手写双层循环
来源：http://pp.muxihuayi.cn

Ruby: nested.flatten
来源：http://ba.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ch.wgjwhj.cn

[D19] 按字段分组
来源：http://hw.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fz.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vc.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://px.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://np.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fa.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://ej.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gc.szsharing.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ax.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ba.yuexingan06.cn

Py:   Counter(arr)
来源：http://mc.nicolike.cn

PHP:  array_count_values($arr);
来源：http://ad.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cc.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cc.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pk.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://ii.nicolike.cn

Ruby: arr.tally
来源：http://um.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bd.nicolike.cn

[D21] 判断是否包含某元素
来源：http://re.shxzukj.cn

Py:   x in arr
来源：http://hi.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://oj.asd995.cn

JS:   arr.includes(x)
来源：http://xx.yuexingan06.cn

TS:   arr.includes(x)
来源：http://fd.yuntaijiaju.cn

Java: list.contains(x)
来源：http://zw.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://co.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://yy.szsharing.cn

C#:   list.Contains(x)
来源：http://sv.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://bt.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ll.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://os.jctech888.com.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ur.jianghongdianzi.cn

TS:   [...arr];
来源：http://pj.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://qd.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xt.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://xk.newstarts.cn

C#:   new List<int>(list);
来源：http://kn.gzmigu.cn

[D23] reduce 累积计算
来源：http://mh.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aj.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bb.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vo.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eq.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ta.9csxet.cn

Go:   // 手写循环
来源：http://vv.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fr.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://el.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ii.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hh.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bk.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ah.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gv.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ln.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vc.shtwfgs.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gt.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fv.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://qg.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://im.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eq.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yl.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ny.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gr.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://no.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fg.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xb.9csxet.cn

[D26] 数组转字符串
来源：http://he.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://qt.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://rr.chemitech.net.cn

JS:   arr.join(", ")
来源：http://kq.9csxet.cn

TS:   arr.join(", ")
来源：http://lh.gzmigu.cn

Java: String.join(", ", list)
来源：http://qj.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://se.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://wf.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://gx.jianghongdianzi.cn

================================================================================
来源：http://rk.9csxet.cn

E. 字符串处理
来源：http://wj.wgjwhj.cn

================================================================================
来源：http://rc.shtwfgs.cn

[E01] 拼接字符串
来源：http://pd.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fr.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pb.shxzskj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wb.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jc.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xg.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gv.9csxet.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vx.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qc.haigaiapp.cn

[E02] 重复字符串
来源：http://ko.9csxet.cn

Py:   "ab" * 3
来源：http://qj.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://hl.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://gv.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://kj.lnxyls.cn

Java: "ab".repeat(3)
来源：http://na.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://gf.bjjhwx.cn

Ruby: "ab" * 3
来源：http://qw.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ub.hahajie.cn

[E03] 截取子串
来源：http://nk.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zd.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ne.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jg.9csxet.cn

TS:   s.slice(1, 4)
来源：http://tz.521024.cn

Java: s.substring(1, 4)
来源：http://oz.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ba.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mz.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://bl.bjjhwx.cn

[E04] 查找子串位置
来源：http://wj.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://we.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://yq.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nb.gzmigu.cn

TS:   s.indexOf("x")
来源：http://wd.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://vj.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://he.hahajie.cn

Ruby: s.index("x")
来源：http://eb.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://hp.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ij.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yo.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cy.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vx.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ff.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wm.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ye.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ix.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cd.huixiangedu.cn

[E06] 替换子串
来源：http://tg.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://up.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://eg.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gr.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://lj.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://di.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fh.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cd.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://xy.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://dp.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qc.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kg.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qw.huixiangedu.cn

TS:   s.split(",")
来源：http://hw.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ko.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hq.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://cz.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wc.nicolike.cn

[E08] 数组按分隔符合并
来源：http://rf.newstarts.cn

Py:   ",".join(items)
来源：http://bj.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://xi.huixinmuqiang.cn

JS:   items.join(",")
来源：http://uo.lnxyls.cn

TS:   items.join(",")
来源：http://bl.shxzukj.cn

Java: String.join(",", items)
来源：http://qw.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://yt.haigaiapp.cn

Ruby: items.join(",")
来源：http://an.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://mx.hnjuh.cn

[E09] 去除所有空白字符
来源：http://md.shxzskj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yj.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://th.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://ar.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://hc.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://lo.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bs.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qg.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wn.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://fd.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://em.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zh.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://bi.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://wp.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ym.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iy.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zj.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://op.hahajie.cn

[E11] 反转字符串
来源：http://iu.wgjwhj.cn

Py:   s[::-1]
来源：http://nx.nszjky.cn

PHP:  strrev($s);
来源：http://ow.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://ey.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://jp.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nd.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jj.huixiangedu.cn

Ruby: s.reverse
来源：http://dz.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wn.nszjky.cn

[E12] 统计某字符出现次数
来源：http://wd.jianghongdianzi.cn

Py:   s.count("a")
来源：http://ho.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://mb.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://xj.huanxung.cn

TS:   s.split("a").length - 1
来源：http://iu.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bo.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://yu.yuexingan06.cn

Ruby: s.count("a")
来源：http://cr.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://ld.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://vi.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://gy.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eb.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cf.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eh.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qi.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zf.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://od.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vb.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://ic.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ut.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wo.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sk.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fo.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fr.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tt.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kn.gzmigu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yj.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://yt.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mj.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bm.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wk.hnjuh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ne.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bg.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wc.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kw.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sp.huixiangedu.cn

[E16] 数字千分位
来源：http://zv.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://zd.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://dw.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mh.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gc.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nd.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ai.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uu.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://tq.bookmarksfly.cn

[E17] 首字母大写
来源：http://yu.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sn.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ic.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pr.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ol.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yh.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uq.colortex.cn

Ruby: s.capitalize
来源：http://nj.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wb.lnxyls.cn

[E18] 模板占位符替换
来源：http://vs.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ze.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ic.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nw.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rb.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qu.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fp.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ag.panjiajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ob.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://vz.szxytkj.cn

Py:   s.splitlines()
来源：http://bl.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://co.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://br.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://eu.huixiangedu.cn

Java: s.lines().toList()
来源：http://jw.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://uv.9csxet.cn

Ruby: s.lines
来源：http://ov.yuexingan06.cn

C#:   s.Split('\n')
来源：http://eu.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://xd.shxzskj.cn

Py:   if not s:
来源：http://sn.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://th.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qv.521024.cn

TS:   if (s === "") {}
来源：http://vq.bookmarksfly.cn

Java: if (s.isEmpty()) {}
来源：http://hg.nszjky.cn

Go:   if s == "" {}
来源：http://ot.muxihuayi.cn

Ruby: if s.empty?
来源：http://bb.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rr.lnxyls.cn

[E21] 超长截断加省略号
来源：http://es.panjiajie.cn


<!-- 参考信息 -->