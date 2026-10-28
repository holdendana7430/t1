代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gzhubu.top/gtofvlcbzo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yueranfly.top/gtgmgrdylz.html

[D25] Set 集合去重与交并差
来源：http://hz.chenzaomai.com/gtgkdfishv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnxiangtu.top/gtorfxyoeu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ivvv.top/gtcrzuooat.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gtkbaidkef.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuetiantiany.cn/gtrxoxvprg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhengqikj.top/gtpzjjxhla.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yanxiufei.cn/gtktiewkus.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtaryvukad.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gogol.net.cn/gtafesphij.html

[D26] 数组转字符串
来源：http://hz.jlsjyb.cn/gttzcrzplq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.meibo888.top/gtqnjrcxzj.html

PHP:  implode(", ", $arr);
来源：http://hz.jlsjyb.cn/gthnvrojee.html

JS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtlrpikkws.html

TS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtjwjchuad.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtbyqntugn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtjacxqfpb.html

Ruby: arr.join(", ")
来源：http://hz.jqgufenzy.top/gtzpaycnmt.html

C#:   string.Join(", ", list)
来源：http://hz.smart0.xyz/gtytioysqy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtijlplqwv.html

E. 字符串处理
来源：http://hz.yuxming.cn/gtjfwlwckv.html

================================================================================
来源：http://hz.jianghu66.top/gttqnetpjb.html

[E01] 拼接字符串
来源：http://hz.cqqwz.cn/gtlmochxro.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtefurwjyn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zdqjudy.top/gttzjjmbgb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtlkotjfjq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtmudzjttt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gtzznoylae.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.bjfxy.top/gtgwumjzsn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.redwolf501.top/gtbkuxmreh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jiagoushi.top/gtippzpttj.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtwqzpxgst.html

Py:   "ab" * 3
来源：http://hz.pengpengdd.cyou/gtoendkjpd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aibaodan.cn/gtivcirwwp.html

JS:   "ab".repeat(3)
来源：http://hz.yonumen.top/gtylhbtvxn.html

TS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gthxkxeofy.html

Java: "ab".repeat(3)
来源：http://hz.ivvv.top/gtgmbhigmh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daxiang520.top/gtsmhstyzu.html

Ruby: "ab" * 3
来源：http://hz.cqqwz.cn/gtowxfvzrg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gtfyjuwquj.html

[E03] 截取子串
来源：http://hz.cucudq.cn/gtlultuqrl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jyoumei.cn/gtqdgkvkuj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cheryme.top/gtzqbxzevu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtvdufkfjo.html

TS:   s.slice(1, 4)
来源：http://hz.zhijiandao.cn/gtgierxopt.html

Java: s.substring(1, 4)
来源：http://hz.daxiang520.top/gtdjmtikla.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gtadjpzfxp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.birdmap.top/gtxwevrsvo.html

C#:   s.Substring(1, 3)
来源：http://hz.wangdashe.top/gtxsvefmup.html

[E04] 查找子串位置
来源：http://hz.xylfe.cn/gtcdulhylo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtpufzrkzd.html

PHP:  strpos($s, "x");
来源：http://hz.cucudq.cn/gtyetytond.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jyoumei.cn/gttbaombtf.html

TS:   s.indexOf("x")
来源：http://hz.quarkkingdee.top/gtaxqmndqu.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gtksyvtokn.html

Go:   strings.Index(s, "x")
来源：http://hz.ydzc1.top/gtweoadiwp.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gtqqzyodxm.html

C#:   s.IndexOf("x")
来源：http://hz.tian-w.cn/gtptohtibi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xziqi.cn/gtqedsaxkn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtxnithuhh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtmxwzhvzt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtkmubklte.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtxvkvwcgo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtmzfiofjd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.feifeiyinyue.top/gtzfemhyyg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xuanzx.com/gtkgnfcxcd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258888.top/gtqwfamrbj.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtotvxujmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.316326.xyz/gtuyjuqowl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xingfuxueyuan.xyz/gttpwewxtl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gthtylrwpr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtmuufdqwv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtnauxapbz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aibaodan.cn/gtqgcqzdjl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.wangshuangyany.cn/gtczkaimir.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxuanxn.top/gtavhxaiyd.html

[E07] 按分隔符拆分
来源：http://hz.xuetiantiany.cn/gtidioykxr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.svipenyu.cn/gtmsddglee.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.iojbl.cn/gtrppkpvfi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cashguo.top/gtlkybeawk.html

TS:   s.split(",")
来源：http://hz.zhixingplan.top/gtamvdmtli.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtwtihbrlg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gtwwnkonpm.html

Ruby: s.split(",");  s.split
来源：http://hz.mhx1999.top/gtqmzpdeay.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxinkj.top/gtnglbonnl.html

[E08] 数组按分隔符合并
来源：http://hz.wangshuangyany.cn/gtpaepvunr.html

Py:   ",".join(items)
来源：http://hz.daxiang520.top/gtlowbthfn.html

PHP:  implode(",", $items);
来源：http://hz.yonumen.top/gtmutwybeq.html

JS:   items.join(",")
来源：http://hz.gotoacloud.top/gtcgmciqro.html

TS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtfjzzzvaj.html

Java: String.join(",", items)
来源：http://hz.bjfxy.top/gtkirzvtos.html

Go:   strings.Join(items, ",")
来源：http://hz.zycfv.cn/gtgmvtaswo.html

Ruby: items.join(",")
来源：http://hz.xuetiantiany.cn/gtcxvoryge.html

C#:   string.Join(",", items)
来源：http://hz.dashuyun.cn/gtfntrppxq.html

[E09] 去除所有空白字符
来源：http://hz.jinqigufen.top/gtwzlepmte.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.0kj1m.cn/gtsxpuvfpc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jyoumei.cn/gtwclelwmg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtsmafhezf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtejcwrfpp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtglhcjhnk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tianlin.xyz/gtwmrgunsq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cdnleiting.top/gtbyliruic.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yonumen.top/gtzhhewofa.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gteooqohvq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenlongwang.top/gtmrhzlekh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gtwlcfgyfo.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangdashe.top/gttwafrbmm.html

TS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtqeotafqa.html

Java: String.format("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtnrwvummk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tianlin.xyz/gtjryfkyke.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hfpthk.cn/gtyyjqaqnl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinyuanbaomall.cn/gtofdsguoo.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtlcxdyktf.html

Py:   s[::-1]
来源：http://hz.yj20258.top/gtulmfqwqm.html

PHP:  strrev($s);
来源：http://hz.svipenyu.cn/gtvcdzzsqb.html

JS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtqcmkchzq.html

TS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtrczhdxwj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ybcxt.top/gthlylfwco.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtsaebwexs.html

Ruby: s.reverse
来源：http://hz.jqgfzy.top/gtrtxolxxq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtnnpbsvco.html

[E12] 统计某字符出现次数
来源：http://hz.zhiwuduotai.top/gtppsiddhs.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtialpyehz.html

PHP:  substr_count($s, "a");
来源：http://hz.zhixingplan.top/gtqdffzqai.html

JS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtdesrbvnf.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtywrrybdb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.quarkkingdee.top/gtlfqjuuxm.html

Go:   strings.Count(s, "a")
来源：http://hz.tanke756.top/gtxmiseimq.html

Ruby: s.count("a")
来源：http://hz.shzxlz.cn/gtgxlssilc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shzxlz.cn/gtndkjzilc.html

[E13] 逐字符遍历
来源：http://hz.yj20258.top/gtfucfsdpi.html

Py:   for ch in s: print(ch)
来源：http://hz.yongpay.top/gtjqlaakse.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxuanxn.top/gtsjbuxtom.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fzhhl.top/gtzcozstbd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gttsqueurx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guowangkeji.top/gtndfjzexz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenzaomai.com/gtjkcsvzoj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.smart0.xyz/gtqmkytrkj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.316326.xyz/gttmwwsavx.html

[E14] URL 编码与 Base64
来源：http://hz.jyoumei.cn/gtmlwtobcd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hysaishi.cn/gtjkvzkhak.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gttvmfoikv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuetiantiany.cn/gtfhjuwrse.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sufxvd.cn/gthctdhpif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.bjfxy.top/gtfgvvftpj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tanke756.top/gtamtzbpoq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yangfankeji.com/gtegjrmadt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.vqdsnc.cn/gtmtdgslmv.html

[E15] HTML 转义 / 反转义
来源：http://hz.hnxiangtu.top/gtidyavkni.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gtpldghbfj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hongshengwenyu.top/gtvwceaaem.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhiwuduotai.top/gtffhsbbnu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuanzhike.top/gtvousmvmi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuetiantiany.cn/gtaawtwzxq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtgyjxwgdh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.kuanghao11.cn/gtgltzjyzo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtzrieqzzg.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtmozqtmya.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtsnnlzytl.html

PHP:  number_format(1234567);
来源：http://hz.zhongyouzk.top/gtgkyoawoz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gticpmhblr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtqolspifi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydzc1.top/gtelfaeekn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cheryme.top/gtwelntcll.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gtchsvetwl.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258888.top/gtkcnjlxzq.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtahwamudz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtswzvgkim.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ppjwa.cn/gtlbwchyll.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtxrdmqpcu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtowwlzccz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.redwolf501.top/gtcbyilcgy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daria6918.cn/gtxbssqley.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtnlyegaql.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.bjfxy.top/gtmhkezphl.html

[E18] 模板占位符替换
来源：http://hz.sxryk.cn/gtpuqrggqs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hongshengwenyu.top/gtvwfrchan.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jyoumei.cn/gtvxzaqhxn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtfebjbzqo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cashguo.top/gthxfvoymy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sufxvd.cn/gtoyxzxgvx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhijiandao.cn/gtvonavtjk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gtmxndmgiw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuetiantiany.cn/gtgrlmnzeg.html

[E19] 多行文本按行拆分
来源：http://hz.jyoumei.cn/gtzaercxmv.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtywilkltp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydzc1.top/gtosfbnflb.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtqopixvsn.html

TS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtzupimzwz.html

Java: s.lines().toList()
来源：http://hz.yanxiufei.cn/gtyftwzgee.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtxtimrwek.html

Ruby: s.lines
来源：http://hz.wangdashe.top/gtjgixzocx.html

C#:   s.Split('\n')
来源：http://hz.cashguo.top/gtqpwwnfjc.html

[E20] 判断字符串是否为空
来源：http://hz.ydzc1.top/gtopuzpgfw.html

Py:   if not s:
来源：http://hz.hysaishi.cn/gtpxemkrkr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.redwolf501.top/gtxizbpyhi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtnwslzumr.html

TS:   if (s === "") {}
来源：http://hz.quarkkingdee.top/gtaelqezoq.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gtiimhdvws.html

Go:   if s == "" {}
来源：http://hz.jqgufenzy.top/gtljbdejlw.html

Ruby: if s.empty?
来源：http://hz.guannengcc.top/gtnqlnglgf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuetiantiany.cn/gtygrpbqae.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtvonmrgzz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtomjapetg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jianghu66.top/gtkulnzpqf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtawbchohr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtfiwipkll.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtkrptiwgc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yueranfly.top/gtzmvefvyg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.mhx1999.top/gthvsklpfp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtavrpmnrk.html

[E22] 字节长度与字符长度
来源：http://hz.ppjwa.cn/gthiscymzh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtfvvvdptu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gticaarwfk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tian-w.cn/gtvuofjdpe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtbwaxoumd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cheryme.top/gtcyzzmhml.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tanke756.top/gtvyoetjle.html

Ruby: s.bytesize;  s.length
来源：http://hz.c1oappe.top/gtxxqlnkny.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.haohaochexian.top/gtfrdiitsr.html

================================================================================
来源：http://hz.havefunace.top/gtugcqujrt.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtzgwypoki.html

================================================================================
来源：http://hz.yonumen.top/gtgmzzeahc.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtmgddmflk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.birdmap.top/gthbgozjdo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xylfe.cn/gtruhmjduh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtdybkswlg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinghuilouyu.cn/gtfwrbcfpo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtfoupsoqx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenzaomai.com/gtqscxgxlz.html

Ruby: File.read("a.txt")
来源：http://hz.hnxiangtu.top/gtclhntaid.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gotoacloud.top/gtdbmecdve.html

[F02] 逐行读取文件
来源：http://hz.yanxiufei.cn/gtjmdowmbu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gotoacloud.top/gtqglasvoj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aizwys.cn/gtlkgcivod.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtdxeomrnl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtqcxuehux.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtxvrxktfe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tianlin.xyz/gtkspwlmss.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.0kj1m.cn/gtjeubwhxw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtdkrimden.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtokeeqtrk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zycfv.cn/gtcjghjuco.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtsuvzqaax.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtnypzbbft.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtahvjjvbp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fengsongda.top/gtpmrunmwg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.kuanghao11.cn/gtfiuegqwz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.fengsongda.top/gtnwgoouum.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtuhzcntgz.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtajvslzxy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gtdgfupiov.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.birdmap.top/gtncudsten.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtjmgbqsih.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtyytxkvhy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.quarkkingdee.top/gtyquikhln.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtzdwqqoko.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.andypj.xyz/gtbbncpfdt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yanxiufei.cn/gtsqpewxqh.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhoulong.xyz/gteturdyjf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.iojbl.cn/gtszbbadbe.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgfzy.top/gtpyxcaxtq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtfvibmngi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtdthzngak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gttddnesak.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhiwuduotai.top/gtwxiamnud.html

Ruby: File.exist?("a.txt")
来源：http://hz.sufxvd.cn/gtwydwbbun.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtwqzsdqqb.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtwzsapatj.html

Py:   os.remove("a.txt")
来源：http://hz.ydjk.org.cn/gtgyvcqpda.html

PHP:  unlink("a.txt");
来源：http://hz.gaohongyu789.top/gttexfsrih.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gtfnmgrthn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtvkapqcid.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtlszjusmg.html

Go:   os.Remove("a.txt")
来源：http://hz.ydjk.org.cn/gtqssocnwx.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtwclmbrmn.html

C#:   File.Delete("a.txt");
来源：http://hz.bjfxy.top/gtkfvybsbh.html

[F07] 创建目录（含多级）
来源：http://hz.guannengcc.top/gtcjkbwtnb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.0kj1m.cn/gtkkdwzeky.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtdfcliwzf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtmvsvychg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gttgpoolkr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gzhubu.top/gtggxyqwmv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtewqfesul.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gtlyiourpv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aibaodan.cn/gtsmfnchxa.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtngcjkbpc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtijthmiwi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtjocrvnvl.html

JS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtgfpasmbt.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtkqrrqquv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gticcqdwnp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hysaishi.cn/gtsqmccute.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtzcqxykxv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtikqouagm.html

[F09] 获取文件大小
来源：http://hz.yvedp.cn/gtijnlekyv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtecgpobxh.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtqdtiroon.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtyfjegxtw.html


<!-- 参考信息 -->