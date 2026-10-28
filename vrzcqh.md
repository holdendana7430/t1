代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hywenlv.cn/gtzjgpokkk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuanzx.com/gtsxonibzp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daria6918.cn/gtkdnqfrpo.html

[D26] 数组转字符串
来源：http://hz.redwolf501.top/gtwkxydoha.html

Py:   ", ".join(map(str, arr))
来源：http://hz.havefunace.top/gttwuxljmr.html

PHP:  implode(", ", $arr);
来源：http://hz.quarkkingdee.top/gtovrctwqe.html

JS:   arr.join(", ")
来源：http://hz.ivvv.top/gtqbgkjsfx.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gtbaghmbua.html

Java: String.join(", ", list)
来源：http://hz.zhongyouzk.top/gtqlswjrvi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtlpbzyaru.html

Ruby: arr.join(", ")
来源：http://hz.wangdashe.top/gtuxmazvrx.html

C#:   string.Join(", ", list)
来源：http://hz.9152youxi.cn/gtsnibgksy.html

================================================================================
来源：http://hz.zhongyouzk.top/gtyqugjedh.html

E. 字符串处理
来源：http://hz.shanyushiyangkeji.top/gtkpiinnbe.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgdhowmdc.html

[E01] 拼接字符串
来源：http://hz.gzhubu.top/gtaapooeiw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yongpay.top/gtiiqyubte.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gotoacloud.top/gtrqbpewij.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtkwyqhtao.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtirqcvccl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shuidangran.top/gtncjppqqp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhaomingkeji.xyz/gteyobfzca.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhixingplan.top/gtjjpgyoxo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hfpthk.cn/gtczjenxlm.html

[E02] 重复字符串
来源：http://hz.guowangkeji.top/gtffcnduef.html

Py:   "ab" * 3
来源：http://hz.sufxvd.cn/gtozfaakox.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yueranfly.top/gtseroppaq.html

JS:   "ab".repeat(3)
来源：http://hz.yongpay.top/gttblsvbxt.html

TS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtzczpvrdk.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtrddxrevd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgfzy.top/gtrlhqsbgo.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtughugwwc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtnzodlffp.html

[E03] 截取子串
来源：http://hz.sufxvd.cn/gtpedosfuj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gotoacloud.top/gtqcoijjno.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hfpthk.cn/gttmwcaepf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtxitqubfk.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gtojmbpvlk.html

Java: s.substring(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtdzuycbhi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenjidiqi.icu/gtnmnjvffg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jyoumei.cn/gtuzmjxlvd.html

C#:   s.Substring(1, 3)
来源：http://hz.aizwys.cn/gtcllkhffv.html

[E04] 查找子串位置
来源：http://hz.ehwqpu.com/gtzprwaqlp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yangfankeji.com/gteqhchhfz.html

PHP:  strpos($s, "x");
来源：http://hz.c1oappe.top/gthhqdrlep.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hongshengwenyu.top/gtjyfdizaa.html

TS:   s.indexOf("x")
来源：http://hz.xinyue.icu/gtbdowfvaq.html

Java: s.indexOf("x")
来源：http://hz.xinyue.icu/gtbjyithgg.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gtladvfbql.html

Ruby: s.index("x")
来源：http://hz.gogol.net.cn/gtnekpkyjy.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtbnmnmjvs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtlguplqhr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pengpengdd.cyou/gtquxmgtop.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shuidangran.top/gtvcitbruv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtanfqgdzb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sufxvd.cn/gtwamoqeqn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aizwys.cn/gtibfcuzfl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yanxiufei.cn/gtzxaenfus.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtmrdwknoi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yangfankeji.com/gtlzilykbn.html

[E06] 替换子串
来源：http://hz.yueranfly.top/gthzyvlhyq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.svipenyu.cn/gtbvlgzguh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zycfv.cn/gtkwdyqiqk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtkuhcfmbj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtahxeucsr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtlzelgxoz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenlongwang.top/gthnccccmy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zdqjudy.top/gtkvifppnl.html

C#:   s.Replace("a", "b")
来源：http://hz.ppjwa.cn/gtzrchewbq.html

[E07] 按分隔符拆分
来源：http://hz.chenzaomai.com/gtosmkdolq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gtginsuacn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yangfankeji.com/gtnwpqucij.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangkeji.top/gtocgmwywf.html

TS:   s.split(",")
来源：http://hz.guannengcc.top/gtlgxzqwom.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangshuangyany.cn/gtybtmpqrx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuxming.cn/gtrvlblwhk.html

Ruby: s.split(",");  s.split
来源：http://hz.xziqi.cn/gtvquzqwbn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shzxlz.cn/gtuvlogcuv.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtjdtpibwg.html

Py:   ",".join(items)
来源：http://hz.yuxming.cn/gtuftbykpn.html

PHP:  implode(",", $items);
来源：http://hz.ydjk.org.cn/gtdmyerrnf.html

JS:   items.join(",")
来源：http://hz.yongpay.top/gtylknsszs.html

TS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtzkjqerqc.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gtidjxqsyb.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gtrvcwqtkk.html

Ruby: items.join(",")
来源：http://hz.kuanghao11.cn/gttypoyuxd.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gtccnzdxvs.html

[E09] 去除所有空白字符
来源：http://hz.xziqi.cn/gtmgergtxy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yanxiufei.cn/gtrlcvvxnh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinghuilouyu.cn/gtyoughslt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtizrkwqkt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtwwxqmjcy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guannengcc.top/gtmwibqgpi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxinkj.top/gttflmjklv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xziqi.cn/gticpgjxas.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj202588.top/gtwrlxlqjo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cashguo.top/gtomcmhywg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pengpengdd.cyou/gtzmhkzdli.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxuanxn.top/gtyrnqpwiw.html

JS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtdwejsfmy.html

TS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtnbnzgqrs.html

Java: String.format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtfwtckdci.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yueranfly.top/gtlxsmakmw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hfpthk.cn/gtrnsaajhy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aizwys.cn/gtmsohxjzn.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtaybtcsbd.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtodsdsuze.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtmlqoiddp.html

JS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtawvdukgp.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtkjkgjdzw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258888.top/gtfebmgkza.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtpwobjiwp.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtevhcdxzc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtwifoommt.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gtokshefhn.html

Py:   s.count("a")
来源：http://hz.nanxinkj.top/gtmvgobgwl.html

PHP:  substr_count($s, "a");
来源：http://hz.wangdashe.top/gtioauthei.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtvwzpnwla.html

TS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtpkpavgcu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtryuleaiu.html

Go:   strings.Count(s, "a")
来源：http://hz.ppjwa.cn/gtwkbwuxzm.html

Ruby: s.count("a")
来源：http://hz.hysaishi.cn/gtnqzlukwd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtragimhap.html

[E13] 逐字符遍历
来源：http://hz.c1oappe.top/gtcusmwgss.html

Py:   for ch in s: print(ch)
来源：http://hz.52xcode.cn/gthsgvdyap.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dashuyun.cn/gtwqbrpbej.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hysaishi.cn/gtisiriakw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtaevxexnu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhaomingkeji.xyz/gtsgxohrle.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aizwys.cn/gtnvhdebtz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.feifeiyinyue.top/gtrkkvmpgn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.mhx1999.top/gtufzdoqgo.html

[E14] URL 编码与 Base64
来源：http://hz.zdqjudy.top/gtydzvgvvo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dashuyun.cn/gtglifhaxh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.havefunace.top/gtdytwekee.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.meibo888.top/gtytocdtxk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xinyue.icu/gttckzgwzn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydzc1.top/gtfxpfbyyp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtcgareyte.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fengsongda.top/gtjqrjqbxq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ppjwa.cn/gtobcdeeci.html

[E15] HTML 转义 / 反转义
来源：http://hz.hfpthk.cn/gtgshruqks.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtuytkyjaz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinyuanbaomall.cn/gtydmpfffl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gthtvglaeb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinqigufen.top/gtipcwcsfa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.svipenyu.cn/gtelxgjwhg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258.top/gtksqpaudc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fengsongda.top/gtbykagbeb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tianlin.xyz/gtbqollocl.html

[E16] 数字千分位
来源：http://hz.cucudq.cn/gtrijwhcfc.html

Py:   f"{1234567:,}"
来源：http://hz.kuanghao11.cn/gtstztoush.html

PHP:  number_format(1234567);
来源：http://hz.pycfn.com/gtqszyvqgx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtxbfhhgkc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtnztumwoy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinghuilouyu.cn/gtwypduzrr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guowangkeji.top/gttdwwjzzp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.kuanghao11.cn/gtvqhincdz.html

C#:   1234567.ToString("N0")
来源：http://hz.chenzaomai.com/gtnzzupirr.html

[E17] 首字母大写
来源：http://hz.shuidangran.top/gtotxqydzc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hongshengwenyu.top/gtmjafvmps.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydjk.org.cn/gtcvfbziot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtqtdvqznc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtuhkejwko.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtisiesumw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.smart0.xyz/gtjzweeler.html

Ruby: s.capitalize
来源：http://hz.xingfuxueyuan.xyz/gtflqyllqa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ydzc1.top/gtqnmwcfvu.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gtaujftyyq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.pycfn.com/gtayfqrjsg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.birdmap.top/gtaipdsyof.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtmxtjvhfr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtxuibkwme.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhoulong.xyz/gtuhptrpxe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuetiantiany.cn/gtdnfdzjxk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dashuyun.cn/gtyhxatqlf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shanyushiyangkeji.top/gtouppscsu.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtnzclzdoq.html

Py:   s.splitlines()
来源：http://hz.hfpthk.cn/gtgnreyguz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuetiantiany.cn/gtpugafeta.html

JS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtudszdjta.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtuwrvlpeq.html

Java: s.lines().toList()
来源：http://hz.gzhubu.top/gtcrztzxjz.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtaafxuiwb.html

Ruby: s.lines
来源：http://hz.ybcxt.top/gtuvrstkrw.html

C#:   s.Split('\n')
来源：http://hz.mhx1999.top/gtgkxibrud.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtyjarlyzp.html

Py:   if not s:
来源：http://hz.birdmap.top/gtlldkuxcc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtkpovrsob.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hysaishi.cn/gtluieazzp.html

TS:   if (s === "") {}
来源：http://hz.jlsjyb.cn/gtoxyqdxzh.html

Java: if (s.isEmpty()) {}
来源：http://hz.daria6918.cn/gtbpfebuby.html

Go:   if s == "" {}
来源：http://hz.hfpthk.cn/gtubjddlvg.html

Ruby: if s.empty?
来源：http://hz.hnqzz.top/gtsvadogpx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtvrctpzsp.html

[E21] 超长截断加省略号
来源：http://hz.cqqwz.cn/gtvcvhsrts.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xinyue.icu/gtezjjptzz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtgagcvxkz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtnypjgfbk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtdokewpqa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtzwipjqsy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhaomingkeji.xyz/gthczyvmke.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nwbrower.top/gtfdskteck.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenzaomai.com/gtktkxqvlo.html

[E22] 字节长度与字符长度
来源：http://hz.chenjidiqi.icu/gtubkasepf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtppmikaev.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtzfdyevbo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtbsgpkuss.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtlphrndgj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.snrcjt.cn/gtwhcubjfj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xingfuxueyuan.xyz/gttuzmlbey.html

Ruby: s.bytesize;  s.length
来源：http://hz.yvedp.cn/gtulpybyui.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xylfe.cn/gtbdghxmmo.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtppwybeyi.html

F. 文件与目录
来源：http://hz.xuetiantiany.cn/gtawcwvgmr.html

================================================================================
来源：http://hz.cqqwz.cn/gtgycicolz.html

[F01] 读取整个文件
来源：http://hz.yonumen.top/gtjignhfcc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yonumen.top/gtvhrmzejs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yangfankeji.com/gtuwpiwuph.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guannengcc.top/gtodwleylb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtifzkqnrv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtabifsnhq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gthgimdlpd.html

Ruby: File.read("a.txt")
来源：http://hz.vqdsnc.cn/gtqquvzdjo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuxming.cn/gtwvzlzpnl.html

[F02] 逐行读取文件
来源：http://hz.iojbl.cn/gtsyrlgqwc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtyhnxohui.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtnejgjplc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtsspyggjr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gtqrwovlfj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtoulkgiid.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtefwruppe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.andypj.xyz/gtaygtdrid.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtdoyejwxy.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gtvqfhtcez.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigfzy.top/gtyklxdvvw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtqpedujkj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtyzryrwjp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtweantawu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtzzgfyxfr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtcodjmrro.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuanzhike.top/gtucdplcpa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtnsarqwuf.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gtthxbadct.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtnqdpumsw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtwnchdbyl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtpizoypsr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtljtbszbf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guowangkeji.top/gtiiziaqqa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtfsztngrm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yonumen.top/gtppnrrlbx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258.top/gtjsevcmgv.html

[F05] 判断文件或目录是否存在
来源：http://hz.sysykeji.top/gttyvggzwh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daria6918.cn/gtcylspqkh.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigfzy.top/gtgomahknd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtpmqjwfxm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtsvgcbvik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtcbghlyex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigufen.top/gtdponqplg.html

Ruby: File.exist?("a.txt")
来源：http://hz.gotoacloud.top/gtktpoigjp.html

C#:   File.Exists("a.txt")
来源：http://hz.hammf.cn/gtwmzqbfxi.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtuukveszk.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gtvdfilhnk.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtdbgwgoud.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gtxdrfavpb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtuwcgwfit.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtebvlhdpn.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtxmfymacr.html

Ruby: File.delete("a.txt")
来源：http://hz.ydzc1.top/gtcxtbaejo.html

C#:   File.Delete("a.txt");
来源：http://hz.zhengqikj.top/gtfluyaxgp.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtckeglagd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtrxmiikbz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtimdfduyk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtkrinmtnj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtdunglhol.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtcryuehcm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtzvzqpush.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cheryme.top/gtrcrnyqzs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jianghu66.top/gtizdhklts.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtcdpmlbbn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtuzcufwyb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gogol.net.cn/gtfkasrbzt.html

JS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gtutiutuzb.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtblolniym.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.meibo888.top/gttrvnmass.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtqmgupmwt.html

Ruby: Dir.children("dir")
来源：http://hz.sweek.top/gtqqucdsct.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sweek.top/gtlbppyort.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtkvuhqosu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtfxfnibqf.html

PHP:  filesize("a.txt");
来源：http://hz.mhx1999.top/gtuwstziqx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtknjsvnfv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtwliqvzde.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtmwlyjdql.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxinkj.top/gtxkxngwjk.html

Ruby: File.size("a.txt")
来源：http://hz.cashguo.top/gtxsjwyuct.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gogol.net.cn/gtbgghbfxs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtfsxjqdbx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtuzdthnxn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gtkakhdojt.html


<!-- 参考信息 -->