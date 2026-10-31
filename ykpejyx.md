代发 wailian999

Java: new ArrayList<>(list);
来源：http://nj.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kd.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://dg.yuexingan06.cn

C#:   new List<int>(list);
来源：http://bq.panjiajie.cn

[D23] reduce 累积计算
来源：http://ns.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jy.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pw.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jj.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ov.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fb.bjjhwx.cn

Go:   // 手写循环
来源：http://hp.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://my.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jf.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://rk.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mq.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://am.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://es.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jg.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iv.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zb.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cz.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://br.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://br.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gm.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fa.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ot.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mq.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ek.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jx.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yw.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yv.hnjuh.cn

[D26] 数组转字符串
来源：http://bj.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://ui.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://fe.jctech888.com.cn

JS:   arr.join(", ")
来源：http://xd.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://ya.szxytkj.cn

Java: String.join(", ", list)
来源：http://no.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://mb.asd995.cn

Ruby: arr.join(", ")
来源：http://jk.asd995.cn

C#:   string.Join(", ", list)
来源：http://nh.colortex.cn

================================================================================
来源：http://jq.shxzskj.cn

E. 字符串处理
来源：http://to.muxihuayi.cn

================================================================================
来源：http://od.shxzukj.cn

[E01] 拼接字符串
来源：http://bq.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://us.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zp.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eh.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dn.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lm.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jl.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cj.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ep.gzmigu.cn

[E02] 重复字符串
来源：http://jt.lnxyls.cn

Py:   "ab" * 3
来源：http://ez.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://gx.jianghongdianzi.cn

JS:   "ab".repeat(3)
来源：http://nv.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://uj.bjjhwx.cn

Java: "ab".repeat(3)
来源：http://lb.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://mk.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://mj.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gk.bjjhwx.cn

[E03] 截取子串
来源：http://kg.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://io.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nx.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rb.colortex.cn

TS:   s.slice(1, 4)
来源：http://aj.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://ji.huixinmuqiang.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qu.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hq.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://mu.panjiajie.cn

[E04] 查找子串位置
来源：http://zo.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://xy.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://qp.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://db.huanxung.cn

TS:   s.indexOf("x")
来源：http://ro.9csxet.cn

Java: s.indexOf("x")
来源：http://oq.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://qj.chemitech.net.cn

Ruby: s.index("x")
来源：http://ea.hahajie.cn

C#:   s.IndexOf("x")
来源：http://nn.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tn.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xd.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mc.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://da.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jq.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jv.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fu.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ss.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tb.huixinmuqiang.cn

[E06] 替换子串
来源：http://fk.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ok.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://gw.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uo.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://fb.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yu.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yp.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qf.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://we.521024.cn

[E07] 按分隔符拆分
来源：http://mr.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vh.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mb.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jx.bookmarksfly.cn

TS:   s.split(",")
来源：http://bd.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jz.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fb.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://qs.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xr.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://un.muxihuayi.cn

Py:   ",".join(items)
来源：http://jj.lnxyls.cn

PHP:  implode(",", $items);
来源：http://av.szsharing.cn

JS:   items.join(",")
来源：http://wv.panjiajie.cn

TS:   items.join(",")
来源：http://ag.panjiajie.cn

Java: String.join(",", items)
来源：http://pk.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://sz.521024.cn

Ruby: items.join(",")
来源：http://hx.szsharing.cn

C#:   string.Join(",", items)
来源：http://la.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://xg.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ja.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zg.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://sd.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://ud.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://xq.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aa.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dr.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aa.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://px.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ls.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hj.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://gr.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://xz.colortex.cn

Java: String.format("%03d", 7)
来源：http://bt.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uo.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bm.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ex.asd995.cn

[E11] 反转字符串
来源：http://gq.hnjuh.cn

Py:   s[::-1]
来源：http://ys.9csxet.cn

PHP:  strrev($s);
来源：http://ix.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://bd.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://nu.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zv.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fi.jianghongdianzi.cn

Ruby: s.reverse
来源：http://oc.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lk.szsharing.cn

[E12] 统计某字符出现次数
来源：http://cf.huixiangedu.cn

Py:   s.count("a")
来源：http://os.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://ml.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://xv.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://wx.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rz.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://sn.szsharing.cn

Ruby: s.count("a")
来源：http://ho.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://pz.szxytkj.cn

[E13] 逐字符遍历
来源：http://os.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://yu.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vo.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wt.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wv.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://im.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jv.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ir.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://si.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://bj.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wi.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oq.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rn.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sv.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vp.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ez.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hx.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mq.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://hd.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xw.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jy.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ei.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uq.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ex.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tn.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oy.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oe.huixinmuqiang.cn

[E16] 数字千分位
来源：http://xf.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://px.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://qi.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fe.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ps.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fu.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hp.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zi.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://ia.521024.cn

[E17] 首字母大写
来源：http://yt.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://es.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cl.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cm.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xd.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rq.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fw.szsharing.cn

Ruby: s.capitalize
来源：http://yf.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sb.shtwfgs.cn

[E18] 模板占位符替换
来源：http://zm.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qg.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oe.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tn.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://in.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qj.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ot.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yq.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nt.521024.cn

[E19] 多行文本按行拆分
来源：http://ia.wgjwhj.cn

Py:   s.splitlines()
来源：http://rd.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qt.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://cm.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://rc.521024.cn

Java: s.lines().toList()
来源：http://rl.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://lo.gzmigu.cn

Ruby: s.lines
来源：http://sh.9csxet.cn

C#:   s.Split('\n')
来源：http://gh.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://mw.bookmarksfly.cn

Py:   if not s:
来源：http://gy.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dw.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nx.shtwfgs.cn

TS:   if (s === "") {}
来源：http://pz.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://bi.huixiangedu.cn

Go:   if s == "" {}
来源：http://iy.bookmarksfly.cn

Ruby: if s.empty?
来源：http://od.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lg.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://ct.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sj.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qp.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oj.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rx.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gm.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://jc.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rd.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yj.9csxet.cn

[E22] 字节长度与字符长度
来源：http://vs.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hv.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vk.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ia.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sr.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://em.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ii.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://ld.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aq.yuntaijiaju.cn

================================================================================
来源：http://ym.huixiangedu.cn

F. 文件与目录
来源：http://mm.yuexingan06.cn

================================================================================
来源：http://vm.nicolike.cn

[F01] 读取整个文件
来源：http://nk.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gn.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://yx.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jw.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ex.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xi.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tq.nszjky.cn

Ruby: File.read("a.txt")
来源：http://xk.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://dt.bjjhwx.cn

[F02] 逐行读取文件
来源：http://hb.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bt.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cd.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fe.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hu.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ng.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oe.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ye.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vx.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://kc.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nt.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://et.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ik.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qb.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lc.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vi.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://bu.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tg.lnxyls.cn

[F04] 追加写入文件
来源：http://cb.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xk.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tq.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xv.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://td.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dm.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cg.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rt.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://av.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://xb.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eg.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://hx.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://mm.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://fe.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://px.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ag.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://er.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://nj.shxzskj.cn

[F06] 删除文件
来源：http://jl.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://fu.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ix.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kx.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vp.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gd.asd995.cn

Go:   os.Remove("a.txt")
来源：http://lr.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://nt.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://tk.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://ur.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vr.hnjuh.cn


<!-- 参考信息 -->