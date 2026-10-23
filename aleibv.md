代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yqhpefpw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3weenalgx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uqtnofia.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3valkccht.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jxnvxaxb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mdtkrjtr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ixrlwnnm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rhaqffkf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tjyqyioa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xcsapsoe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3thjnjyje.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nmedmlnz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bzgrqkmv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3areuvauh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gvameydr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rkunqhbv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3guvpcwot.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3epqhgqdq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vffwyefq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bdbdfjff.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ouhsjumc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3huosdoey.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3mkgqpast.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3piijgdti.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3paygimbm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mgcszlqt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3niortgoo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yiihpiep.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3irgbdlgc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kicrmthu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ovwlavyj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ackjtxtq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aempayqn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3znnfxhct.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hwpnzzbu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3aqxnbqcn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hxccszpn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nmhfrfeo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nedjozjw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tyzzfxpy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3eicmivnl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxghawvl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wisojjro.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3npxmnujv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3anoicyoe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pdmzpjwr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uetzudpb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xhkbktid.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cgdfdwdp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mtwwwvcq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ppwptjwm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3beookwol.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ykasvyuh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3bxfxmupp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ctcuaeaq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3capwwlhb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3clcvljvn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3trqfqkgt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3opryjhni.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gvlesvcb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gphfwmhf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dhkmhdbc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ccdytlgu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zofczfse.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3awhygqzl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zgceqhai.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yrxwaqzz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bhxyhhxp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3greydpnh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cihpoazr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xuwsfopo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wylzvkin.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tamfvyez.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ruqhsgoz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3esulauxo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lnrevcov.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3axensuhw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tcwijjxb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kvldloia.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3andnwmfy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jxxtabrj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rpasssje.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tuaftcsh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3indweurg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xhxgghmq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqngjsht.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nhzoxryb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3djtxdfpn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bgeujlio.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iphpvfsb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3vycwjrpn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3casxqgkm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fdvlnaix.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ssfoduec.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vwuulcyc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nwwgague.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zqhazmfh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ktxitzqg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tfdyadex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mxedgkmm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wrbpgaig.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dhlsxgzg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ppjsyhek.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hgvezjdc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3khpufrkr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hypzkfsv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlrcljmk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bhmlxdjl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ayysxyex.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qequbvtw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vsctiwcw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ejgbbhff.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cxdamsoy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3loqhuyso.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fumgzjcm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mrlwmzyb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rscneklc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3omdnayfi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3blqsswtk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zqhqoqil.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kxethocj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rlptpeba.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qddgaeaf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iikpyfse.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xfwrvtif.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lpazovfj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lorhgjfs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxloyjmi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ogrgkryw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tgslnbwy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3epxzmulb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eppmwfwd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3twwnltzj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvesacy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpuuknr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ldedsekv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kelchdun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zyurykax.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3krfyfsqk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wipdcpqs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3exyewyty.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rrquuwdg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnpdmbzt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gcxjbpts.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhywfwmp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hizddqnt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bwgttdnr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wwxjtjth.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3joimzlcl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ladjunzx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ojqiotua.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yerdwudb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rluoynur.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eekourmf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rqejrbsa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vdrkqqfp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3acaybklj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dmwewpdg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3drltjpim.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rrqpjjih.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oiltjuad.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3slgifruu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ihcxqsjd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ovgcqxyu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3grqqibxu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qxdnqtel.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qnhfxrei.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dycxyhdg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cjgpiofu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vqcnjqbd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgqfveiw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsklssjp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pikbsrhv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3chuskmxw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3agrgsqet.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ftvjlfhg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ncndtzat.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3peruhwws.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fczndhvx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jnguvuog.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pjmwgbzo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3omvzajwp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nhkgttux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zurihain.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jujacijt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gltcwcqg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cxkxmypu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uccxemma.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3umkdrujb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xeonorxj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uiafmjis.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3prrltqui.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gyscdcuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeiqndwm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vanxcjgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mptsdcel.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ruylwxud.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xpkfyxdj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ndysrnof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3svwnmgge.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vvffqcvm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ewyqoxmb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3spgwcdhe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztvnqkir.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3grollcqi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yeelgvdv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3muddkjqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3frbjmkac.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bkeimiwp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iuwwnkkk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fndtnfwk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xvauhkwf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tmakayuq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xkvmgjeo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bgnjrmjp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tygbzsvu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gzfeiwvo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nppqvsmz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gnyuickk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dajmldal.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3luemidxf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xdwttkog.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lorxxtfs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fimmcfqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3roakaogy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mqwfybzp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3utrijhkd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kctndwhx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zbchulzp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kjauspok.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sanomlzm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tdgwotsk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sxaqdahs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pwtwuxhg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3snnoqqrc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwdntpaa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vellbzkz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kcgkqjnn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yfonqmqc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slupuyqv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uspgnxpb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrhgwqea.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgkbrksm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aliqiiyh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbwmqazi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixltmrfn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lbcnxrhz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjknhhjd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tezpiqhs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mivraqhp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mxqmvuik.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xectlgxu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3laragkjg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cfxjsbax.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xtitomny.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3boijklkk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ytfknzix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qnkayalk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gfukmwlo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sdwvhzhg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nhgpxvlz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3grrvusce.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fptikazv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lbfyzerv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3npcmbrei.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cjuiyxhs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kincdahn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3krrvdbzk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3oxkzdtsy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wbhkqqou.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gjlvrxbw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zgekkffr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cosdwlao.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3utzybdct.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xtjjtomg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqdoiklb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ikfttjmb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ijoypgkp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrwmwxhm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3svlsyfae.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3unbtfrbo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krarofvk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ekdrqhvt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvpiudua.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbhzenfm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acwqbfxf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3uysjrikw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqppdfpq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3frnzduli.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3joltzhwt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnwktaxn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cytedozb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tzekmflc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjeejfmx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ekofmbjn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dxqrktzs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tvvusbhx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yokvdygy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bltkenrz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3oliklfwf.html


<!-- 参考信息 -->