代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://va.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rj.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sb.newstarts.cn

Go:   // 手写 map[T]int
来源：http://vm.chemitech.net.cn

Ruby: arr.tally
来源：http://hx.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ni.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://xm.521024.cn

Py:   x in arr
来源：http://xu.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://gp.szxytkj.cn

JS:   arr.includes(x)
来源：http://wo.shxzskj.cn

TS:   arr.includes(x)
来源：http://yv.panjiajie.cn

Java: list.contains(x)
来源：http://jg.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://pe.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://wk.lnxyls.cn

C#:   list.Contains(x)
来源：http://bk.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://yh.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gw.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://go.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xi.hnjuh.cn

TS:   [...arr];
来源：http://qd.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://jp.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bu.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://no.shtwfgs.cn

C#:   new List<int>(list);
来源：http://tu.muxihuayi.cn

[D23] reduce 累积计算
来源：http://sg.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ql.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nz.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ex.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cq.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rq.hahajie.cn

Go:   // 手写循环
来源：http://et.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hv.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://er.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://wg.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yy.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lq.huixinmuqiang.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bf.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qe.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tp.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eb.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rh.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tg.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://cd.panjiajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nl.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bg.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ma.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cs.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jj.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hk.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xo.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://er.nszjky.cn

[D26] 数组转字符串
来源：http://an.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://nb.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://hw.colortex.cn

JS:   arr.join(", ")
来源：http://bc.gzmigu.cn

TS:   arr.join(", ")
来源：http://mo.panjiajie.cn

Java: String.join(", ", list)
来源：http://fr.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://lt.9csxet.cn

Ruby: arr.join(", ")
来源：http://po.huanxung.cn

C#:   string.Join(", ", list)
来源：http://qo.huanxung.cn

================================================================================
来源：http://gq.nszjky.cn

E. 字符串处理
来源：http://fw.shxzskj.cn

================================================================================
来源：http://pw.bookmarksfly.cn

[E01] 拼接字符串
来源：http://od.shtwfgs.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mq.huixiangedu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iw.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mv.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jc.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vu.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zl.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ta.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ku.chemitech.net.cn

[E02] 重复字符串
来源：http://nk.asd995.cn

Py:   "ab" * 3
来源：http://mc.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://wv.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://ie.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://zg.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://me.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://lu.yuexingan06.cn

Ruby: "ab" * 3
来源：http://xf.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wp.nszjky.cn

[E03] 截取子串
来源：http://yc.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gt.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yi.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zg.newstarts.cn

TS:   s.slice(1, 4)
来源：http://yb.hahajie.cn

Java: s.substring(1, 4)
来源：http://zv.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://av.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yf.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://gp.chemitech.net.cn

[E04] 查找子串位置
来源：http://to.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://fj.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://nm.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ba.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://qi.hnjuh.cn

Java: s.indexOf("x")
来源：http://rs.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://cl.colortex.cn

Ruby: s.index("x")
来源：http://zy.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://yk.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hf.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hj.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wy.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ui.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vc.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://st.szsharing.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ly.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jr.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hd.muxihuayi.cn

[E06] 替换子串
来源：http://dt.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sq.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://io.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dw.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://fz.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vd.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jz.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vz.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://ig.9csxet.cn

[E07] 按分隔符拆分
来源：http://qw.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ya.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dr.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ep.lnxyls.cn

TS:   s.split(",")
来源：http://qo.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mn.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ph.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://mh.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uk.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://im.9csxet.cn

Py:   ",".join(items)
来源：http://gt.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://gf.wgjwhj.cn

JS:   items.join(",")
来源：http://xs.gzmigu.cn

TS:   items.join(",")
来源：http://zc.szxytkj.cn

Java: String.join(",", items)
来源：http://ba.asd995.cn

Go:   strings.Join(items, ",")
来源：http://wh.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://ja.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://iz.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://io.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vr.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yg.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://ds.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://lu.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://cn.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fw.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vf.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yz.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ob.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ow.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ai.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://gy.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://ay.521024.cn

Java: String.format("%03d", 7)
来源：http://bz.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pj.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sb.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lw.gzmigu.cn

[E11] 反转字符串
来源：http://rl.chemitech.net.cn

Py:   s[::-1]
来源：http://ks.yuexingan06.cn

PHP:  strrev($s);
来源：http://qp.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://cu.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://yo.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sv.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qk.yuexingan06.cn

Ruby: s.reverse
来源：http://ll.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rn.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://gc.jianghongdianzi.cn

Py:   s.count("a")
来源：http://xn.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://ok.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://rp.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://sx.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pe.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://uq.hnjuh.cn

Ruby: s.count("a")
来源：http://dw.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://oz.huanxung.cn

[E13] 逐字符遍历
来源：http://fo.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://ba.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://no.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cb.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dd.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ky.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ul.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xc.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qg.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://wp.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kn.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nt.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kt.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://og.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dj.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://na.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://af.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wd.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://dm.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sj.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ni.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lp.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ur.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fs.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cf.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://io.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ve.hahajie.cn

[E16] 数字千分位
来源：http://ct.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://ck.asd995.cn

PHP:  number_format(1234567);
来源：http://jq.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hn.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nf.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qj.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dt.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lp.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://wt.yuntaijiaju.cn

[E17] 首字母大写
来源：http://yx.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cf.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://da.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kg.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kp.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ox.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lb.szxytkj.cn

Ruby: s.capitalize
来源：http://ip.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hs.lnxyls.cn

[E18] 模板占位符替换
来源：http://iw.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kv.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oa.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ev.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hq.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zy.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://za.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://in.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wh.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://bk.lnxyls.cn

Py:   s.splitlines()
来源：http://mj.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xk.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://xf.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://jo.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://tu.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://jg.panjiajie.cn

Ruby: s.lines
来源：http://eq.shxzskj.cn

C#:   s.Split('\n')
来源：http://bu.521024.cn

[E20] 判断字符串是否为空
来源：http://ff.szsharing.cn

Py:   if not s:
来源：http://zv.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bz.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yg.9csxet.cn

TS:   if (s === "") {}
来源：http://lu.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://zf.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://nj.yuexingan06.cn

Ruby: if s.empty?
来源：http://dq.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vd.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://ph.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xy.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cu.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xv.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ya.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jm.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://kf.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kg.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mc.huanxung.cn

[E22] 字节长度与字符长度
来源：http://ms.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uw.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rx.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://td.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cu.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rk.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://md.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://xc.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hy.521024.cn

================================================================================
来源：http://px.szsharing.cn

F. 文件与目录
来源：http://bp.haigaiapp.cn

================================================================================
来源：http://lp.shxzskj.cn

[F01] 读取整个文件
来源：http://dr.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wa.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://iu.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ad.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ff.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ys.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oc.nicolike.cn

Ruby: File.read("a.txt")
来源：http://tz.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://wt.shxzskj.cn

[F02] 逐行读取文件
来源：http://nv.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vv.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jn.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ul.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nq.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gg.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ep.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jj.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ph.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://mx.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fn.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ut.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pp.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aw.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rc.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gh.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://lw.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dg.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://qb.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yq.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uq.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xn.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rl.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pg.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://no.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ts.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bk.muxihuayi.cn


<!-- 参考信息 -->