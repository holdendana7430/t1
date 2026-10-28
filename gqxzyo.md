代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtpffjkkvy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xziqi.cn/gtzhozmvyf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxinkj.top/gtqqqnelxj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenlongwang.top/gtruphmyxd.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gtwuoyhvxf.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtiqnonozv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenjidiqi.icu/gtmvrgjcvp.html

JS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtjgcvkeaz.html

TS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtzruktmee.html

Java: "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtzwmpcdbi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.feifeiyinyue.top/gteebhiowx.html

Ruby: "ab" * 3
来源：http://hz.52xcode.cn/gtowctyckj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hysaishi.cn/gtguvrqaux.html

[E03] 截取子串
来源：http://hz.zhixingplan.top/gtlefkhysw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yanxiufei.cn/gtelpgaxxb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.mhx1999.top/gtlsfitgfd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtjwygfhiu.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangtech.top/gtznqjwwkl.html

Java: s.substring(1, 4)
来源：http://hz.mhx1999.top/gtrzsmdovh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.316326.xyz/gtlhzhwumk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigufen.top/gtxznwictu.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigfzy.top/gtbcowixdk.html

[E04] 查找子串位置
来源：http://hz.quarkkingdee.top/gtsajohacd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj20258888.top/gtwhaivfhn.html

PHP:  strpos($s, "x");
来源：http://hz.xinyue.icu/gtypfnwwew.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yonumen.top/gtwbucoklt.html

TS:   s.indexOf("x")
来源：http://hz.yuxming.cn/gteipaweos.html

Java: s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtubggbnkf.html

Go:   strings.Index(s, "x")
来源：http://hz.daxiang520.top/gtqqawwogv.html

Ruby: s.index("x")
来源：http://hz.hywenlv.cn/gtimxjjrum.html

C#:   s.IndexOf("x")
来源：http://hz.jianghu66.top/gtzuudreit.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dianchejie.cn/gtckbpdvux.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gttooyjcdn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cqqwz.cn/gtpoilnagz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gttfbgqppo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.iojbl.cn/gtydhewtkt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtendfrwqm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cashguo.top/gthyezblln.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtqjlkjrdv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cucudq.cn/gtbsemypho.html

[E06] 替换子串
来源：http://hz.cdnleiting.top/gtbvjjqdot.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtkfmesuop.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sufxvd.cn/gtsmfwrusx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtqxgdyplx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gttfsvuudx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtffxsqdqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daxiang520.top/gtxpipvzgb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gtwhfmsbpb.html

C#:   s.Replace("a", "b")
来源：http://hz.ehwqpu.com/gtyzewlbin.html

[E07] 按分隔符拆分
来源：http://hz.daria6918.cn/gtprjzflnh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.quarkkingdee.top/gtsedpuuna.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhengqikj.top/gtnpgmrapa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtoqlahdyi.html

TS:   s.split(",")
来源：http://hz.hywenlv.cn/gtvuiaxdum.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhiwuduotai.top/gtrxvtwkse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigufen.top/gtdxefcjka.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gtjbeugobe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.kuanghao11.cn/gtmfbrcnjr.html

[E08] 数组按分隔符合并
来源：http://hz.sufxvd.cn/gtqgwsdqjb.html

Py:   ",".join(items)
来源：http://hz.birdmap.top/gthospwhzj.html

PHP:  implode(",", $items);
来源：http://hz.guannengcc.top/gtqlrexqws.html

JS:   items.join(",")
来源：http://hz.cqqwz.cn/gtsgymehqx.html

TS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtwlvvbkbr.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtijeadhnr.html

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtgaebcomc.html

Ruby: items.join(",")
来源：http://hz.ivvv.top/gtvbjvcwpp.html

C#:   string.Join(",", items)
来源：http://hz.jinyuanbaomall.cn/gttbclwgfx.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtfnojnflg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtishfajxy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtsfhnfrmo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtrpudykjz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtzqfugglw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangdashe.top/gtqwcjkylh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhijiandao.cn/gtnlfddjeu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xingfuxueyuan.xyz/gtgjfreagm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtmjekasqv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.9152youxi.cn/gthylkcdtm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtvpcvzgyi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sweek.top/gtcfentcgj.html

JS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtekgujkth.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtykxdrvmi.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtfufgudxc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtgyfcwkzp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gtzuwtvoas.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xylfe.cn/gtqsnfwkwp.html

[E11] 反转字符串
来源：http://hz.hammf.cn/gtonvsrvyi.html

Py:   s[::-1]
来源：http://hz.0kj1m.cn/gtogoikjoj.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gtuyhbvexn.html

JS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtguzhkjcz.html

TS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtbiqogvpt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtmhpzqsxp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj202588.top/gtogqlbajr.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtjwwurlvi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtwzsqdpuz.html

[E12] 统计某字符出现次数
来源：http://hz.fengsongda.top/gthfgscxfh.html

Py:   s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtjjuzmaoc.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtjlgzqzgw.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtnvforqze.html

TS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtuhcwsxdy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gtbmkmthit.html

Go:   strings.Count(s, "a")
来源：http://hz.hammf.cn/gtjmuryetn.html

Ruby: s.count("a")
来源：http://hz.kuanghao11.cn/gtqanwdzgk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ehwqpu.com/gtyctspdjq.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtjvpkeurj.html

Py:   for ch in s: print(ch)
来源：http://hz.sxryk.cn/gttmmchjxn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtlmnaxueu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtkhnuiykm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtevyeladx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yanxiufei.cn/gtnplwiurz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yangfankeji.com/gtiypoiuyq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tianlin.xyz/gtkjpurtwd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.52xcode.cn/gtihwzndih.html

[E14] URL 编码与 Base64
来源：http://hz.hammf.cn/gtbcvyxarb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenjidiqi.icu/gtzqmxqhgi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtvnvtpefr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yongpay.top/gttyfmqhrl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fengsongda.top/gtaiyaqnix.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258888.top/gtmxcxruis.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gthqnwmruf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtjfjttlav.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtbbsegrzq.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtkomrwdxr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxuanxn.top/gtgvazxnzz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zdqjudy.top/gtkmzvbavd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hammf.cn/gtiofhalze.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtezuziwqx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tanke756.top/gtsmnudewg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.feifeiyinyue.top/gtwsnpgcuk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtvxgkobih.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cheryme.top/gtxoshqvtv.html

[E16] 数字千分位
来源：http://hz.ppjwa.cn/gtwmgrroht.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtrbitpcjx.html

PHP:  number_format(1234567);
来源：http://hz.birdmap.top/gtnbysobfs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtxtjfcgqw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtbwpbhiye.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhixingplan.top/gtwtwqnhjc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhixingplan.top/gteqgsyspi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtigctpgjp.html

C#:   1234567.ToString("N0")
来源：http://hz.wangshuangyany.cn/gtvxguuhtu.html

[E17] 首字母大写
来源：http://hz.shangyingyoupin.top/gthejfsgqn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ybcxt.top/gtckeirnop.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtctexdbqu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtlwsiwzyu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtmxajxvuc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.quarkkingdee.top/gtesifubbd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sysykeji.top/gtthvtpywi.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gtfhhdlglc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ydzc1.top/gtojnnpcui.html

[E18] 模板占位符替换
来源：http://hz.smart0.xyz/gtdaymzadr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gtvibeqago.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtbwxdrrqo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtzytfxnsd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtnwuyquih.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtgzroltwd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.andypj.xyz/gtdpxbwfmu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gtlmucsteg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258.top/gtbjvdcxvf.html

[E19] 多行文本按行拆分
来源：http://hz.jlsjyb.cn/gtscojiykn.html

Py:   s.splitlines()
来源：http://hz.hammf.cn/gtnijaoerc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtwbxzmavs.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtcydrcxxx.html

TS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gtulsnymvf.html

Java: s.lines().toList()
来源：http://hz.zhixingplan.top/gtzkesfnip.html

Go:   strings.Split(s, "\n")
来源：http://hz.sufxvd.cn/gtuwpkjqwp.html

Ruby: s.lines
来源：http://hz.fzhhl.top/gtjqubvtgi.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtyesdjwhb.html

[E20] 判断字符串是否为空
来源：http://hz.yuxming.cn/gtjlenybeh.html

Py:   if not s:
来源：http://hz.daxiang520.top/gtmfdtqjga.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cqqwz.cn/gtaqytfcot.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aizwys.cn/gtgyfnevig.html

TS:   if (s === "") {}
来源：http://hz.meibo888.top/gtmfkfblhj.html

Java: if (s.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtdeoifjhl.html

Go:   if s == "" {}
来源：http://hz.jqgfzy.top/gtxbrxscom.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtcfogjwqa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.316326.xyz/gtefcdwkqu.html

[E21] 超长截断加省略号
来源：http://hz.pycfn.com/gtpczxdhuc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jinqigfzy.top/gtbgfyasmk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258888.top/gtwpexeqvg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtdxehorcm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtfprhxdop.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtcppkpklb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigufen.top/gtbsmslkfq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gtjqihllma.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.quarkkingdee.top/gtfmrbgagq.html

[E22] 字节长度与字符长度
来源：http://hz.mhx1999.top/gtqydyaqvj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtzdqlnrrf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtdfhpgnzn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtfjpmdktg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtkmbwynli.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sweek.top/gtdofbfkzl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ehwqpu.com/gtygdaaitm.html

Ruby: s.bytesize;  s.length
来源：http://hz.mhx1999.top/gtlxshkihq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daria6918.cn/gtavljibtd.html

================================================================================
来源：http://hz.jqgfzy.top/gtiryfmsgu.html

F. 文件与目录
来源：http://hz.yongpay.top/gtuvlbxmke.html

================================================================================
来源：http://hz.tianlin.xyz/gtbicbjojp.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gtjszexlev.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.guannengcc.top/gtgnjlywke.html

PHP:  file_get_contents("a.txt");
来源：http://hz.9152youxi.cn/gthiwmmrna.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydjk.org.cn/gthhbmupxj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pengpengdd.cyou/gtucfjgndd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtulavdirl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.snrcjt.cn/gtdquwqsxx.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtqnvnxjwi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gotoacloud.top/gtfgkjhdmw.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtdxxdypsi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.snrcjt.cn/gtvgeeacpn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnqzz.top/gttdbizavd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhixingplan.top/gtochoivqv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtjjjgxujx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtrzopvzna.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtflqgqcjn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.meibo888.top/gtqtsmbucn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zycfv.cn/gtbpkvwogg.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtmhhifrdx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shangyingyoupin.top/gtytjvcuap.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.birdmap.top/gtqtubxbsq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtuwktdhqr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtlpgizqdq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gotoacloud.top/gtgjyotkdr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtrgzesrlq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tian-w.cn/gtpjasxdot.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtswvzyurt.html

[F04] 追加写入文件
来源：http://hz.haohaochexian.top/gtkgpihpae.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ppjwa.cn/gthvtntqaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtknvausbt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tianlin.xyz/gtjxsuglga.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtwhgvhbgd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydzc1.top/gtyxdcpuoq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtbvcvavsx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtoekwfjpk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtxonuxwzq.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtikcszhiu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gthgpqreiw.html

PHP:  file_exists("a.txt");
来源：http://hz.fzhhl.top/gtksuqlgzt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtekqgabwf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtlvblpudy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtzybmpspg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shangyingyoupin.top/gtxlatxkih.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gtcqyqnifv.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgfzy.top/gtiddqazuo.html

[F06] 删除文件
来源：http://hz.ehwqpu.com/gtqrxoxnrc.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtchpnvtvj.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gthxgosrfk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtcpmpejia.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtcffpjykb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtwnkjombw.html

Go:   os.Remove("a.txt")
来源：http://hz.tanke756.top/gtgxmzzckp.html

Ruby: File.delete("a.txt")
来源：http://hz.daria6918.cn/gtgmiwbcst.html

C#:   File.Delete("a.txt");
来源：http://hz.tianlin.xyz/gtpjzekjzr.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtxckvhovm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtbqaqhbyz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daxiang520.top/gttjimkdfh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtsdfalxyj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtdqgsxzaq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtbsfnlxae.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aibaodan.cn/gtzobacazc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dianchejie.cn/gtrpjxoxsv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhixingplan.top/gtlrgpxybz.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gtcdhtyjvs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigfzy.top/gtxassyxcl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtyxfflaay.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtvtxevpgv.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtfmeruvbv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtwgilbyxn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pengpengdd.cyou/gtxzyxwzke.html

Ruby: Dir.children("dir")
来源：http://hz.wangshuangyany.cn/gtihvydcls.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtsayomlwx.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtdajtmeal.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gtoajkntvz.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gtbledzusk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtrppdxuch.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtyuzulolw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtlkadbeot.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.bjfxy.top/gtdgjzmgwr.html

Ruby: File.size("a.txt")
来源：http://hz.gogol.net.cn/gthlfwgifm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtnephnrii.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dianchejie.cn/gtauhbsmlw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtmohrxhyg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtrfklmyxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtytgnmhzf.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtrlktndxe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtbgaarekx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtlmaxrvsj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtreufjmmh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gotoacloud.top/gtfdfxymcp.html

[F11] 复制与移动文件
来源：http://hz.zdqjudy.top/gtfkcrzcnq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gthyyzppju.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hysaishi.cn/gtycacsozh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtmstxkfnq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gthhbgsdxe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dashuyun.cn/gtjwzoqkhp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtyqyynenb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtxxsnydrr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtmilcgmtg.html

[F12] CSV 读写
来源：http://hz.xziqi.cn/gtkndtzypz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jyoumei.cn/gtcfbehnws.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtnzdvwvdb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangtech.top/gtemydbvli.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtdlifjgfb.html


<!-- 参考信息 -->