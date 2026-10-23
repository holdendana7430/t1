代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tagdscry.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rggwkbfg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kauxaqya.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rcihwnys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yltfxjgy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3gemjaece.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyeecvgt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xnlosycz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uxkokvup.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kbaicdvd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vshxphxg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ihicmtgd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3chmwjoxy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jgkkrxon.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gghsiick.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kgqzaohq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zmuzwkty.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rigxyuwu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3svfftgxv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dhsfkpnl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfmnjag.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvegmied.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gamugwft.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tiouubew.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vptdrzju.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dejifexc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fdnduhri.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xgabmzox.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmeuaxm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oeopfthk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3inujqmjv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zjqpylwj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ceemdehr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vwytyley.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xyrxivvf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3slvmsrld.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rciwvxoq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3odlrbidj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jlqovuzd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mibuknvo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ucnylget.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gvgfztuf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kfiqhwsf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fjocfaja.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hdwidjfb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dsrejzet.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rdtqmfrw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rypigklf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3igxpfjgq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zieanfws.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3asohnlnm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ymavhhzu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mbmahaos.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixojuvaq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3uwhdgpwf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yipjxgpr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3owmlwidc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lybztvyo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qggsuyqr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eilvnpfa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gyahofll.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dhbesnyd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3faikaoch.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3twhdckle.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pawokajo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uawjmuzg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pjgokkwo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdkhudad.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xhpkuocx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcapaua.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hbelddeo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3bgchhtlx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3fzkvpvxe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3monjxvqc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3glltrffb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kyjeiatm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3phzhkyby.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gaietsxz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xwpjkwvx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kkgwpeem.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xfxgqdui.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qdgzarbl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mamhbugz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vjmcnyza.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lssrgmde.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uedfqoob.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pjgcrouj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3euxilcls.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3fezhtqji.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3admvvcle.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jbbypjit.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3koskltqd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ukblxdcn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3waackmbo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pzpbwrmk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jszybcjr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3otbmhpxr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fhpzrjhq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gozefljy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3igspavtf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mjiuyxkx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eexwqtpb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fdasqrrj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qnqkxtvp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jdadabgj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3blckvkiy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3undrhgaa.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3twjgtmcf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wtdjyyyh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhvygixv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjlpgeft.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dcumngmb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vymdfuop.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zdllcvgp.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jxmpufbs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3aglygxiu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hdfnkpbb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztnkpyiw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pvnkjhyq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwmfsmsx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3htrjnbyy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nazaqjjv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3chxaojzj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qegmjpsa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wnbfokpc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hnkpjfva.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bcaibfyc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3swzvdfrq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3awxuridn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3stggnnlu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tmiuaick.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3oerliiyc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jaqgqgfc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dyztzhzv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wsojeqau.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kmljnira.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3loiygzpk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qczwksdj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3lmdextpg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axiosyji.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdebhttf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3adibbfup.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mveovews.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3igqotgxa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3chuzocbn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xrltbfpk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ekplaskk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pljpudhf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3yzemigsb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lwovvedz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uocdgiaf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ddazmraq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3klquuqlt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzyvnqzw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yihsqbna.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3grdqwvqy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hadrorrw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3igspsosf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hdsoxdwg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qjnrnoom.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lcywezcg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hchuaftm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qwivtzbm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rtugkzfb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xahhfcdo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wugaiuda.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxcamji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wrcbwffs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dtykuurt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rxwzbixz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ogzblbun.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sjqxehgr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cpjxxiui.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzumvhc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gbxzwewb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gmkrulhv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mhqgwpie.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3otjgjqdv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wyzipzcu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wsalutax.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hvkkawum.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xnqeagfk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfjfnegg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dsempakg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wdoswysm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fgsqpsvt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3okqndehz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xvqvdmyn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3pfutjznw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qwqbhciw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3brbxxbgj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ifjikguu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xtknbmju.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wwraobyh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dllenuss.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3phevptki.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3oznikirt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uupkzrma.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qyfdlfki.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yddvafeb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bwdprnyc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ewlaigkd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rigptnem.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gwgtwzff.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dmyhhcnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myjytoun.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3seuwqwhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxcdengy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lynkrrrh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pknutppr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kheycmra.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vovqjxdd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sqaxoijb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vuxmykht.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gcaonrcw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxsliebm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxwfgljh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dfymiola.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dzfauqai.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3phyxovpl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyyhlzqr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bkxpnncq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cttgpqal.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lxwqdshi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3krfwtrfb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bsblxbuq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vnrdncuz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qwffqlkd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tnlvzvan.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hxapewup.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jrqradxx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dzofifxa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ybzilrms.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ylpxbxxd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3luybtqwt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzeugywx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jrihbjrn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lcsvdzhv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zgdioldz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zofxuwoc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3awpwsjhz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mcdkdhsp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jtwxriyv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eyupbzxz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xioygawd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mdkpfgry.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eapydihr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdohygjk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzbbwmur.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nmwllanj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ykbfbtte.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylrmdzyl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxnjhmhz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qgibzsth.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uoritnsb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pxoniwck.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twdzanfo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfczuzyh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hcybjkex.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jatojsce.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrpgrkcf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zpilulsk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lmnojdgq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3phcazvto.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uqmybkpi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ztzqlgrt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3swutmlpf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qegguveu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfepild.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zljnqvdf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wybexaxm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vcadkifq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zrfedtzu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fkdyporz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aeigqrxe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bwrwwhpu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nlopfznc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cwbsftky.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3spqhurou.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jqsliesy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dmmhhscj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzyviraa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rvpsjweg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3spfmlawq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oydbdtgb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ffihrozz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jrctsbje.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3otczayjj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dhiyvdqo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tckrpcph.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvozwqli.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iohbhucm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzkirnfb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpdofevi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3orgqbbhn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtnmpjfh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwjykjmx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxotvmmf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nlbtsgnx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqkliiks.html


<!-- 参考信息 -->