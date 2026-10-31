代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lj.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://jz.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sk.newstarts.cn

TS:   nested.flat();
来源：http://eq.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yk.shtwfgs.cn

Go:   // 手写双层循环
来源：http://eu.haigaiapp.cn

Ruby: nested.flatten
来源：http://ep.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yq.lnxyls.cn

[D19] 按字段分组
来源：http://cy.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rd.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pn.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wk.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rb.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://os.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://qv.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://so.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zr.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://lp.huixiangedu.cn

Py:   Counter(arr)
来源：http://wp.bjjhwx.cn

PHP:  array_count_values($arr);
来源：http://ut.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mh.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ya.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xj.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://dy.shxzskj.cn

Ruby: arr.tally
来源：http://vz.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ly.huanxung.cn

[D21] 判断是否包含某元素
来源：http://ge.huixinmuqiang.cn

Py:   x in arr
来源：http://tv.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://jk.chemitech.net.cn

JS:   arr.includes(x)
来源：http://qc.yuexingan06.cn

TS:   arr.includes(x)
来源：http://mn.muxihuayi.cn

Java: list.contains(x)
来源：http://rl.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://rt.huanxung.cn

Ruby: arr.include?(x)
来源：http://wq.haigaiapp.cn

C#:   list.Contains(x)
来源：http://jh.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://yu.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hx.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oh.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ev.newstarts.cn

TS:   [...arr];
来源：http://ul.9csxet.cn

Java: new ArrayList<>(list);
来源：http://py.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oa.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://ur.chemitech.net.cn

C#:   new List<int>(list);
来源：http://ls.9csxet.cn

[D23] reduce 累积计算
来源：http://dp.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ou.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ry.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yi.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pb.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qy.huixinmuqiang.cn

Go:   // 手写循环
来源：http://fm.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qr.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iw.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://mk.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mu.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ka.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wi.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ze.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vm.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pd.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ep.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ms.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://eh.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kg.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ll.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uo.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ic.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://re.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mx.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://df.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://re.nszjky.cn

[D26] 数组转字符串
来源：http://xh.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ei.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://te.yuexingan06.cn

JS:   arr.join(", ")
来源：http://xp.shtwfgs.cn

TS:   arr.join(", ")
来源：http://lz.szxytkj.cn

Java: String.join(", ", list)
来源：http://uf.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://pv.lnxyls.cn

Ruby: arr.join(", ")
来源：http://ne.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://md.nszjky.cn

================================================================================
来源：http://vp.chemitech.net.cn

E. 字符串处理
来源：http://fc.lnxyls.cn

================================================================================
来源：http://mr.shxzukj.cn

[E01] 拼接字符串
来源：http://lz.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rn.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rw.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xj.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sx.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nz.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://op.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dj.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://op.szxytkj.cn

[E02] 重复字符串
来源：http://mv.lnxyls.cn

Py:   "ab" * 3
来源：http://pz.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://wm.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://vl.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://wz.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://ap.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://sn.9csxet.cn

Ruby: "ab" * 3
来源：http://kx.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cf.lnxyls.cn

[E03] 截取子串
来源：http://fe.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xv.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zy.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ah.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://ke.hnjuh.cn

Java: s.substring(1, 4)
来源：http://rc.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ug.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xp.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://kq.shtwfgs.cn

[E04] 查找子串位置
来源：http://hx.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://ek.huixiangedu.cn

PHP:  strpos($s, "x");
来源：http://sf.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://va.colortex.cn

TS:   s.indexOf("x")
来源：http://jl.jctech888.com.cn

Java: s.indexOf("x")
来源：http://dh.521024.cn

Go:   strings.Index(s, "x")
来源：http://na.bookmarksfly.cn

Ruby: s.index("x")
来源：http://ye.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://xy.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vg.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xf.szxytkj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fv.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ox.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qw.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ri.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kw.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qr.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hc.bjjhwx.cn

[E06] 替换子串
来源：http://wz.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fd.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://lv.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kz.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://aa.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mi.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ba.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zk.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://mt.szsharing.cn

[E07] 按分隔符拆分
来源：http://dw.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sq.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cm.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://za.shxzskj.cn

TS:   s.split(",")
来源：http://nb.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rv.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qi.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://wx.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ul.nszjky.cn

[E08] 数组按分隔符合并
来源：http://vq.szxytkj.cn

Py:   ",".join(items)
来源：http://tk.panjiajie.cn

PHP:  implode(",", $items);
来源：http://kd.szxytkj.cn

JS:   items.join(",")
来源：http://an.hahajie.cn

TS:   items.join(",")
来源：http://wx.yuexingan06.cn

Java: String.join(",", items)
来源：http://nt.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://dr.haigaiapp.cn

Ruby: items.join(",")
来源：http://tl.nszjky.cn

C#:   string.Join(",", items)
来源：http://sk.hahajie.cn

[E09] 去除所有空白字符
来源：http://rf.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jc.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://si.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://rj.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://mb.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://nx.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kd.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jq.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://da.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://wg.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cj.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uo.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://ta.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://fv.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://sa.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dl.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wz.szxytkj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yv.shtwfgs.cn

[E11] 反转字符串
来源：http://ua.gzmigu.cn

Py:   s[::-1]
来源：http://fi.szxytkj.cn

PHP:  strrev($s);
来源：http://ot.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://wp.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://lm.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wn.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qx.huixinmuqiang.cn

Ruby: s.reverse
来源：http://hi.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ud.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://yo.9csxet.cn

Py:   s.count("a")
来源：http://el.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://mz.521024.cn

JS:   s.split("a").length - 1
来源：http://sg.521024.cn

TS:   s.split("a").length - 1
来源：http://tz.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xw.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://oc.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://lb.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://ne.huixiangedu.cn

[E13] 逐字符遍历
来源：http://bm.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://js.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://us.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ah.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sj.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nz.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uf.wgjwhj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pu.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nk.huixinmuqiang.cn

[E14] URL 编码与 Base64
来源：http://bt.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sr.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ps.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oz.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mt.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fl.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mj.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rs.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vy.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://iq.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rn.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nu.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ib.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pe.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zh.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://he.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fb.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ez.bjjhwx.cn

[E16] 数字千分位
来源：http://bc.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://rj.lnxyls.cn

PHP:  number_format(1234567);
来源：http://ua.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ss.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://af.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ju.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bq.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mj.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://vt.9csxet.cn

[E17] 首字母大写
来源：http://no.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uq.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ez.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mh.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xy.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tw.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gy.gzmigu.cn

Ruby: s.capitalize
来源：http://an.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bd.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://le.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vj.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rt.shxzukj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pf.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ws.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rf.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ur.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xp.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://py.szxytkj.cn

[E19] 多行文本按行拆分
来源：http://wc.hahajie.cn

Py:   s.splitlines()
来源：http://bn.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ny.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://hr.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ww.muxihuayi.cn

Java: s.lines().toList()
来源：http://ok.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://if.bookmarksfly.cn

Ruby: s.lines
来源：http://bv.asd995.cn

C#:   s.Split('\n')
来源：http://eq.9csxet.cn

[E20] 判断字符串是否为空
来源：http://mz.gzmigu.cn

Py:   if not s:
来源：http://ew.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gl.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ga.shxzukj.cn

TS:   if (s === "") {}
来源：http://cg.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://ul.szsharing.cn

Go:   if s == "" {}
来源：http://io.521024.cn

Ruby: if s.empty?
来源：http://pn.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yb.gzmigu.cn

[E21] 超长截断加省略号
来源：http://eo.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mt.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mm.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cj.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fh.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gk.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://ea.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://td.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kh.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ct.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://za.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yg.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bt.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ug.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mq.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ed.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://fv.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gk.huixiangedu.cn

================================================================================
来源：http://op.szxytkj.cn

F. 文件与目录
来源：http://ng.huanxung.cn

================================================================================
来源：http://ub.shxzukj.cn

[F01] 读取整个文件
来源：http://vb.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kc.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://tk.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mv.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://im.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hg.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://re.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://xo.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://cw.szsharing.cn

[F02] 逐行读取文件
来源：http://fj.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ud.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xt.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yn.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pl.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vn.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tf.wgjwhj.cn


<!-- 参考信息 -->