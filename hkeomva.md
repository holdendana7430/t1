代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ob.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://hw.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://cm.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tb.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://og.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lr.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xw.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://ti.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wy.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tw.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://qo.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://ct.shxzukj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cr.panjiajie.cn

Go:   // 手写循环
来源：http://ax.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bl.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://so.nicolike.cn

[D15] 去重
来源：http://gr.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bk.newstarts.cn

PHP:  array_unique($arr);
来源：http://yv.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://nm.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://bo.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ry.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rl.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://qn.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://ih.hnjuh.cn

[D16] 求和与平均值
来源：http://rh.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oq.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wc.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vg.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hm.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ks.shtwfgs.cn

Go:   // 手写循环累加
来源：http://kx.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://or.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://ym.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://ji.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://at.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://ed.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ci.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://cq.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mx.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vt.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://om.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://zh.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://zm.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tz.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://un.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ur.asd995.cn

TS:   nested.flat();
来源：http://mq.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qc.panjiajie.cn

Go:   // 手写双层循环
来源：http://ot.shxzskj.cn

Ruby: nested.flatten
来源：http://mb.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wk.huixinmuqiang.cn

[D19] 按字段分组
来源：http://sg.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sk.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tw.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uc.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://az.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qm.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://kh.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vs.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xv.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://rw.shxzukj.cn

Py:   Counter(arr)
来源：http://gm.nszjky.cn

PHP:  array_count_values($arr);
来源：http://qu.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vj.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gx.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pp.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://pb.jianghongdianzi.cn

Ruby: arr.tally
来源：http://rs.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vy.huanxung.cn

[D21] 判断是否包含某元素
来源：http://wx.jianghongdianzi.cn

Py:   x in arr
来源：http://hv.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://gq.shxzukj.cn

JS:   arr.includes(x)
来源：http://fm.szxytkj.cn

TS:   arr.includes(x)
来源：http://xs.szsharing.cn

Java: list.contains(x)
来源：http://vq.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://fb.colortex.cn

Ruby: arr.include?(x)
来源：http://jv.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://xu.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://vy.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fw.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lb.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fh.jctech888.com.cn

TS:   [...arr];
来源：http://cv.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://ez.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lu.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://gc.yuntaijiaju.cn

C#:   new List<int>(list);
来源：http://dj.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://te.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gz.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dm.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hs.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ig.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ao.szsharing.cn

Go:   // 手写循环
来源：http://pd.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ct.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vq.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://rg.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hm.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://md.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://le.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bu.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://de.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mz.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iv.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lb.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://lm.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vt.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kh.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zm.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yi.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://na.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://up.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wp.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mx.chemitech.net.cn

[D26] 数组转字符串
来源：http://dh.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://pf.bookmarksfly.cn

PHP:  implode(", ", $arr);
来源：http://sb.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://bb.huixiangedu.cn

TS:   arr.join(", ")
来源：http://ok.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://od.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://zm.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://hb.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://hk.lnxyls.cn

================================================================================
来源：http://nk.huixinmuqiang.cn

E. 字符串处理
来源：http://cd.muxihuayi.cn

================================================================================
来源：http://ok.wgjwhj.cn

[E01] 拼接字符串
来源：http://mf.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lz.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sn.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vc.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tk.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tg.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qr.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rl.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zk.shxzskj.cn

[E02] 重复字符串
来源：http://wn.haigaiapp.cn

Py:   "ab" * 3
来源：http://un.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://mk.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://fz.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://dp.hnjuh.cn

Java: "ab".repeat(3)
来源：http://wd.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://ry.shtwfgs.cn

Ruby: "ab" * 3
来源：http://to.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ed.szsharing.cn

[E03] 截取子串
来源：http://mv.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bm.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ds.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fp.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://tg.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://rg.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zo.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cb.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://vj.shxzskj.cn

[E04] 查找子串位置
来源：http://fs.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://ir.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://ye.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://er.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://np.yuexingan06.cn

Java: s.indexOf("x")
来源：http://ja.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://dc.shxzukj.cn

Ruby: s.index("x")
来源：http://yv.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://xe.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ha.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oc.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kq.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cz.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tq.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ww.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ej.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ik.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://em.muxihuayi.cn

[E06] 替换子串
来源：http://kq.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uv.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://mv.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hf.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://hd.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mv.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vt.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tb.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ps.hahajie.cn

[E07] 按分隔符拆分
来源：http://gs.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oc.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mf.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mc.jctech888.com.cn

TS:   s.split(",")
来源：http://nd.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ej.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xk.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://xv.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xq.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://vu.muxihuayi.cn

Py:   ",".join(items)
来源：http://br.szxytkj.cn

PHP:  implode(",", $items);
来源：http://qy.huanxung.cn

JS:   items.join(",")
来源：http://md.asd995.cn

TS:   items.join(",")
来源：http://uj.szsharing.cn

Java: String.join(",", items)
来源：http://dd.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://ft.szsharing.cn

Ruby: items.join(",")
来源：http://ac.gzmigu.cn

C#:   string.Join(",", items)
来源：http://ud.hahajie.cn

[E09] 去除所有空白字符
来源：http://dm.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pb.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ah.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://kc.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://ex.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://vq.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sd.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tw.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://or.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://tq.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ls.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pc.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://hf.521024.cn

TS:   "7".padStart(3, "0")
来源：http://dm.521024.cn

Java: String.format("%03d", 7)
来源：http://gt.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dy.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fo.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ao.huixiangedu.cn

[E11] 反转字符串
来源：http://ec.asd995.cn

Py:   s[::-1]
来源：http://yt.521024.cn

PHP:  strrev($s);
来源：http://co.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://cm.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://fd.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vd.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gi.nicolike.cn

Ruby: s.reverse
来源：http://cj.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zi.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://vq.panjiajie.cn

Py:   s.count("a")
来源：http://bo.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://st.9csxet.cn

JS:   s.split("a").length - 1
来源：http://pu.hahajie.cn

TS:   s.split("a").length - 1
来源：http://jf.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uo.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://xm.chemitech.net.cn

Ruby: s.count("a")
来源：http://bt.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://xf.huixiangedu.cn

[E13] 逐字符遍历
来源：http://yp.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://ba.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rv.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://az.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ky.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sx.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vq.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pl.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fj.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://nr.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kg.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aa.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ux.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kn.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fv.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oi.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jt.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gc.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://fk.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tw.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iw.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oi.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aa.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sg.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hw.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ic.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hd.shxzskj.cn

[E16] 数字千分位
来源：http://iu.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://ri.hnjuh.cn

PHP:  number_format(1234567);
来源：http://ya.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vo.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yn.huixiangedu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hm.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hp.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gd.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://ka.shxzukj.cn

[E17] 首字母大写
来源：http://ya.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fj.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oe.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gu.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xc.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wv.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fi.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://jw.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sy.shxzukj.cn

[E18] 模板占位符替换
来源：http://mv.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ur.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vo.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jz.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gv.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hv.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qb.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qf.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ig.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://aa.panjiajie.cn

Py:   s.splitlines()
来源：http://fx.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vm.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://si.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://xm.szxytkj.cn

Java: s.lines().toList()
来源：http://zv.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ap.asd995.cn

Ruby: s.lines
来源：http://co.huixiangedu.cn

C#:   s.Split('\n')
来源：http://bu.521024.cn

[E20] 判断字符串是否为空
来源：http://ru.gzmigu.cn

Py:   if not s:
来源：http://zu.huixiangedu.cn


<!-- 参考信息 -->