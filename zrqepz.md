代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gtppbmuuir.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hammf.cn/gteutggphd.html

[D25] Set 集合去重与交并差
来源：http://hz.guowangkeji.top/gtgdglinxh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnxiangtu.top/gtepgwrwfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.redwolf501.top/gtfqwqdsfv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jqgufenzy.top/gtuymjcmln.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jiagoushi.top/gtgxdtwyfk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hysaishi.cn/gtkrixmihp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ybcxt.top/gtleckezlf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daria6918.cn/gtoapnfsnd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.haohaochexian.top/gtcwhhohep.html

[D26] 数组转字符串
来源：http://hz.shzxlz.cn/gtdzqswwkj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yonumen.top/gtqfgfeyqm.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtkajdfvpl.html

JS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtvqbesvlf.html

TS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtqssqoips.html

Java: String.join(", ", list)
来源：http://hz.cdnleiting.top/gtzhojcsyu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.smart0.xyz/gtcnabmznb.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gthbjzcqoc.html

C#:   string.Join(", ", list)
来源：http://hz.sysykeji.top/gtxiunxanq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqabtosrt.html

E. 字符串处理
来源：http://hz.ydjk.org.cn/gtercycfey.html

================================================================================
来源：http://hz.nwbrower.top/gttnecuwku.html

[E01] 拼接字符串
来源：http://hz.zhiwuduotai.top/gtrahmgwto.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sysykeji.top/gtvsxjoldp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daria6918.cn/gtpkisgybo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuanzx.com/gtpuosafcn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtziqckaoj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.smart0.xyz/gtayolxfff.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hongshengwenyu.top/gtujsykkzs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj202588.top/gtsktkabvy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtgexyyxdj.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gtrwzignlo.html

Py:   "ab" * 3
来源：http://hz.ydzc1.top/gtxdsumeeo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhoulong.xyz/gtfqstmpyd.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gthwtqnuto.html

TS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtxoiokhnq.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtyxcnwrpq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtcaxnzhbf.html

Ruby: "ab" * 3
来源：http://hz.hongshengwenyu.top/gtdyazstca.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtglcqoanv.html

[E03] 截取子串
来源：http://hz.0kj1m.cn/gtoluplvwe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhiwuduotai.top/gtfarbruvs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hammf.cn/gtwshgjcil.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtskodeaej.html

TS:   s.slice(1, 4)
来源：http://hz.vqdsnc.cn/gtwgleqgom.html

Java: s.substring(1, 4)
来源：http://hz.aizwys.cn/gttofvwtfa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jiagoushi.top/gtamcdunix.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cdnleiting.top/gtnlxidspe.html

C#:   s.Substring(1, 3)
来源：http://hz.yangfankeji.com/gtvtcbuhth.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtubxqfphc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.52xcode.cn/gtyjtuqzrv.html

PHP:  strpos($s, "x");
来源：http://hz.tanke756.top/gtcuwazjnj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtqvfflcuu.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtvldxccjc.html

Java: s.indexOf("x")
来源：http://hz.guowangkeji.top/gtwmuyjfft.html

Go:   strings.Index(s, "x")
来源：http://hz.wangshuangyany.cn/gtzzzapyju.html

Ruby: s.index("x")
来源：http://hz.redwolf501.top/gtwpabwgin.html

C#:   s.IndexOf("x")
来源：http://hz.redwolf501.top/gtqmkegdre.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.vqdsnc.cn/gtjmalasgc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.pengpengdd.cyou/gtjtwywqwo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.fzhhl.top/gtrqlnegwo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxuanxn.top/gtrehiyxtr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.meibo888.top/gtyxxlkkdo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj202588.top/gthhvcgler.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gogol.net.cn/gthxjkgila.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ppjwa.cn/gthmqdgdmm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtuygszhlr.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gtpwnkkhgm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sysykeji.top/gtgqdunlyd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtbbjlzthf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtsxspaato.html

TS:   s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gthuwwpmrz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtqsoxxjbb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxuanxn.top/gtwagixmep.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cqqwz.cn/gtlewoswbe.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtlbhseuut.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangkeji.top/gtyakuwhnm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ppjwa.cn/gtrtherxas.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tianlin.xyz/gtnsvkqgpd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jqgufenzy.top/gtmmxyipgc.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtbpogfsjy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tianlin.xyz/gtohmnubjc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhengqikj.top/gtweftcmyg.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtyzsexljd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.smart0.xyz/gtinanwted.html

[E08] 数组按分隔符合并
来源：http://hz.jyoumei.cn/gtjiotsrnv.html

Py:   ",".join(items)
来源：http://hz.yongpay.top/gtssbtkvpg.html

PHP:  implode(",", $items);
来源：http://hz.quarkkingdee.top/gtarkyqfcg.html

JS:   items.join(",")
来源：http://hz.redwolf501.top/gtisqdbeey.html

TS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtjrkeecch.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gthkxllxwc.html

Go:   strings.Join(items, ",")
来源：http://hz.ybcxt.top/gtxpajxpkg.html

Ruby: items.join(",")
来源：http://hz.yvedp.cn/gtcorskhou.html

C#:   string.Join(",", items)
来源：http://hz.chenzaomai.com/gtgeyvzhjs.html

[E09] 去除所有空白字符
来源：http://hz.fengsongda.top/gtggihnkeh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nwbrower.top/gtnakqbnml.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gtljerekya.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtuslclcsr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtqmldaiom.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zdqjudy.top/gtmlqtqukz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aizwys.cn/gthpllzeyh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xinyue.icu/gtjfsohjtx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhoulong.xyz/gtwtssnabk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tianlin.xyz/gtngxcmwnq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtwvrshbyr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gthdieldyl.html

JS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtddimfwjt.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gthjtfynri.html

Java: String.format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtctirpwzz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gthtgtzisn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gtzcybcgch.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtedruavbr.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gtszxemtwa.html

Py:   s[::-1]
来源：http://hz.gzhubu.top/gtjvcizsov.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtdgarvunp.html

JS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtowikrfjg.html

TS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtdrtfwsql.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnqzz.top/gttzwnflfw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhixingplan.top/gthbzwqrfc.html

Ruby: s.reverse
来源：http://hz.zhijiandao.cn/gtzowzsytm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtogbkduby.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gtctxcqfxp.html

Py:   s.count("a")
来源：http://hz.yanxiufei.cn/gtmviqiopx.html

PHP:  substr_count($s, "a");
来源：http://hz.zdqjudy.top/gttkiokugr.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtzejqqeza.html

TS:   s.split("a").length - 1
来源：http://hz.zhijiandao.cn/gtcjfpybun.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtqaswrzdr.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtnxzuipem.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtflzmqtwx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yongpay.top/gtdstijvev.html

[E13] 逐字符遍历
来源：http://hz.shangyingyoupin.top/gtspvlodbt.html

Py:   for ch in s: print(ch)
来源：http://hz.meibo888.top/gtwnnstyhz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.0kj1m.cn/gtoolbltns.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtnampwyok.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtrhwadwnp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pycfn.com/gttbioezvj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuxming.cn/gteeehlhoi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cdnleiting.top/gtvyzceuwb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pycfn.com/gtdqrxfpaq.html

[E14] URL 编码与 Base64
来源：http://hz.dashuyun.cn/gtyefkqndo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sweek.top/gtcwqblztr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtrimtdfkn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gthfzosxvt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hysaishi.cn/gtsnysiihe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenzaomai.com/gtvkdarsgf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sysykeji.top/gtajrkxfxz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fzhhl.top/gtwulbzcey.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sxryk.cn/gtemotjots.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gtlpkfavqj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.havefunace.top/gtjskkhcpx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gaohongyu789.top/gtbvapwkyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.redwolf501.top/gtonnxbbkg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xingfuxueyuan.xyz/gtgebgzhjy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xylfe.cn/gtepuznsnp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yanxiufei.cn/gtatafegxp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj202588.top/gtrypszkfc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtclpkdoin.html

[E16] 数字千分位
来源：http://hz.hnxiangtu.top/gtgppgwrpe.html

Py:   f"{1234567:,}"
来源：http://hz.nwbrower.top/gttblmnbej.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtnvzolqir.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtxigcybst.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtanyrybst.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sufxvd.cn/gtjzxgkwyt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daxiang520.top/gtxsolnern.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhixingplan.top/gtzzjovojk.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtcyqxyodg.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gtuovbkmjc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yongpay.top/gtckjxddgp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhijiandao.cn/gtdlnhguep.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtytigexgy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gthsfbmava.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.svipenyu.cn/gtwxrdtlbe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daria6918.cn/gtcwwzzhoz.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtrdulwoah.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtefbeeyre.html

[E18] 模板占位符替换
来源：http://hz.guowangkeji.top/gtbronopdh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yongpay.top/gtfoyhdnsc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtjamnfcdq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtiwpyjpjq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtbfzuodim.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydzc1.top/gtnkjtumdt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenjidiqi.icu/gtvkahyupa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fengsongda.top/gtxgtztkel.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtfudvttqi.html

[E19] 多行文本按行拆分
来源：http://hz.xinyue.icu/gtiiquvicd.html

Py:   s.splitlines()
来源：http://hz.jqgufenzy.top/gtlrumtxcn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yueranfly.top/gtqskqsltm.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtlyimgynl.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtquikubbz.html

Java: s.lines().toList()
来源：http://hz.gzhubu.top/gtmfqcazzo.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gthcahpsji.html

Ruby: s.lines
来源：http://hz.ehwqpu.com/gtfojyoaqe.html

C#:   s.Split('\n')
来源：http://hz.xylfe.cn/gtxxvrmkdw.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtdyslyxuv.html

Py:   if not s:
来源：http://hz.havefunace.top/gtneboflpk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tianlin.xyz/gtdixkjteo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydjk.org.cn/gtsvnagviq.html

TS:   if (s === "") {}
来源：http://hz.chenjidiqi.icu/gtbatlmoce.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gtsgrdoqro.html

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gtpjtzbiwa.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtcniscasq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtkmxuaicw.html

[E21] 超长截断加省略号
来源：http://hz.ppjwa.cn/gtrdxwprgr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnqzz.top/gtlrclkojb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gzhubu.top/gtadqzzdkv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtyimuwkcm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtbossxqvv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtmuafesse.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtoqwpmqmf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtllzadkhs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.meibo888.top/gtttayhwdz.html

[E22] 字节长度与字符长度
来源：http://hz.jqgufenzy.top/gticlqvkxv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtlslxnnmf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtdtifrwjb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtdqtvigse.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gthruoajwm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.pengpengdd.cyou/gtzdjybzce.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sufxvd.cn/gtpqnaaivi.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangkeji.top/gtetaonikc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhaomingkeji.xyz/gtenododyy.html

================================================================================
来源：http://hz.yuanzhike.top/gtxkmceqex.html

F. 文件与目录
来源：http://hz.aizwys.cn/gtkupnislh.html

================================================================================
来源：http://hz.jiagoushi.top/gtctzcrfqn.html

[F01] 读取整个文件
来源：http://hz.gzhubu.top/gtvjtopqsb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fzhhl.top/gtnlwacqii.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtnjkqvgkq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtypviemeh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hywenlv.cn/gtsnsltuqn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtyvichsig.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.havefunace.top/gtxfqfrvyk.html

Ruby: File.read("a.txt")
来源：http://hz.yueranfly.top/gtxvaoyksg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtaqwrjdix.html

[F02] 逐行读取文件
来源：http://hz.xuetiantiany.cn/gtmrlrlmez.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258888.top/gtquzrsdgz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hywenlv.cn/gtefuwdoho.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtxxvzzvyv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtdxqslvfb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gtcufmsaxe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtxljkiwvc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtzycxaktm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.iojbl.cn/gtbfozfbsn.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtbnskaile.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuxming.cn/gtsrhifvro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtcpdlhscz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtnxptwwaq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtgdeuyvhy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtibjqjshv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj202588.top/gtbhfqmhay.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ybcxt.top/gtqablcqmc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gttcfgecdo.html

[F04] 追加写入文件
来源：http://hz.haohaochexian.top/gtvrgcbbmp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtlwaicsfq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtnujzelqy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnqzz.top/gtkldpmzok.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtvxkkeqrx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuxming.cn/gtrnhxdhmp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cdnleiting.top/gtmazikooq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtlfiipsgd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tianlin.xyz/gtuutgxyzi.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtipcbavce.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtbzdezwzl.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gttpitwnhj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtnkqnzyoy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtbwtqbmko.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtskghwdmc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangdashe.top/gtygzituuu.html

Ruby: File.exist?("a.txt")
来源：http://hz.birdmap.top/gteaqnpokl.html

C#:   File.Exists("a.txt")
来源：http://hz.yj20258888.top/gtwdgvdaoe.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtvxautydj.html

Py:   os.remove("a.txt")
来源：http://hz.snrcjt.cn/gtzjwliwoq.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtnmgegwct.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtewgbrqfr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtemcvodhf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtjaonuhvr.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gtvymiiuyn.html

Ruby: File.delete("a.txt")
来源：http://hz.xylfe.cn/gtnzhcylbr.html

C#:   File.Delete("a.txt");
来源：http://hz.tanke756.top/gtqpeqwnvc.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtrwfnqhnw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtasqaolic.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtnyfjtwph.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtyybrhbpd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtmmqaaqzc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtdkqqophj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtbojulisb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtmgvruurw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xziqi.cn/gtxnoflkgy.html

[F08] 遍历目录
来源：http://hz.daria6918.cn/gtvgzpvjoy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtvktlshag.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shzxlz.cn/gtzonucvqa.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtzpxjawzz.html

TS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtbuytsrhn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtyaywearl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tian-w.cn/gtjkufolil.html

Ruby: Dir.children("dir")
来源：http://hz.jqgufenzy.top/gtvpkndskd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtldssfasy.html

[F09] 获取文件大小
来源：http://hz.andypj.xyz/gtkgbgejaf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yueranfly.top/gtfymgylgs.html

PHP:  filesize("a.txt");
来源：http://hz.sufxvd.cn/gtwihvckqg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtwtqyziou.html


<!-- 参考信息 -->