代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ch.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xj.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qp.nszjky.cn

TS:   [...arr];
来源：http://kw.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://ca.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gv.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://tx.panjiajie.cn

C#:   new List<int>(list);
来源：http://wo.colortex.cn

[D23] reduce 累积计算
来源：http://qw.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qi.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tt.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ub.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tg.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rl.newstarts.cn

Go:   // 手写循环
来源：http://qa.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ve.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yu.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://li.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uo.haigaiapp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qf.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ne.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yi.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dt.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vg.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gh.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ae.asd995.cn

[D25] Set 集合去重与交并差
来源：http://us.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ie.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://is.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ri.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zf.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yw.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pk.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ab.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ml.chemitech.net.cn

[D26] 数组转字符串
来源：http://vy.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://nm.gzmigu.cn

PHP:  implode(", ", $arr);
来源：http://tw.lnxyls.cn

JS:   arr.join(", ")
来源：http://mu.jctech888.com.cn

TS:   arr.join(", ")
来源：http://mc.newstarts.cn

Java: String.join(", ", list)
来源：http://nj.szsharing.cn

Go:   strings.Join(strs, ", ")
来源：http://ww.nicolike.cn

Ruby: arr.join(", ")
来源：http://kt.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://jq.chemitech.net.cn

================================================================================
来源：http://ty.shxzukj.cn

E. 字符串处理
来源：http://df.shxzukj.cn

================================================================================
来源：http://gz.huixiangedu.cn

[E01] 拼接字符串
来源：http://ei.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aq.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wp.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vv.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gx.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ci.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cw.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ol.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wc.shxzukj.cn

[E02] 重复字符串
来源：http://zw.panjiajie.cn

Py:   "ab" * 3
来源：http://yi.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://uw.hahajie.cn

JS:   "ab".repeat(3)
来源：http://mx.9csxet.cn

TS:   "ab".repeat(3)
来源：http://ki.nicolike.cn

Java: "ab".repeat(3)
来源：http://hy.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://dy.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://mk.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oe.szsharing.cn

[E03] 截取子串
来源：http://ax.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ff.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iu.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dk.nszjky.cn

TS:   s.slice(1, 4)
来源：http://gl.szsharing.cn

Java: s.substring(1, 4)
来源：http://ak.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rl.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gx.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://gs.yuexingan06.cn

[E04] 查找子串位置
来源：http://kg.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://dk.newstarts.cn

PHP:  strpos($s, "x");
来源：http://hg.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gk.szxytkj.cn

TS:   s.indexOf("x")
来源：http://zn.szxytkj.cn

Java: s.indexOf("x")
来源：http://gu.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://ve.lnxyls.cn

Ruby: s.index("x")
来源：http://kr.hahajie.cn

C#:   s.IndexOf("x")
来源：http://is.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://es.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ep.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zb.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dd.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://js.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bt.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qz.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xo.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://st.wgjwhj.cn

[E06] 替换子串
来源：http://vj.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xe.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://zk.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ak.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://ii.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hl.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hr.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zf.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://mf.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://nk.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rh.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qm.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ac.szxytkj.cn

TS:   s.split(",")
来源：http://rc.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xg.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ia.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://vx.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sg.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://xs.huanxung.cn

Py:   ",".join(items)
来源：http://ls.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://lf.gzmigu.cn

JS:   items.join(",")
来源：http://rv.jctech888.com.cn

TS:   items.join(",")
来源：http://lt.huanxung.cn

Java: String.join(",", items)
来源：http://vm.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://sp.panjiajie.cn

Ruby: items.join(",")
来源：http://qn.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://ao.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://uk.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nb.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ne.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://dm.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://pk.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://ra.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mh.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zw.szsharing.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xc.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://jj.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xy.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://do.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://wp.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://ne.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://av.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sv.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tv.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ub.yuntaijiaju.cn

[E11] 反转字符串
来源：http://vx.nicolike.cn

Py:   s[::-1]
来源：http://es.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://mq.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://ir.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://lr.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tq.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://br.shxzskj.cn

Ruby: s.reverse
来源：http://xc.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rf.9csxet.cn

[E12] 统计某字符出现次数
来源：http://nc.newstarts.cn

Py:   s.count("a")
来源：http://ds.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://xr.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://sv.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://pq.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lu.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://hx.gzmigu.cn

Ruby: s.count("a")
来源：http://eo.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://eh.panjiajie.cn

[E13] 逐字符遍历
来源：http://jw.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://mc.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nv.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ck.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ie.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kc.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://og.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uz.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xd.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://pm.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xk.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ny.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uf.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wb.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uu.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nd.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ho.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qy.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://ve.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bo.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qq.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vs.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ea.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dy.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qg.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://va.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fu.nicolike.cn

[E16] 数字千分位
来源：http://ts.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://ii.hahajie.cn

PHP:  number_format(1234567);
来源：http://nr.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://el.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yi.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xe.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tu.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qy.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://lg.huixiangedu.cn

[E17] 首字母大写
来源：http://qb.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ef.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hr.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kp.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zw.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dy.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vp.nicolike.cn

Ruby: s.capitalize
来源：http://hp.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mz.bjjhwx.cn

[E18] 模板占位符替换
来源：http://uq.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gq.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tq.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uy.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ea.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ti.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fs.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xm.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fr.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://dl.szsharing.cn

Py:   s.splitlines()
来源：http://oi.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xk.521024.cn

JS:   s.split(/\r?\n/)
来源：http://it.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://dk.shxzskj.cn

Java: s.lines().toList()
来源：http://ic.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://aw.nszjky.cn

Ruby: s.lines
来源：http://oy.hahajie.cn

C#:   s.Split('\n')
来源：http://ru.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://xr.newstarts.cn

Py:   if not s:
来源：http://mu.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ni.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ui.colortex.cn

TS:   if (s === "") {}
来源：http://ff.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://qi.colortex.cn

Go:   if s == "" {}
来源：http://ir.yuntaijiaju.cn

Ruby: if s.empty?
来源：http://il.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kj.9csxet.cn

[E21] 超长截断加省略号
来源：http://eg.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qo.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sl.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://af.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fo.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zc.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://rq.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ac.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kz.huanxung.cn

[E22] 字节长度与字符长度
来源：http://gi.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zd.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ar.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ud.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cy.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lu.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tl.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://rp.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mr.9csxet.cn

================================================================================
来源：http://yg.shxzskj.cn

F. 文件与目录
来源：http://ey.szsharing.cn

================================================================================
来源：http://ue.gzmigu.cn

[F01] 读取整个文件
来源：http://kp.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vg.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://tc.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ty.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zt.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dg.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wg.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://wa.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://rs.panjiajie.cn

[F02] 逐行读取文件
来源：http://xs.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gj.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cs.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xc.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ua.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mg.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tz.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://av.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zn.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://mf.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://od.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zu.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sx.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dc.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qe.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bn.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://by.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zi.jctech888.com.cn

[F04] 追加写入文件
来源：http://bh.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aw.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vr.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dj.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ye.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wk.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ph.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cr.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wp.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://go.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hc.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://fp.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://el.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://qt.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vb.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lu.521024.cn

Ruby: File.exist?("a.txt")
来源：http://ns.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://hx.chemitech.net.cn

[F06] 删除文件
来源：http://gx.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://cg.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://py.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pt.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ew.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://my.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://qc.jianghongdianzi.cn


<!-- 参考信息 -->