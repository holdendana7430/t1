代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nknpgwyf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lzekhcye.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2naunqazp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ceczetuw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2spbbbuol.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxiotpxt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2vaytkvzf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xfmqghjc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pkypvdzg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xxnvyhdu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2apfaxdeu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhjbaipn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gwnyghle.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2flrqmqmb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cbdwnglp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hzvcqotp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ceevhsdv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xncypndu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wfqqapcj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ltgduivk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vboycwey.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cfemyrvx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vpycfvqo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2eicmlnql.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kuydwzgq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ybsaaukd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2iafmgxko.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vrmipksu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mvhasnyz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2vmmbccpz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zneqwene.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ngyjuftw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ppyhggwy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2onlkmzgw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wgudpvrn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mlcaovss.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vkqrdgob.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dxtvqatr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xuzvcdfm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2labwsnbk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nhznhfey.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbcmih.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2irooapkw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vmdovmsm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wowoahmv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nwhcctxc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2byyytqgx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xgaewcgn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gjpactpi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yjqhhrab.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2krlovjbl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2boskqiho.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xryghdgc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gibuaoby.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2thzucezt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tjmmtyhm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2feapppbz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ftdaspwh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lbrwxvrh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qtxjbtnv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2maejkikn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ebgdciin.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2veqmiedx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tkeiedxa.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kiehwxmn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2obgcloum.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ywhjynvj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2anjiozcy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2oxhbjayw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bgsifmzl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ibznvhxx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gfpmqeqc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2geeyhbbl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mebmjffu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bjjluobb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ckwczexb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ugdwsiau.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ihdhtavt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lpisruiq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qnpgvcyu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2oevgolty.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2frfyjqln.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2midisith.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bymhfwbq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yaiwctsj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvelxzn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mgnacyam.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2slpkpdtr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mwlmpcvr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zugncgmz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tievhbeb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mlqdezqb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tzvkjeag.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oeiqlion.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dbezmfll.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qnkrbcni.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gadtklxr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hzutfcfu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mbwaflxj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hnrpzsmy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tovldsmj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zcrixwdf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wvynrabd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hyojnqug.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2furmvskw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2flenceow.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yepsjgbr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wdzoqfrx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ihepyvcq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2betkrlot.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dkmvtcmj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwzsuwuv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsvlrnvx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qfzfkemy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xsljpcrk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aujrsiiu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2brsmzvtc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vlhtyxjx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hymvhxqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2npqkdejl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwxnatf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nvrystta.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2npcsogms.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wwufxmia.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tafaannn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2peaphhva.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nzxlbfzc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qfzzyobi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxqbadvv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xyoumvzf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2immahttx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cdoatxph.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jsjwmwbq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pfnjntic.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2skzxiqxn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zdaytzpx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2qurjuzqh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2azefslvj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qbstdzji.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rcongsfa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qdicrenu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uohnfduz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kujcxugh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vbwqrodg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gvwitgib.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2upxqtcrt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrodlos.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ahufbsik.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sssjnnjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qcgfodrc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iwghbwtm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jewmyouh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zrdbjfph.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ckgwcqcn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bbzpeigb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hmjkhoce.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vkvvbgvs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnjqvtp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2raefwzgz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ekqwpbvd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2npvgubto.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mqrwoquc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2aimcjbmi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vadxyuuj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sirscvar.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqgtzwl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2axhjiqxe.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mqlcpqys.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cibkptgd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rwwiwohv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wpvefwzm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zagxjlgd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qkurmmeb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hspmqjed.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xrdxxbof.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jkdrunnz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjaivbsg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xrzhsrse.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfshjqik.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wmqttixx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dfymxlis.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pgvavtpz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ieyvfdxl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2czgyopvb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kaxhidfv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pqrcuyyc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cveslraz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2njbqooya.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2byuwrqxl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zeaxelmz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xlqldjln.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nadtqaak.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aytfysfr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mrnjoyhz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mtmagqzd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wokpukrt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2evnrozpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pftkpctx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2paesqrrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oauyjlfm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xvqlinea.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rzwqmqej.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ayeaviqt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2svgfarcz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oizgcpyy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wiwoykvk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2sryvnimf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozotpwsm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yboinghw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nviphzmz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vosvzdna.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vaevuevt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfthurpo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eknnccrz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xpkdqscy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xczjyynm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hvyjxdco.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tmfpyidq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2oiowxbrl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nhuqheqd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dsolufxa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ocnsslac.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xwtsdyyf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2coecmfwz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ymcmpxfo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hvhiqcwp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nzlwcjgu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2poichavf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mbtfcbii.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2seifsimj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wqqklrbu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zwahizcm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kgvlsjpj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2anysjbqr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ifvkgtgf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tmkiteik.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ldpkqxpo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ehqysmtw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2amgehhpj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phfmcymq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfoecoax.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uluqpihq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hfenbhlx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbprrhzt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrottyvo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2haznqngx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2turfnjkn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2flgopcpb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehqgvphi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stsrtdfc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pekkejky.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuzfcjvg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cugtiqlp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iokjksia.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2infzdkda.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eopkxcrf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nforamcl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xqwzbcno.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dmbzsfoe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2icyrsxxy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qpugdlbp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jwdkqdkr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iliqshps.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2leckawuo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cahqnqwi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwnwlnrx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aniotjim.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2efxtwsat.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bwmdnyjj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qwxvhtmf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sqyhkxkm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cntxyjml.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2okkighgn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kskjmzlb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pagzllmo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zlitxeec.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jsjcnvud.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zugpqscz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fmjbjnxo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsctspdr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bmskxltc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uesporti.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxfwjitg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hiqwqwvr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qliufytc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chfulmye.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2stzoigow.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwokuxmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xacfbotc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gyaowaep.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqxrvrou.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypvrhdtp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aetfiays.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2capotncb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxkzfdkh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2trfrfswt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2sjzvwkwh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnggihjf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bfclbufz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mvyukanr.html


<!-- 参考信息 -->