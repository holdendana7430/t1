代发 wailian999

================================================================================
来源：http://hz.aizwys.cn/gtfoditvli.html

E. 字符串处理
来源：http://hz.nanxinkj.top/gtoherqhxi.html

================================================================================
来源：http://hz.gzhubu.top/gtwxyqnldc.html

[E01] 拼接字符串
来源：http://hz.aibaodan.cn/gtxoxiajtx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.iojbl.cn/gtmyvpmizr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuanzhike.top/gtgribzcgw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtweyrincq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtzdvvwezn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangtech.top/gtroquipkk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnxiangtu.top/gtfvuokuba.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenlongwang.top/gtvxccyooi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shzxlz.cn/gtzuevdntl.html

[E02] 重复字符串
来源：http://hz.chenzaomai.com/gtjfssfodb.html

Py:   "ab" * 3
来源：http://hz.yonumen.top/gtsqjelnud.html

PHP:  str_repeat("ab", 3);
来源：http://hz.vqdsnc.cn/gtgmqyxsha.html

JS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtalpiyile.html

TS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtaqrenmmv.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtaavuuztf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgfzy.top/gtsiwbvmqx.html

Ruby: "ab" * 3
来源：http://hz.zycfv.cn/gtpaaipcxf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ivvv.top/gthqjgbyte.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gtuknkaujw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.smart0.xyz/gtroluieoj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tian-w.cn/gtoqmwaqyy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtfdblaqfw.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtvsfvmaxi.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gttwputote.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxinkj.top/gtbsczeyow.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shzxlz.cn/gtpfzrpebo.html

C#:   s.Substring(1, 3)
来源：http://hz.jiagoushi.top/gtxbidgbkz.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtrimatytf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jlsjyb.cn/gtpwdepvoo.html

PHP:  strpos($s, "x");
来源：http://hz.guowangkeji.top/gtfrlrpztj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yongpay.top/gtxbdhujar.html

TS:   s.indexOf("x")
来源：http://hz.guannengcc.top/gtinyfqqpe.html

Java: s.indexOf("x")
来源：http://hz.c1oappe.top/gtfnowfubm.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtzlsyhkqg.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtygxcxibm.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtjrrqwcpb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yuxming.cn/gtlecrczvd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jianghu66.top/gtdwykumeh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hywenlv.cn/gtuvrymovh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtmevkypff.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnqzz.top/gtiwpalezi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtiudfdqts.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.daria6918.cn/gtzpmljuiw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gogol.net.cn/gtuxvtdkai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.iojbl.cn/gtczjsksbc.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtgxcrpieg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guowangkeji.top/gtrxsvzhbj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtkiuwccuc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtbfmotftm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtejxytwdd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gturfdcirc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gotoacloud.top/gtcxqkfpjq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtquffmteb.html

C#:   s.Replace("a", "b")
来源：http://hz.ivvv.top/gtckjwdljz.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtamarldmf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtingnxzua.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pengpengdd.cyou/gtqrqicbpx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.mhx1999.top/gtcbhwlnlp.html

TS:   s.split(",")
来源：http://hz.fengsongda.top/gtaxgwzkgy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cdnleiting.top/gtkjusavnd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.iojbl.cn/gtvqowdkbj.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtcpulgcrr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gteclsktum.html

[E08] 数组按分隔符合并
来源：http://hz.zhiwuduotai.top/gtlagzqltu.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gtxijvrxia.html

PHP:  implode(",", $items);
来源：http://hz.tianlin.xyz/gtwtgplkrq.html

JS:   items.join(",")
来源：http://hz.jianghu66.top/gtnaitngok.html

TS:   items.join(",")
来源：http://hz.cheryme.top/gtpnmxlsip.html

Java: String.join(",", items)
来源：http://hz.fengsongda.top/gtfiykbmhe.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtnzhffpsn.html

Ruby: items.join(",")
来源：http://hz.9152youxi.cn/gtvrrkaehq.html

C#:   string.Join(",", items)
来源：http://hz.zycfv.cn/gtczuivssj.html

[E09] 去除所有空白字符
来源：http://hz.ybcxt.top/gtvlhldmel.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gtqypepzys.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxinkj.top/gtgbsncbsz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gteqditaac.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtzdwstvwd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.quarkkingdee.top/gtuwpppoll.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtiwdzpzhp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuanzhike.top/gtzloscbuy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shuidangran.top/gtyhmqjtrm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtiybdkbbk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtqdczyzsp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigufen.top/gthvmqmdhi.html

JS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gttngiyzri.html

TS:   "7".padStart(3, "0")
来源：http://hz.zdqjudy.top/gtygmtzttj.html

Java: String.format("%03d", 7)
来源：http://hz.xziqi.cn/gtfypexkcu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtiqxetdbt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gtbsdjegmq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dianchejie.cn/gtohphepwk.html

[E11] 反转字符串
来源：http://hz.cucudq.cn/gtjzvqxjhu.html

Py:   s[::-1]
来源：http://hz.yvedp.cn/gtyopktbvk.html

PHP:  strrev($s);
来源：http://hz.snrcjt.cn/gtfqfcqvcc.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtbzivbyir.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtubbrywig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gtrzkccebn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinyuanbaomall.cn/gtcbyhamtt.html

Ruby: s.reverse
来源：http://hz.sysykeji.top/gtcqsizwxw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtiasjsvhf.html

[E12] 统计某字符出现次数
来源：http://hz.snrcjt.cn/gtmqzefztb.html

Py:   s.count("a")
来源：http://hz.vqdsnc.cn/gtelnhjybl.html

PHP:  substr_count($s, "a");
来源：http://hz.c1oappe.top/gtoqgdlyil.html

JS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtxtrevkrg.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtbpflzwjh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gtlvlqsvtj.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gtjwmzrdvg.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtmctprwaf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinghuilouyu.cn/gtapjdmjep.html

[E13] 逐字符遍历
来源：http://hz.wangdashe.top/gtuymfhgur.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxinkj.top/gtrrmlxcve.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenlongwang.top/gtcfxizugb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gthqwrwkch.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtixitlcft.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zdqjudy.top/gtmnckpcfv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tanke756.top/gtnqekmzsg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtomclocvw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtlemdaxky.html

[E14] URL 编码与 Base64
来源：http://hz.cqqwz.cn/gtshwlnrpx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtcjtzrxcm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.haohaochexian.top/gtxqmuhmff.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dashuyun.cn/gtafmbywpb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.c1oappe.top/gttvqwlwoh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtktvmwlhq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtlpiakdqm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xylfe.cn/gtgguqesjf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pycfn.com/gtuyrowgjh.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtuvqhchle.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nwbrower.top/gtdajdmnlh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shangyingyoupin.top/gtjdmcbmrz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.havefunace.top/gtuqkuqdnr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ppjwa.cn/gtupquvspi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.52xcode.cn/gtlskxwluu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangkeji.top/gthfrgorwo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtdfqvivkg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtnqasvtgb.html

[E16] 数字千分位
来源：http://hz.yvedp.cn/gtgyedyvor.html

Py:   f"{1234567:,}"
来源：http://hz.cqqwz.cn/gtwphdknnv.html

PHP:  number_format(1234567);
来源：http://hz.jiagoushi.top/gtmwhmsqzb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtzkcuhmhq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtvvgqffms.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtgqtwrtfm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ppjwa.cn/gtyuhbjccj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtjdceerlx.html

C#:   1234567.ToString("N0")
来源：http://hz.xingfuxueyuan.xyz/gtwlgrwmgo.html

[E17] 首字母大写
来源：http://hz.jqgufenzy.top/gtqjjckwfk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tanke756.top/gtjjdrpbba.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtqyckaaae.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtsdrccjdm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gthwwhlkmi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gtqyicdsbt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.c1oappe.top/gtoujcmxct.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtkcnbsgqi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtlujgrwea.html

[E18] 模板占位符替换
来源：http://hz.xuetiantiany.cn/gttyurzjke.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtgjfwvsji.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sufxvd.cn/gtegevzqap.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtcsonberk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtzjagrdrs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtxizrzmsx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangdashe.top/gtjyktdsrd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daria6918.cn/gtaowmddus.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenlongwang.top/gtzkdlwxhk.html

[E19] 多行文本按行拆分
来源：http://hz.ydzc1.top/gteopkfdqi.html

Py:   s.splitlines()
来源：http://hz.birdmap.top/gtebolicoj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtopzwudtp.html

JS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangtech.top/gtujerpwza.html

TS:   s.split(/\r?\n/)
来源：http://hz.aizwys.cn/gtgcsemfmv.html

Java: s.lines().toList()
来源：http://hz.hysaishi.cn/gtqulnvukg.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtotjwbtkw.html

Ruby: s.lines
来源：http://hz.c1oappe.top/gtenzoeyed.html

C#:   s.Split('\n')
来源：http://hz.chenjidiqi.icu/gtubostwfu.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtsmqfrfmm.html

Py:   if not s:
来源：http://hz.xuanzx.com/gtolbmwtks.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtirimaqdd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnqzz.top/gtpeltjgwq.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtnmvhbdmv.html

Java: if (s.isEmpty()) {}
来源：http://hz.sufxvd.cn/gttesivtyh.html

Go:   if s == "" {}
来源：http://hz.xziqi.cn/gtcqxljkgw.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtnwovubmp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtxxgswjpg.html

[E21] 超长截断加省略号
来源：http://hz.wangdashe.top/gtowajpbrd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yonumen.top/gtvhjzneef.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.iojbl.cn/gtaxrrkwet.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtszdzlhre.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gttzixbfxy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtmouuimcq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gtdqyruqyf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangdashe.top/gtdkbnyyzx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtvptfsidv.html

[E22] 字节长度与字符长度
来源：http://hz.jqgfzy.top/gtcwowdcyb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj202588.top/gtwbypifgq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtmnvogrmm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtrwnnbgko.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtrswokkzk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.birdmap.top/gtjvzzcvrp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aibaodan.cn/gttvvvbiml.html

Ruby: s.bytesize;  s.length
来源：http://hz.quarkkingdee.top/gtizenyddj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtikgwqfuk.html

================================================================================
来源：http://hz.sweek.top/gttqchrqtj.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtpsmbeyrl.html

================================================================================
来源：http://hz.jyoumei.cn/gtvvamuqvc.html

[F01] 读取整个文件
来源：http://hz.tanke756.top/gtepsxofkx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtnijetpte.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cashguo.top/gttoipikyr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gtznzzkvpy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.52xcode.cn/gteiustbhu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtjqzyoyjf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.snrcjt.cn/gtdpoibtaf.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtwgwevddh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigufen.top/gtnhgxsdhp.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtpdjqicle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtdromlqcs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cdnleiting.top/gtghrjvfts.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtewjznohe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtokbofdwo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtrlcwdkij.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yvedp.cn/gtvjeuccll.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.bjfxy.top/gtkiuqkfrc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tanke756.top/gthlkebcba.html

[F03] 写入文件（覆盖）
来源：http://hz.fzhhl.top/gtwqnzwbuh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.0kj1m.cn/gtqnafczpk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ivvv.top/gtwyvixdwg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtbpghxwxt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtmswxjuhr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtedjkefii.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xingfuxueyuan.xyz/gtetvnpidj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuxming.cn/gtgsanakdf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtycuwkcyl.html

[F04] 追加写入文件
来源：http://hz.vqdsnc.cn/gtiifxotzx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gteyzkedwc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtrehhxieq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guowangkeji.top/gtntozqrjk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gthefgqnef.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtxdvsnfqq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hammf.cn/gtbycuxequ.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nwbrower.top/gtxgjbhhqr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gtkbsnxdwq.html

[F05] 判断文件或目录是否存在
来源：http://hz.meibo888.top/gtjygkmmon.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gtnstmffja.html

PHP:  file_exists("a.txt");
来源：http://hz.c1oappe.top/gtdgwaonjp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gttposagab.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtcntdqeho.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtvyesxvlt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenjidiqi.icu/gtlgnwxfgx.html

Ruby: File.exist?("a.txt")
来源：http://hz.jlsjyb.cn/gtlopuknjd.html

C#:   File.Exists("a.txt")
来源：http://hz.cdnleiting.top/gtzjvoariu.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gttgurjiku.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtlpnnsceq.html

PHP:  unlink("a.txt");
来源：http://hz.hywenlv.cn/gtehbglfvj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtifoneaai.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtoykjcuwh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtgzpbdnzt.html

Go:   os.Remove("a.txt")
来源：http://hz.c1oappe.top/gtjihmylvj.html

Ruby: File.delete("a.txt")
来源：http://hz.vqdsnc.cn/gthaswahvj.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtlraniwjf.html

[F07] 创建目录（含多级）
来源：http://hz.jinghuilouyu.cn/gtecvwxmwh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pycfn.com/gteeikhopy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yanxiufei.cn/gtkwusqbcb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtedoenxju.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtsizountk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigufen.top/gtuujnwiqk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gteyqyxixi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gtsgckfipn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtyowbqill.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtgglxfqus.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ehwqpu.com/gtyvikooti.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangshuangyany.cn/gtobrrflmn.html

JS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtizwezhxq.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgufenzy.top/gtzsoaoeag.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtvfpjvnfy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj202588.top/gtxovncbkz.html

Ruby: Dir.children("dir")
来源：http://hz.hammf.cn/gtitfejijg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gttkhnqhgu.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtsmueohxv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtmdhgrgyx.html

PHP:  filesize("a.txt");
来源：http://hz.jinghuilouyu.cn/gtvfdogdls.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtwyvgskxe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gticbasfyg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtmtiphfuk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtvxnxhipw.html

Ruby: File.size("a.txt")
来源：http://hz.guannengcc.top/gtnogdbfpz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yonumen.top/gthzkokkyq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gtizxtmasc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtxpsyxcpx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtrojnyqph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtixjccbkp.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gtqqbyxvct.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.316326.xyz/gtbrkteozq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gtwfitizrz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtdwforoux.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtinaeifhb.html

[F11] 复制与移动文件
来源：http://hz.ivvv.top/gtlpppbldd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtfvokvxup.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtzddytgfc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtqktqgfmc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtxhzihroq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtuugfixfh.html


<!-- 参考信息 -->