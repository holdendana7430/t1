代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jyoumei.cn/gtydltkgfa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.9152youxi.cn/gtpzspvhue.html

[D25] Set 集合去重与交并差
来源：http://hz.shzxlz.cn/gtxgvsjsbt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtygeibhll.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jyoumei.cn/gtzqrslbul.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtbygomyfh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtaizrenyy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gttlewidld.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtevxumwcg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhiwuduotai.top/gtqtqsqpvc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hammf.cn/gtwpwrwrhx.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtntdejlwl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.dashuyun.cn/gtneguytiu.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gtpzgnpnkl.html

JS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtpnqnbcyd.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtsnlkfdkc.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtijszeeuq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yongpay.top/gtptwlgnwc.html

Ruby: arr.join(", ")
来源：http://hz.snrcjt.cn/gtesdkyanz.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gtbkvkgvkj.html

================================================================================
来源：http://hz.xziqi.cn/gtfmxmuobu.html

E. 字符串处理
来源：http://hz.nanxinkj.top/gtfolytnhy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlmymfwsg.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gttovcnwpl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xziqi.cn/gtckcltkvb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.havefunace.top/gtpzarhjec.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gturpuvrnr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtnbhscmnz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenzaomai.com/gtcudrvvxz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtisqzqhal.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.birdmap.top/gtdcqkcyov.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtnzwkocfn.html

[E02] 重复字符串
来源：http://hz.sysykeji.top/gtkepdmkfe.html

Py:   "ab" * 3
来源：http://hz.tanke756.top/gtwfsmbskd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yongpay.top/gtqfuxjdeh.html

JS:   "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtomjelexm.html

TS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtdrsacxka.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtevjaljlb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tian-w.cn/gtrouuvbwb.html

Ruby: "ab" * 3
来源：http://hz.sufxvd.cn/gtwbcdqhfi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.haohaochexian.top/gtfplzgthi.html

[E03] 截取子串
来源：http://hz.iojbl.cn/gtoyelmwes.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtpxsfgcpb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hywenlv.cn/gtvjqziucz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtklialteg.html

TS:   s.slice(1, 4)
来源：http://hz.feifeiyinyue.top/gtqvmsnnpj.html

Java: s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtfdxbdfha.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.mhx1999.top/gtgnprzume.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ybcxt.top/gtyigkrlql.html

C#:   s.Substring(1, 3)
来源：http://hz.dashuyun.cn/gtcpaksekn.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gtvszsbchq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtdpcgaprq.html

PHP:  strpos($s, "x");
来源：http://hz.zhaomingkeji.xyz/gtzvyiwspu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tian-w.cn/gtctkasoye.html

TS:   s.indexOf("x")
来源：http://hz.tian-w.cn/gtijjubrjs.html

Java: s.indexOf("x")
来源：http://hz.nwbrower.top/gtvntovyhx.html

Go:   strings.Index(s, "x")
来源：http://hz.xuanzx.com/gtuufvzrze.html

Ruby: s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtaathfece.html

C#:   s.IndexOf("x")
来源：http://hz.cqqwz.cn/gtkpswtbjz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pycfn.com/gtbtzjcszd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhiwuduotai.top/gtsntqogtq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hammf.cn/gtlpwsukel.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtzhrplpcz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jianghu66.top/gtspiohqpn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtnezgluos.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.kuanghao11.cn/gtnjgdbhru.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gotoacloud.top/gtrvvqkehu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nwbrower.top/gttoxgfclm.html

[E06] 替换子串
来源：http://hz.ywan-chungtsiang.top/gtwqgpgppw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgufenzy.top/gtfgievkeq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenlongwang.top/gtzurbmoim.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtphnesafh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtmrikeyhv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gttewdzjlx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenlongwang.top/gtulunogkx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtwvrkdwoo.html

C#:   s.Replace("a", "b")
来源：http://hz.vqdsnc.cn/gthcydealv.html

[E07] 按分隔符拆分
来源：http://hz.gogol.net.cn/gtgdsxwmoe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shuidangran.top/gtfedrswwt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgufenzy.top/gthsbytubz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenzaomai.com/gtsyeckfqo.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtxpbtzier.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.snrcjt.cn/gthqpxkmqf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jqgufenzy.top/gtjuerhgjl.html

Ruby: s.split(",");  s.split
来源：http://hz.hnqzz.top/gtvztvkmpz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.havefunace.top/gtfhatrwhz.html

[E08] 数组按分隔符合并
来源：http://hz.jinqigufen.top/gtezyhcuac.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtwkpkgnnn.html

PHP:  implode(",", $items);
来源：http://hz.shanyushiyangkeji.top/gttvgqczmf.html

JS:   items.join(",")
来源：http://hz.jqgfzy.top/gtdwhvyygt.html

TS:   items.join(",")
来源：http://hz.ppjwa.cn/gtzulisuvo.html

Java: String.join(",", items)
来源：http://hz.zhijiandao.cn/gtgfolzayv.html

Go:   strings.Join(items, ",")
来源：http://hz.gaohongyu789.top/gtgejjstty.html

Ruby: items.join(",")
来源：http://hz.hywenlv.cn/gtteihxoto.html

C#:   string.Join(",", items)
来源：http://hz.cdnleiting.top/gtohpruvto.html

[E09] 去除所有空白字符
来源：http://hz.cashguo.top/gtnrbxsbqp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hysaishi.cn/gtxgsusrmo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nwbrower.top/gtqwjhwxwp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtutoquyid.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtnkfgzpbj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shzxlz.cn/gtdxcexfwe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtlolhnaoz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtdzxbamxg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hammf.cn/gtxtlkzfdo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yvedp.cn/gtksornres.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj202588.top/gtveuvpvwz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ehwqpu.com/gtwnwfmein.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtamfawdfx.html

TS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtwhxorxvt.html

Java: String.format("%03d", 7)
来源：http://hz.meibo888.top/gtqezuymeu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.birdmap.top/gtxzxcpzte.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.andypj.xyz/gtysqkiwjm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.vqdsnc.cn/gtvfezbmfm.html

[E11] 反转字符串
来源：http://hz.quarkkingdee.top/gtjgibwbtd.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gthiovgpmb.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtaxippuaq.html

JS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtvdxfchxw.html

TS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtlbzkcvrr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aibaodan.cn/gtkxxzeztw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gzhubu.top/gtgsthycnq.html

Ruby: s.reverse
来源：http://hz.jqgufenzy.top/gthyebmnjo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtfqoacozw.html

[E12] 统计某字符出现次数
来源：http://hz.chenlongwang.top/gtwudmxivu.html

Py:   s.count("a")
来源：http://hz.sxryk.cn/gtrdjtjgfb.html

PHP:  substr_count($s, "a");
来源：http://hz.daria6918.cn/gtiebjrrxb.html

JS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtzgtqebhn.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtiiwgcnvy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtarqonald.html

Go:   strings.Count(s, "a")
来源：http://hz.wangshuangyany.cn/gtwnwlttly.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtvxculcac.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinghuilouyu.cn/gtcezonxst.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtbrljywtt.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtldykexqs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gogol.net.cn/gtokxtukla.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtaqjhigbq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtwounyufu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jqgfzy.top/gtbiqsxbma.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenlongwang.top/gtgyaishkj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gttnwgirzn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gtpshasuwo.html

[E14] URL 编码与 Base64
来源：http://hz.snrcjt.cn/gtiwdnkian.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gtewkfuvxz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jiagoushi.top/gtltszbyhw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sxryk.cn/gtnlpvxbas.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yangfankeji.com/gtyxpokfur.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtuqyazreb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhixingplan.top/gticiwedgx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gotoacloud.top/gtdhacmtvl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guannengcc.top/gtuyyhfhvl.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtsndjujsx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shuidangran.top/gtdqwouiek.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnqzz.top/gtvkzbzgva.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gogol.net.cn/gtvksvbwyd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtgpznkaye.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fengsongda.top/gtlvqvxowk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gtzkzvxzcl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtpcptukkn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtgddymtit.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gthlpzsxah.html

Py:   f"{1234567:,}"
来源：http://hz.zdqjudy.top/gtelbfsfhr.html

PHP:  number_format(1234567);
来源：http://hz.jqgfzy.top/gthkckpldn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtfcstyokb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtaywhdyij.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtprsrnist.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtqipspevx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinqigfzy.top/gtjmxuurgq.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtcwnhflbz.html

[E17] 首字母大写
来源：http://hz.jqgufenzy.top/gtbueqltlu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtjetnclsy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gtobnfgtjv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gttnijhqcq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtexucrqcr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.iojbl.cn/gtfrpnuzaz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.vqdsnc.cn/gtyaindbbj.html

Ruby: s.capitalize
来源：http://hz.nanxinkj.top/gtbihjtbty.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shzxlz.cn/gtggihbwgs.html

[E18] 模板占位符替换
来源：http://hz.xuetiantiany.cn/gtsglrqvts.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yueranfly.top/gtdophmtjy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sufxvd.cn/gtepyvqqbv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhixingplan.top/gtgbvmlzwy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtornruaom.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.quarkkingdee.top/gtddfxyxwa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtjyzhdldi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jiagoushi.top/gtwswsvrrq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtkftsawmc.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gthqouxeds.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtgsxbaetz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gtbwzkpyjw.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtfdppyxsq.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtllipazum.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gtrxajaaqm.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenjidiqi.icu/gtsmskuyzv.html

Ruby: s.lines
来源：http://hz.xingfuxueyuan.xyz/gthvsomemh.html

C#:   s.Split('\n')
来源：http://hz.jinqigfzy.top/gtoedsdfhd.html

[E20] 判断字符串是否为空
来源：http://hz.zhiwuduotai.top/gtfxikkimm.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtadqopkhq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtyylqluwe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.c1oappe.top/gtgqxxjqqn.html

TS:   if (s === "") {}
来源：http://hz.wangdashe.top/gtedtnumcc.html

Java: if (s.isEmpty()) {}
来源：http://hz.iojbl.cn/gtwezfukwf.html

Go:   if s == "" {}
来源：http://hz.jinqigufen.top/gthrjdqwnn.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtartozhrz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gtbnoijruu.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtcvrtiqit.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gttxbmymdk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daxiang520.top/gtraxkxiga.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtkismgadx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtwmmhdfpq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gthgjytnlw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtleyeildu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yvedp.cn/gtnjhrwbxj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtynqvbzoc.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtocrscsbx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinghuilouyu.cn/gtfitigjot.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtzmhgkaay.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtpkofywmt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtvwqwuhkr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtrxwainui.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtaaogfcgp.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gtdysklhus.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhongyouzk.top/gtpqfvavda.html

================================================================================
来源：http://hz.xinyue.icu/gtqwbiuwgj.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtokqnxjvh.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrktljtdw.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtsknqsvky.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hammf.cn/gtmcgbuvor.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtlzlqelkw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xuanzx.com/gtraeiyyrt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtfllmkpsk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtuetdesjq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtdczfkmvs.html

Ruby: File.read("a.txt")
来源：http://hz.snrcjt.cn/gteisznktd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtnhmrpihf.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtlubxonlr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sufxvd.cn/gttkrfxfbv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tian-w.cn/gttqrgefoa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtmkdpqzcj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtjdxfbwng.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtxgiwnszh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gtvtrsrmec.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jlsjyb.cn/gtdbyhouvh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.52xcode.cn/gtlarnvkvk.html

[F03] 写入文件（覆盖）
来源：http://hz.zhengqikj.top/gtmpfyxshc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.0kj1m.cn/gtpvxlcfxm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.mhx1999.top/gtdkevvmjc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtcnbefabm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtbvktkdfq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangshuangyany.cn/gtsnhdxftm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daxiang520.top/gtrhxhlnrg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinyuanbaomall.cn/gthcdtully.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtuvomauls.html

[F04] 追加写入文件
来源：http://hz.daria6918.cn/gtpkqnysvx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtwhhoqith.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yanxiufei.cn/gtdaamgipx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtmpgewtbo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtcpdrgjmp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.kuanghao11.cn/gtusjffyxt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtkaxqfuit.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gtbqnqzhes.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.redwolf501.top/gtfxkhjrlx.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydjk.org.cn/gtgwbaxzzt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuxming.cn/gtqrfijfea.html

PHP:  file_exists("a.txt");
来源：http://hz.ydzc1.top/gtxdkqvlok.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtlpavrstg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtdfivnfzm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtgzrsskzq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtjbalhgns.html

Ruby: File.exist?("a.txt")
来源：http://hz.jiagoushi.top/gtfkjwsvar.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtbqwzoduv.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtjqvivzus.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtfjkrkvwf.html

PHP:  unlink("a.txt");
来源：http://hz.wangshuangyany.cn/gtrsobvaez.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtuohjxyrp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtuzwlklyl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtiillcemy.html

Go:   os.Remove("a.txt")
来源：http://hz.cashguo.top/gtbgrbhdik.html

Ruby: File.delete("a.txt")
来源：http://hz.yueranfly.top/gticzvtakh.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gtinlvchgp.html

[F07] 创建目录（含多级）
来源：http://hz.ivvv.top/gtxwnarbck.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtvkqjhrwz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtgwnbjoag.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtafqylfem.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtlqiqehwr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.birdmap.top/gtddtlrrss.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gttlenioqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gtphrxregy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.andypj.xyz/gtuflbaasd.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtdzdzduom.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gogol.net.cn/gttqcyhnzi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.9152youxi.cn/gtmqwwzlxt.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtskdzcysy.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtisnwoyoz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtwdvgyvci.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ybcxt.top/gtuzhorupp.html

Ruby: Dir.children("dir")
来源：http://hz.redwolf501.top/gtcqyufujj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtkpzhbzqc.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtyuxrrtqv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.0kj1m.cn/gtgbmmtcwq.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtiyavxqjs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtlihafiaz.html


<!-- 参考信息 -->