代发 wailian999

Java: String.join(", ", list)
来源：http://hz.9152youxi.cn/gtkliqvxuf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinghuilouyu.cn/gtkygrxhmz.html

Ruby: arr.join(", ")
来源：http://hz.hnxiangtu.top/gtmxpanysz.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gtlypsjllt.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgtcresaa.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtqgzwxhql.html

================================================================================
来源：http://hz.jinqigfzy.top/gthzggbiew.html

[E01] 拼接字符串
来源：http://hz.pengpengdd.cyou/gtylgqwpvv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.feifeiyinyue.top/gtvoefbkyg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ppjwa.cn/gtyjxxdyqq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtejssqcsj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtxxsfluvn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pengpengdd.cyou/gtaixeqrim.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtzcolkxwd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.snrcjt.cn/gtihwunsrd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigufen.top/gtmwmmszzt.html

[E02] 重复字符串
来源：http://hz.yangfankeji.com/gtdxcbcbzd.html

Py:   "ab" * 3
来源：http://hz.jinqigufen.top/gtxnjctwwx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gttofjxltf.html

JS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtirgptqqh.html

TS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtpknefhjk.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtsijjlmzg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yongpay.top/gteohcdtst.html

Ruby: "ab" * 3
来源：http://hz.gotoacloud.top/gtlughghjj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhiwuduotai.top/gttxnqifee.html

[E03] 截取子串
来源：http://hz.xylfe.cn/gtcuzpqdnt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuanzx.com/gthodpfnvc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhengqikj.top/gtrsgahajw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtrmhpsczy.html

TS:   s.slice(1, 4)
来源：http://hz.jlsjyb.cn/gttbmdvnzy.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gtdrbmcdcq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ehwqpu.com/gtcuervrjs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gtmrwxecso.html

C#:   s.Substring(1, 3)
来源：http://hz.shangyingyoupin.top/gtiozuzzwv.html

[E04] 查找子串位置
来源：http://hz.yuanzhike.top/gtoxvfgxfo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydzc1.top/gtcxrnbwrk.html

PHP:  strpos($s, "x");
来源：http://hz.fzhhl.top/gtramsdbsh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fzhhl.top/gtjrhawukl.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtemijccar.html

Java: s.indexOf("x")
来源：http://hz.fzhhl.top/gtpypledtt.html

Go:   strings.Index(s, "x")
来源：http://hz.zhaomingkeji.xyz/gtootvbgbd.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtklajjqde.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gtohqvgtbt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sweek.top/gtsbiclkks.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aizwys.cn/gtmbeuqkny.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtlkkehbwy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gtqhdtzkym.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtyfpurnyx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gtzvwoemhz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.meibo888.top/gtuhohwscf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cqqwz.cn/gtetuddzdu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tianlin.xyz/gtwonwerah.html

[E06] 替换子串
来源：http://hz.ydjk.org.cn/gtljdaypoj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.bjfxy.top/gtkgskrqns.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtohhgnxbc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtilfwbcuz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtymvjarke.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtaeswfvgq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gtvpvfxive.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnqzz.top/gtiphigjve.html

C#:   s.Replace("a", "b")
来源：http://hz.tian-w.cn/gthjtqvrij.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtejgwbpgw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.svipenyu.cn/gtgybazmzq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fengsongda.top/gtfskefshv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sweek.top/gteutysxlk.html

TS:   s.split(",")
来源：http://hz.jinqigfzy.top/gtqheqpysn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gzhubu.top/gtbnwpulag.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fzhhl.top/gtrzbmagoe.html

Ruby: s.split(",");  s.split
来源：http://hz.guannengcc.top/gtgxzmpjyt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dianchejie.cn/gtnfalffzk.html

[E08] 数组按分隔符合并
来源：http://hz.quarkkingdee.top/gtjfdyeegp.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gtmptdvoar.html

PHP:  implode(",", $items);
来源：http://hz.zhengqikj.top/gtwjqutljk.html

JS:   items.join(",")
来源：http://hz.pycfn.com/gtscizwjkv.html

TS:   items.join(",")
来源：http://hz.wangdashe.top/gtboqyogbw.html

Java: String.join(",", items)
来源：http://hz.sufxvd.cn/gtewqygaar.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gtjalqshke.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtrpmqxnbj.html

C#:   string.Join(",", items)
来源：http://hz.ydzc1.top/gtnttuuziz.html

[E09] 去除所有空白字符
来源：http://hz.hammf.cn/gtdlvftorg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hywenlv.cn/gtmfiljnzw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgfzy.top/gtevzkwmsb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtqzkyefcn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtbbyhylnx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shangyingyoupin.top/gthpsomsmq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.daria6918.cn/gtqjrlbftx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydjk.org.cn/gtzrlidtnn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtukohusoc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtsyvnjvkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhiwuduotai.top/gtrdfrvrap.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tian-w.cn/gthlnpzvqh.html

JS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtjawlydeo.html

TS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtrodydhwm.html

Java: String.format("%03d", 7)
来源：http://hz.cheryme.top/gtvhxdxvtp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydzc1.top/gtsgiogxlv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gtcvicujgf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.feifeiyinyue.top/gthgzebnpj.html

[E11] 反转字符串
来源：http://hz.gaohongyu789.top/gtyypqzzrs.html

Py:   s[::-1]
来源：http://hz.yanxiufei.cn/gtcwecbcjc.html

PHP:  strrev($s);
来源：http://hz.cdnleiting.top/gticfwznkp.html

JS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtdqdvdimw.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtfdbwaois.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtmjpsjjbw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.vqdsnc.cn/gtvqkfvtpk.html

Ruby: s.reverse
来源：http://hz.chenzaomai.com/gtdkegnabo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtjawefgly.html

[E12] 统计某字符出现次数
来源：http://hz.vqdsnc.cn/gthifiwcpw.html

Py:   s.count("a")
来源：http://hz.c1oappe.top/gtylgjhjps.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gturryomhf.html

JS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gtdmtqwepm.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtfskdcapp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gtjhuofqkb.html

Go:   strings.Count(s, "a")
来源：http://hz.jlsjyb.cn/gtpfinqtjr.html

Ruby: s.count("a")
来源：http://hz.yongpay.top/gthltnrtqn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dianchejie.cn/gtthoyqiio.html

[E13] 逐字符遍历
来源：http://hz.quarkkingdee.top/gtmfwvevnm.html

Py:   for ch in s: print(ch)
来源：http://hz.gzhubu.top/gtmmmmqwam.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gtwffpwpss.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtoregiwtf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtprehetmo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gtsdcbzhcj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yueranfly.top/gtoepnzorv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtjafkncqr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuanzx.com/gtnpdifbpm.html

[E14] URL 编码与 Base64
来源：http://hz.yuxming.cn/gtnsoixmju.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtmjsntcnw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guowangkeji.top/gtlxucnbxu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gtvvvtuagw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.bjfxy.top/gtzcfuclao.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxinkj.top/gtgvvspfkl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shzxlz.cn/gtljuadnrc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.0kj1m.cn/gtuwpcmrqf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtbxxemwdd.html

[E15] HTML 转义 / 反转义
来源：http://hz.gogol.net.cn/gtuywhfiyw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gtctprdfei.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangtech.top/gtlndeqodg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shuidangran.top/gtkufkpawl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhiwuduotai.top/gthqgfzupo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gthobjbfml.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.smart0.xyz/gthhasvohz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.iojbl.cn/gtoglvgfmp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangdashe.top/gtsopaqhoo.html

[E16] 数字千分位
来源：http://hz.nanxinkj.top/gtyqitgzgy.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtezrbotpb.html

PHP:  number_format(1234567);
来源：http://hz.yongpay.top/gtzonizzyu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtplfyqopy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtsmuimxyu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtwomghjqs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtfnhhadpq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sufxvd.cn/gteognfhit.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gtugiblosu.html

[E17] 首字母大写
来源：http://hz.havefunace.top/gtvowbueeb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.feifeiyinyue.top/gtnskxuxxo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtdteskjoc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtdmjdfmzk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtlcrmrpnb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fengsongda.top/gtnrtfaktr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.birdmap.top/gtktnibxwo.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtrnndkmna.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gttwcifana.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gtgvuaadxd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinqigufen.top/gtpyqwvivg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.havefunace.top/gtamljclrh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtklnwvhcy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gttxzspzyg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtwlhfayjf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtlfyessbl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gtywwohstl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dashuyun.cn/gtttawzryt.html

[E19] 多行文本按行拆分
来源：http://hz.dianchejie.cn/gtednycxeo.html

Py:   s.splitlines()
来源：http://hz.sxryk.cn/gtawdgwzgg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuetiantiany.cn/gtuytsrttp.html

JS:   s.split(/\r?\n/)
来源：http://hz.daria6918.cn/gtjeovkpjn.html

TS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtdxeljhis.html

Java: s.lines().toList()
来源：http://hz.yj202588.top/gtglogvoaj.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gtlbpgkovw.html

Ruby: s.lines
来源：http://hz.cdnleiting.top/gtfmingadt.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtuppcjpvg.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtjplgpovz.html

Py:   if not s:
来源：http://hz.jqgfzy.top/gtsvzwvnbk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sysykeji.top/gtcgpljzuh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cdnleiting.top/gttgugffdi.html

TS:   if (s === "") {}
来源：http://hz.yueranfly.top/gtffqjemek.html

Java: if (s.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtuikggrht.html

Go:   if s == "" {}
来源：http://hz.hywenlv.cn/gtdbfxjoju.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtsheazgil.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jyoumei.cn/gturxksrkn.html

[E21] 超长截断加省略号
来源：http://hz.dianchejie.cn/gtqsslxkwi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtaznfuldt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtytcufrfc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtdogpmcgy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtyylwoooo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtrozheslz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj202588.top/gtstvdyyhg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.mhx1999.top/gttzqtmouw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xylfe.cn/gtggvryhzk.html

[E22] 字节长度与字符长度
来源：http://hz.sxryk.cn/gtkdznhjqa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sufxvd.cn/gtkuppbxla.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gtlqarbwhi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtoxrcgkqq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtgetgvrfd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guannengcc.top/gtoyjdfwjv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jlsjyb.cn/gtegsnooof.html

Ruby: s.bytesize;  s.length
来源：http://hz.snrcjt.cn/gtkjfzwsmn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtxrxqmloj.html

================================================================================
来源：http://hz.nanxinkj.top/gtgsqctjkq.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtbsgrpvup.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtnovykmbi.html

[F01] 读取整个文件
来源：http://hz.yanxiufei.cn/gtualyehcg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.svipenyu.cn/gtpktfsboq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yueranfly.top/gtylanaryp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nwbrower.top/gttukjzboh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guannengcc.top/gtfiehvpsj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtmmnuzqyt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtriyjvkyx.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gttijcnmnr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtbirbgzvo.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtlecslzmi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtfafldbws.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gtotmbnvcd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gtfahuwkkj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtmxbbyqgn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtcbjfemts.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ppjwa.cn/gtqtcdbubl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtzrhquuir.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhongyouzk.top/gtqgzfempi.html

[F03] 写入文件（覆盖）
来源：http://hz.iojbl.cn/gtuktzurgt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gtadubrclw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hammf.cn/gtvofgposc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtrbqyoslu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtgdwdhwam.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuanzhike.top/gtwzxcgbcx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gtdahimluv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gttkgwngve.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtjlipfpov.html

[F04] 追加写入文件
来源：http://hz.xylfe.cn/gtbdfruhxg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnqzz.top/gtyqqlnjtr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xingfuxueyuan.xyz/gtwlcdqcxy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtustralyk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtwgzznwps.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ywan-chungtsiang.top/gtjipmxfep.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtbnmwyowa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gaohongyu789.top/gtnsjfhlry.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinyuanbaomall.cn/gtlwkdcadd.html

[F05] 判断文件或目录是否存在
来源：http://hz.yangfankeji.com/gtwuyjsaqo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258888.top/gthxhwuhtr.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gtpjeyomjp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gttendscwu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gthlxczqma.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gthyhtedxo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hysaishi.cn/gtkeohymmb.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtaghbaaza.html

C#:   File.Exists("a.txt")
来源：http://hz.yonumen.top/gtlnpeilyz.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gtubumjfgx.html

Py:   os.remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtbkbkjiaf.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtzzlrtsal.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtltkzsvrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtoamqtloo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtsbkrcunr.html

Go:   os.Remove("a.txt")
来源：http://hz.yonumen.top/gtvviaowev.html

Ruby: File.delete("a.txt")
来源：http://hz.yuanzhike.top/gthfqjnrzg.html

C#:   File.Delete("a.txt");
来源：http://hz.yangfankeji.com/gticcmaihu.html

[F07] 创建目录（含多级）
来源：http://hz.ywan-chungtsiang.top/gtslhexvtm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtdejgaffh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ppjwa.cn/gtxqojibmi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtcpmnmzcw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtvvcbenxw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtjzfkbqic.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtxlarkykv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shuidangran.top/gtxdtgpjhr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daria6918.cn/gtdfqwfgbr.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtorvmrjzy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtfpbsyakr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yongpay.top/gtjulghoxf.html

JS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtschzmlke.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtomxoqhwq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtgpemivxw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtfelagali.html

Ruby: Dir.children("dir")
来源：http://hz.dashuyun.cn/gtpjpqpmxy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.smart0.xyz/gthwbovxxb.html

[F09] 获取文件大小
来源：http://hz.fengsongda.top/gtoclnqqcq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuetiantiany.cn/gttvwoutwv.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtuholnyle.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtaxzpbkhg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtdzptkvob.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gttjjalyhm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydjk.org.cn/gtvcbouexw.html

Ruby: File.size("a.txt")
来源：http://hz.gogol.net.cn/gtejntbsqf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnqzz.top/gtvegwetyn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtyaztilyb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtimeiuomt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.52xcode.cn/gtnzbkfpvw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtzrbhfwfh.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangtech.top/gtqirfnnrg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgufenzy.top/gtyyrwjewp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yvedp.cn/gtfeclhxgp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtqrqfyaxn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gteuqvcbzj.html

[F11] 复制与移动文件
来源：http://hz.hywenlv.cn/gtufgkkwdh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtdyppkegu.html


<!-- 参考信息 -->