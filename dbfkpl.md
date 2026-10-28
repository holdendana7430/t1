代发 wailian999

================================================================================
来源：http://hz.chenjidiqi.icu/gtjmlvioci.html

E. 字符串处理
来源：http://hz.hywenlv.cn/gttmfgybtq.html

================================================================================
来源：http://hz.haohaochexian.top/gtwsdijxba.html

[E01] 拼接字符串
来源：http://hz.mhx1999.top/gtaootmbxe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxinkj.top/gtyivnqukr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.0kj1m.cn/gtiiymteen.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtcncgvmsv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtisxvggcw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gtdnuetbtz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtifjvltqm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zycfv.cn/gtrsiznyqc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtclyewbuk.html

[E02] 重复字符串
来源：http://hz.chenjidiqi.icu/gtfnvjwgon.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gtbvdhuneu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhoulong.xyz/gttldffitr.html

JS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtrdlstcpq.html

TS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gtkmwtkegk.html

Java: "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtdjzaqflb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.c1oappe.top/gtyqwfeipp.html

Ruby: "ab" * 3
来源：http://hz.snrcjt.cn/gtkuxfadug.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.0kj1m.cn/gtzcozlvac.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gthwnzbhli.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yonumen.top/gtnznqucmg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangdashe.top/gtqowargha.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ppjwa.cn/gtodukntep.html

TS:   s.slice(1, 4)
来源：http://hz.andypj.xyz/gtjimtdgbb.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtbrckknuy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.kuanghao11.cn/gtgqdblvex.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gtoizpnlav.html

C#:   s.Substring(1, 3)
来源：http://hz.cqqwz.cn/gtpqmzgmvk.html

[E04] 查找子串位置
来源：http://hz.jinqigufen.top/gtbhrsnrfh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hysaishi.cn/gtsqjtcnsx.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gtffrzeyjw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ivvv.top/gtqirhfepq.html

TS:   s.indexOf("x")
来源：http://hz.cheryme.top/gtwvwrsdjo.html

Java: s.indexOf("x")
来源：http://hz.jqgfzy.top/gtsdsebpjn.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigufen.top/gtvjeilfxv.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gtnfiwpkkc.html

C#:   s.IndexOf("x")
来源：http://hz.jqgufenzy.top/gtclnvqtwx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nwbrower.top/gtuzzxsdow.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtoxgtlpae.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.c1oappe.top/gtbvycqzcq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtksotcdnh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhengqikj.top/gteewohbrb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtzokrsfqy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gthipfdjxf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dashuyun.cn/gtlnrslexf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tianlin.xyz/gtulbvpjqc.html

[E06] 替换子串
来源：http://hz.shzxlz.cn/gtleiccieg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gtpbyuqpgt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gtwahfktjx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtmkeiidtt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtgoozofmu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtuklydtwo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zdqjudy.top/gtycigzfnw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dianchejie.cn/gtlrepbnuh.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtddmkilsm.html

[E07] 按分隔符拆分
来源：http://hz.c1oappe.top/gtvvskofmj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangkeji.top/gtwqrogsgk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jianghu66.top/gtsihcxgqr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aizwys.cn/gtowiabqde.html

TS:   s.split(",")
来源：http://hz.ppjwa.cn/gtcsgyongz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtfrvtmdpl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.c1oappe.top/gtsccfgxjy.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtnjuvvitn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtzrfyfdbz.html

[E08] 数组按分隔符合并
来源：http://hz.zhongyouzk.top/gtjjmkdfuq.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtyvqjojnv.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtxslpoxbb.html

JS:   items.join(",")
来源：http://hz.zycfv.cn/gtspknkndy.html

TS:   items.join(",")
来源：http://hz.0kj1m.cn/gtdvqjecst.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gtlhtweigq.html

Go:   strings.Join(items, ",")
来源：http://hz.vqdsnc.cn/gtwiavnrwe.html

Ruby: items.join(",")
来源：http://hz.ivvv.top/gtpipzfkpl.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtnpocywiq.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gthulwpkaw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xylfe.cn/gtvdfwiocs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xuetiantiany.cn/gtfauaesac.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtssjkvyvk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtwryqtijs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.quarkkingdee.top/gtsvupikcw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xinyue.icu/gtdjzntgjl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daxiang520.top/gtlmyuzpta.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenlongwang.top/gtxhkonglx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.birdmap.top/gtvbvgtmou.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjfxy.top/gtgvkqisqs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ppjwa.cn/gttxwzovhh.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtiswvpfsm.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtylzrpkbl.html

Java: String.format("%03d", 7)
来源：http://hz.wangdashe.top/gtbndcvlgd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtawuadgsg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yueranfly.top/gtyouqcjqz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zdqjudy.top/gtfrkwkdvq.html

[E11] 反转字符串
来源：http://hz.ybcxt.top/gtxqedfwsd.html

Py:   s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtidpfqfbv.html

PHP:  strrev($s);
来源：http://hz.chenlongwang.top/gttsafddey.html

JS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtqjmfaxto.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtdtjpkduw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ywan-chungtsiang.top/gtmgrubbcv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtytfbpkzr.html

Ruby: s.reverse
来源：http://hz.ydjk.org.cn/gtvkqlkogz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtygxwbgob.html

[E12] 统计某字符出现次数
来源：http://hz.aizwys.cn/gtfxgimpkc.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtbvqttbqq.html

PHP:  substr_count($s, "a");
来源：http://hz.fengsongda.top/gtsrggwojp.html

JS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtgugwpzqz.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtvdsdnqwm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtnwnqgtgr.html

Go:   strings.Count(s, "a")
来源：http://hz.sufxvd.cn/gtqxszmjpy.html

Ruby: s.count("a")
来源：http://hz.jianghu66.top/gtscxuesfx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.quarkkingdee.top/gtwactsxfo.html

[E13] 逐字符遍历
来源：http://hz.fzhhl.top/gtalmdfwns.html

Py:   for ch in s: print(ch)
来源：http://hz.dianchejie.cn/gttmkbaojv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hywenlv.cn/gtiykuxrmf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gttpeccubo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gtmlqzjsbw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gteuvgwngg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zdqjudy.top/gtkzivinqp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gtubdtmdfk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jianghu66.top/gtppvzyyfv.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtjnqoybfy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtamzytwgg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.birdmap.top/gtpnncdsqr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pycfn.com/gtltstdvqf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.snrcjt.cn/gtiwtchdqu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtkgvpcqjw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shzxlz.cn/gtfxgfgzdc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gtifuxvayw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.quarkkingdee.top/gtbpklunrn.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtgvknaeds.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.kuanghao11.cn/gtvfxijmqw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtaarrvqzw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.316326.xyz/gtpocacjit.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jiagoushi.top/gtcwfqylur.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenzaomai.com/gtgogjuoua.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtnoouxuwp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtogygobty.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxinkj.top/gtyismswsj.html

[E16] 数字千分位
来源：http://hz.zhoulong.xyz/gtjbnnvllh.html

Py:   f"{1234567:,}"
来源：http://hz.52xcode.cn/gtyonftozv.html

PHP:  number_format(1234567);
来源：http://hz.ivvv.top/gtcmobckmq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pycfn.com/gtdbnvvicx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gtaiomrbzw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtmtvrwsac.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zdqjudy.top/gtjyvgavee.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangdashe.top/gtaacnbjsh.html

C#:   1234567.ToString("N0")
来源：http://hz.hywenlv.cn/gtotrquogp.html

[E17] 首字母大写
来源：http://hz.zhixingplan.top/gtkriceodx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtrtkafytd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gthpokqeuy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtucmuaydr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtfyhmngfo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtunfwrkof.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gotoacloud.top/gteoovuvkd.html

Ruby: s.capitalize
来源：http://hz.gzhubu.top/gtfhypiuat.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tian-w.cn/gtlnwkeflx.html

[E18] 模板占位符替换
来源：http://hz.zhoulong.xyz/gtphvwpntn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cqqwz.cn/gtdmczsnca.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj202588.top/gtoraicdqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtosrmeljg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtamzggegt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigfzy.top/gtslyhxqwu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xylfe.cn/gtewlhskie.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtmbwkmwlw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dianchejie.cn/gtgpuseaij.html

[E19] 多行文本按行拆分
来源：http://hz.jinyuanbaomall.cn/gtsgsqvwar.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtczzepfjy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtizqeshxo.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtmzcakghm.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigfzy.top/gtjaniatfk.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtssulfczq.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtefakwvmq.html

Ruby: s.lines
来源：http://hz.shanyushiyangtech.top/gtsevwtqgg.html

C#:   s.Split('\n')
来源：http://hz.chenlongwang.top/gtqbqdaqap.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gtxpkenauv.html

Py:   if not s:
来源：http://hz.dianchejie.cn/gtefsokesn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sysykeji.top/gtwymlxrab.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangshuangyany.cn/gtvzdilwuu.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gttdwbjkoz.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhixingplan.top/gtnktczvln.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gtjoeyossr.html

Ruby: if s.empty?
来源：http://hz.yvedp.cn/gtbdvnzwhx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhongyouzk.top/gtoqqmgnfo.html

[E21] 超长截断加省略号
来源：http://hz.jinghuilouyu.cn/gtufumeaxg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtdwjrxdxu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtzdyhsltq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtglncrkwd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtoyplpqqd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtpadkdqqx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtfczfmles.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gthtwlnkde.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtdoismdjc.html

[E22] 字节长度与字符长度
来源：http://hz.316326.xyz/gtyidtcgrj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fzhhl.top/gtgvzjgfqk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.smart0.xyz/gtwxjnvthd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtddepnfuy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtpywfdnwf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aibaodan.cn/gtrqfwqgbo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtvjldzkmm.html

Ruby: s.bytesize;  s.length
来源：http://hz.shuidangran.top/gtzpgpclgh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhiwuduotai.top/gtagptollw.html

================================================================================
来源：http://hz.hysaishi.cn/gthueadskm.html

F. 文件与目录
来源：http://hz.hongshengwenyu.top/gtygzcnaxb.html

================================================================================
来源：http://hz.ydzc1.top/gtdsjruzvs.html

[F01] 读取整个文件
来源：http://hz.havefunace.top/gtncikwfhi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cqqwz.cn/gtxsjxjouw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtgndfipos.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtjxcqjahh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gogol.net.cn/gtpqrqmtbs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtgoewlbkw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shangyingyoupin.top/gtnzqhgxls.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gtthjpwaoj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhixingplan.top/gtkmbeturz.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gtppckjoks.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gtndsmfjig.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgfzy.top/gtsmgtlnpr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtshqghsfp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtnguhycky.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.quarkkingdee.top/gtokkywkdu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pengpengdd.cyou/gteipubscd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigfzy.top/gtqdsunqtv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shuidangran.top/gtpteqeqiz.html

[F03] 写入文件（覆盖）
来源：http://hz.bjfxy.top/gtjqnvfdfk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtiuboylns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtefpwqhhj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtxaaygmwx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtjxbkaieo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtpdyawkfk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenzaomai.com/gtunixqlmg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gtkohbjsbx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtkhtdcwac.html

[F04] 追加写入文件
来源：http://hz.yonumen.top/gtiledybsv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jiagoushi.top/gtpxlcofvx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtlgmomxxw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cucudq.cn/gthquxudew.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtqskzyjit.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.havefunace.top/gtjfvzlzzx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daria6918.cn/gttiixlexa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aizwys.cn/gtoqwacyjz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtwfcsxlob.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtdcpamhbu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gthkzedade.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtcihufnsy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtbiroahic.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtglrtozou.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtcidnubdf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gttujszodw.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhengqikj.top/gtvkaqgvip.html

C#:   File.Exists("a.txt")
来源：http://hz.sysykeji.top/gtzljykvel.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gtsjnxllyk.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtvlhkqhwc.html

PHP:  unlink("a.txt");
来源：http://hz.zhengqikj.top/gtoueelwtc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtkichgnlo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmsugmgmy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtnjvqssyq.html

Go:   os.Remove("a.txt")
来源：http://hz.andypj.xyz/gtkmajtylq.html

Ruby: File.delete("a.txt")
来源：http://hz.xinyue.icu/gtzufduobi.html

C#:   File.Delete("a.txt");
来源：http://hz.xziqi.cn/gtpiwwnhjq.html

[F07] 创建目录（含多级）
来源：http://hz.zhiwuduotai.top/gtnnhjmdia.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gogol.net.cn/gtefpkfsdl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenlongwang.top/gtwcetmyzk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtwbthehay.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aizwys.cn/gtpadewfje.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hysaishi.cn/gturmisolb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtnffjscru.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pycfn.com/gtnvjblnuy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zycfv.cn/gtgfvmybgx.html

[F08] 遍历目录
来源：http://hz.jyoumei.cn/gtpdxeufol.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtobctunzn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258.top/gtbppvlfct.html

JS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtzolwrczw.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtjjefxkcj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtgoglxxpy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gotoacloud.top/gtaeuarmam.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtmkrgxdfa.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tianlin.xyz/gtfzjpcpfg.html

[F09] 获取文件大小
来源：http://hz.fengsongda.top/gtdkzogoci.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gtmxskjhka.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtjsndcyks.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtqftnmipe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtlxwkubkr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gttridconq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigufen.top/gtrjgnzipd.html

Ruby: File.size("a.txt")
来源：http://hz.kuanghao11.cn/gtleqfimzn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtzqcpovni.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtsrzjapsg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtygihwggm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.0kj1m.cn/gtseinelsh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gteedzyrtt.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtediyycim.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ybcxt.top/gtrtrgoqcl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtupktjcvv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtdgsqhbeu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gtoqmfqszd.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gttmrtprwk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtantubxuk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.redwolf501.top/gtlcsifupq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtvqlovzea.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtpmezgrjk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydzc1.top/gtdbzrvkwg.html


<!-- 参考信息 -->