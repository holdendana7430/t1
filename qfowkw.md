代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hammf.cn/gtsexnxhks.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtwmhzfafm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yanxiufei.cn/gtjgglswfa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jlsjyb.cn/gtjwazzqin.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtfsiapqxc.html

Py:   "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtncbdlfzm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtlveymyvx.html

JS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtsdjmxegy.html

TS:   "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtysnclqzh.html

Java: "ab".repeat(3)
来源：http://hz.yj202588.top/gtrlqpuuhf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtzhfqtmsz.html

Ruby: "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtwmlthvoo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hammf.cn/gtqxeddnpn.html

[E03] 截取子串
来源：http://hz.zhixingplan.top/gtfcvmdbzg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtwcleizqu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.svipenyu.cn/gtrahjokqo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.meibo888.top/gtqqxrgvzc.html

TS:   s.slice(1, 4)
来源：http://hz.yuxming.cn/gtrvpfsspv.html

Java: s.substring(1, 4)
来源：http://hz.ivvv.top/gtapddtqne.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhiwuduotai.top/gtdhebuuzi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtwshtalwf.html

C#:   s.Substring(1, 3)
来源：http://hz.redwolf501.top/gtqydyrxhv.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gtgioylxrc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtgllxcwdm.html

PHP:  strpos($s, "x");
来源：http://hz.ivvv.top/gtanjieobr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.0kj1m.cn/gtrvqvdpji.html

TS:   s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtcuzhzref.html

Java: s.indexOf("x")
来源：http://hz.dianchejie.cn/gtavempukb.html

Go:   strings.Index(s, "x")
来源：http://hz.tian-w.cn/gtibsimwrr.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtjnzjpwip.html

C#:   s.IndexOf("x")
来源：http://hz.kuanghao11.cn/gthmidfamo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tian-w.cn/gtbgfosqhk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenlongwang.top/gthgkfbjdl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ywan-chungtsiang.top/gtrjdhryuc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtvyulagzh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.svipenyu.cn/gtlfyzuphu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtvjkhurmf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtsrvoaalj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtrzfknhsm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pycfn.com/gtaxfmcpno.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtoajmrgii.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tian-w.cn/gtzzourhrq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtwqaulpfn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtrhyngkpr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtpiifkytk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gteagumkak.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydzc1.top/gtywlrcxeo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhixingplan.top/gtprygxtss.html

C#:   s.Replace("a", "b")
来源：http://hz.ppjwa.cn/gtftowknqi.html

[E07] 按分隔符拆分
来源：http://hz.cheryme.top/gtievqbzvu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhaomingkeji.xyz/gtjeaakpnb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cashguo.top/gthrlleply.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtmraayhnk.html

TS:   s.split(",")
来源：http://hz.sweek.top/gtkxcotzpv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yueranfly.top/gtaswskzdx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daria6918.cn/gtlycombwx.html

Ruby: s.split(",");  s.split
来源：http://hz.haohaochexian.top/gtogtbzxcn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhixingplan.top/gtvrgggxcx.html

[E08] 数组按分隔符合并
来源：http://hz.sxryk.cn/gtvpxvqglm.html

Py:   ",".join(items)
来源：http://hz.gaohongyu789.top/gtakxxmeoz.html

PHP:  implode(",", $items);
来源：http://hz.haohaochexian.top/gtztyzpszh.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtgmsekvqo.html

TS:   items.join(",")
来源：http://hz.hnxiangtu.top/gtzfsoxrie.html

Java: String.join(",", items)
来源：http://hz.fengsongda.top/gtledtfkqq.html

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtdscuntiu.html

Ruby: items.join(",")
来源：http://hz.xinyue.icu/gttsnisuup.html

C#:   string.Join(",", items)
来源：http://hz.snrcjt.cn/gtskdsmoyx.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtrekdubml.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuanzx.com/gtngowvvjp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yongpay.top/gtqgtoladb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtokuokqlo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtoxlhtjig.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtgrmmhzna.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.redwolf501.top/gtkguccgcd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenlongwang.top/gtacgcndww.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jiagoushi.top/gtovjlwmpd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtjvqzzftq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.kuanghao11.cn/gtralbfxzo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pengpengdd.cyou/gtcsbmyefp.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtqwuhulwj.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtlhefdgpr.html

Java: String.format("%03d", 7)
来源：http://hz.hysaishi.cn/gthozjjcyo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sxryk.cn/gtaljehdqp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zycfv.cn/gtpqzbdvyi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gtzkhymbdb.html

[E11] 反转字符串
来源：http://hz.yuanzhike.top/gtznmmwggq.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gtmdgpxzjm.html

PHP:  strrev($s);
来源：http://hz.chenlongwang.top/gtmhfwkbdf.html

JS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtjrhgwyth.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtyrlmpona.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jlsjyb.cn/gthjdgartq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtxncpdmbn.html

Ruby: s.reverse
来源：http://hz.yuanzhike.top/gttnmoliik.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtnbtktusy.html

[E12] 统计某字符出现次数
来源：http://hz.chenjidiqi.icu/gtswniezug.html

Py:   s.count("a")
来源：http://hz.hnqzz.top/gthqeejsql.html

PHP:  substr_count($s, "a");
来源：http://hz.yangfankeji.com/gtecbwwicu.html

JS:   s.split("a").length - 1
来源：http://hz.vqdsnc.cn/gtwuvignnn.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtoizqcqwz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj20258.top/gtsufujizn.html

Go:   strings.Count(s, "a")
来源：http://hz.havefunace.top/gtdvlfkrfu.html

Ruby: s.count("a")
来源：http://hz.sweek.top/gtioyqulkg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtlxzqtrmj.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtwhwsuure.html

Py:   for ch in s: print(ch)
来源：http://hz.meibo888.top/gtnhpiwgow.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gtzpohdill.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtnipdcefi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtztjbavwn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtpbffvtew.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gttpduceab.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenzaomai.com/gtqepodcha.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtfvqrbprc.html

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gtapkjkaqq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtkwmipzvg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangtech.top/gtgcydgzxh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jyoumei.cn/gtgujtbwfo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gtlxoclpbv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yongpay.top/gtywinqrxs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cheryme.top/gtjrmedqus.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.pycfn.com/gtzpvygfev.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtvocuahxd.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtpbodaefq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtlmbbojlr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tanke756.top/gthvixavje.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.andypj.xyz/gtlgyyyzlf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuetiantiany.cn/gtsfetphvv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gtnksjyoen.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gtrxkafdja.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangkeji.top/gthvgikbba.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydjk.org.cn/gtkxudxbhf.html

[E16] 数字千分位
来源：http://hz.shuidangran.top/gtotsaqgiv.html

Py:   f"{1234567:,}"
来源：http://hz.yueranfly.top/gtmpadvzmg.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtmnriqcww.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gthvyxzisk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtbtnurypx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgufenzy.top/gtcgmtjtai.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenjidiqi.icu/gtrqiehief.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gtaxxnaqwi.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtcwlmexfd.html

[E17] 首字母大写
来源：http://hz.yuxming.cn/gtvdjphpzv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gotoacloud.top/gtwyczwdxn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sxryk.cn/gtiokblsni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gttfnytwbl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtfxdwausd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nanxuanxn.top/gtusveoewr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.snrcjt.cn/gtozkfwxsr.html

Ruby: s.capitalize
来源：http://hz.sufxvd.cn/gtggezmren.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtscdcxaje.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtyewsvkar.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.birdmap.top/gtglzligxx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.havefunace.top/gtoeejtczj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtwexjgszz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtttfvvbwn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenlongwang.top/gtakmrxibw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gtnhrqvkxz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jlsjyb.cn/gtuiqyqiob.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hysaishi.cn/gtncbfzdxt.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtykrrpknt.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtyvuwsijj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gotoacloud.top/gtumaxgosm.html

JS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtaycdusjr.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtqgxmpoib.html

Java: s.lines().toList()
来源：http://hz.52xcode.cn/gtokkuotfz.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtouyhlmuz.html

Ruby: s.lines
来源：http://hz.yj20258888.top/gthevhiikp.html

C#:   s.Split('\n')
来源：http://hz.pengpengdd.cyou/gtwrnfchfr.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258.top/gttdxpdpdb.html

Py:   if not s:
来源：http://hz.sysykeji.top/gtaqmdbtai.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yongpay.top/gtdmaynrqs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtqucdmtxc.html

TS:   if (s === "") {}
来源：http://hz.haohaochexian.top/gthtgsiywl.html

Java: if (s.isEmpty()) {}
来源：http://hz.hammf.cn/gtzthvbwkh.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gttrhkkkcn.html

Ruby: if s.empty?
来源：http://hz.pengpengdd.cyou/gtnuhrmxrk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.9152youxi.cn/gtzbdibnor.html

[E21] 超长截断加省略号
来源：http://hz.sxryk.cn/gtcaixwndj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.daxiang520.top/gtgctdqyah.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gtztyqiaul.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtocgruyli.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtrqsccbkk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtyfwcxonw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinyuanbaomall.cn/gtripcwxjq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nwbrower.top/gtltdzzolo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.haohaochexian.top/gtbiayteum.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtaygafnsf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gtkcbjskud.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtnkixdqzp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtfldenxvl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gthrnghylu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zycfv.cn/gtlpymzont.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.feifeiyinyue.top/gtemckznkt.html

Ruby: s.bytesize;  s.length
来源：http://hz.feifeiyinyue.top/gtcrrlsxlj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtkwgedheh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsqhwqcbw.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtdymyhmdc.html

================================================================================
来源：http://hz.smart0.xyz/gtjlknvqtv.html

[F01] 读取整个文件
来源：http://hz.cheryme.top/gtmqapjtuc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.kuanghao11.cn/gtwpdxcxua.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtilnvgdjx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gtjvwpwyhv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtnmtvabxy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtueerwwgm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtngxwbbiz.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtbkyihdie.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangtech.top/gtudqlentp.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtfvmgdqod.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gogol.net.cn/gtowgodqdk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtqdgsgfum.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.mhx1999.top/gtnzmtprsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtoawidqwx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtjyarctqk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuanzhike.top/gtxsopshxj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtxkgcxvvm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtgxaegtuh.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtsglyenfl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gtybsmgzja.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtvlbawkqh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtdmrokzru.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtgdajmini.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtlfxvqbko.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aizwys.cn/gtlzgrqijf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hysaishi.cn/gtcuakodto.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gtqxocjeat.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtkspjsdoz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtkqzfqcqa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sweek.top/gtvifffgil.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtyurttmeu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtbvvkuavk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gthcfzumgj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sweek.top/gtbeuuazsi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gtenvibprf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.vqdsnc.cn/gttzvmjwfn.html

[F05] 判断文件或目录是否存在
来源：http://hz.52xcode.cn/gtbthbnuln.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtrsajewyo.html

PHP:  file_exists("a.txt");
来源：http://hz.yuanzhike.top/gtzpvtopsw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtjgkvyrdc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtmqwgkjtg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtqxftacex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtynhoxsfs.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtcjberlcp.html

C#:   File.Exists("a.txt")
来源：http://hz.daria6918.cn/gtcpmpokex.html

[F06] 删除文件
来源：http://hz.xinyue.icu/gtvlnbtire.html

Py:   os.remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtxjycjmra.html

PHP:  unlink("a.txt");
来源：http://hz.aibaodan.cn/gteyakfubn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtdcnumrxm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtalxjdyha.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gteycyilwj.html

Go:   os.Remove("a.txt")
来源：http://hz.kuanghao11.cn/gtwuqqgtio.html

Ruby: File.delete("a.txt")
来源：http://hz.cucudq.cn/gtixkfjfya.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtfcmabuzi.html

[F07] 创建目录（含多级）
来源：http://hz.316326.xyz/gtcvbaldrc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jiagoushi.top/gthxfxbvka.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtmivojsiv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gtnxvblyhw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtjrfjggpg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxuanxn.top/gtgwkivdpb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gtdzpqfsnx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtigmetzxh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gtrgsxhnme.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gtgjbbbozw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hongshengwenyu.top/gthebbhtch.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtcixjidzm.html

JS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtjmtnbpvo.html

TS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtoetxeimf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtzbjzgodl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtvxkcjwkc.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigfzy.top/gtrldvrsyx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtadcaqcuk.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtequhquhj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtxshploky.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gturullesl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.feifeiyinyue.top/gtomkotdld.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtdzhydmke.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtkiawtdfm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gtdbibxrvy.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtcxjvjmsm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtdwfxxpbz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gtxlqwzrkc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtekkvldjg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gzhubu.top/gtzfisuati.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtreyexwbg.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gtrsrphhgs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuanzx.com/gtpvuatwjj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtmaxbjqoa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtkbprnstp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtqgfxxyfu.html

[F11] 复制与移动文件
来源：http://hz.c1oappe.top/gtwtdwmdvq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gthrazkari.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhaomingkeji.xyz/gtfbhomvwu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtgucjvgkt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtqsqydvkm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtmgpgtnom.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtaiwmgphn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtvipbgtrg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgufenzy.top/gtmsotglee.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gtskkdngho.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtqrowmolk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.mhx1999.top/gtzryaiukc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ppjwa.cn/gtbkyitafh.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtytqyqxsk.html


<!-- 参考信息 -->