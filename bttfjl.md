代发 wailian999

[E02] 重复字符串
来源：http://hz.316326.xyz/gtypckznlj.html

Py:   "ab" * 3
来源：http://hz.nanxinkj.top/gtvkakppzh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinghuilouyu.cn/gttxutsntx.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtcrxnyuto.html

TS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gtqhwcusej.html

Java: "ab".repeat(3)
来源：http://hz.sweek.top/gtmsjbxueo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daria6918.cn/gthizozizr.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gthirnwceo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxinkj.top/gtisbjpjpa.html

[E03] 截取子串
来源：http://hz.tian-w.cn/gtiidnehpi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gtspahqoze.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dashuyun.cn/gtvgvpvdvk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtbsozqeip.html

TS:   s.slice(1, 4)
来源：http://hz.cqqwz.cn/gtomsqixqo.html

Java: s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gteejevxas.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jianghu66.top/gtfucvnfgg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtrtexpjeq.html

C#:   s.Substring(1, 3)
来源：http://hz.bjfxy.top/gtbmorczih.html

[E04] 查找子串位置
来源：http://hz.snrcjt.cn/gtfhkhlktr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pycfn.com/gtubwebfsc.html

PHP:  strpos($s, "x");
来源：http://hz.hywenlv.cn/gtymzrjenn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtnbwpjuyu.html

TS:   s.indexOf("x")
来源：http://hz.ydjk.org.cn/gtvbgeiiqp.html

Java: s.indexOf("x")
来源：http://hz.chenlongwang.top/gtzawsekox.html

Go:   strings.Index(s, "x")
来源：http://hz.yangfankeji.com/gtxtajgfcv.html

Ruby: s.index("x")
来源：http://hz.jinqigfzy.top/gtpcprnrni.html

C#:   s.IndexOf("x")
来源：http://hz.quarkkingdee.top/gtcdaeoftc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.feifeiyinyue.top/gtxufrxbve.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.mhx1999.top/gtizzkpucc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtvezahhif.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gtirauybyh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fengsongda.top/gtmhyafpyf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtmgaortvj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xingfuxueyuan.xyz/gtgbgchpal.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dianchejie.cn/gtnaudjppz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.svipenyu.cn/gtlwxmwfsa.html

[E06] 替换子串
来源：http://hz.ydjk.org.cn/gtuakxlimy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jianghu66.top/gthwkqtvmc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.wangdashe.top/gtlcbfxonm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtluzqkrid.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtmzbdlhpr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtbgdiplrs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jianghu66.top/gtgtqvkuhp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daria6918.cn/gtvbzflofx.html

C#:   s.Replace("a", "b")
来源：http://hz.yangfankeji.com/gtdwixrwvw.html

[E07] 按分隔符拆分
来源：http://hz.kuanghao11.cn/gtoxfroqou.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenzaomai.com/gtxicekcsl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.mhx1999.top/gtzddvzfrj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.c1oappe.top/gtorhmpxmw.html

TS:   s.split(",")
来源：http://hz.tian-w.cn/gtqpwnrtcm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xylfe.cn/gtwtysjcef.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gaohongyu789.top/gtekwqbplj.html

Ruby: s.split(",");  s.split
来源：http://hz.tanke756.top/gttnmpekxk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gaohongyu789.top/gttdqjvesb.html

[E08] 数组按分隔符合并
来源：http://hz.gaohongyu789.top/gtaenptczl.html

Py:   ",".join(items)
来源：http://hz.chenjidiqi.icu/gtwbkwzcoj.html

PHP:  implode(",", $items);
来源：http://hz.gaohongyu789.top/gtdanbctak.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtidyjowzp.html

TS:   items.join(",")
来源：http://hz.jinqigufen.top/gtscugnmhx.html

Java: String.join(",", items)
来源：http://hz.kuanghao11.cn/gtldrioqom.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtpkvfcdnk.html

Ruby: items.join(",")
来源：http://hz.ppjwa.cn/gtuozqziti.html

C#:   string.Join(",", items)
来源：http://hz.mhx1999.top/gtlsgeizno.html

[E09] 去除所有空白字符
来源：http://hz.ybcxt.top/gthbqvkdeu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinghuilouyu.cn/gtypgcuthz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.mhx1999.top/gtfgmmrqmp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtjjwtsxvh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtqkjrhdzp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258.top/gtnvrqkqib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.feifeiyinyue.top/gtnstpgjzv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daxiang520.top/gtwqszaize.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pengpengdd.cyou/gtauusonut.html

[E10] 左侧补零 / 定长填充
来源：http://hz.smart0.xyz/gtmjpwubkp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.kuanghao11.cn/gtogrozked.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.52xcode.cn/gtqrgrbsrn.html

JS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtzatxwqso.html

TS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gteintnlhq.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gtfmorubcq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhoulong.xyz/gttsjqqpxe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtvueqediw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnxiangtu.top/gtlghoxnrg.html

[E11] 反转字符串
来源：http://hz.jinqigufen.top/gttpqquqpt.html

Py:   s[::-1]
来源：http://hz.chenjidiqi.icu/gtdpeahuyi.html

PHP:  strrev($s);
来源：http://hz.ppjwa.cn/gtwbfgjnbd.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtqgmngqxw.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtlnnbsxby.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtowpjounk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhixingplan.top/gtiltllehg.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtxupcajdh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtpagqeosz.html

[E12] 统计某字符出现次数
来源：http://hz.ydjk.org.cn/gtplzlzmfe.html

Py:   s.count("a")
来源：http://hz.yueranfly.top/gtfppcmlas.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtrvrgykhf.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtwgpzdgpk.html

TS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtccxrdyyt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhongyouzk.top/gtokcwydio.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtymabmjru.html

Ruby: s.count("a")
来源：http://hz.sxryk.cn/gtcjeiqaqj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtveqnyyoj.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gtsluvnotu.html

Py:   for ch in s: print(ch)
来源：http://hz.mhx1999.top/gtmgkgxnnm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dashuyun.cn/gtxsfcrbkv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gttkpkpepm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gthcaimkzo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gthoqaufnp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.daxiang520.top/gtfzyxjrmv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gttmygoxmu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtjljxofdi.html

[E14] URL 编码与 Base64
来源：http://hz.jqgfzy.top/gthwclerel.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.vqdsnc.cn/gtijznordl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fengsongda.top/gtyeiblcjm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zdqjudy.top/gtbktwcmjv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yueranfly.top/gtuumuyske.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cucudq.cn/gtreddogwg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.c1oappe.top/gtebpaxxrx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtwqibcypq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shzxlz.cn/gtuswhmpso.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtsudkyiwz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gzhubu.top/gtygedzirf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sufxvd.cn/gtjlzircis.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuanzhike.top/gtsehvhqbk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yongpay.top/gtppetpwwy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhongyouzk.top/gtvwvwshrw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtwsqjxfgb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gthlxestsq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258.top/gtnoiowzrj.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gtbwnhwocc.html

Py:   f"{1234567:,}"
来源：http://hz.xziqi.cn/gtjptevbbi.html

PHP:  number_format(1234567);
来源：http://hz.chenjidiqi.icu/gtyjegbnqt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtpjhoyeik.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtbjtaetdk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gttzrqvnkq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jianghu66.top/gtdryxwhae.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ivvv.top/gtyqvlpbpq.html

C#:   1234567.ToString("N0")
来源：http://hz.chenlongwang.top/gtmhjinbjd.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtdaodaurb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yanxiufei.cn/gtkxcyebzt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtnanryniy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtgoripyxu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtvxlnvxuk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj20258.top/gtfupqrwbg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hammf.cn/gtyxkwkkbt.html

Ruby: s.capitalize
来源：http://hz.cdnleiting.top/gttrzijesg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtjowiqnim.html

[E18] 模板占位符替换
来源：http://hz.fzhhl.top/gtjeqgibbp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtubbejxtc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hammf.cn/gtjsmuzfcf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtgeymacmm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtylbbermv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yueranfly.top/gtindzzfxv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gzhubu.top/gtvyoqsnpd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtrptkgcuz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yangfankeji.com/gttjkdhkpt.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gtrjmoqagt.html

Py:   s.splitlines()
来源：http://hz.jinqigufen.top/gtxevhkkyh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.andypj.xyz/gtxlxtnbeo.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtecywchps.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtgtcalssw.html

Java: s.lines().toList()
来源：http://hz.shzxlz.cn/gtzujvwxzm.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtpzkjamcq.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtuaeekcnh.html

C#:   s.Split('\n')
来源：http://hz.bjfxy.top/gtqcuufrqg.html

[E20] 判断字符串是否为空
来源：http://hz.shangyingyoupin.top/gtkhdlqldx.html

Py:   if not s:
来源：http://hz.yj20258.top/gtofluzntm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gttdqcwjnf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.guowangkeji.top/gtbpqtplcx.html

TS:   if (s === "") {}
来源：http://hz.chenlongwang.top/gtibezzsru.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtnvwfibnl.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gtzzmjwcry.html

Ruby: if s.empty?
来源：http://hz.sysykeji.top/gtkcymdbro.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtapjpdwan.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtsrczpjul.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hfpthk.cn/gtmtzwzbpk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gotoacloud.top/gtcycyvgre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gturvhxiar.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtvshocprs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtfgqtayqg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xuanzx.com/gtfhejoeod.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yvedp.cn/gtkujphwhk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ivvv.top/gtndlgqyia.html

[E22] 字节长度与字符长度
来源：http://hz.vqdsnc.cn/gtfxvziqsh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxuanxn.top/gtpdasjcpp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtqbskjuzu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtymklqvbf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gttzealorf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yanxiufei.cn/gtpfoasorg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtvrfusvri.html

Ruby: s.bytesize;  s.length
来源：http://hz.vqdsnc.cn/gtldcxnuvm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hywenlv.cn/gtrjvhpyrn.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcfusnmef.html

F. 文件与目录
来源：http://hz.vqdsnc.cn/gtqxcxuocj.html

================================================================================
来源：http://hz.aibaodan.cn/gtzbmbivfh.html

[F01] 读取整个文件
来源：http://hz.meibo888.top/gtgbpehiaz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.quarkkingdee.top/gtvhybwnzi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guannengcc.top/gtgvpsisay.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtwxwjeynz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.andypj.xyz/gtduxhlgcc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtggwbevid.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aibaodan.cn/gtygzzlrma.html

Ruby: File.read("a.txt")
来源：http://hz.jiagoushi.top/gtizunzbrn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtsagdjnen.html

[F02] 逐行读取文件
来源：http://hz.jqgfzy.top/gtnpmjfcbi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinyuanbaomall.cn/gtvlnrkqgn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tanke756.top/gtvctmglvc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtkevbydai.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtihhtjoqi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtavujygpx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtpsxxvwuv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gttfayqsff.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhoulong.xyz/gtylteywch.html

[F03] 写入文件（覆盖）
来源：http://hz.tianlin.xyz/gtgvqcceba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.52xcode.cn/gtwuposzmx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tanke756.top/gtrxflvygk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtqxqorhlw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtndihoqoc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinyuanbaomall.cn/gtgcffeish.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xinyue.icu/gtblcbhcub.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gtmxbronmq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtfysazirb.html

[F04] 追加写入文件
来源：http://hz.fzhhl.top/gtobefmnyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtlmulgcnz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nwbrower.top/gtpnrjagmc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtwgkppxoi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aizwys.cn/gtgvhoqtyt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhoulong.xyz/gtnvwzqprn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gtalwkfwoq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhongyouzk.top/gtkvoxydkh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtuaxuovwn.html

[F05] 判断文件或目录是否存在
来源：http://hz.316326.xyz/gtuanmxypx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xziqi.cn/gtljrrgjqr.html

PHP:  file_exists("a.txt");
来源：http://hz.ivvv.top/gtswjvrexz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtygwwvcpl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtcybrdfgo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtovktsouj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtdpbavvjb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yangfankeji.com/gttmsdqbhq.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtxtwgfjyn.html

[F06] 删除文件
来源：http://hz.hywenlv.cn/gtlcjleydd.html

Py:   os.remove("a.txt")
来源：http://hz.zhijiandao.cn/gtgkmfjlhp.html

PHP:  unlink("a.txt");
来源：http://hz.gaohongyu789.top/gtyozwwwro.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtgjkumivv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtakovdgrr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtfajimjss.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtwyrquknr.html

Ruby: File.delete("a.txt")
来源：http://hz.ybcxt.top/gttrmswggf.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtvsqteelp.html

[F07] 创建目录（含多级）
来源：http://hz.ydjk.org.cn/gtkhacwfdo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtzripyasf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hywenlv.cn/gtkysggixf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtmcibwnin.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtppequfup.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtiorkfwtd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.dashuyun.cn/gtfemfaice.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jianghu66.top/gtzuezsbai.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtxlajeqgs.html

[F08] 遍历目录
来源：http://hz.shanyushiyangtech.top/gticaehsxy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gtzzamjhjo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtreunnroi.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtdusfryfl.html

TS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtqyzlgayd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ivvv.top/gtfurtdbzw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtnoqztrvo.html

Ruby: Dir.children("dir")
来源：http://hz.dashuyun.cn/gtgmilxahk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinqigfzy.top/gtrvfqqahf.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtissswjqe.html

Py:   os.path.getsize("a.txt")
来源：http://hz.smart0.xyz/gtuyfdehxl.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtfaehzija.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtbfdjuxaq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gthluqxyhv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtmhnkgivx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.snrcjt.cn/gttikyoyxf.html

Ruby: File.size("a.txt")
来源：http://hz.sweek.top/gtovyqdvho.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daxiang520.top/gtwxfnvzdx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guannengcc.top/gtekkwmcct.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtncrywfcc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtzclybqry.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtrzrqnkuz.html

TS:   path.extname("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtnioctzet.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yvedp.cn/gtvmviaagm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtoyjcyski.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtylxjnozl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dianchejie.cn/gtbzdeovmr.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gtcbunfsdk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtgvcpwcfn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xinyue.icu/gtdlrjuywm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtsaveufjf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtinxiikym.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtkxggdrgh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.mhx1999.top/gtncormcyq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtjhkxerdt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fengsongda.top/gtlcfnqfot.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtmuyzatoc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtioddazvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gtlbogkwli.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.quarkkingdee.top/gtycrpfirw.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtdvcymjdg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yanxiufei.cn/gtrfaxlidq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtccwixhiw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.kuanghao11.cn/gtktuhuyvs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shzxlz.cn/gtqbbxurfh.html


<!-- 参考信息 -->