代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ia.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qd.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vh.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://xb.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ep.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pi.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ds.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://px.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yq.lnxyls.cn

Go:   // 手写循环
来源：http://jx.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://id.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dh.bookmarksfly.cn

[D15] 去重
来源：http://zu.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://br.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://rj.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://in.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://dy.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vh.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wo.asd995.cn

Ruby: arr.uniq
来源：http://ir.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://fg.shtwfgs.cn

[D16] 求和与平均值
来源：http://ht.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://df.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wd.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ta.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://td.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pc.jctech888.com.cn

Go:   // 手写循环累加
来源：http://yz.521024.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vz.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://oy.shxzukj.cn

[D17] 最大值与最小值
来源：http://rx.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://ws.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://qz.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://as.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://ks.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fi.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ic.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://id.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://wr.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://sn.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sf.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://in.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ju.szxytkj.cn

TS:   nested.flat();
来源：http://zn.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ar.haigaiapp.cn

Go:   // 手写双层循环
来源：http://ia.nszjky.cn

Ruby: nested.flatten
来源：http://by.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wr.bookmarksfly.cn

[D19] 按字段分组
来源：http://dw.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lg.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://en.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tm.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://is.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dt.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://lc.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://po.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ab.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://oh.shxzukj.cn

Py:   Counter(arr)
来源：http://rj.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://ol.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yn.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dk.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tf.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://ag.shxzukj.cn

Ruby: arr.tally
来源：http://vu.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bm.huixiangedu.cn

[D21] 判断是否包含某元素
来源：http://sm.chemitech.net.cn

Py:   x in arr
来源：http://ic.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://yy.newstarts.cn

JS:   arr.includes(x)
来源：http://lp.9csxet.cn

TS:   arr.includes(x)
来源：http://oq.huixinmuqiang.cn

Java: list.contains(x)
来源：http://xa.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://hg.huanxung.cn

Ruby: arr.include?(x)
来源：http://yw.lnxyls.cn

C#:   list.Contains(x)
来源：http://kn.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://az.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hb.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tt.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ux.bjjhwx.cn

TS:   [...arr];
来源：http://kk.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://zf.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://am.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://je.hnjuh.cn

C#:   new List<int>(list);
来源：http://lp.panjiajie.cn

[D23] reduce 累积计算
来源：http://kt.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qa.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hv.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lp.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xx.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ty.wgjwhj.cn

Go:   // 手写循环
来源：http://zd.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yd.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ok.shxzukj.cn

[D24] 字典 / Map 基本操作
来源：http://ns.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oe.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ls.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pp.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wd.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rs.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yv.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qd.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pa.521024.cn

[D25] Set 集合去重与交并差
来源：http://zq.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ei.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lf.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qy.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cy.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cu.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fl.bookmarksfly.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ci.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gl.wgjwhj.cn

[D26] 数组转字符串
来源：http://od.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://nn.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://ae.9csxet.cn

JS:   arr.join(", ")
来源：http://lx.hahajie.cn

TS:   arr.join(", ")
来源：http://kg.colortex.cn

Java: String.join(", ", list)
来源：http://ba.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://vy.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://bh.newstarts.cn

C#:   string.Join(", ", list)
来源：http://ew.hnjuh.cn

================================================================================
来源：http://lh.nszjky.cn

E. 字符串处理
来源：http://wk.jianghongdianzi.cn

================================================================================
来源：http://re.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://xl.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xm.haigaiapp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ws.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bz.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gv.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pf.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://my.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fc.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rc.colortex.cn

[E02] 重复字符串
来源：http://fd.gzmigu.cn

Py:   "ab" * 3
来源：http://pq.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://kw.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://em.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://wl.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ka.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://ny.shxzskj.cn

Ruby: "ab" * 3
来源：http://mb.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qt.hnjuh.cn

[E03] 截取子串
来源：http://lw.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zs.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dp.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bc.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://el.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://qs.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pm.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ju.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://kh.9csxet.cn

[E04] 查找子串位置
来源：http://vh.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://wr.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://he.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vj.szsharing.cn

TS:   s.indexOf("x")
来源：http://qx.chemitech.net.cn

Java: s.indexOf("x")
来源：http://ta.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://ab.huixiangedu.cn

Ruby: s.index("x")
来源：http://mc.hahajie.cn

C#:   s.IndexOf("x")
来源：http://cn.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uq.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cf.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dv.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qb.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sv.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hq.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mw.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xo.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ls.jianghongdianzi.cn

[E06] 替换子串
来源：http://tc.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rm.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://dx.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ck.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://um.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pv.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sb.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ul.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://kt.hnjuh.cn

[E07] 按分隔符拆分
来源：http://sd.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rz.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://et.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ay.gzmigu.cn

TS:   s.split(",")
来源：http://ot.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kb.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iz.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://tr.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vk.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://ii.bookmarksfly.cn

Py:   ",".join(items)
来源：http://xu.nicolike.cn

PHP:  implode(",", $items);
来源：http://yy.gzmigu.cn

JS:   items.join(",")
来源：http://sc.9csxet.cn

TS:   items.join(",")
来源：http://rh.hnjuh.cn

Java: String.join(",", items)
来源：http://ev.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://et.bookmarksfly.cn

Ruby: items.join(",")
来源：http://fl.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://hd.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://lz.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jh.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ie.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://cc.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://lo.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://zk.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pt.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wm.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vf.hahajie.cn

[E10] 左侧补零 / 定长填充
来源：http://ye.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://un.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zo.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://sd.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://fd.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://uw.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qy.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fh.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bd.jctech888.com.cn

[E11] 反转字符串
来源：http://wx.521024.cn

Py:   s[::-1]
来源：http://yw.lnxyls.cn

PHP:  strrev($s);
来源：http://ay.asd995.cn

JS:   [...s].reverse().join("")
来源：http://mn.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://uv.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bb.asd995.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vz.huanxung.cn

Ruby: s.reverse
来源：http://wx.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mv.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://kr.9csxet.cn

Py:   s.count("a")
来源：http://ro.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ri.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://iq.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://bl.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sm.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://nd.bjjhwx.cn

Ruby: s.count("a")
来源：http://gk.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://un.jctech888.com.cn

[E13] 逐字符遍历
来源：http://al.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://nj.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://om.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mc.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ff.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oa.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rm.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pd.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mb.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://rx.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ud.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vy.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sj.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bg.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tt.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lt.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qh.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xw.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://wz.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eh.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qm.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kb.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eu.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cr.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jq.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wu.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fg.shtwfgs.cn

[E16] 数字千分位
来源：http://ca.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://se.shxzskj.cn

PHP:  number_format(1234567);
来源：http://hh.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fl.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ne.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xk.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ge.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gd.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://fs.chemitech.net.cn

[E17] 首字母大写
来源：http://ot.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ff.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mc.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mn.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://np.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ki.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://de.newstarts.cn

Ruby: s.capitalize
来源：http://mx.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pk.huixiangedu.cn

[E18] 模板占位符替换
来源：http://wq.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ay.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tz.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ni.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ld.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qp.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jy.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://om.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wo.521024.cn

[E19] 多行文本按行拆分
来源：http://bv.521024.cn

Py:   s.splitlines()
来源：http://jr.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fn.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://to.521024.cn

TS:   s.split(/\r?\n/)
来源：http://mc.chemitech.net.cn

Java: s.lines().toList()
来源：http://sf.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://sc.shxzskj.cn

Ruby: s.lines
来源：http://wb.newstarts.cn

C#:   s.Split('\n')
来源：http://ut.szsharing.cn

[E20] 判断字符串是否为空
来源：http://wd.muxihuayi.cn

Py:   if not s:
来源：http://kw.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xa.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nx.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://gh.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://cp.9csxet.cn


<!-- 参考信息 -->