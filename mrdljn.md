代发 wailian999

Java: String.join(", ", list)
来源：http://hz.dashuyun.cn/gtzeqyscdi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.bjfxy.top/gttjaunmlo.html

Ruby: arr.join(", ")
来源：http://hz.guannengcc.top/gtcjbqjcdc.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtqsuyuzmk.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyjabrvrw.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtzcigfauf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtznpugnwx.html

[E01] 拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtrpqpecgl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dashuyun.cn/gtiwlrqtck.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xingfuxueyuan.xyz/gtfgvgndpb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hysaishi.cn/gtdblupqti.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtprmklmfq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhongyouzk.top/gtzxqthqen.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxuanxn.top/gtqdlcbopt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daxiang520.top/gtgxrukzka.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hammf.cn/gtgndndxhb.html

[E02] 重复字符串
来源：http://hz.vqdsnc.cn/gtwybfwjlo.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gtzfzmvofd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guannengcc.top/gtyovyfvib.html

JS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtrslpxzki.html

TS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtsonbtplu.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gttinathdq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gzhubu.top/gtnqbzvnpm.html

Ruby: "ab" * 3
来源：http://hz.cheryme.top/gtgafalxyz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gzhubu.top/gtxsfhgcty.html

[E03] 截取子串
来源：http://hz.sweek.top/gtavmsobzf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtisnyijku.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhongyouzk.top/gtlitypomy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtcmiugnly.html

TS:   s.slice(1, 4)
来源：http://hz.0kj1m.cn/gtwfxpkebx.html

Java: s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtcfazaahr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guannengcc.top/gtlmbsixtx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ywan-chungtsiang.top/gtznnqaigh.html

C#:   s.Substring(1, 3)
来源：http://hz.nanxinkj.top/gtwswckxpl.html

[E04] 查找子串位置
来源：http://hz.yuanzhike.top/gtllnmecab.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuxming.cn/gtitnzghey.html

PHP:  strpos($s, "x");
来源：http://hz.gotoacloud.top/gtrdabtzql.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtkgldflvk.html

TS:   s.indexOf("x")
来源：http://hz.gotoacloud.top/gtwbfvuudx.html

Java: s.indexOf("x")
来源：http://hz.xuanzx.com/gtvwwbnfox.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gthnughugt.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gtytnpjkks.html

C#:   s.IndexOf("x")
来源：http://hz.yj20258.top/gtqjqjrzpb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuanzx.com/gtisdugmcd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangshuangyany.cn/gtwwvreszz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.nanxuanxn.top/gtbcuncyqe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtbnlmikhe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gotoacloud.top/gtnkorjchq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtgobogtqp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xinyue.icu/gthxscadfb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gttgirfrks.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.quarkkingdee.top/gtrrkufltd.html

[E06] 替换子串
来源：http://hz.snrcjt.cn/gtgsavhnei.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gttioponss.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hnqzz.top/gtbufvhlop.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtigujectu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtgmtqnqco.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtudbcrbmm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guannengcc.top/gtagkuqyjb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cucudq.cn/gtdmpdbenb.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtkktjvrov.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtjfafhgoi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.316326.xyz/gtnwltnsal.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenzaomai.com/gtajfwrmpm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtgcaqlwjj.html

TS:   s.split(",")
来源：http://hz.vqdsnc.cn/gtcsqswmne.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.c1oappe.top/gtunerqeve.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtspzuggux.html

Ruby: s.split(",");  s.split
来源：http://hz.cashguo.top/gtreuatkxx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydjk.org.cn/gtnyffnilf.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtpapdvhxl.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gttedfhpye.html

PHP:  implode(",", $items);
来源：http://hz.feifeiyinyue.top/gtsbjxhigq.html

JS:   items.join(",")
来源：http://hz.cdnleiting.top/gtbesknexy.html

TS:   items.join(",")
来源：http://hz.xuetiantiany.cn/gtsegalxla.html

Java: String.join(",", items)
来源：http://hz.wangshuangyany.cn/gttvgvkvet.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtioxcaqfm.html

Ruby: items.join(",")
来源：http://hz.cdnleiting.top/gtqtixqvoc.html

C#:   string.Join(",", items)
来源：http://hz.zhijiandao.cn/gthiaojdwm.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtmjfrmxja.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtttjkzmiu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhoulong.xyz/gtdykrzlnb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gthuajwckr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtmymbaxcy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gtcalmiluh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtremlupyz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yvedp.cn/gtsligmxye.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ehwqpu.com/gthmtchwdu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ehwqpu.com/gtnhvahnzz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gthqbqljpo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xylfe.cn/gtbbyuokfx.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtvqethrdv.html

TS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gthkcuqccw.html

Java: String.format("%03d", 7)
来源：http://hz.c1oappe.top/gthwyiyqkc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.havefunace.top/gtvcmlvlal.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aizwys.cn/gtmxizjpym.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gzhubu.top/gtzefuwpcp.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gtekvbfwtv.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtjevhfvpo.html

PHP:  strrev($s);
来源：http://hz.xylfe.cn/gthbnrlbbb.html

JS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtnfrlkzuj.html

TS:   [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtdnuftsmw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtpkiksjff.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtjgarncso.html

Ruby: s.reverse
来源：http://hz.chenjidiqi.icu/gtyvpllbdg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtsbkscorz.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtriwhdqju.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtnaqpjzto.html

PHP:  substr_count($s, "a");
来源：http://hz.fzhhl.top/gtedveobeh.html

JS:   s.split("a").length - 1
来源：http://hz.xuetiantiany.cn/gtgjfmxoht.html

TS:   s.split("a").length - 1
来源：http://hz.aibaodan.cn/gtcbezbwkn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnxiangtu.top/gtbloxmeux.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtdxokmkal.html

Ruby: s.count("a")
来源：http://hz.pengpengdd.cyou/gtchioibvn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cqqwz.cn/gtwgyhcqhi.html

[E13] 逐字符遍历
来源：http://hz.redwolf501.top/gtauzowqic.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gtnpnzikku.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtheutjyls.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtxmodeztb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtgdgdlkgv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtifxsjfps.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gzhubu.top/gtmomtxaur.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hysaishi.cn/gtqnlvktis.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jiagoushi.top/gtresuxxjb.html

[E14] URL 编码与 Base64
来源：http://hz.ivvv.top/gtaiivokga.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtlhreduno.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gtiulcuihh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ydzc1.top/gtxvthtagv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nwbrower.top/gtcsqnyxwx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.c1oappe.top/gtfscuaqlc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.9152youxi.cn/gtzzekajux.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gogol.net.cn/gtfdezsojd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cashguo.top/gtxvjaprrs.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtvwredbzy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.smart0.xyz/gtsylzdfkd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xinyue.icu/gtkvpuvotp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhaomingkeji.xyz/gtxlnqdbzd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gtrnxeoyit.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gtrtstyfmh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fzhhl.top/gtghtlrkal.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtmzirkoqx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.feifeiyinyue.top/gtvmiudumi.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gtsfqtoudx.html

Py:   f"{1234567:,}"
来源：http://hz.yonumen.top/gtevjahjjq.html

PHP:  number_format(1234567);
来源：http://hz.daria6918.cn/gtahmizzrp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtqakpmfdx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtlixrskqy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtulodoabn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gtirqojjuk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guowangkeji.top/gtkztlqrbl.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gthdlgkjpq.html

[E17] 首字母大写
来源：http://hz.xziqi.cn/gtaqjnimfb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yueranfly.top/gtlkgifdhq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtjzeqixns.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtwmdljcfx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtpvussaoh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fzhhl.top/gtsmtnvryj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenjidiqi.icu/gtlgfqvfwm.html

Ruby: s.capitalize
来源：http://hz.hnxiangtu.top/gtjwrjvnxr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gtxpwpgdpm.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtzllqiuju.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenzaomai.com/gtlthysxyk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shanyushiyangtech.top/gtgrwlpssn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtuihrklnc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtavcoekpp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhijiandao.cn/gtafqvgzgv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gtyblbzyrx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnqzz.top/gtwkbwqqfk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cqqwz.cn/gtfhsegjgc.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gtavcnzjxw.html

Py:   s.splitlines()
来源：http://hz.ppjwa.cn/gtwbuchtvp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuanzx.com/gtdtxvcywd.html

JS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtsytxlstc.html

TS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtnrjllwex.html

Java: s.lines().toList()
来源：http://hz.sweek.top/gtytoeycei.html

Go:   strings.Split(s, "\n")
来源：http://hz.redwolf501.top/gtksekagmv.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtqizpbmxh.html

C#:   s.Split('\n')
来源：http://hz.xziqi.cn/gtizwxlfyf.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtcvycxnaj.html

Py:   if not s:
来源：http://hz.cheryme.top/gtpeavyxvv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtywkaklod.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangkeji.top/gtjigiojcf.html

TS:   if (s === "") {}
来源：http://hz.tanke756.top/gtdntfqsce.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtpzxgmbsu.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gtfqlhzuin.html

Ruby: if s.empty?
来源：http://hz.yj20258.top/gtbaqaomow.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gtzexuyfqb.html

[E21] 超长截断加省略号
来源：http://hz.dashuyun.cn/gtcuywjlzj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtiaggjcue.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cucudq.cn/gtoiflozgx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtboqhucxw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtngsqspsr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtsawgplgs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258888.top/gtziehlvbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hywenlv.cn/gtohfvfmpb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xuanzx.com/gtirlidurb.html

[E22] 字节长度与字符长度
来源：http://hz.zhongyouzk.top/gtcnuijuss.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gttktgrfgj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtkiwwzieb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtdhlahlzn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtvsrnvdcf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.vqdsnc.cn/gthltlkzaq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenjidiqi.icu/gtizqtnibq.html

Ruby: s.bytesize;  s.length
来源：http://hz.gzhubu.top/gttjlmschy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtpepvxuwh.html

================================================================================
来源：http://hz.fzhhl.top/gtnzmamzro.html

F. 文件与目录
来源：http://hz.aibaodan.cn/gtvsrypfbo.html

================================================================================
来源：http://hz.tianlin.xyz/gtckkxvawv.html

[F01] 读取整个文件
来源：http://hz.daria6918.cn/gtgaurswlh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtidhkgfux.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtnzughpxg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guowangkeji.top/gtlfxgzjwf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtnxljzlyy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtbcwunipf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangtech.top/gtlnvpbxgb.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gtvupntcvb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.mhx1999.top/gtxnpsbnvk.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtqvrnokpo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydjk.org.cn/gtofuxarfl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gttvtvvnmo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gthztsuggy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtawabnpsb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtgramakns.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gterhrqnro.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenlongwang.top/gtunzknanz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sxryk.cn/gtenmnwkki.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtogtnospy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hywenlv.cn/gtdegtnaab.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gzhubu.top/gtlycpcega.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtmpzmhrag.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtngnyaxtk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gttsiiavuh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gtktwqvgeb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cqqwz.cn/gtsctrkbua.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtyilgklel.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtykyyqtki.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangdashe.top/gtixjiumna.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtpwctqvaj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtskcuqydk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tianlin.xyz/gtkzgvqeev.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shzxlz.cn/gtjafbyqcz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yanxiufei.cn/gtrxwftiox.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.redwolf501.top/gtpvexbkws.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gttigjxcrg.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgfzy.top/gthwugijhl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenzaomai.com/gtqcmptvgk.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtoxteaejs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtxptapsat.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtcwjferno.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtdfqhwcml.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhongyouzk.top/gtqvkhhouk.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtablqqrsl.html

C#:   File.Exists("a.txt")
来源：http://hz.9152youxi.cn/gtrljaijij.html

[F06] 删除文件
来源：http://hz.kuanghao11.cn/gtsqwsruce.html

Py:   os.remove("a.txt")
来源：http://hz.shuidangran.top/gteohkmpmg.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtzuvmsyyt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtgasmhrgp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtmradzsjb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtuotkfmsx.html

Go:   os.Remove("a.txt")
来源：http://hz.fzhhl.top/gtchlvyyga.html

Ruby: File.delete("a.txt")
来源：http://hz.9152youxi.cn/gtzvcigdgx.html

C#:   File.Delete("a.txt");
来源：http://hz.zhongyouzk.top/gtwywvbfvy.html

[F07] 创建目录（含多级）
来源：http://hz.tianlin.xyz/gtewhkcnlh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtalniiorv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jyoumei.cn/gtwvoyoqwl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtaofinpsi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtcxxiqtmv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtuuiuifqo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinghuilouyu.cn/gtyshsusmy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtxzoarycr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hywenlv.cn/gtxhzrtpef.html

[F08] 遍历目录
来源：http://hz.andypj.xyz/gtlancyvpe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.mhx1999.top/gtqztwmzqy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.aizwys.cn/gtawveimqa.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtsgjwzlwe.html

TS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtlltlcblo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtqdfzftto.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuanzhike.top/gtocrinvag.html

Ruby: Dir.children("dir")
来源：http://hz.andypj.xyz/gtddpspzrl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtggfwujdh.html

[F09] 获取文件大小
来源：http://hz.haohaochexian.top/gtxdgawnwj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtwrrqonft.html

PHP:  filesize("a.txt");
来源：http://hz.ppjwa.cn/gtpjywetmj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtghofskma.html

TS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtulpowufp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gttekapgco.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gttnfbyqxz.html

Ruby: File.size("a.txt")
来源：http://hz.ehwqpu.com/gtcbitvapu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shuidangran.top/gtbqgeajtd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zdqjudy.top/gtwkkkzgjv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtyjrvihkz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gthhumecox.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtivthyhdz.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtcaiegivi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtwjmjutge.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtrbcuhqkn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtezkgydkh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.9152youxi.cn/gtoaargkoz.html

[F11] 复制与移动文件
来源：http://hz.ywan-chungtsiang.top/gtwpmfxcel.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtknhdikry.html


<!-- 参考信息 -->