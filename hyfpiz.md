代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtgvjcdvmj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtfxvejwmn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cashguo.top/gtopcevxrm.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtgtceywxb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gtfjxqgfdb.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtuuxlgyav.html

JS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtnpniidzk.html

TS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtkefxwnsj.html

Java: String.join(", ", list)
来源：http://hz.feifeiyinyue.top/gteszmyvpe.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuanzx.com/gtkfexucdp.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gtrwtdtawt.html

C#:   string.Join(", ", list)
来源：http://hz.smart0.xyz/gtebwrwrln.html

================================================================================
来源：http://hz.iojbl.cn/gtqukxugxr.html

E. 字符串处理
来源：http://hz.smart0.xyz/gtarzbcien.html

================================================================================
来源：http://hz.cqqwz.cn/gtwhnyrlqu.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gteawrtjgo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtyestfczz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.feifeiyinyue.top/gthtqhjdqd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gttkuqsbfc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtbflbnwpu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenzaomai.com/gtgyvkpdry.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gtwzavulsq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zdqjudy.top/gtvrnyumxx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cashguo.top/gtlhjgsiyf.html

[E02] 重复字符串
来源：http://hz.jqgufenzy.top/gtjjlermxi.html

Py:   "ab" * 3
来源：http://hz.yj20258888.top/gtdnvemvtw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aibaodan.cn/gtloltczts.html

JS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtbkzdrsdc.html

TS:   "ab".repeat(3)
来源：http://hz.guannengcc.top/gtakevayte.html

Java: "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtznqfplwx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yuanzhike.top/gtrnoibuca.html

Ruby: "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtwhsdoijf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.svipenyu.cn/gtydmbmqef.html

[E03] 截取子串
来源：http://hz.yangfankeji.com/gtncypoama.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtrxoypvte.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jiagoushi.top/gtehhpyrbv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtqohbjgqq.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtgmfkpwjb.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gthybxswsp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258888.top/gtjyucswky.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xziqi.cn/gtxfuotjdp.html

C#:   s.Substring(1, 3)
来源：http://hz.vqdsnc.cn/gterbubccr.html

[E04] 查找子串位置
来源：http://hz.iojbl.cn/gtbwqkmyop.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtgkezzill.html

PHP:  strpos($s, "x");
来源：http://hz.yueranfly.top/gtpvtckxpa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenlongwang.top/gtdtpmtdhh.html

TS:   s.indexOf("x")
来源：http://hz.yj20258.top/gtvpnvlbpw.html

Java: s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtelsnqicd.html

Go:   strings.Index(s, "x")
来源：http://hz.mhx1999.top/gtusqmcfwd.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtzqizzfbb.html

C#:   s.IndexOf("x")
来源：http://hz.hywenlv.cn/gtwxemenry.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pengpengdd.cyou/gtzftitkqf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yongpay.top/gtsilnmdcj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtozbkhsdj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtyzydznac.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtnjlzvoxf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gtxxlrsvvh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.0kj1m.cn/gtoikytvjl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guannengcc.top/gtomcbuthk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ppjwa.cn/gtkjfrehiq.html

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtehtyvvcb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenzaomai.com/gtayvjskai.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgufenzy.top/gtuicyjcha.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtohfflfoy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtvgsnaxho.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtcqraqpfa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sxryk.cn/gtmffjthrt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtzjlpjipo.html

C#:   s.Replace("a", "b")
来源：http://hz.aibaodan.cn/gtxhvuryxs.html

[E07] 按分隔符拆分
来源：http://hz.mhx1999.top/gtlfzxauej.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gogol.net.cn/gtevglsjwo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tianlin.xyz/gtyylzowym.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenzaomai.com/gtlwsuioec.html

TS:   s.split(",")
来源：http://hz.zycfv.cn/gtzuwutnlu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangshuangyany.cn/gtrfcxblnz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtxcfiaozg.html

Ruby: s.split(",");  s.split
来源：http://hz.hnqzz.top/gtxzcjzhhl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gtmtzliulq.html

[E08] 数组按分隔符合并
来源：http://hz.hfpthk.cn/gtsriuiffd.html

Py:   ",".join(items)
来源：http://hz.zhijiandao.cn/gtnzkeroou.html

PHP:  implode(",", $items);
来源：http://hz.xingfuxueyuan.xyz/gtadomscmf.html

JS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtvhgzbxqt.html

TS:   items.join(",")
来源：http://hz.yongpay.top/gtvdyishng.html

Java: String.join(",", items)
来源：http://hz.yvedp.cn/gthdzhvnhr.html

Go:   strings.Join(items, ",")
来源：http://hz.zhijiandao.cn/gthigknpfm.html

Ruby: items.join(",")
来源：http://hz.gzhubu.top/gtjxpkfwxz.html

C#:   string.Join(",", items)
来源：http://hz.feifeiyinyue.top/gtzmbwjqgc.html

[E09] 去除所有空白字符
来源：http://hz.zhengqikj.top/gtefhhexeg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtgvmnjzlu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhaomingkeji.xyz/gtkcccsrgj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtipsaicqd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtxuiajcon.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtpztjzgwl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gaohongyu789.top/gtsxmloqii.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.0kj1m.cn/gtkdafshcu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nanxuanxn.top/gtmiixpbmx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenlongwang.top/gttkkpzlta.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hysaishi.cn/gtkktwtlym.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cucudq.cn/gtfovailev.html

JS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtghvnceiy.html

TS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtcrhsgtbj.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtyvqpapum.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gtlscumpjp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.snrcjt.cn/gtxkfklntj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinyuanbaomall.cn/gtkgtahsex.html

[E11] 反转字符串
来源：http://hz.yangfankeji.com/gtwsomfrub.html

Py:   s[::-1]
来源：http://hz.jinqigufen.top/gtxdnjhhqv.html

PHP:  strrev($s);
来源：http://hz.c1oappe.top/gttkbojldu.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtkpcebafj.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtyjhmalnl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guowangkeji.top/gtfpekpoiv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xylfe.cn/gthkrdohwk.html

Ruby: s.reverse
来源：http://hz.hnxiangtu.top/gtzulrtckk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtvbehbzbn.html

[E12] 统计某字符出现次数
来源：http://hz.ybcxt.top/gtrveyswtu.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtpuovslim.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtmhyyjmci.html

JS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gttxmowmlm.html

TS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtpyvjhnqp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtudfugsop.html

Go:   strings.Count(s, "a")
来源：http://hz.xuetiantiany.cn/gtpvdipxtd.html

Ruby: s.count("a")
来源：http://hz.snrcjt.cn/gteimrdsyb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xinyue.icu/gtkpzzfgyk.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gtrizfweyv.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtlzwckdwh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtdlagpmmq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtjkwirgum.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtolasatvx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nanxuanxn.top/gtleztozfx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxuanxn.top/gtcjejswwg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gtbrogvfjk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnqzz.top/gtqhbxhzqs.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtapwxegab.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhiwuduotai.top/gtbjcdklgf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangkeji.top/gthxclnxnl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhongyouzk.top/gtachgpcoj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtmdbrffnf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gtkmpzuybi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhongyouzk.top/gtcztsbpje.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gthqtwvdge.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenzaomai.com/gtkfpmyywn.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtzotwtyxo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gtaxolkldr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.snrcjt.cn/gtvhovvvoh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtohoownqd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtbvomxzox.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtqwgxxojf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtozkgqtfd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gtkzfysmgk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258.top/gtwomcodzu.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtlpxwoena.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtpfiympqg.html

PHP:  number_format(1234567);
来源：http://hz.xingfuxueyuan.xyz/gtbvixkbhf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtzmcbnucl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtpblwpays.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtsxomyfht.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.wangdashe.top/gtqtozmtjk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guowangkeji.top/gtvecbhkqd.html

C#:   1234567.ToString("N0")
来源：http://hz.redwolf501.top/gtfrwnazfg.html

[E17] 首字母大写
来源：http://hz.daria6918.cn/gtramenrae.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtfigaxfxa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.andypj.xyz/gtekrywmrp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtnpodaqeo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gtdnkukijx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dianchejie.cn/gtlerblmxp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jyoumei.cn/gtuldnsgay.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtahvvqyat.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.snrcjt.cn/gtbcacegtd.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtydltjsqc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yvedp.cn/gtgwlldgwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuanzx.com/gtxlqeesmy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtumknfzuo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtjhzcuhvr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenjidiqi.icu/gtiajvvbjh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.feifeiyinyue.top/gtxilptnnr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pengpengdd.cyou/gtohumlgej.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cdnleiting.top/gtymvftqyt.html

[E19] 多行文本按行拆分
来源：http://hz.shuidangran.top/gthqujcgxa.html

Py:   s.splitlines()
来源：http://hz.zycfv.cn/gtyflunsan.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtvpxkgvaj.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtluxkylle.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtosxpzlzb.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtxecuiwjs.html

Go:   strings.Split(s, "\n")
来源：http://hz.sweek.top/gttyzbpzve.html

Ruby: s.lines
来源：http://hz.sufxvd.cn/gtofilkzqx.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gtarkjbznj.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtajcigbbu.html

Py:   if not s:
来源：http://hz.zhijiandao.cn/gtdyfafexb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gttcckdsny.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.birdmap.top/gtnetlntdz.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtvrpgocsq.html

Java: if (s.isEmpty()) {}
来源：http://hz.sysykeji.top/gtcyxylihk.html

Go:   if s == "" {}
来源：http://hz.feifeiyinyue.top/gtutkjnnnh.html

Ruby: if s.empty?
来源：http://hz.haohaochexian.top/gtbcikikfl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxuanxn.top/gtmscloglt.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtmroejyob.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dashuyun.cn/gteicbylql.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gtffsnawqs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtcrwxsqub.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtgfkbfcah.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtocjykavn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aizwys.cn/gtdncxyrvs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jyoumei.cn/gtsulyqmwa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtwpedubri.html

[E22] 字节长度与字符长度
来源：http://hz.jyoumei.cn/gtfiuxuohj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cdnleiting.top/gtsghyrlax.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gttzhkueoh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gttruoqrqv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhijiandao.cn/gtxptggwhb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj202588.top/gthetxxqbt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zycfv.cn/gtgjiejsrg.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gttszzdhcz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.haohaochexian.top/gtcxmlrpav.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtyozafheu.html

F. 文件与目录
来源：http://hz.fengsongda.top/gtldpxjrhz.html

================================================================================
来源：http://hz.snrcjt.cn/gtidgfmicn.html

[F01] 读取整个文件
来源：http://hz.ydjk.org.cn/gtbhvlkcik.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxuanxn.top/gtuhqfszos.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ppjwa.cn/gthjjtqnke.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtwjqrurhb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gthgbvkeux.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gterbyjxww.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtqcyhbgyo.html

Ruby: File.read("a.txt")
来源：http://hz.quarkkingdee.top/gtbpakrmxv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhixingplan.top/gtlhjmpmag.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtbqyhnsvz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cdnleiting.top/gtwvokbzzs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cdnleiting.top/gtyteluzrq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtdrslsqxo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtgtmzkscj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtwsssewae.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shzxlz.cn/gtnwxkbhep.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.meibo888.top/gtlaohiarf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ppjwa.cn/gtugcpaczg.html

[F03] 写入文件（覆盖）
来源：http://hz.nanxuanxn.top/gtnvlwqlfq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtzkccqqor.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtjsgzwilh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtgkyewksv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtgngcfqzx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gtpkhynjxw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xuetiantiany.cn/gtutaepssx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtxzywlawf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenzaomai.com/gtgkunvrft.html

[F04] 追加写入文件
来源：http://hz.yuanzhike.top/gtgrunqona.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.316326.xyz/gthitzzvjz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yanxiufei.cn/gtzscnkxjb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtovekflzr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtjzcqzbyk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtonqegkwr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.svipenyu.cn/gtfescwmfv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydjk.org.cn/gtdgabbehb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gtbhzprejt.html

[F05] 判断文件或目录是否存在
来源：http://hz.yvedp.cn/gtihiykgev.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtcbcepgkx.html

PHP:  file_exists("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtkzprphqo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtakbtomzu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtesfrcsjv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtettrepcn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yueranfly.top/gtqtaslixj.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gthzmhxtao.html

C#:   File.Exists("a.txt")
来源：http://hz.9152youxi.cn/gtawzasxwy.html

[F06] 删除文件
来源：http://hz.svipenyu.cn/gtpdokfhgl.html

Py:   os.remove("a.txt")
来源：http://hz.aizwys.cn/gtafqpqeee.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtumjwnfno.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtkaonbqyw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtngrnebut.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtlifqifzt.html

Go:   os.Remove("a.txt")
来源：http://hz.guowangkeji.top/gtreapdzzv.html

Ruby: File.delete("a.txt")
来源：http://hz.yj20258.top/gtgwssevek.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtyvdmfqdz.html

[F07] 创建目录（含多级）
来源：http://hz.sufxvd.cn/gtgfqioewy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhongyouzk.top/gtdfkwuuyi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yanxiufei.cn/gtxjubmqnf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtbxeygkbd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtclvgarmw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jiagoushi.top/gtedqhqoop.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangshuangyany.cn/gtsvfkksoc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj202588.top/gtzjfswknl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtfxmtabpf.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gtyluravyh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ybcxt.top/gtnobwtltl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinghuilouyu.cn/gtbslpnkon.html

JS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtsfvybcga.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtzdzpuhlz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtyfyrzvac.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtkumnqqca.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtyvnvtvgy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dianchejie.cn/gtecpoublc.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtrlijsiua.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtsthharhx.html

PHP:  filesize("a.txt");
来源：http://hz.meibo888.top/gtdcutjoyk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtodexsaew.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gttwrrlcrz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtjwqnuuvp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gthibrimvp.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gttzmtzzfc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtepgswtlq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gtwlxtxzgh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtwtlewjvi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtonhtozya.html


<!-- 参考信息 -->