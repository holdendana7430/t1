代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gttwphxdmr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sufxvd.cn/gtatsgqqnb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtbplvvtrk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtkdhthpwg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.wangshuangyany.cn/gtihtsohli.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jiagoushi.top/gtttkactir.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtuafddjhc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yvedp.cn/gturlzevjd.html

[E02] 重复字符串
来源：http://hz.fengsongda.top/gtkjwyvlnw.html

Py:   "ab" * 3
来源：http://hz.svipenyu.cn/gtdhczizgs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtkokkxjwq.html

JS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtmfbkgglo.html

TS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtramjxpur.html

Java: "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtjjsywmhs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yonumen.top/gtcjwbbvqt.html

Ruby: "ab" * 3
来源：http://hz.yj202588.top/gtgetshwab.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cheryme.top/gtzwqyoxwc.html

[E03] 截取子串
来源：http://hz.316326.xyz/gtvotoiktd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.bjfxy.top/gtlpisashy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxinkj.top/gtuzdbpoea.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.daxiang520.top/gtexpijduy.html

TS:   s.slice(1, 4)
来源：http://hz.yuanzhike.top/gtgtlyrcuu.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtihfvperh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxinkj.top/gtcdqaermm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sxryk.cn/gtgnwstwpb.html

C#:   s.Substring(1, 3)
来源：http://hz.vqdsnc.cn/gtrlwikwtv.html

[E04] 查找子串位置
来源：http://hz.vqdsnc.cn/gttqhhzpyq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtfnfbkacp.html

PHP:  strpos($s, "x");
来源：http://hz.fengsongda.top/gtoeocluwr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangshuangyany.cn/gtdccusnbw.html

TS:   s.indexOf("x")
来源：http://hz.yongpay.top/gtlscquvzo.html

Java: s.indexOf("x")
来源：http://hz.sxryk.cn/gtsxmozwrg.html

Go:   strings.Index(s, "x")
来源：http://hz.shanyushiyangtech.top/gtulqxuugk.html

Ruby: s.index("x")
来源：http://hz.iojbl.cn/gtuwwwcrug.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtwzkdwpel.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jiagoushi.top/gtwrpkygwp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shuidangran.top/gtffmzxjwq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cqqwz.cn/gtwqkfhwwj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.svipenyu.cn/gtdfmptnha.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtrwuqapsy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtccrjyqpm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigufen.top/gtksybpkkw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtyvgyqmmw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.bjfxy.top/gtirpthxdm.html

[E06] 替换子串
来源：http://hz.haohaochexian.top/gtgfrmfzno.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gzhubu.top/gtxzctyklj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yvedp.cn/gtlgqjyxzi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtbpuoqgdv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtzwflnwlz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtnzdigsxq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aibaodan.cn/gtrtsemysx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtjjjnmpsz.html

C#:   s.Replace("a", "b")
来源：http://hz.andypj.xyz/gtjcrwtvmo.html

[E07] 按分隔符拆分
来源：http://hz.aibaodan.cn/gtoncurcet.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtxtitggnr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtfmvkyoxb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gttmlulatw.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtpqgctbbr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hywenlv.cn/gtvtooqriw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sxryk.cn/gtaamkcmyn.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigufen.top/gtmcxdtjot.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhaomingkeji.xyz/gtbcmdpqjh.html

[E08] 数组按分隔符合并
来源：http://hz.haohaochexian.top/gtkyfhasob.html

Py:   ",".join(items)
来源：http://hz.pycfn.com/gtfpjetddf.html

PHP:  implode(",", $items);
来源：http://hz.xuetiantiany.cn/gtzlpcuosk.html

JS:   items.join(",")
来源：http://hz.yj202588.top/gtqvoyhiyk.html

TS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtocvtpvxa.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtksturqmr.html

Go:   strings.Join(items, ",")
来源：http://hz.redwolf501.top/gttzjgbdmd.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtoxjaflbd.html

C#:   string.Join(",", items)
来源：http://hz.birdmap.top/gtouikcqqy.html

[E09] 去除所有空白字符
来源：http://hz.chenjidiqi.icu/gtpsvitaox.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangkeji.top/gtbwpimtky.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenzaomai.com/gtsnxwzebu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gttfskqmya.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangdashe.top/gtaejhicqb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtttaeyqdt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sysykeji.top/gtopqapuyg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daxiang520.top/gtkpfrjdvo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtwvgmapsf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.snrcjt.cn/gtvboykxvd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gtcpohsweb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hfpthk.cn/gtcshsbwwy.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtfvvtjujy.html

TS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtsriysnko.html

Java: String.format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtntherkfx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.daxiang520.top/gtrsaimcoa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cheryme.top/gtertknezr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gotoacloud.top/gtagmhcepy.html

[E11] 反转字符串
来源：http://hz.jiagoushi.top/gtdmibbocr.html

Py:   s[::-1]
来源：http://hz.snrcjt.cn/gtpeqftjlo.html

PHP:  strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtyozscxnj.html

JS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtwdugdvxe.html

TS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtnirhyrac.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hfpthk.cn/gtfwcvmpsi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258888.top/gtbfqdojzd.html

Ruby: s.reverse
来源：http://hz.jyoumei.cn/gtjrypgbcj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtbdswxcyw.html

[E12] 统计某字符出现次数
来源：http://hz.zhijiandao.cn/gtuorseytq.html

Py:   s.count("a")
来源：http://hz.hywenlv.cn/gteppufbjr.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtiqxjpsii.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtcsqhkimc.html

TS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtoricsvcf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtlhfqckdn.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtlfmjrqev.html

Ruby: s.count("a")
来源：http://hz.ybcxt.top/gtufgvxihd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yonumen.top/gtndihtlzu.html

[E13] 逐字符遍历
来源：http://hz.cucudq.cn/gtxmiqqaey.html

Py:   for ch in s: print(ch)
来源：http://hz.gogol.net.cn/gtytvfduqq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtmdowyfhr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtdizqwbsb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ywan-chungtsiang.top/gtfbzwzdvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gtpjxryrrv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sxryk.cn/gtejiwddyd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yanxiufei.cn/gtqzkgukir.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtpgmsozrv.html

[E14] URL 编码与 Base64
来源：http://hz.yongpay.top/gtmbypafdb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hongshengwenyu.top/gtdyehcvpo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gtfhcsnpsy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sufxvd.cn/gthmsfotrn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhengqikj.top/gtzkzdhwju.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hywenlv.cn/gtursnqebr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gaohongyu789.top/gtmnzygbom.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtaxezvaat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hongshengwenyu.top/gtdpbptcji.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtadpqgdyf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.c1oappe.top/gtmovvgesa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.9152youxi.cn/gtxagdczbh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tianlin.xyz/gtkirlndnf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.316326.xyz/gtdsvrvboo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnqzz.top/gtrozcemkv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhaomingkeji.xyz/gtzuriishx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigfzy.top/gtrfowerzh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yanxiufei.cn/gtiglouyri.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtevamxzbx.html

Py:   f"{1234567:,}"
来源：http://hz.tian-w.cn/gtfvwyvxve.html

PHP:  number_format(1234567);
来源：http://hz.yj20258.top/gtrfcnhaam.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gtmptmhohy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtfqgyaetx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtwlbiylmo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hysaishi.cn/gtbompmdrc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jlsjyb.cn/gtsulxlcqm.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxinkj.top/gtvqbweyxg.html

[E17] 首字母大写
来源：http://hz.ivvv.top/gtnxvthfgi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.aizwys.cn/gtmpyhvhse.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxinkj.top/gtowzdtfzb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtjhchbrsy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gtsyoyypbx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pengpengdd.cyou/gtgtgjrivh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtfzthyajp.html

Ruby: s.capitalize
来源：http://hz.guannengcc.top/gtovkhhlof.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gtpgqqqocu.html

[E18] 模板占位符替换
来源：http://hz.jlsjyb.cn/gtlyogricz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtjgjqfcbx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ivvv.top/gtctbgvbon.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtpjxvxuod.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtonombmci.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sufxvd.cn/gtrwutpvaj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xziqi.cn/gttwohgyir.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gotoacloud.top/gtoalypclo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gthrtdfwnd.html

[E19] 多行文本按行拆分
来源：http://hz.hnqzz.top/gtgfndtemy.html

Py:   s.splitlines()
来源：http://hz.shangyingyoupin.top/gtnqxwxcju.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gotoacloud.top/gtfjpkjzee.html

JS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtogkpyukl.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtvkqorixn.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtgekpxsfs.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnqzz.top/gtpbcoujsj.html

Ruby: s.lines
来源：http://hz.9152youxi.cn/gtpjiffdmp.html

C#:   s.Split('\n')
来源：http://hz.tian-w.cn/gtnrnfqugc.html

[E20] 判断字符串是否为空
来源：http://hz.jianghu66.top/gttqpspwdq.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtoxxtfaiw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtiespuahf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtgdegarqh.html

TS:   if (s === "") {}
来源：http://hz.aizwys.cn/gtbhejxxio.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtbgmpnefh.html

Go:   if s == "" {}
来源：http://hz.nanxuanxn.top/gtuondwgwa.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangtech.top/gtsqwzppga.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuanzhike.top/gttcrrpcxn.html

[E21] 超长截断加省略号
来源：http://hz.yongpay.top/gtsnlrtdqy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtealyyiqr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dianchejie.cn/gtdabezvov.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtnflvynip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtawtzedjw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gttoiwdrak.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnqzz.top/gtmyqjsory.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yongpay.top/gtgzbsqvke.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yueranfly.top/gtkqhiqdur.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtzgixxfli.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtqkrrybky.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258.top/gtfwokgqgo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtbsexxutf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtswsddcnk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gtolstwull.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtmhnwfmbj.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtvedmifnu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gtbgdtlqif.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdtgtaeba.html

F. 文件与目录
来源：http://hz.aizwys.cn/gtdlokdsaj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqjxkhcit.html

[F01] 读取整个文件
来源：http://hz.snrcjt.cn/gttjazjgpb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuanzx.com/gtgfdfyncu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtwpolwcxw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gtvupdumuv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.aibaodan.cn/gtcllyuehe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtivfysrkv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhoulong.xyz/gtdrqrptfp.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtjpypauod.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtqxcggokm.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gtpzawvita.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhixingplan.top/gtinbzvuns.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sweek.top/gtziwcfqnu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gteookvobe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtwlwrdhwy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtzgtbiqlo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtylnilnco.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258.top/gtiwmnjnkn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hfpthk.cn/gtfetxpxcf.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gtibcjthyz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ywan-chungtsiang.top/gttzvufwtr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gteaxvwmjd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtxlrmeava.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtxwjwrtps.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gtdkupsubb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gttwaulgbo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydjk.org.cn/gtydcjpvmv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtpieiigap.html

[F04] 追加写入文件
来源：http://hz.yvedp.cn/gtaasxkpyk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtasurosap.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gaohongyu789.top/gtnjmbeikb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gtegtvanpo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtnfrihsao.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhiwuduotai.top/gtkkjjdzpe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtlpexqqcf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenjidiqi.icu/gtwicrikor.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtsvotuglv.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenjidiqi.icu/gtlcbactkj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.bjfxy.top/gtfpdtlpki.html

PHP:  file_exists("a.txt");
来源：http://hz.jlsjyb.cn/gtpgjxoqoi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtckdmlrwv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtuuzudcwf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtzffohrde.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.smart0.xyz/gtmmksuvep.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtikmxnzdw.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtsyflstvy.html

[F06] 删除文件
来源：http://hz.kuanghao11.cn/gtrktytwnk.html

Py:   os.remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtmfypoesi.html

PHP:  unlink("a.txt");
来源：http://hz.tian-w.cn/gtibzkqglv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gthnrcchdi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gttbdebaqv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtmpahpbnz.html

Go:   os.Remove("a.txt")
来源：http://hz.daria6918.cn/gtmtxfajqb.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtfngucubq.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtfouwoxsz.html

[F07] 创建目录（含多级）
来源：http://hz.jinghuilouyu.cn/gtfpkphvwn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtqashfgjr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtdxepdgnv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gthyjtfzuz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtafxyqhtz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.birdmap.top/gtjhbpyzvp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gthmmhnhxv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtntqkdrrw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gtqouhncny.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gthpxnnfdo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gotoacloud.top/gtccjlrvld.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fzhhl.top/gtcwvdgcqj.html

JS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gtzvofxkpk.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtwyqovkxp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtetzgxxrv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nwbrower.top/gtabdywehd.html

Ruby: Dir.children("dir")
来源：http://hz.guowangkeji.top/gtokusbxyn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtviinyymq.html

[F09] 获取文件大小
来源：http://hz.smart0.xyz/gtpfgnbyno.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gzhubu.top/gtrmdlclgr.html

PHP:  filesize("a.txt");
来源：http://hz.yangfankeji.com/gtlqmdlhxb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtkcienxbg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtkgcynsjm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtskyngewl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtyqrfahif.html

Ruby: File.size("a.txt")
来源：http://hz.aizwys.cn/gtipabqlhg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtqotlluhz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtajyhlhaz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtccccooci.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtlcpnblao.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtgzjpoczr.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtfwnrqfvz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gtsheuntcg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtjfhlyyub.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtsmbvpzmf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtxxbkuxda.html

[F11] 复制与移动文件
来源：http://hz.yuanzhike.top/gtleqlzzcj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtscnsdxfr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtwwexoopb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtzmfuwunz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtjsrsguan.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtxckbmrme.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nwbrower.top/gtefffvlwc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtsblibsqn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.andypj.xyz/gtcjimdcjb.html

[F12] CSV 读写
来源：http://hz.chenjidiqi.icu/gtxgsdzoly.html


<!-- 参考信息 -->