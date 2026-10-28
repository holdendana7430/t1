代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtaqgmyisn.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gtjetuezio.html

JS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtlijgsmlc.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtfnyyvmai.html

Java: String.join(", ", list)
来源：http://hz.shuidangran.top/gtmriuahnq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hysaishi.cn/gtsuyfxwev.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gtswsiapmk.html

C#:   string.Join(", ", list)
来源：http://hz.hnxiangtu.top/gtgauhepvi.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlzpqfels.html

E. 字符串处理
来源：http://hz.birdmap.top/gtqwzybiqb.html

================================================================================
来源：http://hz.jiagoushi.top/gtohwdlgwg.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gtokdckjto.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangkeji.top/gtswingmkd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shzxlz.cn/gtwkzbvqbw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtguqflomt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daxiang520.top/gtxyexfqle.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yueranfly.top/gtrmdvqxpw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shangyingyoupin.top/gtlmhidsen.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ppjwa.cn/gtxpyfwcet.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gtoaupjxrt.html

[E02] 重复字符串
来源：http://hz.jinqigufen.top/gtkkbmjgbk.html

Py:   "ab" * 3
来源：http://hz.aizwys.cn/gtjcdcxbly.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gthbswacqx.html

JS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtnnkvplak.html

TS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gttamzegsq.html

Java: "ab".repeat(3)
来源：http://hz.c1oappe.top/gtfsgzxwry.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ehwqpu.com/gtkzsoirzb.html

Ruby: "ab" * 3
来源：http://hz.bjfxy.top/gtsryvllmn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.9152youxi.cn/gtpemdfapl.html

[E03] 截取子串
来源：http://hz.52xcode.cn/gtearshiqk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgfzy.top/gtzukiiyzq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtvlcgunqz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yvedp.cn/gtnwbzuwia.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtsvzheacl.html

Java: s.substring(1, 4)
来源：http://hz.ybcxt.top/gtrlsijdbi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gaohongyu789.top/gtarhgyzvs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yongpay.top/gtistylids.html

C#:   s.Substring(1, 3)
来源：http://hz.c1oappe.top/gttakexsyh.html

[E04] 查找子串位置
来源：http://hz.jinqigfzy.top/gthqggmnif.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinghuilouyu.cn/gthxcuurao.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtzvghaiix.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.kuanghao11.cn/gtifdemaqp.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtlvxrjurq.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtfgowcnpz.html

Go:   strings.Index(s, "x")
来源：http://hz.xylfe.cn/gtlbuottuy.html

Ruby: s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gthhkogvdf.html

C#:   s.IndexOf("x")
来源：http://hz.wangshuangyany.cn/gtmkzhriex.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hfpthk.cn/gthjldjtqv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangdashe.top/gtahzubfqa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gtkbaasmqj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtnynpajvs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.smart0.xyz/gtmmihnddt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtjuyjdpms.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenjidiqi.icu/gtzaytkebx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hammf.cn/gtuwoofqgn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nwbrower.top/gtpqgkecni.html

[E06] 替换子串
来源：http://hz.zhiwuduotai.top/gtbjwmfjhy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtbazcovtu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.smart0.xyz/gtwavxhnlb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtejmttuzo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gttuqjzpwb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtoatrbaiv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgufenzy.top/gtjhmvkhag.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.kuanghao11.cn/gtifisyiun.html

C#:   s.Replace("a", "b")
来源：http://hz.andypj.xyz/gtxjglhgdf.html

[E07] 按分隔符拆分
来源：http://hz.sysykeji.top/gtqkrsmawc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtxvnjlwpr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangshuangyany.cn/gtdbjcuuqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gtpcnijzlx.html

TS:   s.split(",")
来源：http://hz.jinghuilouyu.cn/gtrhkqcqoe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hywenlv.cn/gtuzqkrcti.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ybcxt.top/gtsdkiteno.html

Ruby: s.split(",");  s.split
来源：http://hz.chenzaomai.com/gtmkurwhwj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258888.top/gtcosimseu.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtjrdpadmv.html

Py:   ",".join(items)
来源：http://hz.ehwqpu.com/gtgetbtees.html

PHP:  implode(",", $items);
来源：http://hz.cdnleiting.top/gtkhgvomna.html

JS:   items.join(",")
来源：http://hz.zycfv.cn/gtclthjcky.html

TS:   items.join(",")
来源：http://hz.yonumen.top/gtxovctodr.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gtyibafuxx.html

Go:   strings.Join(items, ",")
来源：http://hz.0kj1m.cn/gtayttprlk.html

Ruby: items.join(",")
来源：http://hz.wangshuangyany.cn/gtpbaavykf.html

C#:   string.Join(",", items)
来源：http://hz.meibo888.top/gtyzlilslm.html

[E09] 去除所有空白字符
来源：http://hz.tianlin.xyz/gtjsjkzmuu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.fzhhl.top/gtubjoxnir.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gtsxmqyudu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtipsombzo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtuefxjoul.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tian-w.cn/gtrphooopc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtsrlykkss.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gtueblmidf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nwbrower.top/gtlqxpkejx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtsaktqesw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtdmlptlvt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gtxpcntfft.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtkvllndns.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtmwverlok.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtnpvjsmye.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.quarkkingdee.top/gtjenoesue.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtmrlwdygm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.meibo888.top/gtwtumrkob.html

[E11] 反转字符串
来源：http://hz.cheryme.top/gtcpxmxqgr.html

Py:   s[::-1]
来源：http://hz.zhixingplan.top/gtcdamftxx.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtyzqqgpop.html

JS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtbqvcuqos.html

TS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtfdezfwgd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gtitfsstnk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtyjswnczz.html

Ruby: s.reverse
来源：http://hz.xuetiantiany.cn/gtegeivllu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtpicogcfi.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gthrqxxzri.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtoeuepewg.html

PHP:  substr_count($s, "a");
来源：http://hz.shangyingyoupin.top/gtrfxqoufw.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtdggfbsbm.html

TS:   s.split("a").length - 1
来源：http://hz.zhijiandao.cn/gtjsfcqtqp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenlongwang.top/gtarybgmde.html

Go:   strings.Count(s, "a")
来源：http://hz.yj202588.top/gtavxyoxgu.html

Ruby: s.count("a")
来源：http://hz.yanxiufei.cn/gtlfmszzup.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhengqikj.top/gttaxgujla.html

[E13] 逐字符遍历
来源：http://hz.jqgfzy.top/gtqfdonzvi.html

Py:   for ch in s: print(ch)
来源：http://hz.yongpay.top/gttbchzkvh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangdashe.top/gtkffofrft.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.0kj1m.cn/gtgzqaytuy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtczkwtwvd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtyttvbcto.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.andypj.xyz/gtwkwwmmon.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gthcakqovb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shangyingyoupin.top/gtgikwkjwp.html

[E14] URL 编码与 Base64
来源：http://hz.yuanzhike.top/gtpkjihskk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nwbrower.top/gtweqqkazb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuetiantiany.cn/gtdnwosuyu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ppjwa.cn/gtzhaskugw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtuqexnoaz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.vqdsnc.cn/gtqwyxqhyf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xingfuxueyuan.xyz/gtnziwvnas.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.mhx1999.top/gtqyjcfeeu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cheryme.top/gtdwzmaxwa.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhijiandao.cn/gtdhiefvel.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtqzkcwzqd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.fengsongda.top/gtcsjsyinz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtvisvcmqp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pengpengdd.cyou/gtdibswkyh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.quarkkingdee.top/gtwcxmqmva.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jyoumei.cn/gtakowffuo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gteifypzia.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.bjfxy.top/gtmfcvbxrq.html

[E16] 数字千分位
来源：http://hz.jiagoushi.top/gtofbdmrop.html

Py:   f"{1234567:,}"
来源：http://hz.gotoacloud.top/gtluxyofwl.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtmqsrjojv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtbdcbhbab.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtrpaafknb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sufxvd.cn/gtcdojdgmo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gzhubu.top/gtgpwhiatm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sufxvd.cn/gtkhmewvel.html

C#:   1234567.ToString("N0")
来源：http://hz.sysykeji.top/gtqcqpqmns.html

[E17] 首字母大写
来源：http://hz.c1oappe.top/gtkybpkuxr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.andypj.xyz/gtmtufdutr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shuidangran.top/gtjikmtfdo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtujqvjhkr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtyxpdhmjl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shuidangran.top/gtzmwjproh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gtkvcljnpt.html

Ruby: s.capitalize
来源：http://hz.snrcjt.cn/gttnwttfyq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.snrcjt.cn/gtpufbavsh.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtwgktvxok.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cashguo.top/gtrhimfyiy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cqqwz.cn/gtdumfuhqs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtrfhljmfd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sxryk.cn/gtzmtvaamo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gtgltyhcwa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daria6918.cn/gtrgjdmxkb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gteijtnyjr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.quarkkingdee.top/gtizvxebkp.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtkkfyvwaz.html

Py:   s.splitlines()
来源：http://hz.cucudq.cn/gtovnxwuki.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinyuanbaomall.cn/gtutdgllpc.html

JS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtlljlvrgx.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtfbsalahs.html

Java: s.lines().toList()
来源：http://hz.zhongyouzk.top/gtrxevqspq.html

Go:   strings.Split(s, "\n")
来源：http://hz.yangfankeji.com/gtdpuxrxlf.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtwimvhgrl.html

C#:   s.Split('\n')
来源：http://hz.dashuyun.cn/gtocmuqkqs.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gttmkxdrrm.html

Py:   if not s:
来源：http://hz.hysaishi.cn/gtxqwblozo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.bjfxy.top/gtyalfnclu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxuanxn.top/gtchsltikv.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtmcduruiq.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtkpxbgsjy.html

Go:   if s == "" {}
来源：http://hz.yueranfly.top/gtxqszdnus.html

Ruby: if s.empty?
来源：http://hz.chenlongwang.top/gtovegtwkk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258888.top/gthikjfqwm.html

[E21] 超长截断加省略号
来源：http://hz.xinyue.icu/gtnfqslfdk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.redwolf501.top/gtxgeecrpm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.quarkkingdee.top/gtewtoyxdg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gttodzqrku.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtxcrdasan.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtygrzorne.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shanyushiyangkeji.top/gttmgwhdje.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gtopzaeuzm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtusjsidau.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gthmkhywwu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dianchejie.cn/gtnbdkdxmj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yvedp.cn/gtgwfqgghx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtpimfmsrd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtsdeqbogo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.mhx1999.top/gtczdfvhbz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guowangkeji.top/gtottkvhno.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtwnvpytqo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gttvvdvvhf.html

================================================================================
来源：http://hz.tianlin.xyz/gtszyhbdvr.html

F. 文件与目录
来源：http://hz.shzxlz.cn/gtipstcbqb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmevjfztd.html

[F01] 读取整个文件
来源：http://hz.zhongyouzk.top/gtqlytlrdu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtzvfcjfqk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gogol.net.cn/gtbarurugk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.bjfxy.top/gteavbpzlr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hfpthk.cn/gtrenrtxep.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtnbrwvtkc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj20258888.top/gtdsglkqho.html

Ruby: File.read("a.txt")
来源：http://hz.aizwys.cn/gtujtfjdws.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtiadicyye.html

[F02] 逐行读取文件
来源：http://hz.kuanghao11.cn/gtyuenavet.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtniskdlpp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gtiikalfbv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtxtaannaw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gttqhggvfg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtifvsvqsl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shzxlz.cn/gtioqouluz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yangfankeji.com/gtltvedjps.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gzhubu.top/gtnyfljcxi.html

[F03] 写入文件（覆盖）
来源：http://hz.zhijiandao.cn/gtkexbqtkx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.kuanghao11.cn/gtiegxmxjb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtojfbaahb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtwuocprfx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtyvofwywj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtrabymnbr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zdqjudy.top/gtujprvzdt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnxiangtu.top/gtmbzlnvox.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtgctmnvsn.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtclultpsp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtlfbvucfq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aizwys.cn/gtdmeanczd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtwofmakru.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtndgaafvd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fengsongda.top/gtzrdebabg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtysmgnxku.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gtovjbqadj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258.top/gtbiagfjzc.html

[F05] 判断文件或目录是否存在
来源：http://hz.sxryk.cn/gtbzsgeepi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtskhuwmgg.html

PHP:  file_exists("a.txt");
来源：http://hz.yuanzhike.top/gtpszamzwd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtbzglabde.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtbhymczol.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtajyqncyf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jiagoushi.top/gtjlytkggy.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtfdaoaacl.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtygprpbyt.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gtjhbefjit.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtogzssbso.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtyviexvns.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtcukzhqcd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtwtcdqrhz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtqvxyeqqm.html

Go:   os.Remove("a.txt")
来源：http://hz.fengsongda.top/gtsylqcpow.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtjzkpebjk.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gthgnkrxuu.html

[F07] 创建目录（含多级）
来源：http://hz.ydjk.org.cn/gtyltkmnwt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtqcbvakkq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtgepycuqu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gtimkxlcaw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtdusfsgjn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pengpengdd.cyou/gtoxsebwpj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.meibo888.top/gtqahliikp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtgbrdxujv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtpdctmbfj.html

[F08] 遍历目录
来源：http://hz.yvedp.cn/gtfcqiblyp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgufenzy.top/gtfbthstkd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydzc1.top/gtszuffrpu.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtrctqkcrm.html

TS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtajadnrrf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtstrcnkmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydzc1.top/gteksdwsnl.html

Ruby: Dir.children("dir")
来源：http://hz.cashguo.top/gtmdrguqzt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gteevryews.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtbbjyujgd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtdgctafvt.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtamppzgmu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtpcletzzi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtbmangrqv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtqasmfphk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtnayavtok.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtppjkhrcf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.mhx1999.top/gtmgyjolwp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daria6918.cn/gttfqaumri.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtawsccajo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ybcxt.top/gtxsohtdyv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtvuvjptmz.html

TS:   path.extname("a.txt")
来源：http://hz.ehwqpu.com/gtfuusztup.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.havefunace.top/gtsbfobvze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtvkgmordy.html


<!-- 参考信息 -->