代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hongshengwenyu.top/gtyzfaucld.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.andypj.xyz/gtuscioked.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shzxlz.cn/gtffjedwml.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sysykeji.top/gtkhsctpzq.html

[E02] 重复字符串
来源：http://hz.redwolf501.top/gtqzuvqvut.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtyuifujkq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258888.top/gtorttbmne.html

JS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gthwmkxbis.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtxshrdhud.html

Java: "ab".repeat(3)
来源：http://hz.zycfv.cn/gtnyijyzwd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cdnleiting.top/gtmsfavdle.html

Ruby: "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtqczmywhd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuxming.cn/gtouvszlrs.html

[E03] 截取子串
来源：http://hz.haohaochexian.top/gtetqwaemv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydjk.org.cn/gtvvmdusuv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fengsongda.top/gtpottzwls.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtcfrsullr.html

TS:   s.slice(1, 4)
来源：http://hz.xuetiantiany.cn/gtuvdisqsi.html

Java: s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtxuglqpoc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shanyushiyangkeji.top/gtrnqdkttf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gtdmldhidq.html

C#:   s.Substring(1, 3)
来源：http://hz.yongpay.top/gtualqtrsy.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtiipnzddi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtdkukwktb.html

PHP:  strpos($s, "x");
来源：http://hz.xuanzx.com/gtvpiplydr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtzmzddyjz.html

TS:   s.indexOf("x")
来源：http://hz.nwbrower.top/gtfkyijqjj.html

Java: s.indexOf("x")
来源：http://hz.c1oappe.top/gtfhzpkiow.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gtfoowylmf.html

Ruby: s.index("x")
来源：http://hz.wangshuangyany.cn/gtcbmybjxm.html

C#:   s.IndexOf("x")
来源：http://hz.kuanghao11.cn/gtqtguboqo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jianghu66.top/gtdxreyzux.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtzssgweuz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shzxlz.cn/gtgmgmaohn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fengsongda.top/gtebjfzinm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gotoacloud.top/gtqtrkioyh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtvmovwwze.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gtdjifutza.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxuanxn.top/gtcdpxkbrh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tianlin.xyz/gtlasoxyci.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtvjqqcozw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuetiantiany.cn/gtnosorygh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtwikwflzj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtjmvekauw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtxtpreinq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtkebandqo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtlrcyikhs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yangfankeji.com/gtblizpiby.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtjuqmidvx.html

[E07] 按分隔符拆分
来源：http://hz.yueranfly.top/gtxgeycrbv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangkeji.top/gtnggsxllz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gtyaonndzv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ppjwa.cn/gtemlwynhl.html

TS:   s.split(",")
来源：http://hz.aibaodan.cn/gtoimipfwe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.mhx1999.top/gtbhikpvgx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gtuvnxhvyi.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtmozaphgn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtpzdwgqal.html

[E08] 数组按分隔符合并
来源：http://hz.sweek.top/gtnztlfmjy.html

Py:   ",".join(items)
来源：http://hz.jinghuilouyu.cn/gtmgawacjh.html

PHP:  implode(",", $items);
来源：http://hz.52xcode.cn/gtedbnnnuv.html

JS:   items.join(",")
来源：http://hz.fengsongda.top/gtvpiaixoi.html

TS:   items.join(",")
来源：http://hz.yuxming.cn/gtwgsklafh.html

Java: String.join(",", items)
来源：http://hz.ywan-chungtsiang.top/gtopyyznws.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gthdafypwu.html

Ruby: items.join(",")
来源：http://hz.yanxiufei.cn/gtqhjynghe.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gtmptvrukn.html

[E09] 去除所有空白字符
来源：http://hz.zhixingplan.top/gtlfpkoqtn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.0kj1m.cn/gtwniqfzfi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ywan-chungtsiang.top/gtkbcigaom.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtktwlhxep.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.feifeiyinyue.top/gtexbrzmxz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhoulong.xyz/gtyznioktk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.haohaochexian.top/gtgwzlwmvx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shangyingyoupin.top/gtyyuevlzr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtxiyzvqbi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.daria6918.cn/gthvguaxhl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuanzx.com/gtbkbjduzk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj20258.top/gthrsytlsi.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtosclyiwq.html

TS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtlrjfcmsr.html

Java: String.format("%03d", 7)
来源：http://hz.tian-w.cn/gthhruopjl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gtahtdifpt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtssbvqrxt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenjidiqi.icu/gtcekydeio.html

[E11] 反转字符串
来源：http://hz.redwolf501.top/gtmcxuzmmo.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtneimtvif.html

PHP:  strrev($s);
来源：http://hz.dianchejie.cn/gtgpixtegs.html

JS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtkpbrunye.html

TS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtoqlwenbd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.iojbl.cn/gtlwnnzihw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pycfn.com/gtjnhqumxw.html

Ruby: s.reverse
来源：http://hz.ydjk.org.cn/gtlzgpyiqe.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gtpujtgiag.html

[E12] 统计某字符出现次数
来源：http://hz.cdnleiting.top/gtfgiyvkbq.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gthjsadlho.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtmgxkqawq.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtabpwdtpv.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtfiekzsdm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtnyuruvxx.html

Go:   strings.Count(s, "a")
来源：http://hz.ehwqpu.com/gtycrutmer.html

Ruby: s.count("a")
来源：http://hz.cheryme.top/gtoogqjmrw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gtjpnnyrlw.html

[E13] 逐字符遍历
来源：http://hz.chenzaomai.com/gtczenpeie.html

Py:   for ch in s: print(ch)
来源：http://hz.ehwqpu.com/gtiytxmndv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xuanzx.com/gtyehduahe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtyessvkbb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtfwdvlznc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xinyue.icu/gtabszboar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenlongwang.top/gtzzfytzul.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gtnupitbit.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ywan-chungtsiang.top/gtncktmdof.html

[E14] URL 编码与 Base64
来源：http://hz.andypj.xyz/gtmwozlifb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgfzy.top/gterrrcjeb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhengqikj.top/gtbaeonkxq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gtfjrvqdbc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sweek.top/gtblsiiwdr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zdqjudy.top/gtsyhxvnaj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.birdmap.top/gtasstmmxe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xylfe.cn/gtpsirtjbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yongpay.top/gtnhxbfchc.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtzgnjwsgh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gogol.net.cn/gtnsbpzeaq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtwyziltca.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shuidangran.top/gtbmxtjltg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtdcrzawcn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xinyue.icu/gtmyfppjdh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinyuanbaomall.cn/gtlgltjdqj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgfzy.top/gttxemlmaw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shangyingyoupin.top/gtbpswgnpr.html

[E16] 数字千分位
来源：http://hz.yuxming.cn/gtbvzgglkm.html

Py:   f"{1234567:,}"
来源：http://hz.zhengqikj.top/gttywyhtxt.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtybkezjcg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtrjqhtfre.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gteafirgkl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtvbxjkizq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pycfn.com/gtuxwuarai.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hfpthk.cn/gtjhvezobu.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtkzombnte.html

[E17] 首字母大写
来源：http://hz.cucudq.cn/gtvglscdsf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtgdwtmhok.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258.top/gtyoqmxbdj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtzckyxanl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtdwjvcuyx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gtvroujwyg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtwulygkfc.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtzbhuwnjx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gteflzkcec.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gtfqnfbnru.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.316326.xyz/gtmujlwcpb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gttbbfvwci.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtondqrifu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtfvoronir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhixingplan.top/gtbtqaabdi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gtvaqsiwqx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pengpengdd.cyou/gtnyytkvhy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhixingplan.top/gtmpcqeisf.html

[E19] 多行文本按行拆分
来源：http://hz.cdnleiting.top/gtgdysewht.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtvgcavvpw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhengqikj.top/gtkmiahjyx.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtznghnyqt.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtsskiyxzt.html

Java: s.lines().toList()
来源：http://hz.jqgufenzy.top/gtqwrzmmrg.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhixingplan.top/gtxwjgirnr.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gtyjicurvi.html

C#:   s.Split('\n')
来源：http://hz.fzhhl.top/gtcboqdcne.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtveeefplo.html

Py:   if not s:
来源：http://hz.jiagoushi.top/gtsyqjgaav.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ybcxt.top/gtswiixxeg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtfkekiytp.html

TS:   if (s === "") {}
来源：http://hz.cdnleiting.top/gtlfdmgiew.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtuisupsij.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtrznxqciq.html

Ruby: if s.empty?
来源：http://hz.jlsjyb.cn/gtqchdvtsc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj202588.top/gtufrkhhte.html

[E21] 超长截断加省略号
来源：http://hz.bjfxy.top/gthpybgska.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sweek.top/gtwnuanvgz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daxiang520.top/gtjtyzqimy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtivyhjdme.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtnaauqglk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtrohktyif.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtrmthdwub.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gtdzvzlrnd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gtoofztpnn.html

[E22] 字节长度与字符长度
来源：http://hz.shangyingyoupin.top/gtrbwmbzzi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fzhhl.top/gtghgnyxkv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gtxoyaerqw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtzkhjrzaa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtkcfqhxrn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtpczfdzbo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenlongwang.top/gtceqnzcxp.html

Ruby: s.bytesize;  s.length
来源：http://hz.jiagoushi.top/gtpgwaezux.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinghuilouyu.cn/gtoqyujizm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxgxitcbq.html

F. 文件与目录
来源：http://hz.wangshuangyany.cn/gtitoqdthx.html

================================================================================
来源：http://hz.hnqzz.top/gttklscaxt.html

[F01] 读取整个文件
来源：http://hz.chenlongwang.top/gthewdjkjd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gtpycrkkwk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtpeuzsaiw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgfzy.top/gttcaubdlh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jianghu66.top/gtwmoztzpn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtfnrlfdao.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gtzbetzhju.html

Ruby: File.read("a.txt")
来源：http://hz.fengsongda.top/gteazyzvua.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258888.top/gtqbijdedb.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtbxtqzeeh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtukckockh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtnkpeyvlp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtbvvqclgb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gtczegjcaa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtcgobiiio.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cucudq.cn/gtibqkdkzm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtrrpjelhk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ivvv.top/gtlmysadsb.html

[F03] 写入文件（覆盖）
来源：http://hz.jinghuilouyu.cn/gtknochghm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgfzy.top/gtapxjwwys.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zycfv.cn/gthatfoldm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigufen.top/gthejrcqdx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtjpqhdenw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gtvkgpmtao.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gtqfawyluc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.kuanghao11.cn/gttmvebmca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtprpodvpt.html

[F04] 追加写入文件
来源：http://hz.zhoulong.xyz/gtxxocuzyl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sufxvd.cn/gtqzrmkyyl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtkomzexoo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtrthbprde.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtxphnmrvk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ehwqpu.com/gtzxabamrj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtxvgjkgod.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenlongwang.top/gtwbqgotqz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jyoumei.cn/gtpulkizyt.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuanzhike.top/gtjcynukfs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangshuangyany.cn/gteurlckow.html

PHP:  file_exists("a.txt");
来源：http://hz.gogol.net.cn/gtubfuyjyh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtlnxfqpwa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtwkqodsxp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtvhruedwc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.vqdsnc.cn/gtptorpvpi.html

Ruby: File.exist?("a.txt")
来源：http://hz.aizwys.cn/gtnreoaasn.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtndfgqste.html

[F06] 删除文件
来源：http://hz.daxiang520.top/gtrgbhgnft.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtghcknpkw.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtnhcaepll.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtepsumdvd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtornvrzde.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtkvzdzond.html

Go:   os.Remove("a.txt")
来源：http://hz.wangshuangyany.cn/gttrhvvmly.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigufen.top/gtfpxfvuqj.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtlbvkfmms.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtiksfgqwa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jyoumei.cn/gtttmukftx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gtporfwgcs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gthxdeiyfx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtcginitwr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuetiantiany.cn/gtjaynbeau.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jiagoushi.top/gtjpiwmesz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhoulong.xyz/gtaxyxcwvx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hongshengwenyu.top/gttzoyufxn.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtwljjzjlt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sufxvd.cn/gtrgjamefh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtblyawmme.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtqhhociic.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtudfalett.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtkvniyceu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydjk.org.cn/gtitghkimy.html

Ruby: Dir.children("dir")
来源：http://hz.hammf.cn/gtlfitnwwt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aizwys.cn/gtpimgnwjv.html

[F09] 获取文件大小
来源：http://hz.nwbrower.top/gteegdmyxs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydjk.org.cn/gtxvergutk.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtdiryynha.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtckmmfnli.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dianchejie.cn/gtckzlumhj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtyhgppdva.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtydjgxsii.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258888.top/gthiwcpuzo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shuidangran.top/gtdjrlcsqe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pycfn.com/gtuxmeuspf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtpqnpstia.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhixingplan.top/gtlzszekie.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gthycfpbue.html

TS:   path.extname("a.txt")
来源：http://hz.redwolf501.top/gtsybwldly.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jiagoushi.top/gtpwfpmdzh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cashguo.top/gtbkxtprsi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtgclqjlhu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtirbwyzgq.html

[F11] 复制与移动文件
来源：http://hz.jianghu66.top/gtplavhibl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtkfwwdpes.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.andypj.xyz/gtwuhhijnw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtwyfczchg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtjoqdbkag.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtrryacycq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtuptucdbh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtgipvnqxp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gtavqchpdk.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtaqochkjx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtvjtslfpj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtqfejsrhm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtuetqfwmv.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtzkprikjl.html


<!-- 参考信息 -->