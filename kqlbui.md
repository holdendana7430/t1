代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pajpojhp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzpnoepp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2maarrtkn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnbfxlcz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vcjalqey.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qximqpru.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ouceewnx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dicrjexk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2iioqntmo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jccqsetb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2plskelch.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tzodgzye.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gdqaxrnw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2noxblmfb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jtjbmupl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2oksnprvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spnidqsh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2oivuiiqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfjvchyh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ysqfkkyv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2tksupflc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2awjqjcch.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hcbkzmcg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2idpmlfxn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vjuggocg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ialjwrll.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vtegtliy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yswjcpfy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zxggatjk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uxbvntjk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2olbygylg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzgitci.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nltojmqq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wdbchlew.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2icvelusw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qbftsmav.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2tpeafqbz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dfbopjuy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vsjdmrsp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2suctggvh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vgmiwlff.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wrkxhllv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrngoou.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rfdfksqh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2govaszee.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ejxfzhvr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ppzycxkh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tmnxselz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2otfzqejy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cisgokgi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xquioxtg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2buzeosmi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kzzmophy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2trozctdt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dpzsfrsk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uavmcbwb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bckcvdot.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xupkanzl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zsomzugo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kdulacah.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rshtcxur.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mjvolikm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zwpxiwqd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wykfvmgz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ktimbbnu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oihrfrkq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2stescbdr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2heolvpho.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hqluhlrk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fcbtohzh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vjejwoif.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xvhrcgui.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oeibzjjl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yzjufrdv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jthzjhfk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdhmgzik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ebleizol.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kpivudck.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rewmlrye.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjtdpkj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wsdstdjy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vzldverq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2braxiefm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bcoiipsl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pgfghstz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2difmzqhg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2atiwqxvj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpukhxr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhwbppat.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vtislgvs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfhscwj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2etsrcihq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvwtmxg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2grbiclgl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ydabcldy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kzzebfdj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yjajjhmx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nunhebmi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hmahbtqg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pyxqpvqh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ophmtuat.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hcmjdyxz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lxszhvks.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xrucajap.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2krveildt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hofrajrt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tolyapyo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iaipojog.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2osojpesf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vckuqmth.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cphjqgda.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vaxhkaqg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eialtolb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mmdusmuz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ovdlbrnu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2afnejzjc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xyhgdnxc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ltygwscm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gttlbwye.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2plwxcyzy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pcywwral.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2knizrmpw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zthxlqmd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dtaffnkj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2okzhnhwi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tghlyebx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dmidxztx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lgwugtgl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfnbava.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2widokufr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wdzmgjkd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfboctsi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2osrrslxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rztnethr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qqebczlz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ecclwjmv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ykjgtcsi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xuitaaog.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcerinzq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qwjrgqzg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvwvkrqu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xjetrcql.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pakaaoin.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mwsincxg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lvnvtklf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tohmjsun.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzzqgso.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pxkfipic.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bztbmnyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vztakkzq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gfamsvib.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpsrxwe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chumkhmz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2koebnhxz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wtsytvgf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2cdkhgfaf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2erdmuycs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wzfsauzj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fzlpthzq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kkmjqyqc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xjlyplzw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mbfmjldx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2topunikk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vrxcasbh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2egvwjemi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2clnnxjhf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbxiudjt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgpnmusl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxfwzxmj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vqeokhme.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bhvporlu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nrdpgvue.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zknrfcgw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tqhsxcke.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vfjtsjcy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bmzfldnv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ntccqscp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ippulfjn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mrewzpni.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihdvqtlw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2prmoehyj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2epsrdibx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dijmpfqr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2shlzwwhw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkqyayt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qcsobkyq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pzdupgoi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tnxfhwrh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rdfesaik.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cdguagvk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vyahcxmv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rksrmdyo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wyrohldm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enwaibva.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2coommuxp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2atzdpqwp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vunopfzt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nisrngue.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nfpcxzer.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vlbiibib.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2iixbdhhp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xtmlpejk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ykhenzog.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nwcphohj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nlzvvrrw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lqcqumsl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qecgifti.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tfxgpkda.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubenqnhc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aofwxepu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uxlnpnmk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmlvmtsu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xpjjview.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bablihoq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2btuvlqve.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bdykmtmt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xkzbabde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygxyyzqp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2sbqmnmry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ideassir.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwjfatzx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fsnqkboh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymydsjvc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qzpkrbln.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ebzbcgry.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2btaeahjo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tmcnholo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwqeumya.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urvlnsdh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzxthobo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tslkpmod.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cqnkphuj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jxqpugql.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adfgmvuq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oatzgfyb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lasusgah.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xckcuhpf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvmqqsvv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qxvrwnpf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2srixuyfv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yzgfhxxz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nooyladr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mvccdalq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jwyayqvi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yuslrtdl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ozqmpmsu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tlwcziyz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2txhlkwcx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wedbyafh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xsnwxsmi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dbglkwfx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jctounna.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2spttvstl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cjxejscp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ggyqfqdn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ueiiqsby.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dbprqfxx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jigjkyrp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ifenpdoo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhunrvne.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggetyygv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fsbbquuw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cynudiet.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fffpuzfz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgruwkoy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cszlphey.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uygtacko.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gakoouzh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxxuqtqo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcurmduv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2acxwhske.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdmobhgq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmbmfoek.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xqpjmwqz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hctwhvxz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wkiztucf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jyvonkbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xugihsfm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kasrdzoi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gbhailei.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cgptrhlt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rrhbwnbh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vuzplsos.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2untilqtr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2knwqudgc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uimieptz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fuoqbgrm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hzslndpj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fdlzpbis.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pjhqduvp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vcxkttcf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2iinzsidi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pkwbhwgh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqcztbya.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymsofsxm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mqvrubpi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jzgnikps.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2turycezo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zpaxxgfy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwgczekm.html


<!-- 参考信息 -->