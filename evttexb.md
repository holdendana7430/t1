代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bl.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iw.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://lj.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://yq.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://du.shxzukj.cn

Go:   // 手写循环
来源：http://hy.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tz.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ji.huanxung.cn

[D15] 去重
来源：http://vz.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fy.hahajie.cn

PHP:  array_unique($arr);
来源：http://co.asd995.cn

JS:   [...new Set(arr)]
来源：http://ja.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://re.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rh.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://na.szxytkj.cn

Ruby: arr.uniq
来源：http://bc.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://zn.shxzukj.cn

[D16] 求和与平均值
来源：http://xf.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ju.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ud.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xw.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ua.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wx.huanxung.cn

Go:   // 手写循环累加
来源：http://uz.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jr.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://fx.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://lz.asd995.cn

Py:   max(arr);  min(arr)
来源：http://yf.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://yu.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fk.asd995.cn

TS:   Math.max(...arr);
来源：http://wx.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cs.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ns.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://zy.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://db.521024.cn

[D18] 扁平化嵌套数组
来源：http://sj.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nf.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://kh.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eq.yuntaijiaju.cn

TS:   nested.flat();
来源：http://yr.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://io.panjiajie.cn

Go:   // 手写双层循环
来源：http://ez.panjiajie.cn

Ruby: nested.flatten
来源：http://hz.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rt.9csxet.cn

[D19] 按字段分组
来源：http://ri.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://if.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ih.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bu.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fm.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://um.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://lr.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uy.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ck.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://bb.szsharing.cn

Py:   Counter(arr)
来源：http://je.newstarts.cn

PHP:  array_count_values($arr);
来源：http://mv.wgjwhj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jc.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pz.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hc.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://zv.newstarts.cn

Ruby: arr.tally
来源：http://xh.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rf.521024.cn

[D21] 判断是否包含某元素
来源：http://yx.haigaiapp.cn

Py:   x in arr
来源：http://mt.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://tz.lnxyls.cn

JS:   arr.includes(x)
来源：http://fs.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://nm.nicolike.cn

Java: list.contains(x)
来源：http://lv.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://kf.gzmigu.cn

Ruby: arr.include?(x)
来源：http://jx.panjiajie.cn

C#:   list.Contains(x)
来源：http://oy.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://pa.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sb.bookmarksfly.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rt.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hl.521024.cn

TS:   [...arr];
来源：http://xw.9csxet.cn

Java: new ArrayList<>(list);
来源：http://nv.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zu.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://no.chemitech.net.cn

C#:   new List<int>(list);
来源：http://mv.yuexingan06.cn

[D23] reduce 累积计算
来源：http://lo.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ka.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kc.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vy.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ab.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xg.bookmarksfly.cn

Go:   // 手写循环
来源：http://ub.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ml.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bg.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://ez.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dw.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kp.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zf.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ht.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nz.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://co.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rz.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ww.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://jt.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wo.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bi.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vz.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ae.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sk.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hq.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dc.lnxyls.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qm.colortex.cn

[D26] 数组转字符串
来源：http://sr.chemitech.net.cn

Py:   ", ".join(map(str, arr))
来源：http://cy.asd995.cn

PHP:  implode(", ", $arr);
来源：http://qu.wgjwhj.cn

JS:   arr.join(", ")
来源：http://rn.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://mn.huanxung.cn

Java: String.join(", ", list)
来源：http://hv.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://fw.shxzukj.cn

Ruby: arr.join(", ")
来源：http://ug.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://ff.nicolike.cn

================================================================================
来源：http://bj.shxzukj.cn

E. 字符串处理
来源：http://ai.gzmigu.cn

================================================================================
来源：http://eh.newstarts.cn

[E01] 拼接字符串
来源：http://yw.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wk.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uq.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vr.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dd.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rk.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hx.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cg.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://im.muxihuayi.cn

[E02] 重复字符串
来源：http://xt.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://cv.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://xk.nicolike.cn

JS:   "ab".repeat(3)
来源：http://tp.asd995.cn

TS:   "ab".repeat(3)
来源：http://um.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://uc.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://vg.lnxyls.cn

Ruby: "ab" * 3
来源：http://yd.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ao.jianghongdianzi.cn

[E03] 截取子串
来源：http://pd.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rh.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aj.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bt.nszjky.cn

TS:   s.slice(1, 4)
来源：http://xo.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ui.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qu.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gd.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://mq.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://bk.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://ag.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://ud.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ga.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://jz.szxytkj.cn

Java: s.indexOf("x")
来源：http://hn.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://bg.bjjhwx.cn

Ruby: s.index("x")
来源：http://vm.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://fj.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jt.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cg.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vi.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ev.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vb.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ma.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pd.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xa.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ze.jctech888.com.cn

[E06] 替换子串
来源：http://tr.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lc.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://od.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ce.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://ks.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jq.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tu.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ur.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://fv.hahajie.cn

[E07] 按分隔符拆分
来源：http://yk.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ab.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ie.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iv.9csxet.cn

TS:   s.split(",")
来源：http://xz.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xp.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kk.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://wx.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nl.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://ct.bjjhwx.cn

Py:   ",".join(items)
来源：http://ic.asd995.cn

PHP:  implode(",", $items);
来源：http://mw.szsharing.cn

JS:   items.join(",")
来源：http://vi.shxzskj.cn

TS:   items.join(",")
来源：http://jx.gzmigu.cn

Java: String.join(",", items)
来源：http://xz.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://ma.shxzskj.cn

Ruby: items.join(",")
来源：http://hc.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://db.szsharing.cn

[E09] 去除所有空白字符
来源：http://nl.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sw.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zu.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://nc.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://zf.hnjuh.cn

Java: s.replaceAll("\\s+", "")
来源：http://zx.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ob.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ob.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rx.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://mt.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zy.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pg.shxzskj.cn

JS:   "7".padStart(3, "0")
来源：http://hv.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://bb.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://zo.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qq.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ic.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hk.bookmarksfly.cn

[E11] 反转字符串
来源：http://xy.jianghongdianzi.cn

Py:   s[::-1]
来源：http://ye.jctech888.com.cn

PHP:  strrev($s);
来源：http://rr.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://wb.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://xy.hahajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jd.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ct.521024.cn

Ruby: s.reverse
来源：http://xk.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vi.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://tp.huixiangedu.cn

Py:   s.count("a")
来源：http://ji.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://je.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://by.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://gs.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sg.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://uf.wgjwhj.cn

Ruby: s.count("a")
来源：http://dl.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://qm.szxytkj.cn

[E13] 逐字符遍历
来源：http://fn.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://oa.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ee.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tj.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fn.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hj.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sw.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://en.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mi.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://cx.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rh.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://by.shtwfgs.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lt.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lo.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://si.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cs.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://es.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oe.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://rq.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ft.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oz.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rv.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gp.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dp.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ov.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kj.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uy.wgjwhj.cn

[E16] 数字千分位
来源：http://cf.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://vo.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://bh.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qu.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ko.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dk.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qk.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ra.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://fg.muxihuayi.cn

[E17] 首字母大写
来源：http://vt.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fv.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oh.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://th.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lk.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tu.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://io.9csxet.cn

Ruby: s.capitalize
来源：http://lu.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fx.521024.cn

[E18] 模板占位符替换
来源：http://al.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://to.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wj.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gb.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oa.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kl.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ua.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://da.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gb.asd995.cn

[E19] 多行文本按行拆分
来源：http://hw.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://wt.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rm.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ho.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://sa.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://iz.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://xy.yuntaijiaju.cn

Ruby: s.lines
来源：http://xg.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://kg.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://id.shtwfgs.cn

Py:   if not s:
来源：http://eq.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://le.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qe.wgjwhj.cn

TS:   if (s === "") {}
来源：http://og.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://sj.newstarts.cn

Go:   if s == "" {}
来源：http://ik.9csxet.cn

Ruby: if s.empty?
来源：http://je.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://he.9csxet.cn

[E21] 超长截断加省略号
来源：http://lp.wgjwhj.cn


<!-- 参考信息 -->