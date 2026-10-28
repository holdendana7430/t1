代发 wailian999

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtnrjhzmvf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuanzx.com/gtdqbnuctv.html

Ruby: arr.join(", ")
来源：http://hz.andypj.xyz/gtrvwmxdzs.html

C#:   string.Join(", ", list)
来源：http://hz.ivvv.top/gtwowcycuu.html

================================================================================
来源：http://hz.svipenyu.cn/gtbsgxswib.html

E. 字符串处理
来源：http://hz.yvedp.cn/gtqwdujcav.html

================================================================================
来源：http://hz.ybcxt.top/gtkxtsfiha.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtofpovked.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tianlin.xyz/gtpqeoeltd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtnzqyhtxp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtshrcniep.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtcsjxsepz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtymqpeukw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangshuangyany.cn/gtzxukzfej.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sufxvd.cn/gtbeqjence.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.kuanghao11.cn/gtokvcwbga.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtzsjctwug.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtdeumqivh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhixingplan.top/gtqhntdmbz.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtbcpuqegp.html

TS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtchqlapws.html

Java: "ab".repeat(3)
来源：http://hz.gzhubu.top/gtnhrszmbv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gttfpoplxa.html

Ruby: "ab" * 3
来源：http://hz.wangshuangyany.cn/gtiytcskca.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangshuangyany.cn/gtxgyzlwgn.html

[E03] 截取子串
来源：http://hz.guowangkeji.top/gtkepvbpuc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gttrpdicxc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtpugtlfvg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtvmgmswys.html

TS:   s.slice(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtsykyhrgx.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtyerunnvk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinqigufen.top/gthauwsrfx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.smart0.xyz/gtttacxntt.html

C#:   s.Substring(1, 3)
来源：http://hz.cheryme.top/gtsovditup.html

[E04] 查找子串位置
来源：http://hz.bjfxy.top/gtdgrmfhlt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tianlin.xyz/gtyvuittrf.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gtsckcflqq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jyoumei.cn/gtwmdqktwc.html

TS:   s.indexOf("x")
来源：http://hz.52xcode.cn/gtvqyatpwn.html

Java: s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtgiydyxoi.html

Go:   strings.Index(s, "x")
来源：http://hz.mhx1999.top/gtijlsumtt.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtxfxyjgra.html

C#:   s.IndexOf("x")
来源：http://hz.xuetiantiany.cn/gtabglzrbl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtziutskzg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.svipenyu.cn/gtadjcjodr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.andypj.xyz/gtgbbigykw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ywan-chungtsiang.top/gteelfiusi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydzc1.top/gtoahbeayr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gthmsupdak.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhaomingkeji.xyz/gtnjuxccaw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj202588.top/gtjmvslcua.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ybcxt.top/gtmsmyhzvf.html

[E06] 替换子串
来源：http://hz.yuanzhike.top/gtsbooarji.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shanyushiyangkeji.top/gtxmfkshqe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtlgnxwgfw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtcjbzneur.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtwlisqesi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtvfcazeul.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.snrcjt.cn/gtkluvzmtz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.birdmap.top/gtmotliijy.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtxklnkcqp.html

[E07] 按分隔符拆分
来源：http://hz.iojbl.cn/gtflgeyein.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtrkdrgzcq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhoulong.xyz/gtqgrswroo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tanke756.top/gtrnxxriah.html

TS:   s.split(",")
来源：http://hz.nwbrower.top/gtqeiawodl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hysaishi.cn/gtmrkyrero.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuxming.cn/gtqlgvclzl.html

Ruby: s.split(",");  s.split
来源：http://hz.kuanghao11.cn/gtulfgagid.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.vqdsnc.cn/gtolndoiti.html

[E08] 数组按分隔符合并
来源：http://hz.wangshuangyany.cn/gtkqvpunvk.html

Py:   ",".join(items)
来源：http://hz.nwbrower.top/gtskwkbquc.html

PHP:  implode(",", $items);
来源：http://hz.xziqi.cn/gtadxyvuee.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtrirliwfr.html

TS:   items.join(",")
来源：http://hz.jinqigufen.top/gthywvondb.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtceahziqt.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigufen.top/gtiherspml.html

Ruby: items.join(",")
来源：http://hz.quarkkingdee.top/gtnefaotll.html

C#:   string.Join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtkhavfjml.html

[E09] 去除所有空白字符
来源：http://hz.fengsongda.top/gtnbafretk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuxming.cn/gtoequjfmg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.mhx1999.top/gtcabguclm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gogol.net.cn/gtisqduooo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtukamanbf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tian-w.cn/gtqyoznxxp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ybcxt.top/gtqswewxim.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtouzidyhw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gtnmxllcqs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtuqepstkl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtjtkxcmbu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xziqi.cn/gtjnscqcgm.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtkaulmrng.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtobyxeamh.html

Java: String.format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtfxotojsf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtjedyejua.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtsvxrebax.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cheryme.top/gtnvptjvwg.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gtpyswogbt.html

Py:   s[::-1]
来源：http://hz.jinyuanbaomall.cn/gtihmpdgtk.html

PHP:  strrev($s);
来源：http://hz.meibo888.top/gtrecaglvv.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtpgvzjapo.html

TS:   [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtyyqeaohf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nwbrower.top/gtgxjqerrb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gtdfiooldo.html

Ruby: s.reverse
来源：http://hz.gogol.net.cn/gtwqbklplp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtyywpheha.html

[E12] 统计某字符出现次数
来源：http://hz.svipenyu.cn/gtrrirjuly.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gtwgtqccjn.html

PHP:  substr_count($s, "a");
来源：http://hz.yj20258888.top/gtcarojjrl.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtszoklvvj.html

TS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtpgbxlkwt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gzhubu.top/gtnlfspmoa.html

Go:   strings.Count(s, "a")
来源：http://hz.haohaochexian.top/gtrndyxedq.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtvtmgkegd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jyoumei.cn/gtlzlpndst.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtcitvwipi.html

Py:   for ch in s: print(ch)
来源：http://hz.zhengqikj.top/gtveyjmpqu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtciwqbunn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtbvjjfbql.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtsxzhmikz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cashguo.top/gtzspydsap.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhiwuduotai.top/gtgypvgmgc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhengqikj.top/gtyqgzeqaz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yongpay.top/gtcvrjunuq.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gtxwjmiaua.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gtziuptlca.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zycfv.cn/gttokfsxgk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gtwjvgqmxq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gttffwcvwr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.andypj.xyz/gtceoknmbz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.316326.xyz/gtyeqtrfdj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtbtxzyqpv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.meibo888.top/gtsfsoidab.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtmbumzqlt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ywan-chungtsiang.top/gtvfjrojon.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sxryk.cn/gtlzujpsjl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.redwolf501.top/gtznoegjod.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtwtpnrjtf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhoulong.xyz/gtifhfhfqg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenjidiqi.icu/gtlgesfbfa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yanxiufei.cn/gtthugzmyd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnqzz.top/gtpsapecwp.html

[E16] 数字千分位
来源：http://hz.yonumen.top/gtyxkxmwcu.html

Py:   f"{1234567:,}"
来源：http://hz.sufxvd.cn/gttojvpffz.html

PHP:  number_format(1234567);
来源：http://hz.pycfn.com/gtrhdbwocj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtfmsnbjdk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtqgsrvoxh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhaomingkeji.xyz/gtztphjtgr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtjfajwqqp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuxming.cn/gtoxcyqfdt.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gtobikuggh.html

[E17] 首字母大写
来源：http://hz.yonumen.top/gtvtxlafva.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ywan-chungtsiang.top/gtlzctmthg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtbtqhramr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gttgjnwtkl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtparllhfh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.smart0.xyz/gtkjbnvofz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gzhubu.top/gtjxvkxtbb.html

Ruby: s.capitalize
来源：http://hz.jinghuilouyu.cn/gtaozzzdzb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhoulong.xyz/gtcwlaxswf.html

[E18] 模板占位符替换
来源：http://hz.zhaomingkeji.xyz/gtqbybpyht.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.pengpengdd.cyou/gtqgpfnawx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenlongwang.top/gtcjqgupkr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtnuweqnaj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtmoqoydia.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ehwqpu.com/gtchhpclko.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258.top/gtzaisafso.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtcioslest.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhixingplan.top/gtvgmmgoce.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtcwsurflp.html

Py:   s.splitlines()
来源：http://hz.aibaodan.cn/gtsarudppz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuetiantiany.cn/gtplehqmqm.html

JS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtprtvleen.html

TS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtjtqdpcch.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gthlmlpcev.html

Go:   strings.Split(s, "\n")
来源：http://hz.shzxlz.cn/gtdzgbjnfw.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtuixbjdst.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gttdgxbydv.html

[E20] 判断字符串是否为空
来源：http://hz.haohaochexian.top/gthjpnxiak.html

Py:   if not s:
来源：http://hz.birdmap.top/gtgrhxnaku.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtrfblkilj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yanxiufei.cn/gtgzfokeum.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtvzssaodr.html

Java: if (s.isEmpty()) {}
来源：http://hz.316326.xyz/gtagfdnjye.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gteylswdha.html

Ruby: if s.empty?
来源：http://hz.yanxiufei.cn/gtmydrgtgy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shangyingyoupin.top/gtuzsajfvs.html

[E21] 超长截断加省略号
来源：http://hz.quarkkingdee.top/gtphoownmb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sxryk.cn/gtkkebbibz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ybcxt.top/gtfidxfpuk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtxavqtlgx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtmatqngrf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtfrczvley.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtfgpqceen.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtkiwuwpkk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhoulong.xyz/gtjwzrbstx.html

[E22] 字节长度与字符长度
来源：http://hz.jiagoushi.top/gtqzcvqljn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtdbmrjjtn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zycfv.cn/gtflpioqnx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtqdymodes.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtyyutlcdn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nwbrower.top/gtdtmtmyur.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gtwujksyvf.html

Ruby: s.bytesize;  s.length
来源：http://hz.daria6918.cn/gtawawdykk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtjbjkybky.html

================================================================================
来源：http://hz.yuxming.cn/gthkwozvki.html

F. 文件与目录
来源：http://hz.cdnleiting.top/gtqpejppqo.html

================================================================================
来源：http://hz.cqqwz.cn/gtkbxoyxyx.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtkrgbbfys.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jyoumei.cn/gtpiyvpema.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shuidangran.top/gtzcbudokg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangkeji.top/gtpajieebn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xziqi.cn/gthbpufkhf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtmufvtbfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.kuanghao11.cn/gttpdyriwl.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtspptnjhn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dashuyun.cn/gtliabyllz.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtizrziine.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj202588.top/gtxqfidfit.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.kuanghao11.cn/gtjxiwnltq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtxsnedjma.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhixingplan.top/gthqxsydym.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtyyvgzeqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hywenlv.cn/gtxfpkxfqo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtjpnkeljn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fengsongda.top/gtncjwbela.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtuaemdiny.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gtteprxrpb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtmryveytb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtrtjypjrp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtozibsgbx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtgffgtuxc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenjidiqi.icu/gtihxwrgve.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtwkvxkwfo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtghpxogim.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtttvokkni.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtdwvfbrgi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cheryme.top/gtxnovndaj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtjosupkap.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtyglajarb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guowangkeji.top/gtmrejzoam.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigfzy.top/gtyvblhctm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnxiangtu.top/gtinhhrwqh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.havefunace.top/gtmlmolpsi.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxuanxn.top/gtjpbgdorh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtuceungim.html

PHP:  file_exists("a.txt");
来源：http://hz.nwbrower.top/gtdzciuxxf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtjuuferbz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtrfcotxsp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtxeiclirz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhixingplan.top/gtxpjjchjr.html

Ruby: File.exist?("a.txt")
来源：http://hz.9152youxi.cn/gttluojffd.html

C#:   File.Exists("a.txt")
来源：http://hz.xuetiantiany.cn/gthukjlsin.html

[F06] 删除文件
来源：http://hz.yvedp.cn/gtbmjgtoig.html

Py:   os.remove("a.txt")
来源：http://hz.jlsjyb.cn/gtkylkvznq.html

PHP:  unlink("a.txt");
来源：http://hz.9152youxi.cn/gtecouljnu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtsacipqkc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtuewlwifj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gthssgrfff.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtvcgalprt.html

Ruby: File.delete("a.txt")
来源：http://hz.zhoulong.xyz/gtqqhzxnkl.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtravstmno.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gttoxctfyp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtegrljfyl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtabeumjua.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtmfzwnhyy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtgjhawgba.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangtech.top/gtibecewof.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuanzx.com/gtsoytrqrz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hongshengwenyu.top/gtcdwzcntf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shangyingyoupin.top/gtdmmaeqke.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtohjbagfc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtwzyccuqd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gtdhhyjoop.html

JS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtsojbcfgs.html

TS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtgayzieoz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtuyzqapva.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.9152youxi.cn/gtxsscpyml.html

Ruby: Dir.children("dir")
来源：http://hz.havefunace.top/gtxtutuovf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pengpengdd.cyou/gttiwhpnjk.html

[F09] 获取文件大小
来源：http://hz.yuanzhike.top/gtzoeuzdgf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtzdpdrgja.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtokdrhkhj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hammf.cn/gtryagavda.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtmdhkkxfe.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtxuyyzwmf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.redwolf501.top/gtvztucuvn.html

Ruby: File.size("a.txt")
来源：http://hz.snrcjt.cn/gtcplskedb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.meibo888.top/gtbhqczvru.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tanke756.top/gtyptpxcdb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtykdofrto.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtzhujgrax.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtviqbivkb.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gtgkuhurpx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258.top/gtotrrgbgi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuanzx.com/gtsvrcehsi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtuvtntfwp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gtszjzafib.html

[F11] 复制与移动文件
来源：http://hz.nanxuanxn.top/gtqvgcnema.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtpdefbykx.html


<!-- 参考信息 -->