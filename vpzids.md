代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgfzy.top/gttkfgxjhj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jyoumei.cn/gtdymwfcxu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxinkj.top/gtineqcfze.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenjidiqi.icu/gtsoeajuyb.html

[E02] 重复字符串
来源：http://hz.sufxvd.cn/gtkvappnre.html

Py:   "ab" * 3
来源：http://hz.0kj1m.cn/gtgocxrsci.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xuanzx.com/gtviutidrw.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtsvgngvtu.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtaicjkxmy.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtkkncenlo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxinkj.top/gtboadzssu.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtcjubnzie.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.0kj1m.cn/gtncelaifs.html

[E03] 截取子串
来源：http://hz.hongshengwenyu.top/gtbqoopdhy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnxiangtu.top/gtxmpzspqv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258.top/gtocwnaaeb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtuogovtmg.html

TS:   s.slice(1, 4)
来源：http://hz.chenzaomai.com/gtnielskfo.html

Java: s.substring(1, 4)
来源：http://hz.guannengcc.top/gtazkiyzop.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gteawwqlpu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yanxiufei.cn/gtwksphvwo.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtlkbcqvbv.html

[E04] 查找子串位置
来源：http://hz.ybcxt.top/gtytuaepya.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ybcxt.top/gtwpciqimz.html

PHP:  strpos($s, "x");
来源：http://hz.ydjk.org.cn/gtwcjfckrc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxinkj.top/gtspmmsvhn.html

TS:   s.indexOf("x")
来源：http://hz.sweek.top/gtzkacwrgk.html

Java: s.indexOf("x")
来源：http://hz.zhixingplan.top/gtatkzepoc.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gtelbvpuvy.html

Ruby: s.index("x")
来源：http://hz.hysaishi.cn/gttglwslqc.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtqyaldcpl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shzxlz.cn/gtggpdsatq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtnefdawnj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jyoumei.cn/gttgqvqwso.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtsdomsgss.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zycfv.cn/gtfuvkmnjl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtvzjgqhrp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnqzz.top/gtawmrcpvs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtvjeltnef.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtyhbwmcha.html

[E06] 替换子串
来源：http://hz.wangshuangyany.cn/gtxyzvekin.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hongshengwenyu.top/gtwcjnchew.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cqqwz.cn/gtevothzsm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtrapfguax.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtvsekllmc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtvgqfiwqy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ybcxt.top/gtwplltcnk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yuxming.cn/gtdkybcyyi.html

C#:   s.Replace("a", "b")
来源：http://hz.tanke756.top/gtfxzzpcjj.html

[E07] 按分隔符拆分
来源：http://hz.jlsjyb.cn/gtvmxazxfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nwbrower.top/gtsajywopi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gotoacloud.top/gtcjrmdmrt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuxming.cn/gtjjfajmoi.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtxsshadrw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guowangkeji.top/gtokmxkkcm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cashguo.top/gtihystznz.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gttxthxavx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gtsvwefqnv.html

[E08] 数组按分隔符合并
来源：http://hz.9152youxi.cn/gtnztexhas.html

Py:   ",".join(items)
来源：http://hz.nwbrower.top/gtbxesvvmd.html

PHP:  implode(",", $items);
来源：http://hz.havefunace.top/gtsfljumve.html

JS:   items.join(",")
来源：http://hz.gzhubu.top/gthsziqeuf.html

TS:   items.join(",")
来源：http://hz.yj20258888.top/gthkyonbwv.html

Java: String.join(",", items)
来源：http://hz.chenlongwang.top/gtvapfhwsx.html

Go:   strings.Join(items, ",")
来源：http://hz.jinyuanbaomall.cn/gthmspsyso.html

Ruby: items.join(",")
来源：http://hz.jinqigufen.top/gtskkishoj.html

C#:   string.Join(",", items)
来源：http://hz.tanke756.top/gtnwhqithg.html

[E09] 去除所有空白字符
来源：http://hz.smart0.xyz/gtosmmrelx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtxjkmxeyt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.svipenyu.cn/gttmzuhsco.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtlfefjvar.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtiztcekvb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxuanxn.top/gtdptmxzdx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cashguo.top/gtdfdjlcdd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinghuilouyu.cn/gtbafhsyoh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gotoacloud.top/gtkggoxobt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yuxming.cn/gtbhisyqxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guowangkeji.top/gtyoizmljk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hfpthk.cn/gttyvzvrgf.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtkuieobdx.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtnmpfkgmq.html

Java: String.format("%03d", 7)
来源：http://hz.pycfn.com/gtbkinekmq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.c1oappe.top/gtsgjwmmtc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.snrcjt.cn/gtdfgqaqvu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hywenlv.cn/gtociseqho.html

[E11] 反转字符串
来源：http://hz.zhaomingkeji.xyz/gtpksmpkef.html

Py:   s[::-1]
来源：http://hz.nanxinkj.top/gttfrbvltk.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gtxwqibicb.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtnbhcyflb.html

TS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtihoyxowv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangshuangyany.cn/gtlwtjefrk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258.top/gtyerfqkah.html

Ruby: s.reverse
来源：http://hz.pengpengdd.cyou/gtjixwkygs.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtecedlmzm.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gthjyjlhcr.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtnssjotzj.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtedohpwxp.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtygysicsh.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtmsccwvxg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtyogvmfkh.html

Go:   strings.Count(s, "a")
来源：http://hz.yj202588.top/gtaearlrrw.html

Ruby: s.count("a")
来源：http://hz.zhongyouzk.top/gtkhyyobdw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtmkjozcbv.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtvjknrbjv.html

Py:   for ch in s: print(ch)
来源：http://hz.hnqzz.top/gtmqjmbydc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.kuanghao11.cn/gtjffknxnl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtecgwinjr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtlrhneiji.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtzdvgqkie.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtngftrwrk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gtpmujwokv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cqqwz.cn/gtvadyozua.html

[E14] URL 编码与 Base64
来源：http://hz.zycfv.cn/gtaqmvhuic.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtsrodrlba.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jyoumei.cn/gtzxmhexnh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.smart0.xyz/gtpsnhgpdr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sufxvd.cn/gtykoklgkp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ivvv.top/gtswiyuxcd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.haohaochexian.top/gtpqzfjvch.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtegfhluqo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gthumexirf.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtolkjiwec.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtxvpqqfhd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sweek.top/gtbhlggige.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuxming.cn/gtolrhbvks.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cucudq.cn/gtnhqwgtji.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtvaqajnor.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xylfe.cn/gtawnmjpir.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtgybvhplp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gtxhuiiypz.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtywrgkdzf.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gtwphdqcgb.html

PHP:  number_format(1234567);
来源：http://hz.sufxvd.cn/gtziyqqfju.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtnuvvvlrs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtnvkebrzo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daxiang520.top/gttamkqmvs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtprxjebxb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangshuangyany.cn/gtxdcdyygm.html

C#:   1234567.ToString("N0")
来源：http://hz.hongshengwenyu.top/gtvhgkdbgr.html

[E17] 首字母大写
来源：http://hz.sufxvd.cn/gtgnflsqvu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pycfn.com/gtxmrcgxut.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shzxlz.cn/gtbjjdyald.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtyiynpgmh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gthegouwje.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xziqi.cn/gtasupyopz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gtvzvogazg.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtkmiwngva.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.bjfxy.top/gttjbyjzhy.html

[E18] 模板占位符替换
来源：http://hz.sufxvd.cn/gtevekdkqu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hysaishi.cn/gtdyrgfkqk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.smart0.xyz/gtbikjtmtt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtncvgbbor.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gtpoqvrirc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhijiandao.cn/gtmwqvnoxc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jlsjyb.cn/gtlcwxeiss.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtpynwfqrm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtoprfdevq.html

[E19] 多行文本按行拆分
来源：http://hz.9152youxi.cn/gtwoiphtqt.html

Py:   s.splitlines()
来源：http://hz.shzxlz.cn/gtdbkvmbuj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtmqpyjlwp.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtasazzxpk.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangdashe.top/gtvyuubklr.html

Java: s.lines().toList()
来源：http://hz.tianlin.xyz/gtzripdsdo.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangdashe.top/gtiunitxdr.html

Ruby: s.lines
来源：http://hz.cqqwz.cn/gtmrkbwuqd.html

C#:   s.Split('\n')
来源：http://hz.jqgufenzy.top/gtrfqywptu.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtaddbvast.html

Py:   if not s:
来源：http://hz.tian-w.cn/gtncnfjekf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gtnyoujxkr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhaomingkeji.xyz/gtecethrox.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtkwfcbrye.html

Java: if (s.isEmpty()) {}
来源：http://hz.tanke756.top/gtetjundjk.html

Go:   if s == "" {}
来源：http://hz.zhoulong.xyz/gtrevocydu.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gtkzbtmgox.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenlongwang.top/gtebmmmitv.html

[E21] 超长截断加省略号
来源：http://hz.52xcode.cn/gtqgzbrqrs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dianchejie.cn/gtjzbalbwj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenjidiqi.icu/gtwqvwjfna.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtlxwjfxsh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtkwrgujhv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtvlvxhyle.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.smart0.xyz/gtxvvkibte.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.316326.xyz/gtptcdkjzr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gthccazsti.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258.top/gtodbxgrrz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydzc1.top/gtgkflabmd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.meibo888.top/gtzfqcwxku.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtbuydljez.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtoljzaish.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aibaodan.cn/gtrcaszcyn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tanke756.top/gtqhvavwjd.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhongyouzk.top/gtygltessq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtselgugwd.html

================================================================================
来源：http://hz.yueranfly.top/gtsfncuoff.html

F. 文件与目录
来源：http://hz.yueranfly.top/gtzelmsufv.html

================================================================================
来源：http://hz.havefunace.top/gtmwadardi.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtbyuickjg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ehwqpu.com/gtrprdhiwz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtggadjbtd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zdqjudy.top/gtdqtpmkdi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dianchejie.cn/gtmsrgblgl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtbqngsbyn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sweek.top/gtrgmipqtu.html

Ruby: File.read("a.txt")
来源：http://hz.sufxvd.cn/gtcrwqwnub.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxinkj.top/gtnkizsxkn.html

[F02] 逐行读取文件
来源：http://hz.aibaodan.cn/gttjveonon.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtshyiisgo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258.top/gtqrvnumqv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtmnxbrjud.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtetpuyfze.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtdqscwwzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinghuilouyu.cn/gtjjeyqmrd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtzxgvodxn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gtppuefvfv.html

[F03] 写入文件（覆盖）
来源：http://hz.yangfankeji.com/gtngkrwjxu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.snrcjt.cn/gthzjvexvt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ybcxt.top/gtzlriytmb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtxuhdshkb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtsvtxsdcx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.9152youxi.cn/gtvteejvcv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenzaomai.com/gtvpipzvga.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shuidangran.top/gtxdzyeymw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtopbfawbc.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtlcmkiilg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtvifqiwkp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gtcicqxyuv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtxoejaeng.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtwmyhpjnb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtuznqqtad.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtkjrndbbo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.mhx1999.top/gtumqopksi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtruadybxp.html

[F05] 判断文件或目录是否存在
来源：http://hz.daria6918.cn/gtgwvxgkwe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yueranfly.top/gtajatfmxs.html

PHP:  file_exists("a.txt");
来源：http://hz.c1oappe.top/gtejnuxerd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtofsncdky.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gthcedrpfk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtjcaputgr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.c1oappe.top/gtldqwerhm.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtmrlfqppo.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtkbxflknw.html

[F06] 删除文件
来源：http://hz.yueranfly.top/gtxarlpziw.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtzpwskjca.html

PHP:  unlink("a.txt");
来源：http://hz.shuidangran.top/gtsnskxsun.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtaxpoznht.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtacoyoqbf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtxgljutsd.html

Go:   os.Remove("a.txt")
来源：http://hz.sufxvd.cn/gtnrdrzfni.html

Ruby: File.delete("a.txt")
来源：http://hz.gotoacloud.top/gtdemttrhx.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gthymztqrd.html

[F07] 创建目录（含多级）
来源：http://hz.tian-w.cn/gtqlkrdiex.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xylfe.cn/gticlmdane.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gteauovfsp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtozdjeyzd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gtrnjbkwrg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhongyouzk.top/gtwembtkdz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yangfankeji.com/gtbjynxsps.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtztrrerei.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.haohaochexian.top/gtgmketcfh.html

[F08] 遍历目录
来源：http://hz.sxryk.cn/gtrfbsaspo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gtzvphvcwk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shuidangran.top/gtcewsduye.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtiromfyuw.html

TS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtvofsnbdf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtobkhlyle.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtkkedcyew.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtxtrvnyvp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cashguo.top/gtjdetjlcg.html

[F09] 获取文件大小
来源：http://hz.birdmap.top/gtyfvlihoy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gttgrxrdgo.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gtmwdvcnua.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtmvwquqpi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gthfnvbmma.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtawoqboqf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.svipenyu.cn/gtoiecbjsb.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtghfsxqzl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.bjfxy.top/gtjsqtnfqv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtqeuefbgt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtcobvmrvl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gogol.net.cn/gtvsshemnp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtverzsxkz.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gtetzvgirt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtmdwpjhed.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yangfankeji.com/gtqllfxbdc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gttxrybyjw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cqqwz.cn/gtxwwyiyeh.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtoispymot.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtqznmgfwm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenzaomai.com/gtoblbkand.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtwvzllrjy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtqmomajpx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtvzasultr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gtkbcwuxif.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtifmdijcb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtbtckroxc.html

[F12] CSV 读写
来源：http://hz.pengpengdd.cyou/gthxslismf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yongpay.top/gtcqswbvdj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtimtfajcn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gtthubhvvi.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtpkaitpyj.html


<!-- 参考信息 -->