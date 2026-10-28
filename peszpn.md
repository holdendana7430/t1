代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhoulong.xyz/gtstwosbvo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gtslnxarxg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtqdhkaqtq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtenkipkur.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pengpengdd.cyou/gthtcvsald.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtruhodwzn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.316326.xyz/gtsigzwlpz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gtgcalxhde.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtpnxapzev.html

Py:   "ab" * 3
来源：http://hz.xziqi.cn/gtecurivwq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigufen.top/gtpjrpzmzu.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtfanjpmkp.html

TS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gturputasb.html

Java: "ab".repeat(3)
来源：http://hz.daxiang520.top/gtzodeqwsn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.haohaochexian.top/gtrsgoiiso.html

Ruby: "ab" * 3
来源：http://hz.sweek.top/gtqowrzfge.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtljmzicud.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gtkvmyuzxf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xingfuxueyuan.xyz/gtmwltcjsw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtvrmqxgdx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtzjymxqti.html

TS:   s.slice(1, 4)
来源：http://hz.havefunace.top/gtdqaeamgj.html

Java: s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtcnhrjepr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.havefunace.top/gtayzihpdp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtozbkcnzo.html

C#:   s.Substring(1, 3)
来源：http://hz.sysykeji.top/gtldbvkplh.html

[E04] 查找子串位置
来源：http://hz.wangdashe.top/gtlvvggeqe.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtgkatqhwz.html

PHP:  strpos($s, "x");
来源：http://hz.guowangkeji.top/gtvauybenm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinghuilouyu.cn/gtgyubjqft.html

TS:   s.indexOf("x")
来源：http://hz.hywenlv.cn/gtrygyuqhj.html

Java: s.indexOf("x")
来源：http://hz.jinghuilouyu.cn/gtsqyzexyt.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gthocjwjwj.html

Ruby: s.index("x")
来源：http://hz.yuxming.cn/gtyzncqyij.html

C#:   s.IndexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtjzzdmkqe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuanzx.com/gttldjfpxn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.meibo888.top/gtvchznxia.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xinyue.icu/gtzyjsqnei.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gttnqimczd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinqigfzy.top/gtirxrjbrd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtpzmkiirp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jianghu66.top/gtzjstmtsi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tanke756.top/gtkfedvdlt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.feifeiyinyue.top/gtlohhbugd.html

[E06] 替换子串
来源：http://hz.cucudq.cn/gtjutjhuxn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.bjfxy.top/gtdxlynzfo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhijiandao.cn/gtmmwvrsuz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtghcahawl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtkaokxcnf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtzgaydwko.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dianchejie.cn/gthipzfbuo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj202588.top/gtyxlwcdga.html

C#:   s.Replace("a", "b")
来源：http://hz.shzxlz.cn/gtgvumtqag.html

[E07] 按分隔符拆分
来源：http://hz.zhengqikj.top/gtxbyornln.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtrjgxhsdv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtyrbwlzkl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shzxlz.cn/gttafpzuln.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gtlesvfnvt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtomgsenaa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gogol.net.cn/gtvziqzlso.html

Ruby: s.split(",");  s.split
来源：http://hz.zhengqikj.top/gtplzwtkzd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtvvvhdukv.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtjilbqwth.html

Py:   ",".join(items)
来源：http://hz.jqgfzy.top/gtbdezbqmp.html

PHP:  implode(",", $items);
来源：http://hz.zhiwuduotai.top/gtglazjocc.html

JS:   items.join(",")
来源：http://hz.hnxiangtu.top/gtdpnkbqmo.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtjegkmsio.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtgktxjttb.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gtuvcmxcxb.html

Ruby: items.join(",")
来源：http://hz.yangfankeji.com/gtnnrfvrdl.html

C#:   string.Join(",", items)
来源：http://hz.zhijiandao.cn/gtmswqfdgr.html

[E09] 去除所有空白字符
来源：http://hz.zhoulong.xyz/gtlgbrrugz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.fengsongda.top/gttobdtzwa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangshuangyany.cn/gtpvpoyodd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtsqamedkl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xingfuxueyuan.xyz/gtkobfopot.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guowangkeji.top/gtlpekzyqf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cheryme.top/gtwodwkull.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cucudq.cn/gtolbhfyey.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuetiantiany.cn/gtohqaqiyg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.svipenyu.cn/gtklfugkjf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuanzhike.top/gtmerabrou.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxuanxn.top/gtgnsavfey.html

JS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtocqcfpvw.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtcylexsxg.html

Java: String.format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtsngacqix.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtbfcfodfl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtejansmux.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtgvujxhef.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gtlesywdpq.html

Py:   s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtulfcstkk.html

PHP:  strrev($s);
来源：http://hz.jinqigufen.top/gtsyyvyhzo.html

JS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtnqpqzbij.html

TS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gteygumtof.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtnhhpvyed.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cucudq.cn/gtbygypsoj.html

Ruby: s.reverse
来源：http://hz.chenlongwang.top/gtbjaixsky.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtnsyqeazl.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangtech.top/gtvtarmohm.html

Py:   s.count("a")
来源：http://hz.gzhubu.top/gtynwlvonp.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtbafemkvs.html

JS:   s.split("a").length - 1
来源：http://hz.nanxinkj.top/gtzbnogenv.html

TS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtvsuxtmem.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gtfetscltk.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gtveplpsss.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtmfdfcbtq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj202588.top/gtwowcnaki.html

[E13] 逐字符遍历
来源：http://hz.dianchejie.cn/gtealgwlia.html

Py:   for ch in s: print(ch)
来源：http://hz.andypj.xyz/gtgrloxspr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shzxlz.cn/gtynydvffy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtaglflzlx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtjjhcbhmh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtlvtxnhlb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuxming.cn/gtndqeczqk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gtmxigjwns.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sufxvd.cn/gtkwwyieie.html

[E14] URL 编码与 Base64
来源：http://hz.chenzaomai.com/gtlapyzbjt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtycmgwtof.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydzc1.top/gtqezjqosd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fzhhl.top/gtdczlprrw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydjk.org.cn/gtxcipzheq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangshuangyany.cn/gtijkunrxz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pycfn.com/gtuxyuxxsj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangshuangyany.cn/gtkidgjvhk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangdashe.top/gtakwbleuh.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuxming.cn/gthjizfqjt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jianghu66.top/gtfyozxbuz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtzkecgftv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtwdhswsgp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtpeeavrlk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenlongwang.top/gtcsofqsbl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nanxinkj.top/gtdnsksyxf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigufen.top/gtyitkkjof.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zdqjudy.top/gtvkkblqpw.html

[E16] 数字千分位
来源：http://hz.ydzc1.top/gtlgcjebqw.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtdzaalnoc.html

PHP:  number_format(1234567);
来源：http://hz.xuetiantiany.cn/gtywvoersz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtrpfsymay.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtwfoyzrak.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnxiangtu.top/gteqrqikze.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.kuanghao11.cn/gtlnqumxut.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinghuilouyu.cn/gtwwmukzfz.html

C#:   1234567.ToString("N0")
来源：http://hz.ybcxt.top/gtsqjamjfi.html

[E17] 首字母大写
来源：http://hz.yanxiufei.cn/gtpnjedsud.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtreeonvyr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuetiantiany.cn/gtmaajqvla.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.meibo888.top/gtntqcefzi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtdjzqmquw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtpanhhwrl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhiwuduotai.top/gtlnqgxiqh.html

Ruby: s.capitalize
来源：http://hz.tanke756.top/gtvbjneyyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hammf.cn/gtingileln.html

[E18] 模板占位符替换
来源：http://hz.jinghuilouyu.cn/gtjudweypg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hysaishi.cn/gtaulqxutd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sxryk.cn/gtsrryfdhz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gtepismuvu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.meibo888.top/gtrjowvito.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtvcizjtfx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yongpay.top/gtgbvodgpb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgufenzy.top/gtsljxxmsq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangshuangyany.cn/gtgismjebu.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtbaplirou.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtnvibllmu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gtvilyevdn.html

JS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtgvzuijff.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gteeiouwqq.html

Java: s.lines().toList()
来源：http://hz.nanxuanxn.top/gthuxrhxkz.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhaomingkeji.xyz/gtiydhdwrv.html

Ruby: s.lines
来源：http://hz.cdnleiting.top/gtcehmviko.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtmwgxgflz.html

[E20] 判断字符串是否为空
来源：http://hz.feifeiyinyue.top/gtonqfdyts.html

Py:   if not s:
来源：http://hz.gogol.net.cn/gtghillxls.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gtsoepcnls.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtcwevacap.html

TS:   if (s === "") {}
来源：http://hz.chenzaomai.com/gtkyqwzrcx.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydzc1.top/gtoyunodgm.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtswzwobqy.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtnjkczswm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhaomingkeji.xyz/gtxfrovzrm.html

[E21] 超长截断加省略号
来源：http://hz.sweek.top/gtfigywsej.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtiuxtzwbl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtkowuuhfj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtczvlfqip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtzzqffrgl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtfspnvsux.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhijiandao.cn/gtxaeekeig.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtqomfiufg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtpwmtrjoh.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtccityjzi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtamfueach.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtvupehkex.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtinahxwmz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtvxvbznyk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtutnousao.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.smart0.xyz/gtzlcjzrhe.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxuanxn.top/gtzfrzxvpe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenlongwang.top/gtnesuuzyv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqczreyyu.html

F. 文件与目录
来源：http://hz.sysykeji.top/gtmeuxddsk.html

================================================================================
来源：http://hz.iojbl.cn/gtjclscprt.html

[F01] 读取整个文件
来源：http://hz.zhongyouzk.top/gtaveqiwql.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cqqwz.cn/gtonxfuqyv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtpddnjjnp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gtxhbjqmon.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgfzy.top/gttelrcatd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gthdybxokx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tianlin.xyz/gtzvplxtbk.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtrbhsyqep.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtihkfajam.html

[F02] 逐行读取文件
来源：http://hz.fengsongda.top/gthvbcrmni.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gthnktkwhk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtgkrpjlyf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtbgetkuzg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtlnwmkqqj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtvdjvbgha.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yonumen.top/gtrmfeaipa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gturmrvzqf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gtqedxvtdj.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtlkukfhmh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ywan-chungtsiang.top/gtmlrxrkzv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.andypj.xyz/gtztguzisk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtlqwzcoej.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtftfwfoir.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cashguo.top/gtirukqsge.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtnabsrnsd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.52xcode.cn/gtpvepmjfk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtfgwvghve.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtsrnoebba.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shangyingyoupin.top/gtjzkbaxco.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtdlkfinex.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtdshnuzhd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtbzadwwpa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yonumen.top/gtiodeatbi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgfzy.top/gtqskkbyeq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtflohcxof.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.meibo888.top/gtintwqkmu.html

[F05] 判断文件或目录是否存在
来源：http://hz.jlsjyb.cn/gtpfdpvtrd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtrwbzblxb.html

PHP:  file_exists("a.txt");
来源：http://hz.cashguo.top/gtwgrctaip.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gthzvgkmoq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gtkcssgoxn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtdlblsnvm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ppjwa.cn/gtzcmosmpz.html

Ruby: File.exist?("a.txt")
来源：http://hz.nwbrower.top/gtmsabbmem.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtstoxzsqr.html

[F06] 删除文件
来源：http://hz.pengpengdd.cyou/gtugpumgti.html

Py:   os.remove("a.txt")
来源：http://hz.tianlin.xyz/gtpyzgsmtf.html

PHP:  unlink("a.txt");
来源：http://hz.redwolf501.top/gtzjnziqbe.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gttyqgnbfz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtjhxwewmf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtounzksgo.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtepjxpbqp.html

Ruby: File.delete("a.txt")
来源：http://hz.ybcxt.top/gttcmxqyvf.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtzupsdrur.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtubecvrrz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtfrezstyi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gzhubu.top/gtubtxwoyo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtbjifayss.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtshdkpuxg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sysykeji.top/gtzoqtigvr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gtpbbcwjmk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtmdpnnbjn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtofenfhic.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtmqmlesln.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtrbwvajsf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtsvwbjpxt.html

JS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtugvbobdq.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtsuguvadn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtuzmhfrxo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtudtinaho.html

Ruby: Dir.children("dir")
来源：http://hz.shuidangran.top/gtehbyrvrb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hongshengwenyu.top/gtwwchwyug.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gtomnvjntw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.pengpengdd.cyou/gtacgyvkpa.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtxicsbwmf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gthedbisea.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtouuptpti.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtscyrjqje.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.quarkkingdee.top/gtowgdzemk.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtdohueiwv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuxming.cn/gthewyacgv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtpveytbqc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtrztvuqef.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.52xcode.cn/gtlspplcpo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtpeisryfd.html

TS:   path.extname("a.txt")
来源：http://hz.xinyue.icu/gtqvalxnfs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuxming.cn/gtrbebunjv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gttemifkcm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gthmnvilah.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aibaodan.cn/gtbzhzgosh.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtjtajexvm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtzbjalshy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtxelexjhh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtrohgyjrh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtumzgzvtp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sweek.top/gteeemxbyf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zycfv.cn/gtukypisfb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtobasbrle.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangkeji.top/gtsxshmvii.html

[F12] CSV 读写
来源：http://hz.yvedp.cn/gtcoqgyelg.html


<!-- 参考信息 -->