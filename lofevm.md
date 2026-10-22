代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iqxapxmu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzfktbkw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ngpptzmr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bvcagfsl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qogsregn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2woojoxyo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vnflqzom.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2atrpinrk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ozkffejf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vzilcnqk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hddkaqrt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mkcvwzko.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2srmpczuw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ujyhantm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pkkxgfgh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ckqipzam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmrzfrzg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2khesrmuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyeadfdy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ticvfbdc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fmdphlht.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jmbyehub.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rgqrfdrc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qzaozbrm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhsgowtd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wicpdhyj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fupxdazc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2psaodfxi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vdtrcntv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2joanyiwn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pjflquzf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2epdeeuab.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdgrcxm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kmdiqrob.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdecuvj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wbobkmhv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hgsxomvh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2guiyejdc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zoystjco.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pvpiruvt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ltvllrww.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hqebdhpy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jpshryds.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bgfepraa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2rqybvlgw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jytfgcae.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yqimxadm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cucnassw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qvhkjeun.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2koqfnrzm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dozwdjef.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2olnzelji.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bblvltvw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2odcgothk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pvwkkpfg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ibcoqqpo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2etidcgjj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2adjpqido.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vdfjqkny.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qtkvfbke.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rvvvpnpo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2cgjnbxbg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wqsmfbae.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lzqlyyzw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jyjigire.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dzfgfjse.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwwrmnvt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zneilzkp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dzslmyja.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fwfywzgl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jewjtzei.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nsfisrll.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pobdsfeb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ymogecls.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2thkllidk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2szmiqjqv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cfqcsvns.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wuqmypgs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ojbrzdpn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xajivtgz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qxoqkrhe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2svghhrby.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qkuyrjhx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2sobqdbgp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lnrthwzh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lmrevynm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qwidotri.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dybjxkjg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2csytwcks.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gvvqzblu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kdzdoyqq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2petlsepq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uhcxkotq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2sijfboyy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lgvvembx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jcqyvgmi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bppwsfaa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rqrvhhdm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lqdxeqtt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hjyhtdow.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pnwjfntj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zqhmevxv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjyxawp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jbtempxp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xmlwwwyq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yrhlhrrh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vttkjrgo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bummzkig.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pudryxbs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ydkuhpeg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2geqppwbw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rijmkcdy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bqwyzdgk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uglqyyxx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jotpfrad.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sunolhiy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bzqyynyj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dkxpdlrs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bvilgvnb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wpkpldlm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kdlhteeo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jarlwfbx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oddxwcnq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ofonmcgm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2yzncedrf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wkctwhsm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2euikbsxq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cqjygjju.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgguvxz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrzjcqc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2syxiyjor.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kzvqjsnp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfafdhgi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cmqlcasy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yitlqndz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxcfpssj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2seaczone.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2uunrbdfs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qkzgscfi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2spjcfvtv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uerwphzs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2awpolwbi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lgvtmctg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zijsspyv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbjtrjx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qyylpjjl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vndwpptv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nhrzacup.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lizcpzao.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nedvbemq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lotnluvr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snypiqff.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbhypssq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzddinn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2laxuanoj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2elxxpxaw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hjbrhauy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gnchhipr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hkrleibx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2otuwknpc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fmnbkdvp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zybgyhui.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2twknikoz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lkdktomq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2skpsnnwf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kczdqxmd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujaaghob.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jovhssac.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onecvnme.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2piksxngx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2flyjsuve.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2orwrzojv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cuzonswa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nhfntavw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2iwttrpky.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sowsazgv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wireyatn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wgjjcwmc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdqyajy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zgaucchw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnkujoll.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fntosiee.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2iowutgae.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgtvngqn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2utrfjihs.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pykcxeja.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2naomuxgh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sxkztcnl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nkadoobq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xuiwxxir.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lxlllocq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2usjcmiwp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2phubfrwk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qikxcydl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2acfhatrj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiaucsyy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zbuxmlrw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jgepgihz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npzbgxbt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2pltofvgj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vxdzohux.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2crptcnlu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jcdioirn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2swtmvvfm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vsdcexjv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fhteqnqj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2arjmkgso.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mefejvbz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2itthlpdc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vfqvihmi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ppldsiai.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lgzejbfa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2twbzfayn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fcgzurtr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jarwvkec.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vslayras.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hzclhayr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfrldops.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dsqivgqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtempoie.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhzczzpq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2giudmxcf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ykjrbsbj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jopsbvqn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qmpreqrz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2czhgsxfi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2deaaevxf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhyzabmw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfvyjhfc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgwihiav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2sotgfbsh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsunnlzs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmgfzpvt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vscmhham.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ygyomwja.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2szmtseim.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2sltyvaco.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2kyccsacx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jlacypjz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qmfzchqw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ygxaxqqo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tvxdacnx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mmewurha.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2htklkmoc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jukqdstt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bpvshood.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2shbqdwhc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nluzhkyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oqsuxdjt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tjketixd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eleevkra.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pxpubktf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vzqeyclv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cfhufdtt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ztdxsyil.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rmqphfwk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2imcjgflq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mavriwfu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dcrcdtdl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxlqctio.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvuojvpi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2plhwbxzv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2sogbpsrg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tluetkha.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpvyapjp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jmuqjwca.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bydrrljc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eldqpwpq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oietdxeh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xotungnc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nitedaxu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qualflzq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opesbnne.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2arjcvdsp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2doabrwmf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lpzdnnaf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lmbkounb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mmklfkqn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2krptgsed.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2onveufyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2klnvlwpp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eweobqob.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kkvpwylz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wnnyylml.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cpmsjrio.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjhdroqk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kllahrua.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zrmkogiy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ohdpkkht.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wtravgop.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dlsqqhwz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2smrdesqe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ngsallxn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghfnejet.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rdztkxvn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2auksgils.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ywglvdgq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aiqdtuhp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jhoihtxf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plgfgcyn.html


<!-- 参考信息 -->