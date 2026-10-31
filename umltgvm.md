代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://va.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vs.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ev.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://oj.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oo.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tz.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://pn.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://uk.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ew.gzmigu.cn

Go:   // 手写循环
来源：http://kb.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qh.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nl.szsharing.cn

[D15] 去重
来源：http://cw.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ay.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://gg.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://om.asd995.cn

TS:   [...new Set(arr)]
来源：http://ks.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://df.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tb.hahajie.cn

Ruby: arr.uniq
来源：http://xx.asd995.cn

C#:   list.Distinct().ToList()
来源：http://fk.huixiangedu.cn

[D16] 求和与平均值
来源：http://tw.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ur.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rt.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zu.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yt.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://br.hnjuh.cn

Go:   // 手写循环累加
来源：http://sx.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ee.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://jy.szsharing.cn

[D17] 最大值与最小值
来源：http://wm.521024.cn

Py:   max(arr);  min(arr)
来源：http://ok.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://gw.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hp.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://bz.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zg.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wv.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://jz.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://bh.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://jl.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tj.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://lo.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gz.9csxet.cn

TS:   nested.flat();
来源：http://qt.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sq.panjiajie.cn

Go:   // 手写双层循环
来源：http://rb.9csxet.cn

Ruby: nested.flatten
来源：http://nm.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lz.jianghongdianzi.cn

[D19] 按字段分组
来源：http://jf.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vz.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mp.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kc.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eh.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://iz.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pp.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yx.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://nv.9csxet.cn

Py:   Counter(arr)
来源：http://tr.newstarts.cn

PHP:  array_count_values($arr);
来源：http://vc.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bz.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bt.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lp.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://rh.shxzskj.cn

Ruby: arr.tally
来源：http://uf.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fe.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://up.bookmarksfly.cn

Py:   x in arr
来源：http://yz.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://bh.yuexingan06.cn

JS:   arr.includes(x)
来源：http://me.wgjwhj.cn

TS:   arr.includes(x)
来源：http://gj.shtwfgs.cn

Java: list.contains(x)
来源：http://gt.521024.cn

Go:   slices.Contains(arr, x)
来源：http://yk.colortex.cn

Ruby: arr.include?(x)
来源：http://hj.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://fq.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://nw.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sd.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gq.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://do.jctech888.com.cn

TS:   [...arr];
来源：http://se.huixinmuqiang.cn

Java: new ArrayList<>(list);
来源：http://kr.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tb.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://ho.gzmigu.cn

C#:   new List<int>(list);
来源：http://fy.hnjuh.cn

[D23] reduce 累积计算
来源：http://pn.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ca.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bt.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lz.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qd.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ev.shxzskj.cn

Go:   // 手写循环
来源：http://np.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cb.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://at.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://qh.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oc.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eg.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://og.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mq.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vf.yuexingan06.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://in.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lt.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://af.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://mz.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rj.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yo.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://br.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ue.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gg.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qv.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ot.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pu.asd995.cn

[D26] 数组转字符串
来源：http://gt.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://rw.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://sm.hahajie.cn

JS:   arr.join(", ")
来源：http://wn.asd995.cn

TS:   arr.join(", ")
来源：http://xm.gzmigu.cn

Java: String.join(", ", list)
来源：http://ry.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://dw.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://lb.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://uf.yuntaijiaju.cn

================================================================================
来源：http://ig.jctech888.com.cn

E. 字符串处理
来源：http://up.muxihuayi.cn

================================================================================
来源：http://sl.nicolike.cn

[E01] 拼接字符串
来源：http://ek.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ej.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wh.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pm.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pe.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hm.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ja.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qv.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eg.wgjwhj.cn

[E02] 重复字符串
来源：http://yq.asd995.cn

Py:   "ab" * 3
来源：http://mh.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://kx.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://ef.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://vl.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://yy.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://sn.asd995.cn

Ruby: "ab" * 3
来源：http://up.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qa.shxzukj.cn

[E03] 截取子串
来源：http://io.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cl.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rl.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://re.9csxet.cn

TS:   s.slice(1, 4)
来源：http://cu.colortex.cn

Java: s.substring(1, 4)
来源：http://nj.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://og.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uy.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://ix.shxzskj.cn

[E04] 查找子串位置
来源：http://au.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://pb.huanxung.cn

PHP:  strpos($s, "x");
来源：http://qg.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dl.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://wa.panjiajie.cn

Java: s.indexOf("x")
来源：http://lt.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://ji.chemitech.net.cn

Ruby: s.index("x")
来源：http://ud.newstarts.cn

C#:   s.IndexOf("x")
来源：http://ta.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pe.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ed.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ve.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gl.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gt.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://la.colortex.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vr.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://av.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ef.jctech888.com.cn

[E06] 替换子串
来源：http://jg.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bi.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://pp.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lw.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://cg.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vd.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://li.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ad.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://wl.szsharing.cn

[E07] 按分隔符拆分
来源：http://gk.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wr.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fc.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qg.panjiajie.cn

TS:   s.split(",")
来源：http://lo.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mm.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wb.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://nf.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jv.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://ib.newstarts.cn

Py:   ",".join(items)
来源：http://tb.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://gk.szsharing.cn

JS:   items.join(",")
来源：http://se.gzmigu.cn

TS:   items.join(",")
来源：http://va.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://oc.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://sb.bjjhwx.cn

Ruby: items.join(",")
来源：http://zk.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://ku.shxzskj.cn

[E09] 去除所有空白字符
来源：http://mq.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wt.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wi.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://vu.chemitech.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://rh.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://ht.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qo.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ai.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oh.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://sl.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cp.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mh.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://sm.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://bb.nszjky.cn

Java: String.format("%03d", 7)
来源：http://fm.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aj.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ep.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qg.panjiajie.cn

[E11] 反转字符串
来源：http://xl.newstarts.cn

Py:   s[::-1]
来源：http://un.chemitech.net.cn

PHP:  strrev($s);
来源：http://ff.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://yw.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://to.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ke.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cr.hahajie.cn

Ruby: s.reverse
来源：http://ke.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://il.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://le.bookmarksfly.cn

Py:   s.count("a")
来源：http://ko.asd995.cn

PHP:  substr_count($s, "a");
来源：http://lg.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://gj.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://cw.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ng.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://un.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://rp.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://vh.nicolike.cn

[E13] 逐字符遍历
来源：http://dc.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://bb.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oc.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hj.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mw.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ta.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pe.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wo.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nr.asd995.cn

[E14] URL 编码与 Base64
来源：http://oe.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ke.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eg.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rb.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ec.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wx.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://up.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xa.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ii.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://ly.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pw.newstarts.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uc.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xc.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://da.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kv.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wp.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ks.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://st.shxzukj.cn

[E16] 数字千分位
来源：http://dl.nszjky.cn

Py:   f"{1234567:,}"
来源：http://jh.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://zw.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ly.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://np.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ui.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ve.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fn.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://wd.jianghongdianzi.cn

[E17] 首字母大写
来源：http://hq.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bn.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ws.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vv.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ij.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zq.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kf.shxzukj.cn

Ruby: s.capitalize
来源：http://uo.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wj.asd995.cn

[E18] 模板占位符替换
来源：http://cc.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lz.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mb.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xl.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lu.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tl.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fx.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oz.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rd.newstarts.cn

[E19] 多行文本按行拆分
来源：http://lz.huanxung.cn

Py:   s.splitlines()
来源：http://kf.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ub.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://bn.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://zs.shxzskj.cn

Java: s.lines().toList()
来源：http://zf.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://ey.hahajie.cn

Ruby: s.lines
来源：http://vb.shtwfgs.cn

C#:   s.Split('\n')
来源：http://zf.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://uw.bookmarksfly.cn

Py:   if not s:
来源：http://st.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://of.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gd.panjiajie.cn

TS:   if (s === "") {}
来源：http://cr.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://xw.panjiajie.cn


<!-- 参考信息 -->