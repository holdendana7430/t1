代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zycfv.cn/gtcgbdxzyv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cashguo.top/gtrmypercs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtosdcnnvb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtjxrmcvrq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tian-w.cn/gtdulqxmlb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.dianchejie.cn/gtfomvcvbl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.guannengcc.top/gtxxxfsvec.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tianlin.xyz/gtadatbiwt.html

[E02] 重复字符串
来源：http://hz.zhongyouzk.top/gtttkhkgcm.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtdtectard.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuanzhike.top/gtqoshhqnb.html

JS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtzhaneotv.html

TS:   "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtktyjdslm.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtdxidwsmj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.feifeiyinyue.top/gtmmrgeadm.html

Ruby: "ab" * 3
来源：http://hz.birdmap.top/gtpvdgmdzu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jianghu66.top/gtliuibfbm.html

[E03] 截取子串
来源：http://hz.daxiang520.top/gtrloozlqp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gtigglnfaa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgfzy.top/gtphsozakz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtkojmprin.html

TS:   s.slice(1, 4)
来源：http://hz.gogol.net.cn/gtkcaczuao.html

Java: s.substring(1, 4)
来源：http://hz.52xcode.cn/gtpneefyld.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.wangshuangyany.cn/gtveeztswj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gtjuqqxanx.html

C#:   s.Substring(1, 3)
来源：http://hz.guowangkeji.top/gtlhusmgey.html

[E04] 查找子串位置
来源：http://hz.xuetiantiany.cn/gtihnqvdeh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fzhhl.top/gtnkmlsaft.html

PHP:  strpos($s, "x");
来源：http://hz.snrcjt.cn/gtzbycvuoz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.aibaodan.cn/gtxwvlsjvk.html

TS:   s.indexOf("x")
来源：http://hz.ppjwa.cn/gtmsflnscl.html

Java: s.indexOf("x")
来源：http://hz.andypj.xyz/gtcynkdzwl.html

Go:   strings.Index(s, "x")
来源：http://hz.wangdashe.top/gtxqhpotfp.html

Ruby: s.index("x")
来源：http://hz.yueranfly.top/gttdazslph.html

C#:   s.IndexOf("x")
来源：http://hz.jianghu66.top/gtzueqbhjr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydjk.org.cn/gthawrytyr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.mhx1999.top/gtpfsrpwww.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gtplfztegf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtevtlkoal.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.svipenyu.cn/gtepmylkro.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtroqijshq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.pycfn.com/gtwjvyzotg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aibaodan.cn/gtlsemaxfd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.snrcjt.cn/gtjbyazlen.html

[E06] 替换子串
来源：http://hz.jinqigfzy.top/gtgyhgvgyl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.andypj.xyz/gtbpylaqly.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenlongwang.top/gtewjsdcpg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtniwjkfvq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtfjfakxun.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtairibhtp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtvsgnrpnv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtcceuqwsw.html

C#:   s.Replace("a", "b")
来源：http://hz.jiagoushi.top/gtlbwaqbqc.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gtgktsgjda.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.svipenyu.cn/gthaaqlxyd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtpuphnmeh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydzc1.top/gtnlatrblo.html

TS:   s.split(",")
来源：http://hz.xuanzx.com/gthfuzvndq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sweek.top/gtuzgdqjfv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinyuanbaomall.cn/gtoaucxsik.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gtscqldmla.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gogol.net.cn/gtqknuakcy.html

[E08] 数组按分隔符合并
来源：http://hz.pengpengdd.cyou/gtfsogivii.html

Py:   ",".join(items)
来源：http://hz.dashuyun.cn/gtpxkonctp.html

PHP:  implode(",", $items);
来源：http://hz.sysykeji.top/gtywfxaiap.html

JS:   items.join(",")
来源：http://hz.hammf.cn/gtvpcalret.html

TS:   items.join(",")
来源：http://hz.yonumen.top/gtoksnjxdt.html

Java: String.join(",", items)
来源：http://hz.gogol.net.cn/gtyxmbqace.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gthffewhwm.html

Ruby: items.join(",")
来源：http://hz.hnxiangtu.top/gthrhtobpm.html

C#:   string.Join(",", items)
来源：http://hz.tian-w.cn/gtdyyryqub.html

[E09] 去除所有空白字符
来源：http://hz.feifeiyinyue.top/gtnnayuhsf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtcrzpkrra.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.52xcode.cn/gttszcnwes.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtphvxvqeu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jiagoushi.top/gttvvgfaxl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhoulong.xyz/gtanszdyyh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtsfuduauj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtcuixjuuz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtyufknhbf.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gaohongyu789.top/gthkpvrhvz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xylfe.cn/gtawgbjwtn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ivvv.top/gtcjqdgnko.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gteplsnbfc.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtaklelgha.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtncdniial.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtnlpnoily.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zdqjudy.top/gtfcpwfdpf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj20258888.top/gtsaolhzti.html

[E11] 反转字符串
来源：http://hz.ivvv.top/gtqlmalfsn.html

Py:   s[::-1]
来源：http://hz.hywenlv.cn/gtmhkswkzc.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtdolbuxpw.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtgjlgokqe.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtibyfopwr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.iojbl.cn/gtbupxqwsn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gtucvqiott.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gtxrwtyett.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtadpvrijv.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtugaestgj.html

Py:   s.count("a")
来源：http://hz.dashuyun.cn/gtczrqevsy.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigfzy.top/gtzyxrwyug.html

JS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtfapelftv.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtwfhtnoyy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtactdyexf.html

Go:   strings.Count(s, "a")
来源：http://hz.ybcxt.top/gtrnyvsgda.html

Ruby: s.count("a")
来源：http://hz.316326.xyz/gtilbhvbqz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.mhx1999.top/gtwaqrdwcq.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtgnidlngo.html

Py:   for ch in s: print(ch)
来源：http://hz.pycfn.com/gtjmogadyw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yueranfly.top/gtrdgkulwl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtqtpumlnb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtfskqlokg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtcoleemwc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yangfankeji.com/gtwlzfhnmy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuanzx.com/gtjgtcqmwf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.52xcode.cn/gtifkyqphe.html

[E14] URL 编码与 Base64
来源：http://hz.andypj.xyz/gtvexixufa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtfyjwijpj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuetiantiany.cn/gtbwvyjnno.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.9152youxi.cn/gtxckwomrp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinyuanbaomall.cn/gtgxyagnuq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gtkntawkby.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gttkauthxd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgfzy.top/gthencjblp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hysaishi.cn/gtsnhdibzj.html

[E15] HTML 转义 / 反转义
来源：http://hz.sweek.top/gtagpnirnl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gtaakoriwn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtkustnxdr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtqrwjxkak.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtfkiwrvgg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.pengpengdd.cyou/gthhmmvadm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtwcozzyyf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtcrwckvhf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dianchejie.cn/gtkwxinxfr.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtrkhbtzgn.html

Py:   f"{1234567:,}"
来源：http://hz.yvedp.cn/gtarhldsuy.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gtrarlcmyn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtcwjxpaib.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtgxfzkagd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhengqikj.top/gtqwghakln.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.kuanghao11.cn/gtccnncjvr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hysaishi.cn/gtthqzmlrh.html

C#:   1234567.ToString("N0")
来源：http://hz.guannengcc.top/gtniggdjsm.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtcyffksic.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gttkwuhqlu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shangyingyoupin.top/gtgdwcveot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtdgbcuhbd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtdepgokry.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cqqwz.cn/gtnhzfcwcn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtabkkevhz.html

Ruby: s.capitalize
来源：http://hz.haohaochexian.top/gtzkdxeobf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gtifnifcjp.html

[E18] 模板占位符替换
来源：http://hz.zhijiandao.cn/gtqtjhkysk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtvikluaac.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gttavkxocn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangshuangyany.cn/gtruoclgqv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtqsstkrmj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shzxlz.cn/gtggsilxru.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shzxlz.cn/gtxgycazch.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.mhx1999.top/gtopeiucvh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhiwuduotai.top/gtswzdghjg.html

[E19] 多行文本按行拆分
来源：http://hz.iojbl.cn/gtgerfbbbv.html

Py:   s.splitlines()
来源：http://hz.chenzaomai.com/gtuqzfiphv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gttfqathdp.html

JS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gtkgwospaq.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtvnufjezt.html

Java: s.lines().toList()
来源：http://hz.daxiang520.top/gtqcqwazvv.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtyofikemi.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gttysyayws.html

C#:   s.Split('\n')
来源：http://hz.zhoulong.xyz/gtorqjdird.html

[E20] 判断字符串是否为空
来源：http://hz.jlsjyb.cn/gtnupcwecy.html

Py:   if not s:
来源：http://hz.shangyingyoupin.top/gttdaicqxo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gotoacloud.top/gtexbmqche.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhengqikj.top/gtkaclksth.html

TS:   if (s === "") {}
来源：http://hz.haohaochexian.top/gtsjakhrci.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtvpesyszj.html

Go:   if s == "" {}
来源：http://hz.haohaochexian.top/gtyhplrulb.html

Ruby: if s.empty?
来源：http://hz.nanxinkj.top/gtbnhkmbcn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtdzfwpxrh.html

[E21] 超长截断加省略号
来源：http://hz.wangshuangyany.cn/gtuizukzgq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pycfn.com/gtiwezrdca.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtagcktzfn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtwlpbbjjk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtqcfwkewr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtrxgyxsaw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenzaomai.com/gtyqgpqpee.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sxryk.cn/gtzvfuukoa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtvakktzsa.html

[E22] 字节长度与字符长度
来源：http://hz.daria6918.cn/gtjzeogsbm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtvapcppel.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gthncpwxgb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtmrohwcop.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gtqvcggzlw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gtfbiznloe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtaldiwuah.html

Ruby: s.bytesize;  s.length
来源：http://hz.iojbl.cn/gtaxpnhvuh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gtftvohnvr.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcpctivzx.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtitdrrdrk.html

================================================================================
来源：http://hz.zhoulong.xyz/gttpgcbfyw.html

[F01] 读取整个文件
来源：http://hz.hnqzz.top/gtwpqjwwco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtclfgwhmf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydzc1.top/gtasetyjcb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtnnbsbhen.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xinyue.icu/gterlmsria.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtalaykgaw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gtzjmdezlv.html

Ruby: File.read("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtchsjqwoy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.mhx1999.top/gturttdukd.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtkyfmawbc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gtkbvkjlyx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtlxptwfju.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtjxibnrer.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtdfargmbx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gthdeqysjk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtsgfiksqp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gthflmmsby.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hfpthk.cn/gtpxduurol.html

[F03] 写入文件（覆盖）
来源：http://hz.shzxlz.cn/gtiwhhvhxk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gttnwguzoc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtilfwcanx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gtpwfwuhst.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtmtqaoack.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cqqwz.cn/gtkyewiznv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.kuanghao11.cn/gtncsvjrzk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtjmrxdehl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtyakvtlxy.html

[F04] 追加写入文件
来源：http://hz.yuxming.cn/gtsrbzpqhz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gtgpqoxcct.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gttulduehg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtqfhpfxsd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtfujcwcmw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenzaomai.com/gtgogdfhmi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xziqi.cn/gtlgvkbwlv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtvsezoloj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtneomjnye.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigfzy.top/gtfnfcnpon.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinghuilouyu.cn/gtsvsmtlrh.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gtcguekimp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtbzpztqsa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtgstrtiax.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtrurcvsqo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.mhx1999.top/gtgzxnloeq.html

Ruby: File.exist?("a.txt")
来源：http://hz.9152youxi.cn/gtidznuvej.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtftziuoss.html

[F06] 删除文件
来源：http://hz.shangyingyoupin.top/gturpqqjxs.html

Py:   os.remove("a.txt")
来源：http://hz.nanxuanxn.top/gthbdjgkeb.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtvhpxevss.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtmrrvzjac.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtpqczebbs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gthwiktgyg.html

Go:   os.Remove("a.txt")
来源：http://hz.yongpay.top/gtokfzxfez.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gtiuggkvur.html

C#:   File.Delete("a.txt");
来源：http://hz.cucudq.cn/gtyoohggjw.html

[F07] 创建目录（含多级）
来源：http://hz.sxryk.cn/gtoxwjrryo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gtpojyccjx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nwbrower.top/gtfbkhdmfb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hywenlv.cn/gtqjqjammc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gticphvbjq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gthnpuotdc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shzxlz.cn/gtdumuszhj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtqvdxvvuw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.9152youxi.cn/gtwokewjwr.html

[F08] 遍历目录
来源：http://hz.ydjk.org.cn/gtxxxhtylw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtzqczuowe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnxiangtu.top/gtgufvjzow.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangtech.top/gtqlybkbeh.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gtltrpyzdd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtjtzlglxh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnqzz.top/gtpybigtyc.html

Ruby: Dir.children("dir")
来源：http://hz.xingfuxueyuan.xyz/gtpfirecnv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtjuekcnct.html

[F09] 获取文件大小
来源：http://hz.yj20258.top/gtfehbwfzq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.birdmap.top/gttrhucvit.html

PHP:  filesize("a.txt");
来源：http://hz.yanxiufei.cn/gtfycdkqvv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtdcgzledt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtnfehjnca.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gthqfmhupx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinghuilouyu.cn/gtbjwfdfyw.html

Ruby: File.size("a.txt")
来源：http://hz.52xcode.cn/gtibhpveiz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xinyue.icu/gtfjtpnepi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtueagdqfo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gtrzgslqtt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.haohaochexian.top/gtfsicsnkm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtpqtguxep.html

TS:   path.extname("a.txt")
来源：http://hz.0kj1m.cn/gtfdpnxzal.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.vqdsnc.cn/gtoncoiihx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtqifdpsui.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtiagyzjux.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gtcdzusynm.html

[F11] 复制与移动文件
来源：http://hz.chenzaomai.com/gtvdnqcpjg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtouhfwjll.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtowewcvyj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtqxgetdff.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gttenofzaz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenjidiqi.icu/gtjmqroihn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sysykeji.top/gtvmqoxmte.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtksacpfww.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtuwyonolc.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtjbnantbj.html


<!-- 参考信息 -->