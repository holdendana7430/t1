代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guannengcc.top/gtlubosuzt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cashguo.top/gtadrvltyh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenlongwang.top/gtgeumosgt.html

[D26] 数组转字符串
来源：http://hz.hnxiangtu.top/gtokbwvwbd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sxryk.cn/gtsaufvozy.html

PHP:  implode(", ", $arr);
来源：http://hz.hongshengwenyu.top/gtikkklcqj.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtdtuetimo.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtwrdcuvim.html

Java: String.join(", ", list)
来源：http://hz.yj20258.top/gtfhhfjkog.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gzhubu.top/gtursnzaes.html

Ruby: arr.join(", ")
来源：http://hz.yangfankeji.com/gteevpoktn.html

C#:   string.Join(", ", list)
来源：http://hz.mhx1999.top/gtolvirnxi.html

================================================================================
来源：http://hz.daria6918.cn/gthrgegnfx.html

E. 字符串处理
来源：http://hz.yanxiufei.cn/gtosiobhzv.html

================================================================================
来源：http://hz.tianlin.xyz/gtioryuxek.html

[E01] 拼接字符串
来源：http://hz.cashguo.top/gtjvglarvc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sweek.top/gtfqpwzyed.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhijiandao.cn/gtfxhfgfjw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtoqdvvsel.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtjmqfkoft.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jianghu66.top/gtepzguofh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yueranfly.top/gtzewdafof.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinyuanbaomall.cn/gtbdkaivrd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jianghu66.top/gtyrssbrne.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtavcttafw.html

Py:   "ab" * 3
来源：http://hz.pycfn.com/gtcclsltrt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhixingplan.top/gtzitqmvmt.html

JS:   "ab".repeat(3)
来源：http://hz.xylfe.cn/gthfrygymu.html

TS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtlwrptgtc.html

Java: "ab".repeat(3)
来源：http://hz.yuxming.cn/gtatxjuvpo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.meibo888.top/gtmdoguzdw.html

Ruby: "ab" * 3
来源：http://hz.yongpay.top/gtlugwfhoc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenzaomai.com/gtlmgkpdxv.html

[E03] 截取子串
来源：http://hz.andypj.xyz/gtbrfvcvgc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtlaostbtq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gtutylnejb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sxryk.cn/gthnssajqq.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtuboertcl.html

Java: s.substring(1, 4)
来源：http://hz.gzhubu.top/gtnjxmidft.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.redwolf501.top/gtdzyhooop.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.fengsongda.top/gtdhemsxgc.html

C#:   s.Substring(1, 3)
来源：http://hz.hywenlv.cn/gtgwbczxdt.html

[E04] 查找子串位置
来源：http://hz.zycfv.cn/gtzmbdnlvq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hammf.cn/gtiyzuwvfi.html

PHP:  strpos($s, "x");
来源：http://hz.yueranfly.top/gtlwylctoe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.316326.xyz/gtwyryegns.html

TS:   s.indexOf("x")
来源：http://hz.smart0.xyz/gtofxiusnw.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gtwpufsvrw.html

Go:   strings.Index(s, "x")
来源：http://hz.guannengcc.top/gtyasuscpv.html

Ruby: s.index("x")
来源：http://hz.yueranfly.top/gtpqcxkoul.html

C#:   s.IndexOf("x")
来源：http://hz.hongshengwenyu.top/gtbhfzkeut.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shangyingyoupin.top/gtlsdnjubp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pengpengdd.cyou/gtnqwlrwvf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.316326.xyz/gtuyyuverz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtqivppkfd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenjidiqi.icu/gtfqyyutzv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtrlgwmhya.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yueranfly.top/gtbtvjxxsv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jyoumei.cn/gtfqpcuscz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhoulong.xyz/gtkqzncinp.html

[E06] 替换子串
来源：http://hz.haohaochexian.top/gtyghkudtg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtqylbgbge.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtnemwvxgg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtnrtbsyef.html

TS:   s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtmmtentnz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtqkmnpqhw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jiagoushi.top/gtreyvfixe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ybcxt.top/gttrdjoxrk.html

C#:   s.Replace("a", "b")
来源：http://hz.gaohongyu789.top/gtcveruptz.html

[E07] 按分隔符拆分
来源：http://hz.dashuyun.cn/gtilhuzihh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtbwposghx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxuanxn.top/gttdnuqmbo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.haohaochexian.top/gtepccuaok.html

TS:   s.split(",")
来源：http://hz.mhx1999.top/gtociujuhx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258888.top/gtmvtsfbtg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yongpay.top/gtfsbgwrou.html

Ruby: s.split(",");  s.split
来源：http://hz.yuanzhike.top/gtmycpnudt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fengsongda.top/gtvntpvqhj.html

[E08] 数组按分隔符合并
来源：http://hz.shanyushiyangtech.top/gtzghdvlqc.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtrfkcklys.html

PHP:  implode(",", $items);
来源：http://hz.tianlin.xyz/gtmpugtvyv.html

JS:   items.join(",")
来源：http://hz.dianchejie.cn/gtxyxejjmr.html

TS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtrhnzzyxi.html

Java: String.join(",", items)
来源：http://hz.jlsjyb.cn/gtiskxigym.html

Go:   strings.Join(items, ",")
来源：http://hz.aizwys.cn/gtitkxnbwo.html

Ruby: items.join(",")
来源：http://hz.aizwys.cn/gtnqogauwf.html

C#:   string.Join(",", items)
来源：http://hz.ivvv.top/gtmftemkes.html

[E09] 去除所有空白字符
来源：http://hz.9152youxi.cn/gtoluagfjy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtidccffed.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cheryme.top/gtwtbwnysp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtlgaktzts.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtpspzxwvo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gteockdcdo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dashuyun.cn/gtlbdaancs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.smart0.xyz/gtvinzegfw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cashguo.top/gtgsklykra.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgufenzy.top/gtddlgxwzu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.c1oappe.top/gtuydxuenu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.0kj1m.cn/gtaltbyblp.html

JS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtabybgxiv.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtbivqnklc.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigufen.top/gtfosjxjbd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gtbonnfkzv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tian-w.cn/gtdbxauvsf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinghuilouyu.cn/gtlpyucrwv.html

[E11] 反转字符串
来源：http://hz.52xcode.cn/gtpyzqmcej.html

Py:   s[::-1]
来源：http://hz.yvedp.cn/gtnkrjunnl.html

PHP:  strrev($s);
来源：http://hz.chenjidiqi.icu/gtufuqdwyp.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtkvdsetif.html

TS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gttcpjwftm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.0kj1m.cn/gtwdlnqumb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtuvnetggo.html

Ruby: s.reverse
来源：http://hz.52xcode.cn/gtvrhurjqr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtdfnmghoy.html

[E12] 统计某字符出现次数
来源：http://hz.yuxming.cn/gtjgkgalax.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gtqqpmdedh.html

PHP:  substr_count($s, "a");
来源：http://hz.ybcxt.top/gtjatgiyoz.html

JS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtccsfvfvq.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtkkbaaqll.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtqdilwnfa.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtvrujqdxd.html

Ruby: s.count("a")
来源：http://hz.smart0.xyz/gtwuymgexk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.daxiang520.top/gtiosghaix.html

[E13] 逐字符遍历
来源：http://hz.aibaodan.cn/gtfyfuskli.html

Py:   for ch in s: print(ch)
来源：http://hz.tianlin.xyz/gtbcqeyurc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangtech.top/gtmyuxtpdc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hongshengwenyu.top/gterwxcxsc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hysaishi.cn/gtyvvlojat.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigufen.top/gthxdgbjnm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yangfankeji.com/gtpwhnntfm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tianlin.xyz/gtwblhiwcw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtgmagjsev.html

[E14] URL 编码与 Base64
来源：http://hz.jinyuanbaomall.cn/gtbbwxvvqh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gtwmaefboc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gotoacloud.top/gtrqlfdpls.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zdqjudy.top/gtnhrlopii.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shuidangran.top/gtkrmnvyvt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tian-w.cn/gterhnjyew.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yanxiufei.cn/gtclzvyqld.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigfzy.top/gtfiueuzyi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhongyouzk.top/gtqcozygll.html

[E15] HTML 转义 / 反转义
来源：http://hz.haohaochexian.top/gtjjryeibq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.316326.xyz/gtzoloavmq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.iojbl.cn/gtrireqrzx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ivvv.top/gtevskykbu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.andypj.xyz/gtwshvytql.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtmyfrwmlk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gtfcfgxosg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dashuyun.cn/gtebaruzuo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtihqbcdaa.html

[E16] 数字千分位
来源：http://hz.guannengcc.top/gtnsjmuawi.html

Py:   f"{1234567:,}"
来源：http://hz.jiagoushi.top/gtanzzmuru.html

PHP:  number_format(1234567);
来源：http://hz.fzhhl.top/gtyfylplgc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtycszortn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtlouugxhq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gthommuxrw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtarwwegcy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxuanxn.top/gtfwzdwrwm.html

C#:   1234567.ToString("N0")
来源：http://hz.wangshuangyany.cn/gtdapvfqov.html

[E17] 首字母大写
来源：http://hz.jinyuanbaomall.cn/gtojskjqdk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.kuanghao11.cn/gtrhmixxcb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gthiwunuiq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtmmpcglay.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtfnhteiyz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.bjfxy.top/gtvnobzvuv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhixingplan.top/gtorxrxlcl.html

Ruby: s.capitalize
来源：http://hz.yueranfly.top/gtwkegetue.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtwbmvkbab.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gtxzqobmih.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fzhhl.top/gtqdnviooo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtmobxeism.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtyttxpbla.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtpdmqpcoj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.kuanghao11.cn/gtnfikkfoh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yvedp.cn/gtlolgulzb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dashuyun.cn/gtqkpodykc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtjlpwlfbk.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtobazptst.html

Py:   s.splitlines()
来源：http://hz.jlsjyb.cn/gtiqrhcdcx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hysaishi.cn/gtrgshhsys.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gttblnqriu.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtzlbqypuz.html

Java: s.lines().toList()
来源：http://hz.yuxming.cn/gtzxyyhzwr.html

Go:   strings.Split(s, "\n")
来源：http://hz.shangyingyoupin.top/gtzwvrlutu.html

Ruby: s.lines
来源：http://hz.zhijiandao.cn/gtqvgvgead.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtsgegtwou.html

[E20] 判断字符串是否为空
来源：http://hz.yanxiufei.cn/gtsdwstsia.html

Py:   if not s:
来源：http://hz.wangdashe.top/gtosarbzdp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtswefzarm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hongshengwenyu.top/gtozpktfsb.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtgeyvibvh.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtfgxjwdfy.html

Go:   if s == "" {}
来源：http://hz.guowangkeji.top/gtjncstfpn.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gtivwcpcta.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guannengcc.top/gteoknhvrj.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtiqddlebm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.daria6918.cn/gtcyyzgfdv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtqqqdbegm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtxxiswzgq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtbvrhmuqc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtdsyjkfjf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ivvv.top/gtqhylcgoj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtibfpkhdq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtvgoljxhe.html

[E22] 字节长度与字符长度
来源：http://hz.sufxvd.cn/gtbxctecrf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangdashe.top/gtievyskcw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtgtsleass.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtrcakqtqf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtwmaxxjem.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.vqdsnc.cn/gtdeqrtcmq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gtfdmiprlz.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigfzy.top/gtxldcqpdr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zycfv.cn/gtilzmpbex.html

================================================================================
来源：http://hz.jinqigufen.top/gtmcnxfkok.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtacwstmpd.html

================================================================================
来源：http://hz.xuanzx.com/gtyluvsvsa.html

[F01] 读取整个文件
来源：http://hz.hammf.cn/gtjkmiouqf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daxiang520.top/gtmciciith.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gtczwybzip.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yongpay.top/gtjtsspdfv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtygkflmae.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtvrmofjob.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aibaodan.cn/gtdtejuxil.html

Ruby: File.read("a.txt")
来源：http://hz.meibo888.top/gtaeluthzh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgufenzy.top/gtdgsemlvx.html

[F02] 逐行读取文件
来源：http://hz.wangshuangyany.cn/gtskuycdmo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinyuanbaomall.cn/gtqmteecrp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shuidangran.top/gtgmkiziwx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtpiazkrgx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtybgxqqkv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtgwvckqpc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtkmojuiuc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ehwqpu.com/gtbqvgnrpa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtibvqksuf.html

[F03] 写入文件（覆盖）
来源：http://hz.cheryme.top/gtvuolmfwb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhixingplan.top/gtitmxwkts.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sxryk.cn/gtszbdrrib.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtfixkpnzn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtfbcppqvr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuanzx.com/gtmaiouxrp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtzdncmczo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ivvv.top/gtymuqvnnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtxovyplrz.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtmejjcami.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gthdrkodvi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gtknbqlrrv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtigkacfjp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtamzofiav.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pycfn.com/gtppijxnct.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigufen.top/gtnlafnvea.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhongyouzk.top/gtrbhfulxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtizocbogm.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gtynmfbyro.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtbwbtdzcw.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtrwrlfntw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtrovjomgr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtbroxebzd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtllxtzycg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenjidiqi.icu/gtffulvcjs.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtmmwfixbc.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtadpvtjyv.html

[F06] 删除文件
来源：http://hz.shzxlz.cn/gtrfyaljtb.html

Py:   os.remove("a.txt")
来源：http://hz.haohaochexian.top/gtkofhfxng.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtcxzgwkjt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtplwbwstw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtxpjfbcfa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtjzklxbyc.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtdbjmcpcv.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtrbihuhhd.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gtkjntedpv.html

[F07] 创建目录（含多级）
来源：http://hz.wangshuangyany.cn/gtqlnkmlhv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtddocdwlx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gogol.net.cn/gtrcnzamco.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gogol.net.cn/gtancfrtks.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtroorlvic.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtbycxhykc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtvricjnis.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.0kj1m.cn/gtzlfanbfu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.mhx1999.top/gttznaxudj.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtfacasupl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gtesevucws.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jiagoushi.top/gtpfzbpfzh.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtuxzepfnr.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtqfqucwsx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtdqjyfyro.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtstuhgqbb.html

Ruby: Dir.children("dir")
来源：http://hz.yonumen.top/gtrioqjsgb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtlrqtbiyj.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtxjlueqmb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.vqdsnc.cn/gtwcdtgywx.html

PHP:  filesize("a.txt");
来源：http://hz.yonumen.top/gtjyoukwhg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtwcdpqvhg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtsxhyvtat.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtadqteqwx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shzxlz.cn/gtrdyxtkvk.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtpghdqmap.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtkzudnhbn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtycnrckqa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtojjzlhik.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zycfv.cn/gtbabcamhe.html


<!-- 参考信息 -->