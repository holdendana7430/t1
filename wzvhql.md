代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtpedirszp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenjidiqi.icu/gtoiwtehgx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gthrdgmsal.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtlqdfhunu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yvedp.cn/gtadquwqsr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinghuilouyu.cn/gtpefhmvyh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuanzhike.top/gtwnydgewd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.andypj.xyz/gtallzyrsk.html

[E02] 重复字符串
来源：http://hz.guannengcc.top/gtzhwgtthu.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtfwsparjm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shuidangran.top/gtrkrqukbk.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258888.top/gtizxkfufl.html

TS:   "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtzhplnsog.html

Java: "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtyzpvteqp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtvkmxzxjz.html

Ruby: "ab" * 3
来源：http://hz.cashguo.top/gtmawhaekz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cheryme.top/gtlordshmh.html

[E03] 截取子串
来源：http://hz.chenzaomai.com/gtlgwkdiqj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hfpthk.cn/gtzytzuihy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yonumen.top/gtsipwuwvt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sysykeji.top/gtdaclauzq.html

TS:   s.slice(1, 4)
来源：http://hz.ehwqpu.com/gtepcalehy.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtmyhnbwux.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xinyue.icu/gtonkuqgmo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtntnlctwa.html

C#:   s.Substring(1, 3)
来源：http://hz.bjfxy.top/gtvbvuowkp.html

[E04] 查找子串位置
来源：http://hz.nanxuanxn.top/gtrotxuyrm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gaohongyu789.top/gtqjvxzqks.html

PHP:  strpos($s, "x");
来源：http://hz.sufxvd.cn/gteiuasxfe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.haohaochexian.top/gttmsyisik.html

TS:   s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtwdegjnwn.html

Java: s.indexOf("x")
来源：http://hz.cucudq.cn/gtqhpderly.html

Go:   strings.Index(s, "x")
来源：http://hz.bjfxy.top/gttuumxgwk.html

Ruby: s.index("x")
来源：http://hz.chenjidiqi.icu/gttbwdfvdn.html

C#:   s.IndexOf("x")
来源：http://hz.nwbrower.top/gtuvqqegfv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daria6918.cn/gtsvttcgin.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daria6918.cn/gtmbtlqdji.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gtcpehceza.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhongyouzk.top/gtyimdjune.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gtskvooqus.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtsalfidhg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenjidiqi.icu/gtulkpzqfr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtfhvwdtfe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtzyznfedw.html

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtzpuyitoi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cashguo.top/gtvhjapfar.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.quarkkingdee.top/gtfujsmvch.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtjrkxrinn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtctkdajgo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtddtldgtf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.bjfxy.top/gtknmlyycm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shuidangran.top/gtvnvryxcz.html

C#:   s.Replace("a", "b")
来源：http://hz.ybcxt.top/gtvxvypxmv.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtqvsxrhoh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hfpthk.cn/gtafwuipug.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtbfejinbo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gtdrcekehu.html

TS:   s.split(",")
来源：http://hz.aizwys.cn/gtjntbcxez.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxinkj.top/gtssqskahs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtadkfwwdo.html

Ruby: s.split(",");  s.split
来源：http://hz.meibo888.top/gtaiqkglou.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinqigfzy.top/gtjlwianlj.html

[E08] 数组按分隔符合并
来源：http://hz.jinyuanbaomall.cn/gtxnflhqrz.html

Py:   ",".join(items)
来源：http://hz.zhaomingkeji.xyz/gtzjpavvrw.html

PHP:  implode(",", $items);
来源：http://hz.yj202588.top/gtcutxbuot.html

JS:   items.join(",")
来源：http://hz.gaohongyu789.top/gtrpntcrwk.html

TS:   items.join(",")
来源：http://hz.dianchejie.cn/gtfmkchncg.html

Java: String.join(",", items)
来源：http://hz.gzhubu.top/gtmsvpitum.html

Go:   strings.Join(items, ",")
来源：http://hz.meibo888.top/gtermkzury.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtsmdisysu.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtkfiwsjzp.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtgovmusse.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gtewelteez.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhaomingkeji.xyz/gtknzndjyn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtwhzzkwvg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtnnopcgvy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtocpffhgw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhoulong.xyz/gtyzasppur.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gtvatxojvb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gtcatoumgj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cucudq.cn/gtifmtkqoh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gteeocsrle.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ywan-chungtsiang.top/gtrnthzgzs.html

JS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtavqnbxjy.html

TS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gthlmswuui.html

Java: String.format("%03d", 7)
来源：http://hz.zhoulong.xyz/gtpfqzjmhj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.havefunace.top/gtxuwilcqd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gtljcnxzho.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinghuilouyu.cn/gtpmfatlsd.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtivpyyeps.html

Py:   s[::-1]
来源：http://hz.hfpthk.cn/gtkrihlzfy.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtmrblwhpw.html

JS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtpxeptuta.html

TS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtmtudhdgw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tianlin.xyz/gtowabppjt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.316326.xyz/gtrlnbycpp.html

Ruby: s.reverse
来源：http://hz.fzhhl.top/gtvvdvvlmj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtwmwriflu.html

[E12] 统计某字符出现次数
来源：http://hz.yonumen.top/gtcvzbilzp.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtqbfoitto.html

PHP:  substr_count($s, "a");
来源：http://hz.vqdsnc.cn/gtgujcnngb.html

JS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtejppvatq.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtcjcpvvds.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jiagoushi.top/gtorshsofb.html

Go:   strings.Count(s, "a")
来源：http://hz.quarkkingdee.top/gtpjqtifhn.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtkktijfll.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gtagfnizhv.html

[E13] 逐字符遍历
来源：http://hz.yonumen.top/gtnpqsuomr.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtqsfuvuqn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yonumen.top/gtrtginpdb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gtohlpmjhs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtllixpugs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xziqi.cn/gtcfaibbtb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtoboglovb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinghuilouyu.cn/gtjdwlwumn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigfzy.top/gtbecxrknm.html

[E14] URL 编码与 Base64
来源：http://hz.zhixingplan.top/gtdgspqkeb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.kuanghao11.cn/gtrbwopehg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhengqikj.top/gtaexjxmwi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hammf.cn/gtokahkdan.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gtlrvgirpv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtsitmaycx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jiagoushi.top/gtltzuzyzt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj202588.top/gtngoeaoew.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuanzhike.top/gtoyrzyldd.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenjidiqi.icu/gtjjgjspll.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtsmzuakgu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtmoofutqm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ivvv.top/gtcricnccy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtoucudqsz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cheryme.top/gtqhijfzoz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.meibo888.top/gtucchewml.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigfzy.top/gtolxugftl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hysaishi.cn/gtornsvhiw.html

[E16] 数字千分位
来源：http://hz.0kj1m.cn/gtusbrufzl.html

Py:   f"{1234567:,}"
来源：http://hz.shzxlz.cn/gtkhrlaeog.html

PHP:  number_format(1234567);
来源：http://hz.xylfe.cn/gtgryfgsag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtzukkjvjc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtduoblrhp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pycfn.com/gtbtfwsaqh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.haohaochexian.top/gtyvpnacmk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhongyouzk.top/gtjdccvmfi.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtbtkduzyy.html

[E17] 首字母大写
来源：http://hz.hammf.cn/gtjannhhpa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tianlin.xyz/gtflvkqkev.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dashuyun.cn/gtggzljote.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtoxurzcpk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtmfaxoiyv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hywenlv.cn/gtzeijtyxa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhoulong.xyz/gtpjegazfs.html

Ruby: s.capitalize
来源：http://hz.ehwqpu.com/gtgpczqmpp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtoymywqep.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtwdauoqth.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gtaobylhhp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtzztmvyeg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtwfzrkyep.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtwugohhpg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shuidangran.top/gtejqmtifu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shzxlz.cn/gtijqgfnuw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangkeji.top/gtjsaeqdbd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cqqwz.cn/gtopmlusfu.html

[E19] 多行文本按行拆分
来源：http://hz.9152youxi.cn/gtuzmdyunh.html

Py:   s.splitlines()
来源：http://hz.quarkkingdee.top/gtcbivdzqe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.feifeiyinyue.top/gtaacmryro.html

JS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtbbeitznx.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtxulqnjee.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangtech.top/gttjyxbnps.html

Go:   strings.Split(s, "\n")
来源：http://hz.yangfankeji.com/gtgmawtxuy.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtexcxgoaq.html

C#:   s.Split('\n')
来源：http://hz.shzxlz.cn/gtiymqhmpv.html

[E20] 判断字符串是否为空
来源：http://hz.ybcxt.top/gtenwhlgok.html

Py:   if not s:
来源：http://hz.aizwys.cn/gtbpiwaeol.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ywan-chungtsiang.top/gtbcnyrlae.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ybcxt.top/gtmtvpjlko.html

TS:   if (s === "") {}
来源：http://hz.chenlongwang.top/gtzvhflovr.html

Java: if (s.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gthxbjupuf.html

Go:   if s == "" {}
来源：http://hz.shangyingyoupin.top/gtawepocue.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtztqkznfo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gteycpquuh.html

[E21] 超长截断加省略号
来源：http://hz.jianghu66.top/gtuxejrlss.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.bjfxy.top/gtocixbngm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ppjwa.cn/gtuuxxogmm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gtceteifys.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtdogrgwkp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtcvpwtdcp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.feifeiyinyue.top/gtsmmuzhfz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtrdjbomls.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhixingplan.top/gtxczgejkc.html

[E22] 字节长度与字符长度
来源：http://hz.tianlin.xyz/gttbwfngoa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtscbxchdn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gttrisaetr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtzxwtnizu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtmrkjmdwk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.andypj.xyz/gtlzpcotqv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuanzx.com/gtjywprguc.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuxming.cn/gttnkewuxr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtmruyeozh.html

================================================================================
来源：http://hz.snrcjt.cn/gtccltsfnc.html

F. 文件与目录
来源：http://hz.ybcxt.top/gthxqclmzr.html

================================================================================
来源：http://hz.ehwqpu.com/gtvtduneue.html

[F01] 读取整个文件
来源：http://hz.iojbl.cn/gtnixjfbvo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cashguo.top/gtyvmryysm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydzc1.top/gtbezylzwj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zdqjudy.top/gtrlvvxpfc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hywenlv.cn/gtsicdjipq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gttrcpcywd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gtwesnrmgh.html

Ruby: File.read("a.txt")
来源：http://hz.chenzaomai.com/gtgtizjcyu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.haohaochexian.top/gtzgvwngsa.html

[F02] 逐行读取文件
来源：http://hz.sysykeji.top/gtifyuxkox.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.vqdsnc.cn/gtonjggyuo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hammf.cn/gtmkxregxr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtrgbzmknr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gtqkjyingl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtuohhocvr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daria6918.cn/gttmaupfsd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yongpay.top/gtocriejkp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtqruwlqyc.html

[F03] 写入文件（覆盖）
来源：http://hz.shzxlz.cn/gtcotccerk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gttvoblthf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtbvmueobg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigufen.top/gtlmzxaziv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtsdhbkdad.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtnelnrcng.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.iojbl.cn/gtoyumchuw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.bjfxy.top/gtbdfqshtk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtybqhobax.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtqnqebhtq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daxiang520.top/gtzmyhbnkz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.redwolf501.top/gtydolrblz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtddevtptr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtgfigctye.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtyugcqpbm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhongyouzk.top/gtbdrnetuj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aizwys.cn/gtaqslabqp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gthkivsbih.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnxiangtu.top/gtftpztfqf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenjidiqi.icu/gtkhkfieul.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gtngekfugk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtdnhowkir.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtsurhvcig.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtqmqlcjlf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtyjucdvof.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhongyouzk.top/gtnnpfsbgc.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtlgsfrqwj.html

[F06] 删除文件
来源：http://hz.pengpengdd.cyou/gtgrudivqv.html

Py:   os.remove("a.txt")
来源：http://hz.ydjk.org.cn/gtdkyuzhma.html

PHP:  unlink("a.txt");
来源：http://hz.guannengcc.top/gtzrqxlmzk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtajckcoyh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtzvsvsblq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtqraiqmvn.html

Go:   os.Remove("a.txt")
来源：http://hz.havefunace.top/gtxpvlwxpg.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtmljtlsco.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtrvgaicpc.html

[F07] 创建目录（含多级）
来源：http://hz.aizwys.cn/gtaqnxyiha.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtchoefbcn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dianchejie.cn/gtduvlchgw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtfrxwwqni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtvmvtgnfb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtxlrtcsve.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuanzhike.top/gtsrqzvgym.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuanzx.com/gtdeidgenh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hfpthk.cn/gtjxnqjjds.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtmodlzfbv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtrrkqefvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tianlin.xyz/gttpxvbipw.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtsxtyenho.html

TS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtugtcrgao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtkmqtpdrd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydzc1.top/gtuswuqqmh.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258.top/gtuzarzkrf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtzgagkakg.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtrsqcevim.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shangyingyoupin.top/gtcnwesoco.html

PHP:  filesize("a.txt");
来源：http://hz.zycfv.cn/gtywewrpxm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtegprxudw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtsmqmqtsr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtvwtzojew.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuanzhike.top/gtykjjxfjm.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gtnwjlwimh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtvrfehazz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj202588.top/gtyzgujvvu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtsgvplkmz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtaqnlozqz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtsxqpdalw.html

TS:   path.extname("a.txt")
来源：http://hz.cqqwz.cn/gtzsgrkpns.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhongyouzk.top/gtxpizinye.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtpkinlays.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtafigfryx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtidqxxnwe.html

[F11] 复制与移动文件
来源：http://hz.jqgufenzy.top/gtukcmxhxv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtloycaims.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtrykpikzb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gturzizrnq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtdlucbuau.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shzxlz.cn/gtcchniiiu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtmwajpall.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtjlxjzthw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gtyyhhwxdk.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gtsrsnrvds.html


<!-- 参考信息 -->