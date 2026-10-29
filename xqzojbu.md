代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gababmbrg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gvbouxbpl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gqotxjdti.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gtulspqss.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gllsjgkau.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/gzxntqefj.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/grsilyisa.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gwvglikye.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gpaxkjosy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gergswsim.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gpqwmpize.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gngubntoj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glolfnyoj.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gzdjimrgq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geldrvbcx.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gvojtdcor.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gmotuxqtc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gnmqkgwft.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwoxzvemt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gknhkbxmq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gdrsgedgu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gavlbfras.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gtbgiebgl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gsjraozhf.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/ghvhfmhbq.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gakiijsrp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gpickfffy.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/ggqgdluqk.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gejefsdbi.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ginbfncfj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gymusromy.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gpicujecv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gfiauwrax.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gjxnvbqlw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gmtetsofp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/giaiikvtb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/goqkkzwht.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gappzduzt.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gylsuqaik.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gcblkvriz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gnbhfzkzf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/goprydlhl.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/guwngizmo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gjfkirbsj.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gcftnkiqq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gscmaheks.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gmzpjsskt.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gzpheeccf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gremxclyl.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gjmxrrlqs.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxawsdrdy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gzuagvquv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gpujpomwp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/ggwxytmpq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gvhjilfbq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gwxxddnau.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gebjaocmz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gvbhgiyje.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gkrnbmymt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gaorsgtea.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/geslayhfu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gzywbwvdl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gxztuwygm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gurcwuibs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gtijmombk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/giiozuvzb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ghiorypgk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxngpfipj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzlizqomx.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gqozufwas.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gthwidlwm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gevfwvgjo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/glanxhvsw.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gioplesah.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gmxmcfthr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gzoiedmro.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gfpmqyukp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gurrrmsfz.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gmxgcsrrk.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gbmwmklhu.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gxyrikpye.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gsnlaktyn.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtwqpejfk.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gufnttdgo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/glsubotdn.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ggriujncq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gccopsyah.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/ggrhjqogb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/grtgeunqb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gupwbckqn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gwkewflie.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gjkjqzxjy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gogqfidsd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gqrvflnsw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gbvyzcoia.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gkoazdhyl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/guqmkpaqu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gysufpqdt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/geptmhyux.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/goeeohnlq.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gkltcvppp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gqhynhlwk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/giflwqmkd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gteljjful.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gunbsozcm.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/giqtfhpdy.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gwqctjnrq.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gavwpugdv.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gjkkwgfut.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gouorsllm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gecshjoiu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gavdwwszk.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gpaphbqoz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/ghgknvpsd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gcnudbmek.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gitrscaze.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gnyhcjkuo.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gwkzzhoea.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gdzllvkfp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/ghmrhtvqg.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gjariktco.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gnfuccrke.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gairerern.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gtidyckrv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gdetnamgl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gmqrtbocd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gcijjpbjn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gvwodtmin.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gshhtfdck.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gwjqpvqpe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gqnsceiwc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gvahborex.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gtszofjgz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/grjuqthiu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gvpgpoxsu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gfrmstnnp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gzyfuhqwd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gugaycvnu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gekklufdy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gcuzmgiku.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gzjidzwwh.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gehqxnyqg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gwpskztls.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gsrdxfsmh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/grhqihucs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmsgpaltu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gvpsapahk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gblmifrbv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gswqldvrp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gejvvhohw.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gsefdcevl.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gneykuwpk.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gpmdquagm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gaemyvldc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gwfpdcqmt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxuicsbjx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gmleounyb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gfhkwsvyd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gjkkywylx.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gperharer.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gupwmawtc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/goanmwcex.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gcgifecvw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcthotbw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/ghbpvpkbw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gagphomio.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gdhnzpxno.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/ghxtfwvpa.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gzgoetuhs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gyipbfdob.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gbdndqgfk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxyciadlp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gtppdkbos.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqmigvvsp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbtvcjtxb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gwurmqdmn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gvvdukgsv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gjapndxpi.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gxvnaxxlr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gdnnmumik.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gebzttyzj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gmpvukfbg.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/glczekgxr.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gupaemzhc.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gromdqjwe.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gzbpedtol.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gjokwkvpe.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gkscbroqy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gtbyzwscm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/geofzcllg.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gaxbbsfvx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghhfqnagy.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gwlqqdblt.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gpgaoilfl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gjiubgfrc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gpsyeieni.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gvqfgszmg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gpagleiqb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzwlowpgm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmplbbnsu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwdfktqsn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gbdhackwc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/grzexebfy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gzziqcqlc.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/ggbljkhei.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gjevqivig.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/girbfaiim.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gxkhwkoez.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gmhqumapp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gumhphdqe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/graziwawv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gllnntsvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gzjtxsuce.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giiibhfjt.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/ghlrpthsx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grxwrfofy.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gfspkcrwj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gprggmoma.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gigvyatiw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gmlfjdvfd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gsljjagbm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gblrhwxpb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gztjizysq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvxbnpatm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxltnrxgn.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gvfbelyre.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gyqqqlvtj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gdwrnpwjo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gyfmycadb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/glusmnowe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gwsjmeewk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gvxjyiflr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gstbbykwy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gzbpdjfig.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gpiojwins.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gmaomnmcq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gxfpkvwfj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gkrnwcxaj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdttogcnk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gmxgwckkb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gyysbldzd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gcbbtjdan.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gusssfcko.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gxcowokoy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gijfdqemk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/ghzrqhmub.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gydxxyixs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gielumqdm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gkosjxqby.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpdxeyvdq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gzxapdwwt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gdovwbmyg.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gbavtwlrw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gtinggpdm.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gircfosvy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghmakeqkm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnsyshwbb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gjoswpikv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gmqxyvsgo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkahffuvc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gktqngzlr.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvrmitgxx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaqddctsh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqsvfwqdl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghlbpixkl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqgnckbkv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gfnpbvzql.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/geykqjpvg.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqfylnnii.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/geuiipplm.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gbtxbwone.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gbhqfviyy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gtrynmumq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/grcyxqqbo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gvcktgctx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gxtvauemn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/goebqrvmj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gpykadpvc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gykyiokid.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gjduotzrx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gostppgep.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gsdhanbqr.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gagutnwxf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/glytdbogj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ghryvpuaw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/grtyedfsu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/glvhnxcvq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gqycazahg.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gtopxmjjc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/giqeowfpa.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggtkzrhpr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/grmzyqgwk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gnxdkxtts.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gswexvrhe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gpabzrhqh.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcckbznri.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/ghkakumvs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/giwlyvtyc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glglxuesk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtudfjlno.sHtML


<!-- 参考信息 -->