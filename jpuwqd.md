代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xabiupts.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vcgkkugk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpmwrkuw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkiofprk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lusvhulc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pgamjixu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qvcjmfmd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hzjmjaex.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2etblzahh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kntrgcvh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2avrnefma.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rertydse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crtouosb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2humislyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozyafcfk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rurfrilk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hhzicnki.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mahtaipf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2svmddmzu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pqmhklya.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzyxusez.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pmbxyfwt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qxrhggpg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fpaeyvta.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pmhdfnfw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ztbzviqa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vrqhokhi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukjvfkqq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhyzgcol.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcuipkgn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2lkdfjeta.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kudbndnc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2oazunbrh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kebvtntk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wrzkuoot.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xededzfs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gilaaiin.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nssgplrs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lheliouv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ymeicblb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tccwjimo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfimiwif.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2erveotdj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2facalrnq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qrgedaiy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xgqfidie.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jkpgldrn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gchjctkr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xxqpckse.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nhhkuavf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rfhihday.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ifqajbqp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oguilbti.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2saesjyps.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jyausdrh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ihjosqqm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nvynbwwr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bltxrdfp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aenbxaln.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sirqdrop.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2haqsvwvg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mjrfxqpg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bfnzntwy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jyylbvjj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pybexzjr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vinkljgd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qhllhmeq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2smczznyi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xrecfbok.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sectdxww.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tzgrxgsy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zayukuua.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lvuayldj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yzzkofho.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kysnarwr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsnfncsy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rxnpqejp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qcxgnawg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jnkbtqok.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dvrsufao.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ynyvbbly.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bskuwoxq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nqbmnwju.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nsmcpcry.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cqxoltnq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fetyjucu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bmjwqefj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2uovwypzx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gigklzqc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vxceabnr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2msoakjry.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hceqfmxs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nuudpotw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ngvhhuqh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2bmbsioap.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lvwrpgpk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fqtheucp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2prmvhxrl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wzsoeeff.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ynkdyray.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2awhrigcl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hmudfihn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oarwyvsu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrvvopf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2phnlfsgq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cbqyfvte.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2iytdzmtg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjovrjlu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zeeoushg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oweverlm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lcsiiiku.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ohqwsljy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rcmdujtg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ffobigwh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qjqimotv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yynrupsu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ngggxkhc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bjrhhkzb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vkxoeasy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2gtqhhbrc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rxtsrzbl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eojftilk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pdnzvvwf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2coedcsbr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2eaoocdnn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2fhswtahi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltbwjhap.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhppiwfn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qiqivjxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2firvizoa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ysxmtrpj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zschlwpv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xiijuojr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2obqygvcs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2haivwouq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lucmujsi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hqlkjgjs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eskuvele.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2scpfduuf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dapfaxzg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2abrzzezq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xfeotlqm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qygcxxmj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbcvome.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lhfokxut.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gbeutbcd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uxyyujjr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvlvpsk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bnpszkde.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rvhmhcba.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ruuejyeu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jmnbvdsl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2imobgbep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vzkoyeyy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ksaygiei.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qiezqhst.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2didgazbx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vzxannap.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zehrnutj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jzfepjof.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qtxqxowx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2paihhewa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytojzdpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fulhtiro.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmztmzeu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sfkrwceq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gyinsfrs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vjbxqsok.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2znrnldei.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vzswfdrp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bmlkhlpm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rltpwnzw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tvcsvgtv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xtykidwu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sqvqshuc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqbyyqyt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bcjhodco.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2azkkmsav.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gcrwzmbb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2idlsctgg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cuksakfz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ybvnbzlm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tznithrw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xjoncwxl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rrlkxjpv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rvabclml.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lqvaityt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ivvnlwwd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hwhavlnk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwskhokv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzdubezv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmxbeagm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwbhld.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dtrjtfmy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2thbtxtti.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rywmunbj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tzvggofl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ybnbmuuf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zxmhnobz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qhntdibm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cbrarrrc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xrvfceky.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ktsusoce.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jwzwkqta.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qlecmxzi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xbpmxqvb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qjmvyjxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yifajpio.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fmhsnibn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ubpasdrw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2txjbafkk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2islczmhb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dcyprkqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwodeyvu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2obdbqufx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkjqcaid.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjxeprvy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2djmqnpql.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ihxekqoz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fvlngvhh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xrqwjhvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2moenintf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ydewkert.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcgetuau.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tthetnub.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tasszgyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zotptkhr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lphrbyzg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkqewdtq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvmtawec.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2iyzqlhbp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lopkgcel.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bjlybpui.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ndeqhugb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jrjraoyo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2flxluqtx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2avqjhmgl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hmlhddij.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2swzweilh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tpsknszb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ogtivrrq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wootscou.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ocvlityi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxjxcnwv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mhybiigz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jnkavnoh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ayqspayg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ftlnjfgl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmxhmtb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jmdpgkbv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vcsfvacs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wfvggsul.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dihnnfce.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pbsmwtju.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dfzzdfnt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aaqbrlmr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2julzgewd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwqgzmlx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2trmwrflg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbqkfqgy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbjeisge.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yxhzshel.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbudjwer.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ouiuwblx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwraiyay.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uenrwnis.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sufzmabb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkbuylqf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkcwczge.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cpugwkuu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pdvtddco.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xchlyehp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bbngaawo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2teqwdpxd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ywtpjgnu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jjhhaasp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmnxvkt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nbfqonis.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xfbqbxib.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gsiuftay.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2aqamrbev.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqfehfvx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nmdjtczy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cvjxiarr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vtdpiotc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sycaiypr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2qlirakiz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kbbryqsz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jyicnigq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nemacyce.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvnmdnoi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wlmhuuxp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wmoetevh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tysytckz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vxgdcoxr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfowctau.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2slsfzwud.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mostsgft.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tuxmxvmp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hwgcvgjh.html


<!-- 参考信息 -->