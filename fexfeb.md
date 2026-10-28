代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cqqwz.cn/gtcnpsviut.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ehwqpu.com/gttlspaowc.html

[D25] Set 集合去重与交并差
来源：http://hz.zhengqikj.top/gtohlzdhdt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.havefunace.top/gtgbsyrqdw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.daria6918.cn/gtigaskmib.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hysaishi.cn/gtxiscmlal.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hysaishi.cn/gtpfxzcfyn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtjywhirxr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.havefunace.top/gtvwlqvzvg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuetiantiany.cn/gtsjhktjps.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuanzx.com/gtijqrnrlf.html

[D26] 数组转字符串
来源：http://hz.sxryk.cn/gtpngqfjwn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhoulong.xyz/gtinsrgmdd.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gtmvztduyj.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtqikstagh.html

TS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtvfaksvjl.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtngqwuvrx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tanke756.top/gtrcsyllpd.html

Ruby: arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtxjaqzkyz.html

C#:   string.Join(", ", list)
来源：http://hz.snrcjt.cn/gtrbclktxc.html

================================================================================
来源：http://hz.gzhubu.top/gtkifxkczx.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtgrysygpk.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmkpkazxo.html

[E01] 拼接字符串
来源：http://hz.shuidangran.top/gtiuwfahuc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenjidiqi.icu/gtfxtmnykk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guowangkeji.top/gtzegxfcod.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtmouadvoa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtnkbkkbbv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangkeji.top/gtfnirfcqz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangkeji.top/gtkqwfqbzw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuxming.cn/gtejwwflzt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangdashe.top/gtauydfprc.html

[E02] 重复字符串
来源：http://hz.hnqzz.top/gtnbervwxi.html

Py:   "ab" * 3
来源：http://hz.shuidangran.top/gtfosgglkd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtjsinbikx.html

JS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtcehjakul.html

TS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtjmsclygo.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtalldzjcu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgufenzy.top/gtrtrtuijr.html

Ruby: "ab" * 3
来源：http://hz.hongshengwenyu.top/gtjbdappsk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.vqdsnc.cn/gthinuhleb.html

[E03] 截取子串
来源：http://hz.hfpthk.cn/gtodzlgioi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.snrcjt.cn/gtvrqxhpit.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydzc1.top/gtzrzfqszu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yongpay.top/gtldcojtfu.html

TS:   s.slice(1, 4)
来源：http://hz.hammf.cn/gtadwhrwin.html

Java: s.substring(1, 4)
来源：http://hz.9152youxi.cn/gttlaqmwmu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydjk.org.cn/gticgtbjrs.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtuehkpjox.html

C#:   s.Substring(1, 3)
来源：http://hz.hammf.cn/gtovhdmgju.html

[E04] 查找子串位置
来源：http://hz.xylfe.cn/gtztvbjfsz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtklnnqmuz.html

PHP:  strpos($s, "x");
来源：http://hz.zycfv.cn/gtmqrnhdyt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtsfweiwgq.html

TS:   s.indexOf("x")
来源：http://hz.chenzaomai.com/gtjngfxmki.html

Java: s.indexOf("x")
来源：http://hz.chenzaomai.com/gtooiwnlle.html

Go:   strings.Index(s, "x")
来源：http://hz.quarkkingdee.top/gtsxemnrgv.html

Ruby: s.index("x")
来源：http://hz.vqdsnc.cn/gtlnjyzmxp.html

C#:   s.IndexOf("x")
来源：http://hz.fengsongda.top/gtscepwxrr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sysykeji.top/gtcwxxmnvx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zycfv.cn/gtlueuwzit.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.bjfxy.top/gtfkfzzerm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtikoxkiwt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtueuafsjy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtnxbdxiur.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zycfv.cn/gtnqbfllvl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnxiangtu.top/gtdilhyfia.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sufxvd.cn/gtlwdojhmd.html

[E06] 替换子串
来源：http://hz.hammf.cn/gtptoupbma.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuanzhike.top/gttuneevnx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pycfn.com/gtjqfqclkf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtupgkxvck.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtdcyoogbf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtqydzewiu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgufenzy.top/gtizjxathl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gttfzvftvu.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtdcoqszfz.html

[E07] 按分隔符拆分
来源：http://hz.yangfankeji.com/gtrxatyrtk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnqzz.top/gtyvoqljwc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gtmikyqiik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ppjwa.cn/gtogygdxpj.html

TS:   s.split(",")
来源：http://hz.yanxiufei.cn/gtlahosmfs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zycfv.cn/gtfetmhnde.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhoulong.xyz/gtctoqgvlw.html

Ruby: s.split(",");  s.split
来源：http://hz.quarkkingdee.top/gtctlljduk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gteybxhzmx.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtpmnclmdx.html

Py:   ",".join(items)
来源：http://hz.havefunace.top/gtngqjbepq.html

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtdvpaqluj.html

JS:   items.join(",")
来源：http://hz.dianchejie.cn/gttldomvmm.html

TS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtvkbvpgcl.html

Java: String.join(",", items)
来源：http://hz.iojbl.cn/gtjpxqeyul.html

Go:   strings.Join(items, ",")
来源：http://hz.yanxiufei.cn/gtvyqlltpc.html

Ruby: items.join(",")
来源：http://hz.kuanghao11.cn/gtgwzbvoqu.html

C#:   string.Join(",", items)
来源：http://hz.nwbrower.top/gthhkuhaip.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gthuomhkij.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ybcxt.top/gtkxmtjanz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtiaabioja.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtrkustgog.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtiufxlvxs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ybcxt.top/gtuhodfbdc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gtuwttbwax.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtzjzxfsef.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jlsjyb.cn/gtrosupbml.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhongyouzk.top/gtmykhjhup.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cashguo.top/gtjwhnandq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jlsjyb.cn/gtwvlumuaj.html

JS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtrjsynthz.html

TS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtsunfbsxx.html

Java: String.format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gttnaiqgze.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtytobxxfo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shuidangran.top/gtxnjbqbse.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.meibo888.top/gtwgwbirji.html

[E11] 反转字符串
来源：http://hz.xylfe.cn/gttbdlhylr.html

Py:   s[::-1]
来源：http://hz.daria6918.cn/gtvurptiev.html

PHP:  strrev($s);
来源：http://hz.nanxinkj.top/gtyllbsxwo.html

JS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtumtxqocp.html

TS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtnxnuqcmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtpsuweyne.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tian-w.cn/gtisdjfceb.html

Ruby: s.reverse
来源：http://hz.52xcode.cn/gtpwwfypyd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtzlqzthxc.html

[E12] 统计某字符出现次数
来源：http://hz.meibo888.top/gthnbnmcgo.html

Py:   s.count("a")
来源：http://hz.nwbrower.top/gtdwyiakxl.html

PHP:  substr_count($s, "a");
来源：http://hz.hysaishi.cn/gtszmspnci.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtitrmabhv.html

TS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtfequfjwm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yangfankeji.com/gthvueqybx.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtbcnijlsp.html

Ruby: s.count("a")
来源：http://hz.cashguo.top/gthtqfnfhj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gthsqmwuns.html

[E13] 逐字符遍历
来源：http://hz.fengsongda.top/gtydbrpwtp.html

Py:   for ch in s: print(ch)
来源：http://hz.jyoumei.cn/gtnzxcqwio.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.birdmap.top/gtdstyskwe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtfnkcpocd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtvwqjaxql.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shangyingyoupin.top/gtebkcybuw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dianchejie.cn/gtjmffjxdw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.snrcjt.cn/gtavnunuwj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sysykeji.top/gtfpzgqfjf.html

[E14] URL 编码与 Base64
来源：http://hz.shangyingyoupin.top/gtwxhootur.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtlyvjhxsl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj202588.top/gtrfkptabe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jiagoushi.top/gtzbvsyfnh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zycfv.cn/gttkumpgnw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yuanzhike.top/gtmvldioer.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gtxxzvvuwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.bjfxy.top/gtjdwczfkh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.redwolf501.top/gteifzmbti.html

[E15] HTML 转义 / 反转义
来源：http://hz.tianlin.xyz/gtlkzyxywr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cheryme.top/gttxovdfdv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ivvv.top/gtdmnkzwrw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtvqlelvpq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yanxiufei.cn/gttmdxkbsn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dianchejie.cn/gtgayhukzi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.52xcode.cn/gtizxswxbx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daxiang520.top/gthhhsjhtq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gzhubu.top/gtgncuuidf.html

[E16] 数字千分位
来源：http://hz.daxiang520.top/gtdczjzzjc.html

Py:   f"{1234567:,}"
来源：http://hz.jinghuilouyu.cn/gtvlqvimlh.html

PHP:  number_format(1234567);
来源：http://hz.cdnleiting.top/gtmrxcvtbr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtmyhqtavm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtnvdyunan.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yanxiufei.cn/gtqvfbtnfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.vqdsnc.cn/gtegammqwr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.haohaochexian.top/gtrmumjtsk.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gtojqvkyag.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gtfpuarsbu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gtqoltvsjc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pengpengdd.cyou/gtzxsljywg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtaduwzkfr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtqvttdeui.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yvedp.cn/gtozqixtxm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtdczbnspl.html

Ruby: s.capitalize
来源：http://hz.shuidangran.top/gtoaahwhch.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtmzxbwlkt.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gtbljrmqgh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtdamyhryk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gttmmarifz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtherlwekq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gthxvjxarf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.birdmap.top/gtnuktidxs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgufenzy.top/gtxqeafpvd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtmgplnjpp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtnbewsxhi.html

[E19] 多行文本按行拆分
来源：http://hz.fengsongda.top/gtrepowhyz.html

Py:   s.splitlines()
来源：http://hz.aibaodan.cn/gtvuknrekf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gtqvpwoxoj.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtxzoddfld.html

TS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtuexzwvmx.html

Java: s.lines().toList()
来源：http://hz.meibo888.top/gtgsungywm.html

Go:   strings.Split(s, "\n")
来源：http://hz.pengpengdd.cyou/gttkldojec.html

Ruby: s.lines
来源：http://hz.yj20258.top/gtxwwftcfj.html

C#:   s.Split('\n')
来源：http://hz.vqdsnc.cn/gtxmtpxnyb.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtiyywrcgy.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtpklyykwu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jyoumei.cn/gtwbadwjtx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hysaishi.cn/gtgzldouku.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gttmwrgsbb.html

Java: if (s.isEmpty()) {}
来源：http://hz.daria6918.cn/gtqkahqzxv.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gtgdejadgw.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtnpfptrhp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtzzmyykmr.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtdlhdbzpx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dashuyun.cn/gtjftjlint.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgufenzy.top/gtddpikuxi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtwkcehmhg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtluqmjygy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtpsisoxjs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtikqbnzyl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gthfjzjqai.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtyugofdhi.html

[E22] 字节长度与字符长度
来源：http://hz.vqdsnc.cn/gtmdkeidze.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cucudq.cn/gtxwglszcm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gteombhbna.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtphbohvqo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtyubkvovd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtmpacsvuf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258.top/gtydanswkm.html

Ruby: s.bytesize;  s.length
来源：http://hz.gzhubu.top/gtdollslwf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtsgumivwe.html

================================================================================
来源：http://hz.sweek.top/gtdjirfmyj.html

F. 文件与目录
来源：http://hz.yongpay.top/gtcfhzmegh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrpgyjqbk.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangtech.top/gtseuizbpz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gaohongyu789.top/gtyrtqrtru.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shuidangran.top/gtywnptuzi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtrepnvszk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.0kj1m.cn/gtbfxsrwrg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtwuoovlxd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtboubwrvs.html

Ruby: File.read("a.txt")
来源：http://hz.jqgfzy.top/gtqvbbygnh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtfucgthoj.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gtwltuogwr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shzxlz.cn/gtassstfsd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtvvvnxqcf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtvvcpysep.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtixvuqwhs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtsuoemrfv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.mhx1999.top/gtsmpwewyp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinghuilouyu.cn/gtyhuklalc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.svipenyu.cn/gtkpgieiew.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangtech.top/gtimpmrkrx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtbllkqjeq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtrjafzzqy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtowichqpa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtrphhzpsl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.redwolf501.top/gtvumtcbvt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtwvtcybut.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.vqdsnc.cn/gtqeubepmm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cheryme.top/gtzaryahfj.html

[F04] 追加写入文件
来源：http://hz.zhixingplan.top/gtlktwudio.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daxiang520.top/gtjdfnadnj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pengpengdd.cyou/gttddbgstd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gttctccalm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtgqmbdryt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtpqtvznwn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fzhhl.top/gtghnyppfc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtbdgxoevr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtpbcdcacg.html

[F05] 判断文件或目录是否存在
来源：http://hz.ppjwa.cn/gtwwbnfuzy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtcyyojdwg.html

PHP:  file_exists("a.txt");
来源：http://hz.ydjk.org.cn/gthmbmutbf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtkamfafqs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtcrlysjgw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtyjaazefl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.haohaochexian.top/gtrzglkhoq.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtcrqhozpv.html

C#:   File.Exists("a.txt")
来源：http://hz.hysaishi.cn/gtsnuuhayp.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtovaweqqo.html

Py:   os.remove("a.txt")
来源：http://hz.aibaodan.cn/gtcpyhgbqr.html

PHP:  unlink("a.txt");
来源：http://hz.ehwqpu.com/gtrflvqphc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtgbtjdxqi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtcszyrrke.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gttvvvccoe.html

Go:   os.Remove("a.txt")
来源：http://hz.mhx1999.top/gtycurfoxu.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxuanxn.top/gtntrdlyme.html

C#:   File.Delete("a.txt");
来源：http://hz.316326.xyz/gticgessjc.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtbultynxb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cucudq.cn/gtgkkifqnc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hywenlv.cn/gtxvzyvics.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtdpxmxrhi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtcwkonzbj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenzaomai.com/gtwydifthv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.dianchejie.cn/gtlmasmoaj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jlsjyb.cn/gtmzysqnnb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.316326.xyz/gtpjaqbqfw.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gtnajhrhqf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xziqi.cn/gtcawfyeim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gttdddtcay.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtwrxhgddz.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtammxvpao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.havefunace.top/gteinbptpq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tian-w.cn/gttphapvgv.html

Ruby: Dir.children("dir")
来源：http://hz.hywenlv.cn/gtynjariew.html

C#:   Directory.GetFiles("dir")
来源：http://hz.52xcode.cn/gtmvqdgcoq.html

[F09] 获取文件大小
来源：http://hz.c1oappe.top/gtujjnwxlm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtacvngvdk.html

PHP:  filesize("a.txt");
来源：http://hz.52xcode.cn/gtzejagdzb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtptsniwbw.html


<!-- 参考信息 -->