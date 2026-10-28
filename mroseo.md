代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dianchejie.cn/gtarniuhsv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fengsongda.top/gtaevduqju.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gzhubu.top/gtfpxnalsw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yongpay.top/gtoalextit.html

[E02] 重复字符串
来源：http://hz.fzhhl.top/gtsowcqdaq.html

Py:   "ab" * 3
来源：http://hz.tian-w.cn/gtphxpsfgb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtqmfmlsja.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtuklhvjlc.html

TS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtbfxuvpxl.html

Java: "ab".repeat(3)
来源：http://hz.sysykeji.top/gtrqdkunay.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pengpengdd.cyou/gtwqazfjrl.html

Ruby: "ab" * 3
来源：http://hz.daxiang520.top/gtkgjqzwog.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnxiangtu.top/gtavxntcui.html

[E03] 截取子串
来源：http://hz.dianchejie.cn/gtbgmjtfjv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhijiandao.cn/gtxvlbgoip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtcubzhcko.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtytxtqglu.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigufen.top/gtnsqfnqcx.html

Java: s.substring(1, 4)
来源：http://hz.yonumen.top/gtirygakdy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.svipenyu.cn/gtdfljthpp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigfzy.top/gtrfcoxawh.html

C#:   s.Substring(1, 3)
来源：http://hz.cashguo.top/gtdydaicfj.html

[E04] 查找子串位置
来源：http://hz.jinghuilouyu.cn/gtihhjevzf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtfuawulyu.html

PHP:  strpos($s, "x");
来源：http://hz.nwbrower.top/gtzuljxahj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hfpthk.cn/gtbhetmmdc.html

TS:   s.indexOf("x")
来源：http://hz.sxryk.cn/gtqiplpyol.html

Java: s.indexOf("x")
来源：http://hz.shuidangran.top/gtvcrvsymq.html

Go:   strings.Index(s, "x")
来源：http://hz.yongpay.top/gtsxecwcxt.html

Ruby: s.index("x")
来源：http://hz.tian-w.cn/gtjchszjaj.html

C#:   s.IndexOf("x")
来源：http://hz.cucudq.cn/gtyfqkrifo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.svipenyu.cn/gtwuztkgpy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tianlin.xyz/gtskurjzwn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jianghu66.top/gtyfghgijn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtvxpkuqxi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtrxcqvvcp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtbtbbnajw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtyepwyqjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.316326.xyz/gteqfdfdar.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.andypj.xyz/gtzknnikfa.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gtnfdqjhic.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.snrcjt.cn/gtbsgrreio.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.fzhhl.top/gttxobuvdk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtclabsdta.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtiuaiiaxm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtidnpsrpi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtyusrsdik.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtipuzovbf.html

C#:   s.Replace("a", "b")
来源：http://hz.ehwqpu.com/gtxnpsqfrl.html

[E07] 按分隔符拆分
来源：http://hz.jyoumei.cn/gtktbnsusi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtpkzpltom.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtptkvflpn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gzhubu.top/gtedqoijqa.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtigceodlu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cdnleiting.top/gtiggicutr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhijiandao.cn/gtgxdypkdj.html

Ruby: s.split(",");  s.split
来源：http://hz.fengsongda.top/gtjqbsodvs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yongpay.top/gtmsiyjemb.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gtuxvwufst.html

Py:   ",".join(items)
来源：http://hz.jinghuilouyu.cn/gtegwghobc.html

PHP:  implode(",", $items);
来源：http://hz.aibaodan.cn/gtrllbkahm.html

JS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtarzylyms.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtxyycwihc.html

Java: String.join(",", items)
来源：http://hz.zhongyouzk.top/gtzelzvuzc.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gtlrvuejru.html

Ruby: items.join(",")
来源：http://hz.jqgfzy.top/gtjjyetkvs.html

C#:   string.Join(",", items)
来源：http://hz.havefunace.top/gtrhnplime.html

[E09] 去除所有空白字符
来源：http://hz.iojbl.cn/gtiagbzfpx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hysaishi.cn/gtybjpxfvs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sweek.top/gtinugdahz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtlsdcyauh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtofweqtnw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtjmlrwehn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtxdqgiiam.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtisewxjrp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.andypj.xyz/gtuxhsuafs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhixingplan.top/gtwuxlfloy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxuanxn.top/gtjqthmteu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hywenlv.cn/gtfdeozjux.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtonjywwok.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtcdamuqxk.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtgjrbpgoq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cqqwz.cn/gtkuzzrkut.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhengqikj.top/gtmzlccbxf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pengpengdd.cyou/gtxedqxoxx.html

[E11] 反转字符串
来源：http://hz.nwbrower.top/gtyefmzyqx.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gtjzdsxvsz.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gttwutgbgy.html

JS:   [...s].reverse().join("")
来源：http://hz.ivvv.top/gtswoaoeks.html

TS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtwziixqcv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtxdsraege.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gtwzcsvsmq.html

Ruby: s.reverse
来源：http://hz.jiagoushi.top/gtbjkhiqhq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gtgtdsfpwe.html

[E12] 统计某字符出现次数
来源：http://hz.gaohongyu789.top/gtvqiobfbs.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtwbrpnrtd.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gthwdxtslf.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtnijexmgt.html

TS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtzvbduftg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gtdchqypxt.html

Go:   strings.Count(s, "a")
来源：http://hz.havefunace.top/gtuljiouiy.html

Ruby: s.count("a")
来源：http://hz.pengpengdd.cyou/gtqovzezsc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aibaodan.cn/gtmsmrfhub.html

[E13] 逐字符遍历
来源：http://hz.ydjk.org.cn/gtcclsfddi.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtpvhfwrxu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhixingplan.top/gtshyvsdeh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtqgcgkwwa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtswzwxzdq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cashguo.top/gtcqmuarak.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shangyingyoupin.top/gtszqwmjvg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yonumen.top/gtcltlbsqx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtspofkmap.html

[E14] URL 编码与 Base64
来源：http://hz.0kj1m.cn/gtnifrvwmv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtcvcbfpzn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gtfcmjudge.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gttaymznve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgufenzy.top/gtoeveiies.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daxiang520.top/gtcmrjcccm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tanke756.top/gtlhkaozsr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigufen.top/gttogmaipf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dashuyun.cn/gtrfxgcttz.html

[E15] HTML 转义 / 反转义
来源：http://hz.birdmap.top/gtdsvueino.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hfpthk.cn/gtfofkrnpb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj202588.top/gtpkrwumtm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gtathdrwpl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.bjfxy.top/gtcjnjkvya.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xziqi.cn/gtgqtbrjuh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tianlin.xyz/gtqjkgfawb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtrbpprbio.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gtkmnaonnq.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtjgtxsvlt.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gthpmpklmv.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtekohkwwh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yvedp.cn/gtgevsgoam.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtxvmkjzfb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtupuebytq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtooksuktf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daria6918.cn/gttfzgdxwh.html

C#:   1234567.ToString("N0")
来源：http://hz.shuidangran.top/gthjliutfg.html

[E17] 首字母大写
来源：http://hz.haohaochexian.top/gtbzghvysc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yanxiufei.cn/gtbhznwkuf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtwodokmno.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtucflpwtq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtlyhuqdym.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtkcrthddn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtpzbjbkti.html

Ruby: s.capitalize
来源：http://hz.wangdashe.top/gtdwannczt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhijiandao.cn/gtkytsvpma.html

[E18] 模板占位符替换
来源：http://hz.nanxinkj.top/gtnaklqucp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daria6918.cn/gtdeanntps.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtcutwybaq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtijlphcim.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtbvhvmijg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.kuanghao11.cn/gtgguljkfs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pycfn.com/gtkxyfmpgf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhiwuduotai.top/gtqxjimaby.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gaohongyu789.top/gtfoghdyzp.html

[E19] 多行文本按行拆分
来源：http://hz.nwbrower.top/gtyjviumcb.html

Py:   s.splitlines()
来源：http://hz.vqdsnc.cn/gtfmcdtoab.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtacoheeyl.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtljfzqaym.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtfsjxppsc.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gtqcmejndj.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gtsnbgfsac.html

Ruby: s.lines
来源：http://hz.nwbrower.top/gtviqnxphx.html

C#:   s.Split('\n')
来源：http://hz.ppjwa.cn/gtfzuvxwbx.html

[E20] 判断字符串是否为空
来源：http://hz.feifeiyinyue.top/gtaixsemqp.html

Py:   if not s:
来源：http://hz.xuetiantiany.cn/gtjqwjxbhz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yuxming.cn/gtvacvkbfq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgufenzy.top/gtxzzpvsfd.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gthxgipkfo.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydzc1.top/gtaabvalqq.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtslxqaace.html

Ruby: if s.empty?
来源：http://hz.aibaodan.cn/gtyrcalavm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.andypj.xyz/gtixlcizhv.html

[E21] 超长截断加省略号
来源：http://hz.hfpthk.cn/gtaimfbmwg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtlzngfyyj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhengqikj.top/gtvwhacjyo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtbhqgehps.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtqalapsxv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtxwkjpelz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cashguo.top/gtqrskqahm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jiagoushi.top/gtkgxkxpwk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258.top/gtjdefltdc.html

[E22] 字节长度与字符长度
来源：http://hz.pengpengdd.cyou/gtmfqminwi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.kuanghao11.cn/gtmrqwsius.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtnijqzekv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtgkpbcmic.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daria6918.cn/gtieprcskb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gtlfwpmbdy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gtezqsalrg.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydjk.org.cn/gtpqigfthm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhongyouzk.top/gttpwfnznn.html

================================================================================
来源：http://hz.xziqi.cn/gtgypgtliy.html

F. 文件与目录
来源：http://hz.zhiwuduotai.top/gtbiwalunm.html

================================================================================
来源：http://hz.haohaochexian.top/gtfsxlusdi.html

[F01] 读取整个文件
来源：http://hz.pycfn.com/gtdeqtvpik.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gtavpxzwsn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtkuiezxbq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnqzz.top/gtqrbmepwn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtiqhbjozr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gthyuorvbs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj20258.top/gttsxjveuj.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtawvwmesx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtktgdisgm.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtxoubgcww.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangdashe.top/gtjkynunnc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hammf.cn/gtgvylklyh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtqnpkxngf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtstoakcav.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtjlvbnhlo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yangfankeji.com/gtpyohrgav.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.aizwys.cn/gtxjvtazwe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtfgnjbbrr.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtftqpwdfc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtfflmquhn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ivvv.top/gtzjidtlia.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtsblofuhk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtefcdjdyi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtjevpxgvf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.feifeiyinyue.top/gtgfjyznoy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtnqetpefb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.smart0.xyz/gthbfdxewt.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtkexsllmj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtmzwrpgcz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.52xcode.cn/gtkzfpwgab.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtlmxrfvxc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gthdsfeghh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cdnleiting.top/gtkprcmmht.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtinqivsfy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtsmplgwwl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sweek.top/gtoecrlyfx.html

[F05] 判断文件或目录是否存在
来源：http://hz.birdmap.top/gtuhiztbav.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gtwpiqlbmy.html

PHP:  file_exists("a.txt");
来源：http://hz.sweek.top/gtkkkowskm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gthdmntffw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gthuzveucc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtvxffpxco.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gtqjimkgbt.html

Ruby: File.exist?("a.txt")
来源：http://hz.bjfxy.top/gtpdwlagqr.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtgngrrott.html

[F06] 删除文件
来源：http://hz.gzhubu.top/gthpmetzhz.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtwvqbgmtg.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtgttvyraj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtmbxbmuft.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtgqtazxtg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtbzokfapf.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtrmnvrxtm.html

Ruby: File.delete("a.txt")
来源：http://hz.zhongyouzk.top/gtosaeqxom.html

C#:   File.Delete("a.txt");
来源：http://hz.gzhubu.top/gtdkvjmsjc.html

[F07] 创建目录（含多级）
来源：http://hz.yongpay.top/gtgaqbbsyc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtptafengg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pycfn.com/gtxmflmakd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtzgcxjmnc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtcbkueozy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gotoacloud.top/gtjowrgjxj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtlavenwff.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenzaomai.com/gtqjgmswhj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtxkpxfkml.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtmllspnss.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gtrwrrxcih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhixingplan.top/gtwfbplgyo.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtkuohzkbs.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtegiabkah.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gticayzvjd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhijiandao.cn/gtpqnjxmer.html

Ruby: Dir.children("dir")
来源：http://hz.guannengcc.top/gtewvhtuhm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tianlin.xyz/gtontncvcm.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gtjccqznjj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhengqikj.top/gteudkwtoq.html

PHP:  filesize("a.txt");
来源：http://hz.mhx1999.top/gtbeqdrrla.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtsukvmcbd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtrjdihynf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtpwbgwhaq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtpwlhfiwe.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gtamwbdisq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtozkwbxls.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxinkj.top/gtbthjrmgl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtammypmlz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtwtionnip.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtnuyxumnh.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258.top/gtkwqctsla.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.bjfxy.top/gtsxbqctxi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtbdcwmfur.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtfedvtadi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gttqrtuasi.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtkjkcmhww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtjowysdjo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aibaodan.cn/gtoxfdmtpd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtxxeyezan.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtlfezafkr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.smart0.xyz/gtqgvgklls.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zdqjudy.top/gtfeafkoap.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtoyxstbdj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gthymhnwtv.html

[F12] CSV 读写
来源：http://hz.aibaodan.cn/gtcviqxpld.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtqytuaize.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gthxnblcal.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtlwqcaklv.html

TS:   // 同上
来源：http://hz.ydjk.org.cn/gtfituzovd.html


<!-- 参考信息 -->