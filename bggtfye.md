代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://et.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kv.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://yg.huixinmuqiang.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bs.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jb.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://vl.lnxyls.cn

Py:   Counter(arr)
来源：http://aq.9csxet.cn

PHP:  array_count_values($arr);
来源：http://zt.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fb.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gn.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ly.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://vn.huanxung.cn

Ruby: arr.tally
来源：http://hm.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://db.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://pi.colortex.cn

Py:   x in arr
来源：http://gc.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://hf.asd995.cn

JS:   arr.includes(x)
来源：http://ny.shxzukj.cn

TS:   arr.includes(x)
来源：http://mm.huixiangedu.cn

Java: list.contains(x)
来源：http://ke.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://hn.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://vq.shxzskj.cn

C#:   list.Contains(x)
来源：http://us.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://uj.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zu.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gx.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yl.521024.cn

TS:   [...arr];
来源：http://pv.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://mg.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://na.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://oe.szsharing.cn

C#:   new List<int>(list);
来源：http://va.chemitech.net.cn

[D23] reduce 累积计算
来源：http://pj.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kt.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bb.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bz.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xh.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vl.jianghongdianzi.cn

Go:   // 手写循环
来源：http://ka.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ii.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rd.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://jd.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xb.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kz.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rv.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vy.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bs.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ff.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mt.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ll.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://rp.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://st.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ad.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://si.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fc.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ok.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xr.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dv.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nl.jctech888.com.cn

[D26] 数组转字符串
来源：http://zj.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://iv.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://sj.huanxung.cn

JS:   arr.join(", ")
来源：http://uq.bjjhwx.cn

TS:   arr.join(", ")
来源：http://nt.huixinmuqiang.cn

Java: String.join(", ", list)
来源：http://up.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://cl.shxzukj.cn

Ruby: arr.join(", ")
来源：http://jw.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://zt.jianghongdianzi.cn

================================================================================
来源：http://eo.9csxet.cn

E. 字符串处理
来源：http://dd.nszjky.cn

================================================================================
来源：http://ar.wgjwhj.cn

[E01] 拼接字符串
来源：http://tv.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bp.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://my.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ad.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ay.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fl.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vi.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hq.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnjuh.cn

[E02] 重复字符串
来源：http://zh.jctech888.com.cn

Py:   "ab" * 3
来源：http://dx.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://gh.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://qc.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://ec.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://vf.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://mb.huanxung.cn

Ruby: "ab" * 3
来源：http://wq.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xu.wgjwhj.cn

[E03] 截取子串
来源：http://vw.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ov.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://le.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uv.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://nx.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://vt.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xh.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dt.asd995.cn

C#:   s.Substring(1, 3)
来源：http://tq.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://iq.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://cc.521024.cn

PHP:  strpos($s, "x");
来源：http://ah.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fh.lnxyls.cn

TS:   s.indexOf("x")
来源：http://dl.521024.cn

Java: s.indexOf("x")
来源：http://vd.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://bq.nicolike.cn

Ruby: s.index("x")
来源：http://yt.hahajie.cn

C#:   s.IndexOf("x")
来源：http://lw.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gq.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tu.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wb.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nc.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rh.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dz.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yc.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ql.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vl.hnjuh.cn

[E06] 替换子串
来源：http://rv.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yi.huixiangedu.cn

PHP:  str_replace("a", "b", $s);
来源：http://fs.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fv.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://gh.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zm.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rb.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kn.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://po.nicolike.cn

[E07] 按分隔符拆分
来源：http://gg.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wa.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wf.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bd.jianghongdianzi.cn

TS:   s.split(",")
来源：http://me.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mg.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ze.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://zf.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ua.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://hh.shtwfgs.cn

Py:   ",".join(items)
来源：http://nr.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://tb.haigaiapp.cn

JS:   items.join(",")
来源：http://hw.huanxung.cn

TS:   items.join(",")
来源：http://rs.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://sb.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://rg.lnxyls.cn

Ruby: items.join(",")
来源：http://uv.nicolike.cn

C#:   string.Join(",", items)
来源：http://fe.shxzskj.cn

[E09] 去除所有空白字符
来源：http://xf.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dc.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yh.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://hr.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://no.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://md.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fj.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ds.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uq.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://vv.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vq.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ho.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://sb.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://tu.colortex.cn

Java: String.format("%03d", 7)
来源：http://nl.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fg.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ij.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pa.muxihuayi.cn

[E11] 反转字符串
来源：http://bg.yuntaijiaju.cn

Py:   s[::-1]
来源：http://ou.hahajie.cn

PHP:  strrev($s);
来源：http://rw.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://sf.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://bf.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aw.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xh.shxzskj.cn

Ruby: s.reverse
来源：http://wp.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kz.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://qa.newstarts.cn

Py:   s.count("a")
来源：http://kq.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://ku.huanxung.cn

JS:   s.split("a").length - 1
来源：http://yw.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://jz.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jb.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://je.panjiajie.cn

Ruby: s.count("a")
来源：http://sv.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://iq.bjjhwx.cn

[E13] 逐字符遍历
来源：http://kn.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://fk.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jd.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://at.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wz.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://di.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sm.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ol.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jf.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://lj.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://po.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fy.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vz.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ol.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ve.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wy.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yy.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oz.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://kn.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cl.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fx.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lo.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mq.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kl.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dx.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tj.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pj.yuexingan06.cn

[E16] 数字千分位
来源：http://pa.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://np.szsharing.cn

PHP:  number_format(1234567);
来源：http://dh.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kz.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xt.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ph.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nv.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vq.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://tv.hahajie.cn

[E17] 首字母大写
来源：http://ra.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ar.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dj.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zq.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bf.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ub.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kl.muxihuayi.cn

Ruby: s.capitalize
来源：http://iq.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bn.wgjwhj.cn

[E18] 模板占位符替换
来源：http://cd.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ni.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yq.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qk.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vh.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pe.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oj.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kx.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zf.colortex.cn

[E19] 多行文本按行拆分
来源：http://mf.newstarts.cn

Py:   s.splitlines()
来源：http://gg.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eb.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://gt.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://sg.lnxyls.cn

Java: s.lines().toList()
来源：http://vu.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://bk.chemitech.net.cn

Ruby: s.lines
来源：http://uk.lnxyls.cn

C#:   s.Split('\n')
来源：http://hu.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://zo.bjjhwx.cn

Py:   if not s:
来源：http://ea.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zm.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ls.newstarts.cn

TS:   if (s === "") {}
来源：http://dh.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://eu.muxihuayi.cn

Go:   if s == "" {}
来源：http://fp.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://cs.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zx.asd995.cn

[E21] 超长截断加省略号
来源：http://st.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xr.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lo.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fq.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ps.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dd.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ct.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iw.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nu.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://ja.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jo.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ig.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://go.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pu.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pe.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bd.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://mx.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wo.huixinmuqiang.cn

================================================================================
来源：http://qb.huixiangedu.cn

F. 文件与目录
来源：http://yq.shtwfgs.cn

================================================================================
来源：http://sz.521024.cn

[F01] 读取整个文件
来源：http://dw.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kp.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://tx.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bx.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sr.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sp.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sw.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://oq.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://he.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://wd.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sn.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dn.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ng.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pw.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cm.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oi.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fi.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hb.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://fa.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ya.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jv.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pg.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hc.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ek.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xf.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://ap.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ik.szsharing.cn

[F04] 追加写入文件
来源：http://kt.jianghongdianzi.cn


<!-- 参考信息 -->