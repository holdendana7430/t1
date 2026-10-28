代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtlfzvjdqe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gtilrtwozj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtcpmwefcl.html

[D26] 数组转字符串
来源：http://hz.chenzaomai.com/gtbeyonpkb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gaohongyu789.top/gtdzcnpaey.html

PHP:  implode(", ", $arr);
来源：http://hz.pycfn.com/gtjuwqichn.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtsomhhluj.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtmciftatb.html

Java: String.join(", ", list)
来源：http://hz.sweek.top/gtyutewjpw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigufen.top/gttvffjoqc.html

Ruby: arr.join(", ")
来源：http://hz.cucudq.cn/gthhnpcozu.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gtujxzwhgn.html

================================================================================
来源：http://hz.ydzc1.top/gtrqdwevac.html

E. 字符串处理
来源：http://hz.tianlin.xyz/gtyedtwahy.html

================================================================================
来源：http://hz.guannengcc.top/gtpwlqruon.html

[E01] 拼接字符串
来源：http://hz.gaohongyu789.top/gthogbsyrn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtwwfbksip.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.mhx1999.top/gtrfndwjaz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtjldyfdjj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.c1oappe.top/gtpwlmsmvo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gthaxoixtj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhaomingkeji.xyz/gtvjngiker.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhijiandao.cn/gtvkandjgh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnqzz.top/gtmgthdpks.html

[E02] 重复字符串
来源：http://hz.gotoacloud.top/gtrrodcdal.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gtgokgjtza.html

PHP:  str_repeat("ab", 3);
来源：http://hz.iojbl.cn/gtrhclgtqh.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtevtzaujx.html

TS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtkaphhoks.html

Java: "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtghopwdmp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yuanzhike.top/gtipwdngoy.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtkgfwmgoy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daxiang520.top/gtcwbnmrxa.html

[E03] 截取子串
来源：http://hz.sysykeji.top/gtuyogipht.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuxming.cn/gtgarelwes.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gogol.net.cn/gtcllkrgup.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtmxnttskx.html

TS:   s.slice(1, 4)
来源：http://hz.bjfxy.top/gtdtmrxtgy.html

Java: s.substring(1, 4)
来源：http://hz.dianchejie.cn/gthzdqdjds.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxuanxn.top/gtsemrrlgk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xylfe.cn/gtrnrasxqx.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtlvfthxxa.html

[E04] 查找子串位置
来源：http://hz.hfpthk.cn/gtukqueyhu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yangfankeji.com/gtvkcxxgsu.html

PHP:  strpos($s, "x");
来源：http://hz.ybcxt.top/gtnfjjvqxi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.0kj1m.cn/gtlopvuoag.html

TS:   s.indexOf("x")
来源：http://hz.0kj1m.cn/gtwfydcbnj.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtsdqkygnl.html

Go:   strings.Index(s, "x")
来源：http://hz.tanke756.top/gtvskmgete.html

Ruby: s.index("x")
来源：http://hz.shuidangran.top/gtusnrbgpm.html

C#:   s.IndexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtmrnenpdq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.52xcode.cn/gtnasqnfbn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nwbrower.top/gtdodsnugx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.316326.xyz/gtwaamzjke.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtifkgdjbn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sysykeji.top/gtibsyqryd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtlhefjxrm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xziqi.cn/gtlowmxoip.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenzaomai.com/gthppqtanq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuxming.cn/gtzcmforbj.html

[E06] 替换子串
来源：http://hz.zhengqikj.top/gthnsfcibk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.meibo888.top/gtcoecfflb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hongshengwenyu.top/gtspfatktr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtxjsixdke.html

TS:   s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtnxqgkzew.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtmsnjcqwh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtoynegnii.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.quarkkingdee.top/gtwbbzkpuq.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxinkj.top/gtuamlhbsp.html

[E07] 按分隔符拆分
来源：http://hz.hnqzz.top/gtzcngvuut.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cashguo.top/gtswdgssjz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhijiandao.cn/gteykwargc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zdqjudy.top/gtmteqbgsj.html

TS:   s.split(",")
来源：http://hz.52xcode.cn/gtocrrcrzq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtocbszbcl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gtxzzwzhfq.html

Ruby: s.split(",");  s.split
来源：http://hz.gaohongyu789.top/gtptcmwyjz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pengpengdd.cyou/gtnqfrwphl.html

[E08] 数组按分隔符合并
来源：http://hz.aibaodan.cn/gtxsxllmii.html

Py:   ",".join(items)
来源：http://hz.fengsongda.top/gtohebyxsv.html

PHP:  implode(",", $items);
来源：http://hz.iojbl.cn/gtlhnhkamh.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtuplakidf.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtztqhholi.html

Java: String.join(",", items)
来源：http://hz.feifeiyinyue.top/gtqfwecsng.html

Go:   strings.Join(items, ",")
来源：http://hz.cucudq.cn/gtcbnpofdd.html

Ruby: items.join(",")
来源：http://hz.hongshengwenyu.top/gtixzhpwto.html

C#:   string.Join(",", items)
来源：http://hz.dashuyun.cn/gtzgghqodo.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtwyknalfk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtxheraczf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.iojbl.cn/gttxorheim.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtlzqidzsj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtkxguudse.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtbzgkuuuq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.0kj1m.cn/gtjphcfvyh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtrougjsld.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daxiang520.top/gtcfackqwm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtipkfftla.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gtdeeqhfem.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gaohongyu789.top/gtmntnbpvg.html

JS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtsqdaqbda.html

TS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gteolrinxx.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtzqfbyzse.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aizwys.cn/gthknuubxx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtejdccdxi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinyuanbaomall.cn/gtshdpwppl.html

[E11] 反转字符串
来源：http://hz.havefunace.top/gtzqlrhebh.html

Py:   s[::-1]
来源：http://hz.chenzaomai.com/gtcfbormqk.html

PHP:  strrev($s);
来源：http://hz.pengpengdd.cyou/gttjtlzxrv.html

JS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtxpmthtdk.html

TS:   [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtwwduplfo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuxming.cn/gtmfbgvzor.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gtouogndzl.html

Ruby: s.reverse
来源：http://hz.redwolf501.top/gtrirtnhoy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtsplfaesx.html

[E12] 统计某字符出现次数
来源：http://hz.hywenlv.cn/gtqpxsdriw.html

Py:   s.count("a")
来源：http://hz.ybcxt.top/gtkcnkymdq.html

PHP:  substr_count($s, "a");
来源：http://hz.fzhhl.top/gtburbppye.html

JS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtfoolmoqc.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigfzy.top/gtmkacqcrz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gtqcztrsui.html

Go:   strings.Count(s, "a")
来源：http://hz.fengsongda.top/gtpaeyjsdn.html

Ruby: s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtvwjddpos.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gtzjphiisu.html

[E13] 逐字符遍历
来源：http://hz.9152youxi.cn/gtcosbgyaj.html

Py:   for ch in s: print(ch)
来源：http://hz.zhoulong.xyz/gtnttmswko.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dashuyun.cn/gtmvdjweqw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtvzbqbznd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtldbauzgf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guannengcc.top/gtwjizsabu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtnrdmgqhn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yvedp.cn/gtngqjcipu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtcoxtyvmw.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtngojghyo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ywan-chungtsiang.top/gtpdfaqibi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gtfbztdoep.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ppjwa.cn/gtifgzqyxv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hammf.cn/gtnbzxrdbv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fengsongda.top/gtwhljnsko.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gthkzwjpzn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aibaodan.cn/gtgsybaruc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258888.top/gtochgepuj.html

[E15] HTML 转义 / 反转义
来源：http://hz.feifeiyinyue.top/gttbuowkuz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shangyingyoupin.top/gtamyfvzbc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuetiantiany.cn/gtiyytalhq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dianchejie.cn/gtijmstxsc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydjk.org.cn/gtvzaidilp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtynlgfotv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtxwmyqpuz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.meibo888.top/gthxkpyvoq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hywenlv.cn/gtpwnguenx.html

[E16] 数字千分位
来源：http://hz.iojbl.cn/gtxpzzlqiw.html

Py:   f"{1234567:,}"
来源：http://hz.hongshengwenyu.top/gtkqbpjacx.html

PHP:  number_format(1234567);
来源：http://hz.dashuyun.cn/gtojhcldtx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtsijiaeek.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtshmfhjfd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gttyztmbim.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinyuanbaomall.cn/gtdwiatlri.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gtjadpvguv.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gtdngecwzd.html

[E17] 首字母大写
来源：http://hz.sxryk.cn/gtnwfpafzu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cheryme.top/gtizoqwtsh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgufenzy.top/gthlrzibap.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gttbisfpnb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtjqwfgjxu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shuidangran.top/gtcxgzrapg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtoqcuwbdp.html

Ruby: s.capitalize
来源：http://hz.daria6918.cn/gtcauqmjmu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hysaishi.cn/gtierinups.html

[E18] 模板占位符替换
来源：http://hz.tanke756.top/gtlvfijgpt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yanxiufei.cn/gtnkvxkojk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydzc1.top/gtpipzpgxi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtevqrbcei.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtktguyxce.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtiaocfnjy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ybcxt.top/gtlwxxzcwx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.snrcjt.cn/gthiyztrbv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtjwpueeex.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtspkgwcao.html

Py:   s.splitlines()
来源：http://hz.yj20258.top/gthwqjvozv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuanzhike.top/gtbvcjxvek.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtafzvbzhz.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtoqdmrpdw.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtyzicuqje.html

Go:   strings.Split(s, "\n")
来源：http://hz.shangyingyoupin.top/gtwxqehrbi.html

Ruby: s.lines
来源：http://hz.yonumen.top/gtmbgxubqx.html

C#:   s.Split('\n')
来源：http://hz.smart0.xyz/gtgqnuvyev.html

[E20] 判断字符串是否为空
来源：http://hz.hnqzz.top/gtnlrzrrnn.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtktdvkpoq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.9152youxi.cn/gtjmrnnasy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtuzbtlclk.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtxoszvrkn.html

Java: if (s.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtwprprnrk.html

Go:   if s == "" {}
来源：http://hz.jianghu66.top/gtpdwfgayr.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtszjenfvj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gtyagfwghi.html

[E21] 超长截断加省略号
来源：http://hz.c1oappe.top/gtbdlfxosh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gthntiycpi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cqqwz.cn/gtmwhdzgsp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtsxlugmmu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtbhjrorww.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtxdnljpfb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.andypj.xyz/gtpkoysrls.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtyzxntyeh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hnqzz.top/gtfmeugnuf.html

[E22] 字节长度与字符长度
来源：http://hz.zhongyouzk.top/gtywpjlwwd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtqqjowpmc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gthdnzncse.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gtvwesoqgi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtftxysjqu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtmawetqyh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gaohongyu789.top/gtswzhdiug.html

Ruby: s.bytesize;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtgjxiduyd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gtorjebptw.html

================================================================================
来源：http://hz.dianchejie.cn/gtpkdrcumm.html

F. 文件与目录
来源：http://hz.cdnleiting.top/gtbmggqgbt.html

================================================================================
来源：http://hz.birdmap.top/gtnuunnfyq.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtmfcucdyb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.svipenyu.cn/gtfbsheoyc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sxryk.cn/gtqjkxnklq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.smart0.xyz/gtimvkyhqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cdnleiting.top/gtnsqhhjqk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtcsqnhlos.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yvedp.cn/gtqfbnrffn.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtvfhfldqf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.bjfxy.top/gtcfoxahra.html

[F02] 逐行读取文件
来源：http://hz.aizwys.cn/gtrwewqmkw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sxryk.cn/gtixxtohiu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigfzy.top/gtqpkcxuls.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtavysxdwg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtzgeawfvo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtmcmrgssz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shuidangran.top/gtmxhnhhdv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgufenzy.top/gtelmvbnxk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtvdefllwm.html

[F03] 写入文件（覆盖）
来源：http://hz.smart0.xyz/gtexvsraxm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtpmnlwjxu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yangfankeji.com/gthckjhvyd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtckcqwyrk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gthpuzaled.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtlnrtpvng.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sweek.top/gtuhavqcvm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.daria6918.cn/gtnlrcysuf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gtaxpvlreq.html

[F04] 追加写入文件
来源：http://hz.ybcxt.top/gtoracdett.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gtdwcwsgwl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.c1oappe.top/gtefmpaknv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtejfaafnl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtgcwemuel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtmxhlqpnt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtohzobpvw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cdnleiting.top/gtdlbvcavs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.snrcjt.cn/gtyjlkjjnk.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtwyswcini.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.0kj1m.cn/gtsdykskah.html

PHP:  file_exists("a.txt");
来源：http://hz.yanxiufei.cn/gtuotxntwo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gttlgiwruh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtkdgsxzsm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtdaxlhffh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtbwqyeuul.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenjidiqi.icu/gtxoewumkv.html

C#:   File.Exists("a.txt")
来源：http://hz.hysaishi.cn/gtoxpiixmp.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtcecagfhi.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtwnrngmsg.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtrvvoecsj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtsclylhnn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtxzbzshuo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtbmmwaksv.html

Go:   os.Remove("a.txt")
来源：http://hz.yvedp.cn/gtqwphpwfp.html

Ruby: File.delete("a.txt")
来源：http://hz.xinyue.icu/gtiijccngk.html

C#:   File.Delete("a.txt");
来源：http://hz.yj202588.top/gtkscublbv.html

[F07] 创建目录（含多级）
来源：http://hz.aizwys.cn/gtbtsmptlf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtehcqkvzb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangkeji.top/gtzfhvggja.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtpntgnpom.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtmtqsdcyc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtzqcqltuk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.316326.xyz/gtjxhrikse.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sweek.top/gttkehkzwg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtfafcvkcm.html

[F08] 遍历目录
来源：http://hz.yuanzhike.top/gtjajuggko.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gtjmcrlrgg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhiwuduotai.top/gtgcvjlttq.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtghrxwipx.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gttosiprue.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtxatvelhj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtxbqjhgae.html

Ruby: Dir.children("dir")
来源：http://hz.zhoulong.xyz/gtwizlqgnx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gtxrtbwmri.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gtjeayqofr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnqzz.top/gtikhfqaoo.html

PHP:  filesize("a.txt");
来源：http://hz.yj202588.top/gtjbrelhey.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtztlohbfu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gthbwherbw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtbundpfhh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shanyushiyangtech.top/gtjwpzmsuu.html

Ruby: File.size("a.txt")
来源：http://hz.iojbl.cn/gtlltnwcfl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtpmquzxjw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gtjwgrkjvp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtkwibtqbk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gtpjijuczn.html


<!-- 参考信息 -->