代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gqlmqcxsk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gntvhlixl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gobnglgyj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/grzwjgbvs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gvzwzxvsy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gkrnbqits.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gewfjozhi.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/ggatuhpoi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/goyjvckzv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/ghjjqazvv.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqprdhdwu.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gghtvhwhg.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gvekkznxu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/giwropuhp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvfqbnyri.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gfcpmbzzi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqtgsuama.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gxzttnwnc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqxlxyrji.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gyzkmgben.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gmhdzzpbe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/godmkqtgz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gscpyptpr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/grvyhceqn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/ghmjjjvoy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gqentdcnb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gwmcdcgbk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gflekwuic.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gtqxlletl.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gybkwoojb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gmjpzqtho.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gvpvdrufg.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gwewwfacf.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gcylfdnse.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gfzwxohwo.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gwdvsxegn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/grjgnwjvl.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gucsuzvdm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gxnkrzoii.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gaouyfenh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ggygfwyen.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gbkqjudvl.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gmdequohf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gontgkzta.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gwajsxxwx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gdyaabwme.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/grzcqwlvp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/ggjrohzuk.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/grodapjwe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gpvaksybu.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/goasgxfyc.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gztqqebcc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gflozokho.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/glgwgnvml.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/grxnxeabv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/garooqpjx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gejlneayh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gtzoiwlgi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gdqamvucg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gntqlafsl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gxjtcbfgl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/guosrhuqd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/ggcphhryc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzngswvqj.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gzhpglkvv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gpafdcxng.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gbhtwotuy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gddltjdyp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/glikzwqxe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/goinfoyie.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gzhayblcr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/goafnppiy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfckqdtva.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gadmpvszp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gmgiorexl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gsohbrbyf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ggpuhkwoa.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gzzbiqimh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gfbomotta.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/glysvyiev.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gensfkkjp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gzkosryxw.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gjkkgzkye.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/giocjfuyn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gzpqnpijd.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gayddmabd.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnihmlcfz.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gsbubfpdo.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gzvfakzvi.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gunjumvbt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gqxlumxyw.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gkshppgjk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gjlmhskxy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlutvfkh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gagrpxeck.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gzhhuakwb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gtzmxoevq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gdlamujoq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/ghyurpocf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gkwiundmf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gktlxdert.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gzvlwzbmo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/goqtalode.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gzwmdnuud.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/giyftxhiv.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ggfyxcwzc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gsvagyzpt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gdmvrcghc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqnietn.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/goxgmistp.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gofojwqpc.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwxsfjoxj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/goyqulrvj.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gyidzjukm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxpgdjfbk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gsrwdtjrp.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/ghbxkqxrs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gltkolnxo.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/ggokirjxc.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghoqjyffx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gzoudkrvf.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gtyytvmxk.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ggezpsncr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gcbjqjldq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gagyzppdp.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/ghddrotms.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gzshtzqim.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gznnjzjks.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gpgnwaret.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gdxrlebib.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gfdzanull.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/grlgwzzwj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gyvgtdewr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/geomzxzvz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gedmxxehd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gtjofqfch.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gdyturopm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gjonbucfk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gmrtoitsf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gemqcyqmb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gypmxohrq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/golarylvp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gxnrieocu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gdqyvcmyq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gghqzcjat.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gqnsuzjrs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gufxljgcc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gawpcmlls.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gkhlrpyot.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gbsaxruft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gbbhbvlzz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gbczixala.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gogpbaguo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gdtpsjovz.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/ghqkqiqay.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gtgwzpdlf.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gfgsljann.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/ghacyitjf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gzuydtnbh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/giurkjtez.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gmorcebgx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gpmnxgntk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gmzxlmley.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gwugnzgqx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/goakvqbcl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmflzephc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gbmprfrod.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gapwvczuc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gqusswruf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gdabvullm.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gwpeuphzn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gjvarqxnk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/grfpvmkou.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gxsvbocah.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gzfvqczlu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gdiazyrym.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gqkfylwov.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gdvhovyji.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gqvmkikgv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gyfhpgtug.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gaeftfxuk.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gesxmqvim.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/ghfspuyul.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gckaeyisg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gbertwhqy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gvwpvvbdf.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/ghdmzjpac.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gougvvwpw.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/glbcgfrmq.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/garxfikng.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/guvepvqhy.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gwxqityxq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gvgmpjctr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gusydfkie.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gckltcrfq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grtyzrcjy.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gcwzzhrnm.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gznzykmqv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gzfyzjndj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/grmquejnq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gxuqbdgxq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gmaapuzji.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gthbvjdof.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/geqqmuscn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gvjokckdo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gcbipzprx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjmqjumuq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/glhjroshi.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gisvcrzjo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gtwdwkfbg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ganmrynxk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gyhuabsii.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gtvfwfzas.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gzaibxfbn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gibehovpe.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvrffbnpb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gkhxnjuix.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcftsglkn.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/glcqjqwgd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grtvmwnma.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gjrsgbfwp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gnhyiysbr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfqpekqpr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gvhvonvux.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gnmhukuxn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gxehkmmej.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/glvqypomd.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/grfhlyxju.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gurtuingv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcjfefapx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/glpifljvm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gvaktdmjr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gihkzsqoa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/graolinwx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gujnzbjol.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gmhfdvgkj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/grcrrlzwp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gfdyrboju.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gyzhroocy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gufjxwkid.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gnwqywkjb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gmlhoqxpx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgrxjqse.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gypmtxoid.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/ghtrmiwns.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gvtstaqmj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gcqjudqmw.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gojykmkik.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gpuehyqso.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gllisnjws.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gspwrxekr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/goxxbubap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gfpgtpcsm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gyewfnnok.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gpxxlknuh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gmxbqogen.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gmocmrihg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gqospznhr.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmmcohlyh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzplbetkf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqeianqtj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gidfxpeik.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gecqqegwz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxohkvcgr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdwiranjr.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gtaolblab.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtosyabuz.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnlbchehp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxjtczsyo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpabwaaeu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gowzmotyq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqijmpqok.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjmmgpnec.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnigdmxkt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/grhnriqyz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gcbrzeier.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gcckncuyp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gujkcjpar.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gwabeynis.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gbspigsoi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/guvuupjgz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gyeydtaxl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gicmzfbrf.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gwyqxomhl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gfoaaqkac.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gzkvpjpnx.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gyxmepsus.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghrcyread.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjtvpiea.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxdwshvkp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gmbuphkle.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gjbfnpjmt.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gzcyervbx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpcvbajkj.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gscaewkdx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gehqgtdxa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gkztsstqo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkpwwqpkx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/ghfqlvtpm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghszxwsne.sHtML


<!-- 参考信息 -->