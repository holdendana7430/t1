代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://at.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cb.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ex.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://ng.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lt.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hl.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://uj.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://at.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zp.huanxung.cn

Go:   // 手写循环
来源：http://yt.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hj.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://va.szsharing.cn

[D15] 去重
来源：http://ut.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ib.asd995.cn

PHP:  array_unique($arr);
来源：http://bn.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://qp.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://xk.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cw.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yg.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://zf.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://kp.szxytkj.cn

[D16] 求和与平均值
来源：http://uj.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tu.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qp.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ok.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vl.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://od.nszjky.cn

Go:   // 手写循环累加
来源：http://xf.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://td.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://zx.huixiangedu.cn

[D17] 最大值与最小值
来源：http://pf.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://fp.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://yw.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mh.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://ca.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://as.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bd.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://ub.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://gf.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://vi.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://le.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://vw.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wj.hnjuh.cn

TS:   nested.flat();
来源：http://ap.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://it.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://mw.shxzskj.cn

Ruby: nested.flatten
来源：http://zp.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ty.colortex.cn

[D19] 按字段分组
来源：http://cc.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sp.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ng.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aa.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://la.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yk.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://wk.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mg.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wp.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://af.shtwfgs.cn

Py:   Counter(arr)
来源：http://td.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://ho.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dw.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ai.hahajie.cn

Go:   // 手写 map[T]int
来源：http://qf.gzmigu.cn

Ruby: arr.tally
来源：http://fa.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tn.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://ma.muxihuayi.cn

Py:   x in arr
来源：http://hy.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://cn.wgjwhj.cn

JS:   arr.includes(x)
来源：http://nx.wgjwhj.cn

TS:   arr.includes(x)
来源：http://tq.szxytkj.cn

Java: list.contains(x)
来源：http://iq.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://un.521024.cn

Ruby: arr.include?(x)
来源：http://pk.bjjhwx.cn

C#:   list.Contains(x)
来源：http://yn.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://sg.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fb.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bp.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9csxet.cn

TS:   [...arr];
来源：http://gn.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://hr.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://co.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://nu.huanxung.cn

C#:   new List<int>(list);
来源：http://sn.huanxung.cn

[D23] reduce 累积计算
来源：http://wm.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nz.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fi.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://en.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hu.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rh.9csxet.cn

Go:   // 手写循环
来源：http://ix.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pd.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lb.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://wx.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bq.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dw.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ny.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pn.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fz.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ql.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ym.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pj.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://eb.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://be.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vf.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pl.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tx.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ij.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uu.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zi.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hx.huanxung.cn

[D26] 数组转字符串
来源：http://lc.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://bv.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://cm.yuexingan06.cn

JS:   arr.join(", ")
来源：http://sa.huanxung.cn

TS:   arr.join(", ")
来源：http://wl.wgjwhj.cn

Java: String.join(", ", list)
来源：http://oi.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://ur.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://tv.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://bn.jianghongdianzi.cn

================================================================================
来源：http://tz.colortex.cn

E. 字符串处理
来源：http://il.hnjuh.cn

================================================================================
来源：http://lk.shtwfgs.cn

[E01] 拼接字符串
来源：http://ns.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://so.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vb.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fa.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eb.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kc.szsharing.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xx.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xx.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vh.yuexingan06.cn

[E02] 重复字符串
来源：http://zm.newstarts.cn

Py:   "ab" * 3
来源：http://ys.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://du.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://wf.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://df.gzmigu.cn

Java: "ab".repeat(3)
来源：http://pq.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://np.521024.cn

Ruby: "ab" * 3
来源：http://bt.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vz.lnxyls.cn

[E03] 截取子串
来源：http://ou.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://os.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gv.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fu.szsharing.cn

TS:   s.slice(1, 4)
来源：http://mo.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://po.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lz.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ik.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://gt.shxzukj.cn

[E04] 查找子串位置
来源：http://sp.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://zm.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://lb.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vq.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://yn.newstarts.cn

Java: s.indexOf("x")
来源：http://kv.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://vk.yuexingan06.cn

Ruby: s.index("x")
来源：http://pa.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://fe.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qe.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://om.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fu.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tu.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ls.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nv.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gj.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jf.hnjuh.cn

[E06] 替换子串
来源：http://hz.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wh.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://eu.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bc.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://ef.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sc.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pt.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yp.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://kz.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://kd.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oj.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qc.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nx.huanxung.cn

TS:   s.split(",")
来源：http://xw.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://st.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://md.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://eb.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ai.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://dd.9csxet.cn

Py:   ",".join(items)
来源：http://ry.hnjuh.cn

PHP:  implode(",", $items);
来源：http://bk.9csxet.cn

JS:   items.join(",")
来源：http://ln.newstarts.cn

TS:   items.join(",")
来源：http://pz.haigaiapp.cn

Java: String.join(",", items)
来源：http://du.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://ut.shtwfgs.cn

Ruby: items.join(",")
来源：http://sg.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://fz.panjiajie.cn

[E09] 去除所有空白字符
来源：http://wx.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ca.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ql.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://qe.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://us.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://to.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ez.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pe.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uh.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://gb.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hd.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qn.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://yy.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://gk.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://sv.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tf.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ui.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bi.lnxyls.cn

[E11] 反转字符串
来源：http://cf.9csxet.cn

Py:   s[::-1]
来源：http://wi.521024.cn

PHP:  strrev($s);
来源：http://xh.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://zu.colortex.cn

TS:   [...s].reverse().join("")
来源：http://vu.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ut.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ne.newstarts.cn

Ruby: s.reverse
来源：http://rd.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ly.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://xk.nicolike.cn

Py:   s.count("a")
来源：http://yv.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://sc.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://vp.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://kd.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qa.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://wc.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://tl.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://hw.huanxung.cn

[E13] 逐字符遍历
来源：http://pp.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://gr.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zs.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qi.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pz.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ow.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zs.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dv.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lr.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://np.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ls.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kd.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ek.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xx.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fw.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ai.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ad.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://de.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://kr.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hq.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nz.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xz.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dr.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eb.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bv.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lr.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ib.shxzukj.cn

[E16] 数字千分位
来源：http://ji.szsharing.cn

Py:   f"{1234567:,}"
来源：http://bd.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://lo.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ag.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nb.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qd.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ci.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://se.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://ko.huixinmuqiang.cn

[E17] 首字母大写
来源：http://rj.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qd.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://my.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ys.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://th.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vs.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iv.gzmigu.cn

Ruby: s.capitalize
来源：http://lt.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jg.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://tt.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lk.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jb.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dr.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zm.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tf.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sf.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://np.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ww.huanxung.cn

[E19] 多行文本按行拆分
来源：http://bp.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://ui.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ef.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://mv.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://tq.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://mv.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://nv.muxihuayi.cn

Ruby: s.lines
来源：http://kt.asd995.cn

C#:   s.Split('\n')
来源：http://qd.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://gr.muxihuayi.cn

Py:   if not s:
来源：http://uk.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zm.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yq.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://ya.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://mn.szxytkj.cn


<!-- 参考信息 -->