代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.smart0.xyz/gtxrljwkho.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gzhubu.top/gtggmzgnfu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigufen.top/gtklkvkyxg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtpwfthixl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gtfhgtcpfw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jlsjyb.cn/gtfdnbrweo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.havefunace.top/gtiguygzcw.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtmfxjjsts.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shuidangran.top/gtzvtqagof.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtavbnufet.html

JS:   arr.join(", ")
来源：http://hz.sweek.top/gtkxbfdzme.html

TS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtyowvbvuj.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtxqvhgoec.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtkvbilpmg.html

Ruby: arr.join(", ")
来源：http://hz.meibo888.top/gttgztmgfh.html

C#:   string.Join(", ", list)
来源：http://hz.hfpthk.cn/gtxlaiykyz.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttolqjdxq.html

E. 字符串处理
来源：http://hz.yj202588.top/gteqiqabzj.html

================================================================================
来源：http://hz.yanxiufei.cn/gtfllpqbdi.html

[E01] 拼接字符串
来源：http://hz.cdnleiting.top/gtbgijbvnz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.feifeiyinyue.top/gttbhycwbz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.c1oappe.top/gtnvwehuir.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gteglewyqn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.52xcode.cn/gtvyorbpxc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxuanxn.top/gtczwlwjtq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ivvv.top/gtwaxcnyjl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gtefqgvrhb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hywenlv.cn/gtqhkixvci.html

[E02] 重复字符串
来源：http://hz.vqdsnc.cn/gtyoirfoge.html

Py:   "ab" * 3
来源：http://hz.dianchejie.cn/gtivqfzyzd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jlsjyb.cn/gtspjiaitq.html

JS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtfaztxfeb.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtgvtdabwf.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtizintpsw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hongshengwenyu.top/gtcymktgtc.html

Ruby: "ab" * 3
来源：http://hz.cheryme.top/gtwrhlzvav.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sxryk.cn/gtlxjrmdfb.html

[E03] 截取子串
来源：http://hz.ppjwa.cn/gthksifhcy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jlsjyb.cn/gtjlhcokyl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.andypj.xyz/gtbzlmmwbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuxming.cn/gtutokgvwf.html

TS:   s.slice(1, 4)
来源：http://hz.shangyingyoupin.top/gtlxhliinv.html

Java: s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gtvmprlpbf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ppjwa.cn/gtwlcvoxhf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hfpthk.cn/gtsyprinyz.html

C#:   s.Substring(1, 3)
来源：http://hz.yonumen.top/gtcqnfwgcq.html

[E04] 查找子串位置
来源：http://hz.zdqjudy.top/gtelcazzma.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yanxiufei.cn/gthvfgiqxt.html

PHP:  strpos($s, "x");
来源：http://hz.ydjk.org.cn/gtgspypecp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gaohongyu789.top/gtmllrejan.html

TS:   s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtsczuupha.html

Java: s.indexOf("x")
来源：http://hz.chenzaomai.com/gtyqihiymx.html

Go:   strings.Index(s, "x")
来源：http://hz.chenjidiqi.icu/gthqgrtyaw.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtgsaxixhh.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtoqiildom.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.0kj1m.cn/gtykbytewi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hammf.cn/gtvslhsbyc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhijiandao.cn/gtmmbkwitt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtglahutby.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenjidiqi.icu/gtuhsawszv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ehwqpu.com/gtoamatjik.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nwbrower.top/gtjzbieznx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangshuangyany.cn/gtdoqteecl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fengsongda.top/gtxlhncfdw.html

[E06] 替换子串
来源：http://hz.dashuyun.cn/gtcqjebuua.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtmizlccar.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinyuanbaomall.cn/gtfpttukxy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtmkuyxcct.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtaoqrsawy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtvboqcoos.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aizwys.cn/gtejlkuonl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.c1oappe.top/gtpsfekwlq.html

C#:   s.Replace("a", "b")
来源：http://hz.zdqjudy.top/gtgrsrdpnd.html

[E07] 按分隔符拆分
来源：http://hz.0kj1m.cn/gtaohfrsfp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fzhhl.top/gtsopmpztf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shangyingyoupin.top/gtljgbfrjt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yvedp.cn/gtkmayblam.html

TS:   s.split(",")
来源：http://hz.daria6918.cn/gtnagovdvd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtotvfhxie.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yonumen.top/gtdjjaarxp.html

Ruby: s.split(",");  s.split
来源：http://hz.xziqi.cn/gtvsiusrqa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ybcxt.top/gtuxcsrnoj.html

[E08] 数组按分隔符合并
来源：http://hz.sxryk.cn/gtttfntcfx.html

Py:   ",".join(items)
来源：http://hz.nwbrower.top/gtfaxljlup.html

PHP:  implode(",", $items);
来源：http://hz.yongpay.top/gteppygmha.html

JS:   items.join(",")
来源：http://hz.xinyue.icu/gtldxhyrsl.html

TS:   items.join(",")
来源：http://hz.nanxinkj.top/gtredlacal.html

Java: String.join(",", items)
来源：http://hz.shuidangran.top/gtlkueghql.html

Go:   strings.Join(items, ",")
来源：http://hz.hongshengwenyu.top/gthoxdzzlo.html

Ruby: items.join(",")
来源：http://hz.chenzaomai.com/gtqwjhuuan.html

C#:   string.Join(",", items)
来源：http://hz.jlsjyb.cn/gtjdbutmcm.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtzpwitcob.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtjnikregn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aizwys.cn/gtcsnpnicf.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtqnbigmzx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gttjicbabj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtlejipoas.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gzhubu.top/gttqwigxhd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yvedp.cn/gtwlamzeuy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuetiantiany.cn/gtrmjphjmk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yongpay.top/gtrcqstbsg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtsnmalaxz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xziqi.cn/gtnwrfskpw.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtlqncbiax.html

TS:   "7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtfongqddp.html

Java: String.format("%03d", 7)
来源：http://hz.dianchejie.cn/gtubjudoim.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jlsjyb.cn/gtomwdlohs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtyzfqfmbh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.52xcode.cn/gtkdfjkelo.html

[E11] 反转字符串
来源：http://hz.aibaodan.cn/gtpkdzndwb.html

Py:   s[::-1]
来源：http://hz.jlsjyb.cn/gtxouemyrz.html

PHP:  strrev($s);
来源：http://hz.yanxiufei.cn/gtgpakippt.html

JS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtafvuutjn.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtryogjsnh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xingfuxueyuan.xyz/gtgekwpukp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtetrsvuwm.html

Ruby: s.reverse
来源：http://hz.sxryk.cn/gtvdpabqwq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtlawcwltw.html

[E12] 统计某字符出现次数
来源：http://hz.yuxming.cn/gtoiuhhapi.html

Py:   s.count("a")
来源：http://hz.jqgfzy.top/gtiboavssa.html

PHP:  substr_count($s, "a");
来源：http://hz.xingfuxueyuan.xyz/gtfoqljqwi.html

JS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gthmqjifnm.html

TS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtuhlsrtng.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtucpjoylu.html

Go:   strings.Count(s, "a")
来源：http://hz.cdnleiting.top/gtpzkezofs.html

Ruby: s.count("a")
来源：http://hz.jqgufenzy.top/gtwyvimoiq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aibaodan.cn/gtfwysysad.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtnsdownow.html

Py:   for ch in s: print(ch)
来源：http://hz.zhijiandao.cn/gtbywxmnlm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangkeji.top/gtllvbxzaw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtbekbizyw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtmuoqonks.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangdashe.top/gtkdolcffe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.iojbl.cn/gtavqhpgjg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.redwolf501.top/gtqafmumpo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jlsjyb.cn/gtyosgrvsl.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtywqsaxou.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgfzy.top/gtxfdycdgr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gtimxzbrlc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dashuyun.cn/gtsubkfglc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zycfv.cn/gtytkhpepu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pengpengdd.cyou/gtgeeagieq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yonumen.top/gtqnjuubki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fzhhl.top/gtcugjmkbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ppjwa.cn/gtgokseysz.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gtxlsaqpnl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daxiang520.top/gtpxadwylx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jyoumei.cn/gtkginsxfi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtqxqxpfle.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangtech.top/gtexxymdmo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.redwolf501.top/gttlwxqepk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.vqdsnc.cn/gtqqhjgbam.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gtmvgxqwmx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zycfv.cn/gtlvemtxjn.html

[E16] 数字千分位
来源：http://hz.yonumen.top/gtnvpmpufy.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtrizyfgxd.html

PHP:  number_format(1234567);
来源：http://hz.yangfankeji.com/gtpmqxpsoi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guannengcc.top/gtzgtnnuul.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtrjfmfatf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gtbiostkib.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shzxlz.cn/gtjroqfzfl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinyuanbaomall.cn/gtpcaafkfo.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtkbkbsgvk.html

[E17] 首字母大写
来源：http://hz.svipenyu.cn/gtxoobiter.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.andypj.xyz/gtaoumoggr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtjfswqwoz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtpohunxlm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtotrcjzpc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gtxluhxxoe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cheryme.top/gtuhmgkudj.html

Ruby: s.capitalize
来源：http://hz.cucudq.cn/gtfnddjsaz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ivvv.top/gtsmgtqhlo.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gtwiowmbpp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jlsjyb.cn/gtvzxaqhcr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj202588.top/gthqeozeis.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtuqmuvhmd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtjyuixcri.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.pengpengdd.cyou/gtytixnzbg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sweek.top/gtpatuthbz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgufenzy.top/gtqkdnnxlp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dianchejie.cn/gtmrdageuq.html

[E19] 多行文本按行拆分
来源：http://hz.gaohongyu789.top/gtrgslhdny.html

Py:   s.splitlines()
来源：http://hz.nwbrower.top/gtepiojjeh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtwvwmjtaw.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gttrdierda.html

TS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtegdtxvgz.html

Java: s.lines().toList()
来源：http://hz.sweek.top/gtabdybohh.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gthwykivhl.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtyhbbxiyp.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtlvxkrvkv.html

[E20] 判断字符串是否为空
来源：http://hz.chenzaomai.com/gtjpplguxz.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtyvybhsdj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zycfv.cn/gtomffqnvw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtjsxfynjh.html

TS:   if (s === "") {}
来源：http://hz.yj202588.top/gtchfjsghi.html

Java: if (s.isEmpty()) {}
来源：http://hz.xziqi.cn/gtduyfexlx.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtspjpqddv.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangkeji.top/gtinwpbfhk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtdxhmidzt.html

[E21] 超长截断加省略号
来源：http://hz.xziqi.cn/gtpvmjedoy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gthueaptzn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hfpthk.cn/gtiogwqpxl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtawmnnxlt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gteayyskwg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtkrsviqnb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtsvxvoipp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jyoumei.cn/gtionzkxor.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.316326.xyz/gtccbkyojv.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtguyhzdsj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shuidangran.top/gtnyrphbww.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtaowwmzey.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtpnkgmcqk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtjxnsjzbe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hammf.cn/gtpcmwznvo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ehwqpu.com/gtdjkqcpxm.html

Ruby: s.bytesize;  s.length
来源：http://hz.jlsjyb.cn/gtvwjyjddy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guannengcc.top/gtyxrzwmfj.html

================================================================================
来源：http://hz.9152youxi.cn/gtamaaepzi.html

F. 文件与目录
来源：http://hz.shangyingyoupin.top/gtbexbegrf.html

================================================================================
来源：http://hz.yj202588.top/gtgydebhdo.html

[F01] 读取整个文件
来源：http://hz.hfpthk.cn/gtyromtgrd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fengsongda.top/gthmmhjfte.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gaohongyu789.top/gtbmfvyrfn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xingfuxueyuan.xyz/gtjoygdzah.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtrnasmoup.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtvqavjlih.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtcesdpdxo.html

Ruby: File.read("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtplcdrmdg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nwbrower.top/gtzftjsncu.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gtyskgpqgv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.316326.xyz/gtkapqbsee.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xylfe.cn/gtrvpylhjc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtmofeuewk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gtpwdlrval.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtjtkvxbji.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.svipenyu.cn/gtllxrmoep.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jyoumei.cn/gtnohnsxyq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtozteqsgo.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtkxvzzfhu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.meibo888.top/gtklkvmhqb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtopxmeddg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtmuacuzao.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gttgtxtmnb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenjidiqi.icu/gtelahzmhh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.andypj.xyz/gtoscctayo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtuogkbmrm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gthxzwfelg.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gthemctclr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtejonxjnm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.meibo888.top/gtiogarqoj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtkpxmtgxp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtgvitlvmq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxuanxn.top/gtbxpmhtez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.meibo888.top/gtlelyhcna.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtxeanygcd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtwtrudlhx.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtdukydaym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtwhnysark.html

PHP:  file_exists("a.txt");
来源：http://hz.xuetiantiany.cn/gtlbsbeqnu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtcoiunmzb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtjxlqotde.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtwfhtbrec.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtbrtiyyvx.html

Ruby: File.exist?("a.txt")
来源：http://hz.zdqjudy.top/gtwpakkxbq.html

C#:   File.Exists("a.txt")
来源：http://hz.hnxiangtu.top/gteojfczpr.html

[F06] 删除文件
来源：http://hz.chenzaomai.com/gtpiqayjcr.html

Py:   os.remove("a.txt")
来源：http://hz.zhongyouzk.top/gtjuuhevyi.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gtevqzyxbc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtuydlzfuh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gttaqtkswd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtyvqlistw.html

Go:   os.Remove("a.txt")
来源：http://hz.hywenlv.cn/gtbljppspu.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtpjnctjkh.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gttrjnfyfy.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtvvmwjrmc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zdqjudy.top/gtgyxmczax.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtcfjevdxe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gteafjhxtp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtpqivfdhc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhaomingkeji.xyz/gtcztxgovm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xingfuxueyuan.xyz/gttfovzjai.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigfzy.top/gtoizosbsh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangshuangyany.cn/gtsydjhprb.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtczmibmxo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zycfv.cn/gtagngexsj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.0kj1m.cn/gttkewnpnf.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtgaotlclp.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtrgtddvaa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtmzooxdpl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hysaishi.cn/gtrcfntghm.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtohjsmbrq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.smart0.xyz/gtknkbrmeb.html

[F09] 获取文件大小
来源：http://hz.jinqigufen.top/gtnphirudb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtpwyqsmdl.html

PHP:  filesize("a.txt");
来源：http://hz.guowangkeji.top/gtmdptojhz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtionfwmuy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gtyimwdkwg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtzhjcykos.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangdashe.top/gtdanbevpo.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gtmaknwiai.html


<!-- 参考信息 -->