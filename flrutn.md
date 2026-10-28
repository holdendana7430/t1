代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenlongwang.top/gtdqtopopr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ybcxt.top/gtwuwehstl.html

[D25] Set 集合去重与交并差
来源：http://hz.aizwys.cn/gtuzsqyicq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yanxiufei.cn/gtdxagugjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.andypj.xyz/gtjeneheld.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gtelniqgng.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cheryme.top/gtqmkeopsx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sweek.top/gtrkgjxcjs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtoykvsqhb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnqzz.top/gttwrbeous.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daxiang520.top/gthngaqpkw.html

[D26] 数组转字符串
来源：http://hz.jinghuilouyu.cn/gtxvkxinax.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cqqwz.cn/gtligmkoqo.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangtech.top/gtgeeimvwo.html

JS:   arr.join(", ")
来源：http://hz.yj20258.top/gtwznotgll.html

TS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtkevanfcn.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtzkcfvfbm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtcwjbcwsv.html

Ruby: arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtdtqglovi.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtwgmosxns.html

================================================================================
来源：http://hz.havefunace.top/gtkifudfbm.html

E. 字符串处理
来源：http://hz.pycfn.com/gtjmjimjvv.html

================================================================================
来源：http://hz.yuxming.cn/gtikjkczjf.html

[E01] 拼接字符串
来源：http://hz.ehwqpu.com/gtwpnyrtoy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhaomingkeji.xyz/gtmyxltjap.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtggvaphjz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtifwohbpv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtnmpnktzl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pengpengdd.cyou/gtpqudzuij.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtamilpauk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgufenzy.top/gtkukazrqa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gtnsncsjbh.html

[E02] 重复字符串
来源：http://hz.zhengqikj.top/gtyiwbbrus.html

Py:   "ab" * 3
来源：http://hz.meibo888.top/gtdolwwahg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fzhhl.top/gtmmdbrjog.html

JS:   "ab".repeat(3)
来源：http://hz.guannengcc.top/gtnmsimbhq.html

TS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtpcxmhqfw.html

Java: "ab".repeat(3)
来源：http://hz.zycfv.cn/gtxgijayrj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtfengpdzc.html

Ruby: "ab" * 3
来源：http://hz.yj202588.top/gtwrnmixkn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.mhx1999.top/gtqsysmtci.html

[E03] 截取子串
来源：http://hz.316326.xyz/gttjzbfxjn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtnncrhqek.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtdxxbvtpc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xziqi.cn/gtpcwxkbsn.html

TS:   s.slice(1, 4)
来源：http://hz.yongpay.top/gteajikjca.html

Java: s.substring(1, 4)
来源：http://hz.ybcxt.top/gtxqqntzkn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aibaodan.cn/gtpnmjudte.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuanzhike.top/gtihiwvmxn.html

C#:   s.Substring(1, 3)
来源：http://hz.cucudq.cn/gtezgkhjnz.html

[E04] 查找子串位置
来源：http://hz.xinyue.icu/gttxudjtmc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dianchejie.cn/gtinjcrfco.html

PHP:  strpos($s, "x");
来源：http://hz.zhixingplan.top/gthbsrgtzv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtdwfohpos.html

TS:   s.indexOf("x")
来源：http://hz.zhixingplan.top/gtmwywqcuh.html

Java: s.indexOf("x")
来源：http://hz.cucudq.cn/gtqnngtmyy.html

Go:   strings.Index(s, "x")
来源：http://hz.cdnleiting.top/gttkwgsyld.html

Ruby: s.index("x")
来源：http://hz.sweek.top/gtnztyglot.html

C#:   s.IndexOf("x")
来源：http://hz.zhijiandao.cn/gtmvcisgnt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinyuanbaomall.cn/gthwefycbw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuanzx.com/gteotluyfy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.fzhhl.top/gtjafdprxt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gthbgxksce.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dashuyun.cn/gttmhpdcxb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtithtwckg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sweek.top/gtqyzmmqip.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtyfftmgqz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hongshengwenyu.top/gtmqmqpjev.html

[E06] 替换子串
来源：http://hz.hammf.cn/gtaoaywfid.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yvedp.cn/gtrthhwlwk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jianghu66.top/gtscevcmgk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtlccgtcpw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtcoysgcoz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtgekzlcax.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.haohaochexian.top/gtwzzeyokg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aibaodan.cn/gtbrhxiiwg.html

C#:   s.Replace("a", "b")
来源：http://hz.yuxming.cn/gtyqqevigg.html

[E07] 按分隔符拆分
来源：http://hz.316326.xyz/gtjvayssop.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yueranfly.top/gtzsqamtsi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gtkdlgwmag.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ywan-chungtsiang.top/gtgnxqscxh.html

TS:   s.split(",")
来源：http://hz.xinyue.icu/gtqqtfxaki.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhengqikj.top/gtizpesjrs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gttcrjacua.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtykxuchbf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuanzhike.top/gtptnjayld.html

[E08] 数组按分隔符合并
来源：http://hz.shzxlz.cn/gtsbnrvrlz.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gtsgyqeoay.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gtnehxsgyl.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtmctvqpie.html

TS:   items.join(",")
来源：http://hz.chenlongwang.top/gtirbuoopw.html

Java: String.join(",", items)
来源：http://hz.gogol.net.cn/gtxkxcgbjo.html

Go:   strings.Join(items, ",")
来源：http://hz.fengsongda.top/gtjzffynzi.html

Ruby: items.join(",")
来源：http://hz.wangdashe.top/gtsodpteyh.html

C#:   string.Join(",", items)
来源：http://hz.snrcjt.cn/gtiybboxja.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtjabvfmyh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gogol.net.cn/gtzgynirbi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gttwbojovv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtedfolgqn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtzrzsgvii.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sysykeji.top/gtwedcwbvc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aibaodan.cn/gtntcsfpan.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenjidiqi.icu/gtwbgcoozw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258888.top/gtjugyqpuj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yvedp.cn/gtxojpghpd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.mhx1999.top/gtuwqfvqcy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sweek.top/gtnxodytwb.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtpteplcnh.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtcrwdbuvo.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtrmsmtntf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xziqi.cn/gttgcdqvjl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gtafmaqyou.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangtech.top/gtgfpzbupd.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtdobtijck.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtrzqctszq.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtzctgxupn.html

JS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtirozmogv.html

TS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtgfpdotzt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gotoacloud.top/gtfhfgomzf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aizwys.cn/gtlxcshpxw.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtsubppape.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtsmhygawb.html

[E12] 统计某字符出现次数
来源：http://hz.vqdsnc.cn/gtmsbsluiu.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gtwxunudqf.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gtwnxfrkyl.html

JS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gtfcqchluu.html

TS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtatkqlzqp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jianghu66.top/gtdkntiypn.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtivuvdsez.html

Ruby: s.count("a")
来源：http://hz.yuanzhike.top/gtbhovzpgn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gteeufufco.html

[E13] 逐字符遍历
来源：http://hz.nwbrower.top/gtchwypdym.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gtoygnxrdo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gttshncnmx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtvsdnwpcr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtjepyruue.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtbmktqxjk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtfmhisbop.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtdcpvwmjm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtvusjzwcw.html

[E14] URL 编码与 Base64
来源：http://hz.gogol.net.cn/gtmcbesvxm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.vqdsnc.cn/gtpurnmrwq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aibaodan.cn/gthyovfcqc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.316326.xyz/gtiqhtiaho.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zdqjudy.top/gtckgygzej.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258888.top/gtxcmmbjla.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aibaodan.cn/gtgeqoynpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtvxgzxuir.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhiwuduotai.top/gtkomrrvzr.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenzaomai.com/gtjawzgzuw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtwdgzftqt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shangyingyoupin.top/gtwjxynxlo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.vqdsnc.cn/gtlelfpipd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258.top/gtrbihipgy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtzbmkkfln.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.smart0.xyz/gtuzwrojps.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ivvv.top/gtonkwvxwl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.quarkkingdee.top/gtweqmmbtc.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtvnqsgujx.html

Py:   f"{1234567:,}"
来源：http://hz.hnxiangtu.top/gtqhgixtjk.html

PHP:  number_format(1234567);
来源：http://hz.xuanzx.com/gtrothxsuh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtyotilaji.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuxming.cn/gtixfjtqgy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aibaodan.cn/gtbmlonklq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhengqikj.top/gtjehfrenf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gotoacloud.top/gtonvjrcff.html

C#:   1234567.ToString("N0")
来源：http://hz.hnxiangtu.top/gtfctcdulz.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtoswolody.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtwsmxqopq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.c1oappe.top/gtfklnrjxt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtjfygakpi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhixingplan.top/gtuakoydih.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtcogxrrsx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sxryk.cn/gttpompeug.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtlfhpsmfo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.havefunace.top/gtijlmiore.html

[E18] 模板占位符替换
来源：http://hz.redwolf501.top/gtkcgnkpfj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtmdbxxmzn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gtiyefvhtt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenlongwang.top/gtifmuxlqb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtduynwcku.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ehwqpu.com/gtikqynhju.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuetiantiany.cn/gtxzcfrskx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtjhpelxmz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.andypj.xyz/gtfqfncwrz.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtqttchsmv.html

Py:   s.splitlines()
来源：http://hz.ywan-chungtsiang.top/gtcdngiecj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gtjajtfvds.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtomxgqpcu.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gthgidybum.html

Java: s.lines().toList()
来源：http://hz.316326.xyz/gtpkkqaijw.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangshuangyany.cn/gtlhnzcveo.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtoabjuapv.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtwvfzsjez.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtoxscyhzo.html

Py:   if not s:
来源：http://hz.hammf.cn/gtzfvqfmju.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.andypj.xyz/gtdmbdpfnk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aizwys.cn/gtzerggsuk.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtvtlzbmpw.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gthypbxqxx.html

Go:   if s == "" {}
来源：http://hz.jinqigufen.top/gtwthyharh.html

Ruby: if s.empty?
来源：http://hz.kuanghao11.cn/gtjeaqcnag.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sufxvd.cn/gtfqujivmq.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtctatzchu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dianchejie.cn/gtemspmmll.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.haohaochexian.top/gtwclxyild.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtuaavgijk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtsvvwiwam.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtanyikkoy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gtjoyaitlf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtyolmapur.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtsdbkkyfu.html

[E22] 字节长度与字符长度
来源：http://hz.jinyuanbaomall.cn/gtroskddwy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hfpthk.cn/gtjnsttuvv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtzecmdajy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtaivbprym.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zdqjudy.top/gtiotvoxkt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sweek.top/gtqgqbbafx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhaomingkeji.xyz/gtmquzbfoo.html

Ruby: s.bytesize;  s.length
来源：http://hz.shuidangran.top/gtwektqtxg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yongpay.top/gtapbvioox.html

================================================================================
来源：http://hz.tanke756.top/gtnuehcmrf.html

F. 文件与目录
来源：http://hz.birdmap.top/gtebvjqmzq.html

================================================================================
来源：http://hz.birdmap.top/gtwkdphxxk.html

[F01] 读取整个文件
来源：http://hz.yueranfly.top/gtgdpxzcbb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenzaomai.com/gtykacclzh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuxming.cn/gtdwzxdvdz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydjk.org.cn/gtkuputtiq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtdjkbmksw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtionnzxlt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenjidiqi.icu/gtqxaxnpvr.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gtiutbwggu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gtsupeppfe.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtojvxpqru.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.316326.xyz/gtwaaabfyi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.smart0.xyz/gtvwqsvbgz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtcdrxvnww.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shzxlz.cn/gttdkmudsq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtxugqukrs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jyoumei.cn/gtjooxcdvs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ybcxt.top/gtyhbdxvta.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtfphbpzts.html

[F03] 写入文件（覆盖）
来源：http://hz.nwbrower.top/gtuiwdhwmj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtypkabtng.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtkcgrgkjb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtgvygvscb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtspscjuvb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gaohongyu789.top/gtlntaynqf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtyakrylbh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtkahhbcdq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cheryme.top/gtfzblunfm.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gtucfmhvxj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtldjzwjso.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tian-w.cn/gtdujvkfin.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnqzz.top/gtelldzkox.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtxbbveash.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shuidangran.top/gtmosiuzdx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aizwys.cn/gtitxdtioz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gttyeisjxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.smart0.xyz/gtvcpgmrnw.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhaomingkeji.xyz/gtcujnvcip.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gtielfyqda.html

PHP:  file_exists("a.txt");
来源：http://hz.yongpay.top/gtxeniuueh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtgzapvayc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtyqqfznfk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtzwpyevmw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pycfn.com/gtwstctynm.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhongyouzk.top/gtnbxtwdqr.html

C#:   File.Exists("a.txt")
来源：http://hz.hnxiangtu.top/gtwmmnfrzm.html

[F06] 删除文件
来源：http://hz.yuxming.cn/gtjwdrafrp.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtevgivqva.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtyhblripa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtlbyzcxrw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.redwolf501.top/gttesimabc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtyaooemig.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtgzxvhxbu.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtlasibpoy.html

C#:   File.Delete("a.txt");
来源：http://hz.nwbrower.top/gtjzdtkhxn.html

[F07] 创建目录（含多级）
来源：http://hz.52xcode.cn/gtkjtbthkj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xziqi.cn/gtsxdzwvwj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydjk.org.cn/gtycsavllg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtpfczwmbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtugkqqnul.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.meibo888.top/gtnbowgmhz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj202588.top/gtaonlokfu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gticsbolbz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.c1oappe.top/gtozemptln.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtwlrfusqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtttsfvniv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.aizwys.cn/gtfsynigox.html

JS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gttntvcfza.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtzmvbiwqy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtqaxvzfla.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.iojbl.cn/gtrynurlhw.html

Ruby: Dir.children("dir")
来源：http://hz.xinyue.icu/gtxifeyxgn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuanzx.com/gtjjimyfvx.html

[F09] 获取文件大小
来源：http://hz.jinqigfzy.top/gtubxvasoh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yonumen.top/gtbgkmvjtj.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtfhgpkkxu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtupeprdip.html


<!-- 参考信息 -->