代发 wailian999

[E02] 重复字符串
来源：http://hz.shanyushiyangtech.top/gtekqjgule.html

Py:   "ab" * 3
来源：http://hz.gogol.net.cn/gtnryddzzk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shzxlz.cn/gtfcuqopct.html

JS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtwbfgxlne.html

TS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtznrdsiyn.html

Java: "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtqbprffdc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yuxming.cn/gtsmilkfxf.html

Ruby: "ab" * 3
来源：http://hz.zdqjudy.top/gtnggbezxm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.c1oappe.top/gtbqcliiso.html

[E03] 截取子串
来源：http://hz.ppjwa.cn/gtplcbovlu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sweek.top/gtipqbtchc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtsodknjpk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.bjfxy.top/gtoeucczyr.html

TS:   s.slice(1, 4)
来源：http://hz.gaohongyu789.top/gtnjwshbpr.html

Java: s.substring(1, 4)
来源：http://hz.birdmap.top/gtpnnyawjy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuetiantiany.cn/gtjghgqidi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hongshengwenyu.top/gthtpfawlw.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258.top/gtslqdemga.html

[E04] 查找子串位置
来源：http://hz.zhaomingkeji.xyz/gtrozdnqtm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenzaomai.com/gtdjskyehf.html

PHP:  strpos($s, "x");
来源：http://hz.daria6918.cn/gtpqiahwnr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtycjprrhq.html

TS:   s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtllylmtad.html

Java: s.indexOf("x")
来源：http://hz.jqgfzy.top/gthcoxvdwl.html

Go:   strings.Index(s, "x")
来源：http://hz.xylfe.cn/gtyeishllk.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gtkcebqzzp.html

C#:   s.IndexOf("x")
来源：http://hz.jiagoushi.top/gtzlxejkaf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cashguo.top/gtywbgqghs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jianghu66.top/gtofxtgbce.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.svipenyu.cn/gtxvuclyno.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gtfuduzjsc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj20258888.top/gtvjbvkpof.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtlnenwkeb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtgghpjmha.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydjk.org.cn/gtpxphqxba.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.kuanghao11.cn/gtmwadysui.html

[E06] 替换子串
来源：http://hz.jqgfzy.top/gtsauqovwv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigfzy.top/gtyubleuam.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jianghu66.top/gtzsqgwuwa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtuylhrenb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtawandokq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtxmizlbqu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cqqwz.cn/gtpnvuhmga.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xinyue.icu/gtcszexyqk.html

C#:   s.Replace("a", "b")
来源：http://hz.fengsongda.top/gtgojfkxyy.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gtmgdwzuqf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.aibaodan.cn/gtzbguznto.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuetiantiany.cn/gtqnpznsbp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fengsongda.top/gtipzxerbh.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtwhipjedx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hywenlv.cn/gtptkjzpnn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuxming.cn/gtzrhhxlba.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtvbnlwpbx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tian-w.cn/gtsyhdnwjt.html

[E08] 数组按分隔符合并
来源：http://hz.kuanghao11.cn/gthkehauck.html

Py:   ",".join(items)
来源：http://hz.ehwqpu.com/gtmnjoddwd.html

PHP:  implode(",", $items);
来源：http://hz.yj20258.top/gtlwphxjwv.html

JS:   items.join(",")
来源：http://hz.mhx1999.top/gtxpoplhoy.html

TS:   items.join(",")
来源：http://hz.dianchejie.cn/gtzstlsybi.html

Java: String.join(",", items)
来源：http://hz.haohaochexian.top/gtsikfvwyh.html

Go:   strings.Join(items, ",")
来源：http://hz.kuanghao11.cn/gtjvzwyico.html

Ruby: items.join(",")
来源：http://hz.xziqi.cn/gtvljvktox.html

C#:   string.Join(",", items)
来源：http://hz.0kj1m.cn/gtmlhmnhsy.html

[E09] 去除所有空白字符
来源：http://hz.pengpengdd.cyou/gtueqnddio.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gtgzgkabqk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gtjvyycpsc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtqkixiryg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.redwolf501.top/gtaslafzos.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuxming.cn/gtvsmdvopl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtgeyjdtnq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.9152youxi.cn/gteluzjrjo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhongyouzk.top/gtkoetdibd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258.top/gtykkejclx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gtcegdfpkf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yonumen.top/gtbpzetrso.html

JS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtxifphxna.html

TS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtzhyylskj.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtmznjbihm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtfxjtoaam.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gtnbkmeygj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtiwwyqwbz.html

[E11] 反转字符串
来源：http://hz.xingfuxueyuan.xyz/gtkpdopmgu.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtbkgcskjk.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangtech.top/gteznnnrcu.html

JS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtoomhmfcw.html

TS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtrhiobbhq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtcsmdqvbj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gtelhtkqub.html

Ruby: s.reverse
来源：http://hz.nanxinkj.top/gtljnsiciu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtwekckgpl.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtkejvjqym.html

Py:   s.count("a")
来源：http://hz.dianchejie.cn/gtpsbfmlwh.html

PHP:  substr_count($s, "a");
来源：http://hz.nwbrower.top/gtrsxcswpc.html

JS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtnrnxhmgq.html

TS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtukrggliu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxinkj.top/gtxslsufzv.html

Go:   strings.Count(s, "a")
来源：http://hz.ydjk.org.cn/gtoyiliyuh.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtqnbkgyxa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ppjwa.cn/gthqnnetav.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtkyxftdtc.html

Py:   for ch in s: print(ch)
来源：http://hz.zhoulong.xyz/gtyfsxqrlw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gtrumczevj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gttdkoslyo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtnmmkmqbz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.andypj.xyz/gtkkbmoskb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ppjwa.cn/gthykyhdrc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtbjxnnwme.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinyuanbaomall.cn/gtszkqwgzl.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gtlmudaavj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fzhhl.top/gthmacpevv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yongpay.top/gtmzrmwhpo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.52xcode.cn/gtkxxpafri.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinghuilouyu.cn/gtyiqxezvc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxuanxn.top/gtvsqomcmu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtnrbeuaya.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hammf.cn/gtsbcvefml.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pengpengdd.cyou/gtsxxfsruy.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gtiqxjocjs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtkaequwka.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydjk.org.cn/gtnjqifssv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gtuohevfdm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gogol.net.cn/gtednccvsj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gtpsdepoew.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258.top/gtkzjerhwx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtngezqjxx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangdashe.top/gtxtwgpttw.html

[E16] 数字千分位
来源：http://hz.xuetiantiany.cn/gtsaaqfjnq.html

Py:   f"{1234567:,}"
来源：http://hz.redwolf501.top/gtmttxrqpq.html

PHP:  number_format(1234567);
来源：http://hz.bjfxy.top/gtgiuhuiow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gtjmsfgyuy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gttgjwzagb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shuidangran.top/gthvbmjaqr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xylfe.cn/gtzbqzvuwu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.feifeiyinyue.top/gtyixxrkhx.html

C#:   1234567.ToString("N0")
来源：http://hz.cucudq.cn/gtdkypoaot.html

[E17] 首字母大写
来源：http://hz.jianghu66.top/gtjzscjcun.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gtupbjjewr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhiwuduotai.top/gtkmhuqgnm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtdhnlkbbk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gtikqarbwg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.quarkkingdee.top/gtlwkmhckz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cqqwz.cn/gtmawduiku.html

Ruby: s.capitalize
来源：http://hz.svipenyu.cn/gthqvpuwhf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yonumen.top/gteqmohupu.html

[E18] 模板占位符替换
来源：http://hz.jlsjyb.cn/gtfwkqhdwv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hywenlv.cn/gtsmludalu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtblyzubqn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gthcfdbpoy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtekaejucj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daria6918.cn/gtdtlbanwc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jiagoushi.top/gtyohztxxc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtkmilowpu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.mhx1999.top/gtolrwsjzc.html

[E19] 多行文本按行拆分
来源：http://hz.guannengcc.top/gtbdzumhjz.html

Py:   s.splitlines()
来源：http://hz.zhengqikj.top/gtjsuudnkk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ywan-chungtsiang.top/gtrcpioksr.html

JS:   s.split(/\r?\n/)
来源：http://hz.vqdsnc.cn/gtqhsqxeia.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtfyhboeyi.html

Java: s.lines().toList()
来源：http://hz.tianlin.xyz/gtbnareikv.html

Go:   strings.Split(s, "\n")
来源：http://hz.jyoumei.cn/gtowdbltiw.html

Ruby: s.lines
来源：http://hz.feifeiyinyue.top/gtgvpwrnio.html

C#:   s.Split('\n')
来源：http://hz.svipenyu.cn/gtplagwcia.html

[E20] 判断字符串是否为空
来源：http://hz.chenzaomai.com/gtpczgyxjr.html

Py:   if not s:
来源：http://hz.52xcode.cn/gttzhedkpt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuanzx.com/gtjxbvklcd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sxryk.cn/gthoxkabsl.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtsmmrhgnx.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtmxzdiwgs.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtldojwvlt.html

Ruby: if s.empty?
来源：http://hz.dashuyun.cn/gtuwzsbtjc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtdcadjxhe.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtmgcbhgwv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtdrotfeit.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtjiccwjwf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtjfgqiuul.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtlbchjkej.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtkbaudbki.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.vqdsnc.cn/gtnyknooib.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtlieaqebx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gtzmpchcnt.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtskzlvgne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.meibo888.top/gtgqwsaxst.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtxvdmozkd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtsciyekuj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtdexfxbui.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xziqi.cn/gtrpkbtgvt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.52xcode.cn/gtohfdghrn.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gtaqqfqory.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.havefunace.top/gtkfyezfmc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvaadcgpo.html

F. 文件与目录
来源：http://hz.316326.xyz/gtmnsaazcx.html

================================================================================
来源：http://hz.52xcode.cn/gtfqgvttzo.html

[F01] 读取整个文件
来源：http://hz.wangdashe.top/gtgmtuqooq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangshuangyany.cn/gtxtbmifsq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtvqdvnsoz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigfzy.top/gtvrovjmkt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jyoumei.cn/gtpkhabrzp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtjnhfsfgp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtaogclxrn.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gtpeffngee.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtfnxmcued.html

[F02] 逐行读取文件
来源：http://hz.ppjwa.cn/gtdtucwbpf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinghuilouyu.cn/gtstbysfjs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtkrfsposz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtkhraiiqt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtzpxehkxv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtymqxtnvf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zdqjudy.top/gttdvehpkr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gtvlkdhnhk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gtbkfzoorh.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangtech.top/gtfyfdaanf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ppjwa.cn/gtkqemljeh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gtyqcpduuv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtpwyywjbo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtovctbjtm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gteukjunbe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtreoereub.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuanzhike.top/gtzlwdukjy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtdatnhoxm.html

[F04] 追加写入文件
来源：http://hz.52xcode.cn/gtbmoampmd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aizwys.cn/gtawowuquz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtlgzgokfu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtparmpjtz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtbhnksvvg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhixingplan.top/gteqwgieak.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtllpqwcwe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtkhtpjksn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jyoumei.cn/gtfdywmdzq.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtnmlycnev.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.52xcode.cn/gtqyvogrtp.html

PHP:  file_exists("a.txt");
来源：http://hz.ybcxt.top/gtrygrcixw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtppzwzucq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtmxwifbew.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtegivtpvh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.c1oappe.top/gtneglecon.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj202588.top/gtkoflzdbn.html

C#:   File.Exists("a.txt")
来源：http://hz.hysaishi.cn/gtityvofhz.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtfxbabhpl.html

Py:   os.remove("a.txt")
来源：http://hz.zhijiandao.cn/gtwcqbrsjd.html

PHP:  unlink("a.txt");
来源：http://hz.zhoulong.xyz/gtcyfewhvs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtyfotfwwt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gtmdjydjnt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtbnijxyog.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gthmucpmvd.html

Ruby: File.delete("a.txt")
来源：http://hz.hnxiangtu.top/gtlqryjyqm.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtqvpchwqq.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtgpsarxgu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnxiangtu.top/gtsqgrcwhy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtmmgxwgzh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtxugdllhp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtipmfpmlp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtrsgkluid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sufxvd.cn/gtovfzrtzo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pycfn.com/gttfbvayhb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jyoumei.cn/gtkpznmvuc.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gtktriudqq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hysaishi.cn/gtstyxqaeh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shanyushiyangtech.top/gtnhrymukc.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtofnukrry.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtuydbmdth.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtdzrtpwzs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangshuangyany.cn/gtvetvpjxq.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtwwvorzrj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.snrcjt.cn/gtasghmhcv.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtpxewlloy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhoulong.xyz/gtarhmmfcv.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtsckfvbcc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtrpqidlhu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gthelcouqc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtrvmduegy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pengpengdd.cyou/gtsfvmlsoe.html

Ruby: File.size("a.txt")
来源：http://hz.hywenlv.cn/gthkwlkoup.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gaohongyu789.top/gttwkspjhp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.9152youxi.cn/gtonxgzhnf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtmjtmbfyb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jlsjyb.cn/gtlrobvbri.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gthpfitlie.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gtfwqreesy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.svipenyu.cn/gtgboimzch.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtmcdhdrzw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtwnyckypu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuxming.cn/gtzmargdsa.html

[F11] 复制与移动文件
来源：http://hz.yj20258888.top/gtbmkiojei.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtxumtpfqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangdashe.top/gtbdvvcsaj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtsnouidqp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtbafvzryp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sxryk.cn/gtlrvfrajy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cashguo.top/gtwwbossof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtyxxewewo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangkeji.top/gtlwnontup.html

[F12] CSV 读写
来源：http://hz.dashuyun.cn/gtkjjxbiki.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtotnuwwbt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtiozttjld.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtknjmdcrc.html

TS:   // 同上
来源：http://hz.jinqigufen.top/gtwqxxmvjh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtnpdthujz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gtfichtdsx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtegnjxtbn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ehwqpu.com/gtucwuulur.html


<!-- 参考信息 -->