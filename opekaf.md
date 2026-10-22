代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vhjrvyka.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mybaldnn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wkjacxlp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qywehyys.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nnbexfln.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qberiekw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pukugoqq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rkopguio.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2egxjihfh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iboljyiw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2iuasfkuv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nrqlzvru.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwmqiah.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ikwkhnir.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufudaruw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kuxykwpz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ffecinvu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ljjscajz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zoksyzfi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lpddsbxc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hfebresc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eybkikog.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxrogjv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bobsktag.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qnpncsxr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytebcmls.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kumpurnd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fihdxpok.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hwgapnfs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2cfyrmifq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2geefsezz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2khgqkqsh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2edfnqieg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2drxxhrgk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jrwqwrax.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2acfeginx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jyoivuxy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gdnpredj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ajfttjyx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ontpmusp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oqrcxksj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2frqejmoj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fyguramk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eypucfdj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wubyeasq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwzyckuf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2uifhgpvc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lxocusgv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ttdjqcfj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jgmfrwtv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2damtvxyt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxnsiopq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iglwazap.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2feclkblz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vaccuxwm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2auehwapa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uukkcuzo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yqusjutw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wknsnjkc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kngdihdi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xgdbsoxp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lbwplwgh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hrvlhbkh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hcswpbpx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hcjfbnxn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cgnejrcu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sxcvkygd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gdffhwif.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gvvordbv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2prrtxafo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qsteqtvr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mdtizrsn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgehsnq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xgzznmkm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pqiuzvcu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2motrxwiy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iwvpnfhv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2eqeqtard.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ddzytsvr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jzbkdqgc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pdijryzi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ddhapiri.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2aotzqihv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kkhoseck.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hwmvwalg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sogfvstn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ymisckcu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xmraautx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kxjflrxr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdwbpiad.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fawyrlxk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrujsves.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nzpjifsr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nfyqpybw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mntfyjky.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2juumvurs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xmhbevif.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yjjuzumy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vjilhtfu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lwuyfwuw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bhzcqlnx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ahlrugoa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bvtflekq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qzokdsfn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bmxvughc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2noqjzuyh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2eyywpkhk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lksaixnh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kxxxyuki.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2snzzcxso.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrqtyefm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qnbitkdt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rrwhpdwx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sutgrxhi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qlakxrix.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jnfybpti.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2niuzvxhi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ubwkzmfq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdnbgaxm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pujjhfvu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njhcraxm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uglredgo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qbdxkpug.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uptvogrw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2itsxwbpc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ubfnnxdp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xaioabrk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vgkixoic.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2octawooi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fepbvuqs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2aojlttdd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgcqhdwr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gpnkqcka.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xenscvgk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vxyoguyb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2tdxgiqpv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ttuoxyzx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nwlwbxzo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lgldzqfk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nbpfwqlk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2emoembch.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2swivmzeu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qsvoqvwb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2exnoztbp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tjwnesbv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tcaapdfn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vltloqmt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qqfmofmo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wfynzvme.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hagjpzoi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2otdxvyqi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ibpklzqf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zcgehzxz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jxmahtxb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ixuxikjl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dcjqukwl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2muoydybk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mhitmxkw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ajfxvuzh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nwjgemqf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddbgaazb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cmxlbgez.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kxewrgli.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2krakxjvt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qcvvurrt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gopwtiau.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gozimvdj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nyfuuivq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dnkoiteo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jwrnnefq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ksqjssdz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2msokdbts.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nghmqvyd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2snwuuahu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2oahnktvk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwzgohlt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mdxlzblu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qfrbbzdg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2iuqhctxw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qejfxttg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rcoqbvdc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dtwclgqi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kccmjndl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lwsoejlb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2txsjoajh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vyncwpbb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ogrzhzca.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2inttlsdl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2imaspsyu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2caqknhnh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nqteaqtf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2frikejjh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2isoaagxy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jotqvomx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wkeycucm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yulbplub.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qvavwnde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knfwjuyl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tthxvhqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouogokhw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2knpvrjef.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vksxpijb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pocrpdui.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bogewcma.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wkcrqkig.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eckqlzzp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nflohyuu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2psrbjdnp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vimqwrmm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mzifkikh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2sewxvnyf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2aqkjchro.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2leoxqbpy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmndgtcs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2itxjprlf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rriktpbn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dibfhljp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilkvcwbd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dysduocx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2elcaxknn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oujotcso.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gmdzoutk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aqifxpvu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vqqomkwd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xhydzzlj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sbyzevgm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sxtsvepu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nngmafyv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ypmhmswt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cgkwlhad.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oovlbmlu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hfgvplzq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fspagpbu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jjbbnjmm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gacttyvd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oieqibin.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xapnsnhr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qwzrfvgs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yrluvstk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxcvpirc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgmmkqlx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ogojpkpu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2iolshlsh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gydceoxy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2culdqpmd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ughpyjxm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtorcgns.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fofdnozk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zangrizq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akcbhdvo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nqixuolb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kddlehgm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uribtvmm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pemiwyvn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mjcwxzkv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2frvefkck.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ewxnarey.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wirfplgs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2onjlsqly.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zzuwbihx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2oqcssetr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2eydwhliy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vkyzhmkg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vtfvqkso.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pzdrxziv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2czdviucq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wzyueguo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gtimsqsb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lbsebuab.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dpwyfufy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jvdbitul.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cqptgxtx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2twzkdukq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugpnnvot.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2svxqylau.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hjiemcnz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ljuuzrcm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xbtnyskg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2iikwckwn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzvwsebp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ivqbgdmz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jblsbwui.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnxjkrbf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2joeepisd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvvxhieq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqnkajsp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xmubltyn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ontholgc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wigoibdw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqsqayrf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pljebyfp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rznshshr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kqopwblh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gaotgbje.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbtffwld.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lodlzcux.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rknoacmq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2czfhlhry.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2omwtkwlz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2sdlcxieh.html


<!-- 参考信息 -->