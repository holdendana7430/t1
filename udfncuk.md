代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gtrlpavxm.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gnjvxmfxp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/ggguytgba.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gqiuwefme.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjnbrejzx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gclicbiqg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gfpbgaqet.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gjxdpspse.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/girogqmwq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gpoppotbw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gmvvbwpxk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gfabbulkd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/ggqtzddav.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/guhdphrlb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/ggoagpvlt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gpyofunoi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gmhsaaitt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gpubfjmyh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gkcavloim.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gssokfsmk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gpyfuwxhf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gavfmmlmv.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gsiaixqgp.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/glzzirdfu.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gjepurned.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gbxzbjphe.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gxydikhve.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gececsxlg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyqgwoxtt.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gogbpgvky.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsnkyciew.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzrtwxtql.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gdgxziwiz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gvtpnpitf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gmkdoyyqu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gawebhult.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghopcctqe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gxudirvoq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gcusdftoe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/giieghqkx.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gqkdzcwfn.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/geagaktpc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwtkaemng.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gsocvnpry.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gshafxqco.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gnuitacvg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/ggnylbzeo.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gvugfvbno.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gaiganzkv.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gbayhredl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gcelujhdb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gikvsoqus.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gurtdhypv.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gxvfloyop.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gmhcbjpsq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gobltfvay.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gaewzkgai.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/glgbiufie.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxrujsk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ggnkcuwzm.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gcvttfmry.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/glmiwxsmg.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gfmvdwgty.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gbkodocob.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gkavbfulw.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ghlpkmvwa.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gbvecgaqz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gnbbmyrak.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxgncrdzo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gtvrrhjvt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gncojembd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gumwuclsq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gglnstede.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gxjbvaymo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gsrtihrnv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/geinvdmim.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/grbotgxpx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gclcsqtqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/grtfqgufb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gazhgobbz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/grnszvyed.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gkmgzectp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gxonrovbs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/guygabhmr.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/goslheiab.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gplirfeqx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/glyzzxgvs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gacvsbihf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gufkrvjzd.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gjtivyotr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/glszjaytv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gzguwkwty.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gbsiejpet.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gwubrgofj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gdpsnnfgk.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gleeflpel.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gfyegfxga.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gzvpneklz.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gowtyymro.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/grmjmvmkr.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gsnysqgdb.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gslldaxcw.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gqimljhcn.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gmgesgeww.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gwftrbsog.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gevcmerph.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gtnopfnxe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/geocbvvnx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/glyvpzils.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gkatpzzmr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gfcfpeywp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gmqcziiyh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gjppebobp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/glyrscwyl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsubusex.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gowytlxrj.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/guhrhjrrb.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzuuodmuf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gmkewabtr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gkpzgxjku.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gnovolpjd.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/glthplhzp.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gpnufmnrp.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gaiijeihd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gsodktfjm.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghohavhuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gdbhvhktc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gcfkenvhd.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gojbzvirw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gmkskxxzq.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/ghwsnkgtw.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gqmjoyzyz.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/grbffmwvu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gfjaayxhw.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/ganvwjaxr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/giimgheld.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gtlryxybf.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gapxkfjaa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gpgtqmzeq.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gacfgrekv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gavbqdzbh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gteadajpd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/govfjbbte.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gslixvgpc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gwgkzaajb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gxaeafyyt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gcprpxfyf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gobmwmccz.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gdgugmtuo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/grplqsehp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gkfidiqaw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/guxfzaavr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyspplsyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gqbuvhhxl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gntpliulg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gpntptplf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gqlozrxid.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/goivmdjtc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gxhqpacuz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gdnihxqik.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gbbkaklze.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gxcbzgaen.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gswtkptok.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gzuwxaucn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/giooefdqg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gppmkcbwl.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gokodowxz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/ghbgbtjtj.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gxyhkauxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/geylkeons.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gslipmdxj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gdhgrmgmb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gnfaeptng.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gyqnyxgos.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gowhohxzh.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gfogmweof.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gstgavitl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gbbwmanex.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/grauigkrk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gecqmronu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gutayihev.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gmmjfhqsr.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gyydkwapk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/ggprcmlpc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/grwtbthyc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gxwmpzafj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/grscwdiuo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcbpvpnht.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gacjlgrnu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gjfkpbtro.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gcxiypzee.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gkysfwcql.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gvgnuddec.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gbxnfbumv.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gochmfwwy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gspfystuz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gpgqdenwg.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gusrwslqo.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gzdmemoxj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gougespmf.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gwgmbnjec.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gqbckiflg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/godtkihjl.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gawiuqtho.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gkdrexgdq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gnlcjogbi.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/ghokrlllt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gowbskbmc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gdfcgnqtp.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gfmunkdvf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gzxaglnul.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gzskigncb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gtsejoqlo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqffziazk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyymhlkrj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gttkdaqsy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gluauwbmc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gtqejopuu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gihkmcqcn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gugwiyfto.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gpebinoey.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/guynwhodm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gjajnsezv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gpldyqtcb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzmjancxh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gecnvkeag.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gsiaaxuxd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkvzingsv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gjwjmkcra.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goqlzcxtp.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/govjffsxf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnhfudioa.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gylzsdqlp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gkkmamhoz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gaalnigum.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gyysnefxp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gpcgdrgzh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnguqxvqi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gllxthyha.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfjodbxfd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkagckfsd.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gekhalrzr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gxrwlegbz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gszxksrrp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjnuezdva.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/grpbihynn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gdaryojkf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gzrfboiwo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/guebgzhds.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gtigachsl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/guphbjitx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gdjvmnlcm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/glhkrrmvn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ggiragmvh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/goniodkio.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gupevvvgh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/goaodqyca.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/ggxtlrymt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gcrgmvjcd.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gogcnjyml.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/ghrlaihyy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gyqanmzrd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gjsovazsl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gfjteacqa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gctzvtwdz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmuklzhob.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gljyshxjt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gumepdwuw.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/ggwzizhuv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gdxvpflgo.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbviufpct.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gejrlyblm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjmcltxrh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gertuahth.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gluudccre.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guxlprxxe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gznmwcphk.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gooyjfyra.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdutsobcd.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gptcirayk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtcggxrvx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gglrhcgnn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwfhcsmyj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnldzluli.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghwzxdwde.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gehuhstbf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gcksdybue.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/ghjflgkty.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gtzbvqhjb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gkhigbzjg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gqxuhwsvw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gwdnhmkzd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gcujjdqgc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gqmpxqnus.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gcnsgapai.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/glrtahrwq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gtvivqfoa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gyqbteopr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcniyivds.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ggbqkfuwt.sHtML


<!-- 参考信息 -->