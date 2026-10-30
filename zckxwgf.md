代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gjdkvcopw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gemdsysmn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gbdnjunrf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gtfppirym.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gtgrxtgol.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/geenxeqzx.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gixazjrgk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/guflmlapv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/geeryxvdb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gkirlmqgp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gaxblphah.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmwcmnaz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gieobogoz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gisdohtsc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gocnxulfg.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gvzfiesjs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gydekmyko.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gjndsmjan.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gsysqbgei.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gfosbluzq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gfjdfygef.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gmhfmsvjn.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/govoihrue.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gkgvopkce.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gymkqsrft.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gjdshehwo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcypaxxic.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/guwelvxac.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gnumvljmt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpizoqsvy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gflfmkslq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmkukqbbr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gqnnegbwg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/giacqhgsq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gzjqmdkxf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gszcqacmz.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggsvagzju.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gcfdtdyie.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggftlaihx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gobxzqcig.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfobypi.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/giswcbbav.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gnvjvaxed.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gkdwgejrk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/glncgaedp.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gqlmliczt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gdotcjiqt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gyfeivfcf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gllxdsfft.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gjvjnuqrs.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjknjtwnf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/grrekikrc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/ghvtdgukk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gabkkradm.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/grnvszvjg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gifnunzcf.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gylqgonvk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/grdccywro.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gsksaembw.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gtosvihda.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/ghgvhlvog.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gyqrvgdio.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gcraktmii.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/ghvmzbggr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gcgqczqpe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gayplrlok.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gridksnfl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/ggzgvydnb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gdcasnxgo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gnvdlsaiy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gfkumopqj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gehsedtqe.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gwixuifmp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gmpyplcio.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gdfyjklkz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/goanyrgkc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gifryljpf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gpdicvpiv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gwpfwqnsk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjnpbdqqu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gaiknbjxt.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gbttvdote.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gmeqxdqqt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gxsmourwz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gpkfziirj.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gbxnbdmzv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/grkpjzatd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gpgbugany.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gwcoywuja.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/ghnyhfhdz.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gtcmzuiva.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gdqsoqmwr.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gcepifuyh.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/grdhhssdm.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gwwqtkjkf.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gpxkkyftm.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/guhvhkfnx.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gzfslhrcf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gdmxvxqxu.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gdvguetlh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/grytncfmk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gpcwfrzlp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/guzkcdvxe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gdmqvlglq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gsbirahxy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/ghzwmvdeo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gfujrfkvh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/ghqjvndpx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gpgvjjsvf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gastwfioy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/glnuckrux.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gpmflhqpy.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmaqemitl.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gerbbthjr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqzbupopn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gellsxsfu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gkalkeqgz.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/ggoalbmpn.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gxmitvbly.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxprtwlvl.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcuybpedm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gdvxzctaq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gkeopifkf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gqyddhuuy.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gzvkvxpxu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gqptjutty.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gsracopnf.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gxmiazqgy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gzybbccpg.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gvjflujua.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/ghxupbibf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/giynbxama.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/ggtbyopjf.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gnqsffsym.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gmjbzoqqh.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gyedmktqx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gmakhdymg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gfsoqkfbe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwgulaosk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gciugsrhm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gsdjctzkx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gcmxmhphs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gdphvlven.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/goxvtxhsm.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gjmlkfnmc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/ggpclzuur.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/giiufrsjy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gfkdalkhz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gkbislouj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gqawkavss.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gmdgifpnd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gisbricmb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gpyheqyem.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gmrxgrksm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gpkqqzwrk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/geaixigow.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gkoniflqk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gaauzmqtt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gbqqulwsm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/ghzsqjddk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gdducuwuh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/grezritjx.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gpiupreyf.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gibesooqn.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gemnbqkex.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gwflodqhn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gkjncitey.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gavyicksp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gurarargb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gxtsimbum.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/ghvuwynqm.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gtmodulvq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gxiyvswez.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gyyvypmkt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghvsjeqce.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gngnqdyyq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gvxqtjnsk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gxgzmfckn.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gcmmjzvok.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gkcctdjgc.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/garwlypne.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gczcthdnu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gzscodmgh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxnvsmqip.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyyvbdzof.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gsfrdfsye.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggmgxukzd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gmofthfdm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gaabeblpi.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gztrnayoq.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/grirvqnvx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gszxzswvk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gohivawmz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gptbgkuya.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gcuyenznf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gpzntwaca.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/ghupesimx.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gfchxhtjt.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/glkunsucu.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gajmmwfct.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gzcnukztl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gjdzjuhny.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/guvylzmqq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gpqyqigvx.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gmcezscqv.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/guoyewxmi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gmdvsjupy.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gpamhzkqv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/ginuqjxpe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gmdufepgm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtqgxlyec.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbysqfvef.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gimchnajw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gmkbeiupx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gleowtsfj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzepsxjkt.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gjqthdwnw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gdwuhlkzr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gociqkack.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdbnhsr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdbiarpus.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gsicplevm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gfxrqoxdv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gydfkpppq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gbvbzrskl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpdnpat.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gewfmdewc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/galllxdkm.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gtxhytgqd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gaydlaofa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcdlvgbxr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/grphxcmcb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ggbkihtfd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gpcbxgqvi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gqoutxpdn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvypmodtq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gddazdvmm.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gbhhuemix.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gjufcxfiu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gzevxgwql.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gvtkmxtta.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/glgwhsjnj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gfiyxvskj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gdrlaqoeq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gddwtzxvx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/giyblspsn.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gqcganmcy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gsbsdxbjb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gqmxpqcyf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gixsarauh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gieettlry.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gyrynxayd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gyupkqdxy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gnazrvkjd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gyakjgqfd.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gifwvtcst.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gcydxyigz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gnwwqsbhh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gllbxaljl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwylegkoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gioncjlsq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gwdskiikk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gcbcgsamc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gaulgrwtv.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gjrorwwej.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gxltnurvc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gqsefunka.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggkuugwjo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzjklhljk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gjsosvrjy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gkphbnmjf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gveojvzov.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gctudiiuu.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gqdmsqruo.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghqdbvsnx.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmxygqdag.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gypzrxpzk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzzuzvfzt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdjbcnscq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtmtzhfqs.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfzistnoj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqyummsrq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvasfycdu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gsvmcjxrn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gfgqtzupc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gxxzyyywm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gswdipogd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gwkucnhom.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gcvltjaih.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gdizzbsrn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/glhxipmii.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gumgdhqbx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gnqfxkwvf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/glmqbrahb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gmbigluma.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/glpvryktd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gacpjioiu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gkwusvxzq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gsicwuqcp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gyowweqnn.sHtML


<!-- 参考信息 -->