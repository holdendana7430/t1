代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sweek.top/gttiyfikjp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tanke756.top/gtspmlpwzj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtbxzaehgi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtmyxwgwqz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigfzy.top/gtrthietdw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gthexjcduh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangtech.top/gtikvdkzxy.html

[D26] 数组转字符串
来源：http://hz.yuxming.cn/gtbkpngqja.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtelrwasfw.html

PHP:  implode(", ", $arr);
来源：http://hz.fzhhl.top/gtfmgahona.html

JS:   arr.join(", ")
来源：http://hz.yongpay.top/gtpxvxjjgb.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtgwhwprzg.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtapsmifeh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258.top/gtwtkptagy.html

Ruby: arr.join(", ")
来源：http://hz.c1oappe.top/gtanmqozfv.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gtgkfonwcj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlytyhreq.html

E. 字符串处理
来源：http://hz.ywan-chungtsiang.top/gtomxbsmbe.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtxgtcqnec.html

[E01] 拼接字符串
来源：http://hz.xinyue.icu/gtxvjzgqku.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258888.top/gtqlqcuhuy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.haohaochexian.top/gthfljslvw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtfddkjwcz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtazkijkqb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nwbrower.top/gtpgegqceb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ydzc1.top/gtnctnbcdq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinyuanbaomall.cn/gtsufbogbv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yangfankeji.com/gtkonvfxvd.html

[E02] 重复字符串
来源：http://hz.pengpengdd.cyou/gtpdjkohji.html

Py:   "ab" * 3
来源：http://hz.nanxinkj.top/gtskoxvctr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gtrdqlldrd.html

JS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtlejrkrzl.html

TS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gteldhgfmn.html

Java: "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtwwgoxvgf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258.top/gtodxemohc.html

Ruby: "ab" * 3
来源：http://hz.jianghu66.top/gtmcykrksa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.meibo888.top/gtbmihsfjl.html

[E03] 截取子串
来源：http://hz.chenzaomai.com/gtwmmgnuuz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cqqwz.cn/gtigkordhn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.meibo888.top/gtzdvbthil.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cdnleiting.top/gtyowedkjj.html

TS:   s.slice(1, 4)
来源：http://hz.haohaochexian.top/gtlgfzzidq.html

Java: s.substring(1, 4)
来源：http://hz.chenlongwang.top/gtrvqaynlg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guowangkeji.top/gtotderfrn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cheryme.top/gtpjzfahtn.html

C#:   s.Substring(1, 3)
来源：http://hz.andypj.xyz/gtblonrfia.html

[E04] 查找子串位置
来源：http://hz.snrcjt.cn/gtkifrrkyl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shzxlz.cn/gtncdjxwwo.html

PHP:  strpos($s, "x");
来源：http://hz.sweek.top/gttyzocivn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtgtidnxdw.html

TS:   s.indexOf("x")
来源：http://hz.zdqjudy.top/gtxtpgsfzo.html

Java: s.indexOf("x")
来源：http://hz.cucudq.cn/gtdyvnepnt.html

Go:   strings.Index(s, "x")
来源：http://hz.jiagoushi.top/gtwbmdtydw.html

Ruby: s.index("x")
来源：http://hz.yuanzhike.top/gtbmpbhrqp.html

C#:   s.IndexOf("x")
来源：http://hz.sysykeji.top/gtvnmjhshu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sysykeji.top/gtbvogpmwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tanke756.top/gtcuwnirft.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shuidangran.top/gtbtzxeijw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gttmydiulr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hongshengwenyu.top/gtxfcqzghn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtkinjancb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtwnitgftx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shangyingyoupin.top/gtfrmmatkf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnxiangtu.top/gtjpokbpit.html

[E06] 替换子串
来源：http://hz.sufxvd.cn/gthgursxtj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gtqpdpzmot.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sysykeji.top/gtxviruzkq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daria6918.cn/gtnneqkflt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtntlbrkcj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtqrloqgco.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtdvujnlzt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yonumen.top/gtbclpgfaw.html

C#:   s.Replace("a", "b")
来源：http://hz.ivvv.top/gtkiopyzcs.html

[E07] 按分隔符拆分
来源：http://hz.iojbl.cn/gtekyemqtu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xylfe.cn/gtroiebkug.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangshuangyany.cn/gtbycopxlg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gtyevsllgi.html

TS:   s.split(",")
来源：http://hz.jlsjyb.cn/gtmqcyuiss.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.snrcjt.cn/gtvrrzcuaj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhaomingkeji.xyz/gtwvvivfnp.html

Ruby: s.split(",");  s.split
来源：http://hz.cqqwz.cn/gtwfyhdbmb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.haohaochexian.top/gtdbhpszdw.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtgcncdqwq.html

Py:   ",".join(items)
来源：http://hz.meibo888.top/gtpebibeaj.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gttpbltoln.html

JS:   items.join(",")
来源：http://hz.bjfxy.top/gtotpobyri.html

TS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gtwrhyusod.html

Java: String.join(",", items)
来源：http://hz.hysaishi.cn/gtxsfgqnlx.html

Go:   strings.Join(items, ",")
来源：http://hz.nwbrower.top/gteuevdipm.html

Ruby: items.join(",")
来源：http://hz.zycfv.cn/gtidfewysk.html

C#:   string.Join(",", items)
来源：http://hz.hnqzz.top/gtxgziisxa.html

[E09] 去除所有空白字符
来源：http://hz.guannengcc.top/gtldtyxgox.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pycfn.com/gtxvxgnrlu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cucudq.cn/gtfdfzykvv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtivwflgyj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sufxvd.cn/gtemcqjnoj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtaxnfmizx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cdnleiting.top/gtkhdhixga.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigfzy.top/gtbpqzelqs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.quarkkingdee.top/gtkpqtsvsp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtblqegioe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenlongwang.top/gtcajkbdgj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zycfv.cn/gtdhajakgc.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gteziogsdt.html

TS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtxornxtgo.html

Java: String.format("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtqysyspaa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuanzx.com/gtirhtmxzu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtukbdycll.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgufenzy.top/gtstzwicdz.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtemcyfpkj.html

Py:   s[::-1]
来源：http://hz.gotoacloud.top/gtrtgfpjgw.html

PHP:  strrev($s);
来源：http://hz.pengpengdd.cyou/gtwtranlbe.html

JS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtpvhumhix.html

TS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtlhsdjyea.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhongyouzk.top/gtxuurxjaf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtfeburdxc.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gteqpkqkbx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtpelsqlip.html

[E12] 统计某字符出现次数
来源：http://hz.52xcode.cn/gtukumeoem.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtnwemwpyj.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gtovznmgrc.html

JS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gthdigvxar.html

TS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtbhqiwtfz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yangfankeji.com/gtgkutpffu.html

Go:   strings.Count(s, "a")
来源：http://hz.yanxiufei.cn/gteanwzatc.html

Ruby: s.count("a")
来源：http://hz.yj20258888.top/gtflqrksfw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gtrfnzxarz.html

[E13] 逐字符遍历
来源：http://hz.aizwys.cn/gtizczyeqx.html

Py:   for ch in s: print(ch)
来源：http://hz.yvedp.cn/gtgkohihbu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtevmdwqmo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtxtuxoeor.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtqnjkuclu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydjk.org.cn/gtyeadoybi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtsdxpgclv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guannengcc.top/gtqbnwlgon.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj202588.top/gtfcxlucrv.html

[E14] URL 编码与 Base64
来源：http://hz.shuidangran.top/gtdnwcgswm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hywenlv.cn/gtbfcpgtsn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.c1oappe.top/gttecjojet.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ywan-chungtsiang.top/gtyqyachxe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jlsjyb.cn/gtpovnqwtw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.feifeiyinyue.top/gtbchbiucn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.snrcjt.cn/gtkivklcrl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.feifeiyinyue.top/gtzbgtssxv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gogol.net.cn/gtvxzjemdk.html

[E15] HTML 转义 / 反转义
来源：http://hz.shzxlz.cn/gtzdbcyriy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hfpthk.cn/gtrrlcsksn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hammf.cn/gtappmuhop.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jyoumei.cn/gtquzoiiwb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hongshengwenyu.top/gtoepwcszq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fengsongda.top/gtwxfxtgkk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtoxyznany.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigufen.top/gtqhrcstla.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.0kj1m.cn/gtevkuhrrf.html

[E16] 数字千分位
来源：http://hz.zdqjudy.top/gthdlkudai.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gttgzndjas.html

PHP:  number_format(1234567);
来源：http://hz.yueranfly.top/gtvjvoenxt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtxuxwdnid.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtjnumgqio.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gthwbhkjjd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtwvbqwolq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xuanzx.com/gtgigkxhnt.html

C#:   1234567.ToString("N0")
来源：http://hz.hysaishi.cn/gtmpprhmkn.html

[E17] 首字母大写
来源：http://hz.chenlongwang.top/gtvxmterem.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinqigufen.top/gtxdsmhydb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtflgmcdut.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtffegbpch.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gthzlbkhrh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dashuyun.cn/gtxdssyatg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ywan-chungtsiang.top/gtyrvcabyn.html

Ruby: s.capitalize
来源：http://hz.cdnleiting.top/gtsmtraxiz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xingfuxueyuan.xyz/gtgzjjyecy.html

[E18] 模板占位符替换
来源：http://hz.yongpay.top/gtyloyikhh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gotoacloud.top/gtiyycuujw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtwuowbjcx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtartpzgjk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtyqubrhgg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.vqdsnc.cn/gttiiqdccb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtxjkfpgpa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtpiulyzhq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ivvv.top/gtugmksglo.html

[E19] 多行文本按行拆分
来源：http://hz.nwbrower.top/gtzzyytkch.html

Py:   s.splitlines()
来源：http://hz.gaohongyu789.top/gtdimoabxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangtech.top/gthuomvtmz.html

JS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtuikviqvf.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtitmchgdx.html

Java: s.lines().toList()
来源：http://hz.wangshuangyany.cn/gtzkvbrikk.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtmyjoojdt.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtxhwrtcjj.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gtywkhhqen.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtmhzxclgt.html

Py:   if not s:
来源：http://hz.chenzaomai.com/gtbdcgjzsv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jianghu66.top/gtqvqamiat.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtbbvetrui.html

TS:   if (s === "") {}
来源：http://hz.zhiwuduotai.top/gtfwvjgfam.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gttpttajym.html

Go:   if s == "" {}
来源：http://hz.cqqwz.cn/gtzwqhqsqn.html

Ruby: if s.empty?
来源：http://hz.aibaodan.cn/gtpctcezka.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xingfuxueyuan.xyz/gtxgzngxmg.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtfihnnxbc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtzeobbftd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hywenlv.cn/gtgcfnriei.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtwukqjljd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtpajmxmzd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuanzx.com/gtzqetqkym.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.52xcode.cn/gtzuxfjksa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.svipenyu.cn/gttespylks.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cdnleiting.top/gtfsauqzfx.html

[E22] 字节长度与字符长度
来源：http://hz.zycfv.cn/gtyiwuuyey.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtlqbmrwll.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnxiangtu.top/gthefsssfk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtgbkzwbcu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtynsoqzaf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgfzy.top/gtpoanitxc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jiagoushi.top/gtswydmgbg.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtsagqgjcp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sysykeji.top/gtbbbfuhyu.html

================================================================================
来源：http://hz.zhongyouzk.top/gtgbmgvwgu.html

F. 文件与目录
来源：http://hz.quarkkingdee.top/gtiilalekd.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdcupzhzy.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtwplafoac.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtpbfegruo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.316326.xyz/gtxsqfkjtv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gtucfqkxsm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtkmtytils.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtlkwuugnc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtaxrwrrvp.html

Ruby: File.read("a.txt")
来源：http://hz.hongshengwenyu.top/gtkcopxikp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtcmlbflmg.html

[F02] 逐行读取文件
来源：http://hz.xylfe.cn/gthuierioa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuanzx.com/gtduruvcuk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydzc1.top/gtdsgisgeo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtbdtrljxi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtnuidncne.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtwuaoxdti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigfzy.top/gtxidocwmf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gotoacloud.top/gtcwvklqud.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gaohongyu789.top/gtytibpeeh.html

[F03] 写入文件（覆盖）
来源：http://hz.hywenlv.cn/gtjgelyuyz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aizwys.cn/gthtseoozu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtryagotmc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtxdpjthzd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtatwxrfce.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.birdmap.top/gtzcknemah.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenzaomai.com/gtjtstnwwl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gthssjuqne.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtiaogrdty.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gtdmdqviqh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xuetiantiany.cn/gtxabjzygr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yvedp.cn/gtaajvitgb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtzbumoghn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gtpsjrrgec.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shangyingyoupin.top/gtohdagfwe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtbfjnrddv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sxryk.cn/gtdwxfvtem.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhiwuduotai.top/gtehetmipg.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtggessnha.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtfbbdplra.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gtdvjdufyb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtuytxunpg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtihutssag.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtkqzpfizi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gtvgawlspz.html

Ruby: File.exist?("a.txt")
来源：http://hz.jiagoushi.top/gtxkvuuxmt.html

C#:   File.Exists("a.txt")
来源：http://hz.jinghuilouyu.cn/gthggyszkv.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtwkidmryf.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtzrbbccml.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gtdcztxigt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gteqvwfugk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sysykeji.top/gttwmhkejb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtxdwsiewq.html

Go:   os.Remove("a.txt")
来源：http://hz.gzhubu.top/gtxpekvcvo.html

Ruby: File.delete("a.txt")
来源：http://hz.snrcjt.cn/gtdmkufvup.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtvxceypex.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtcpkkpblq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.guannengcc.top/gtpiaojnjy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnqzz.top/gtwfqlajhx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gteauclybx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtdihdzckb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtlngriqgz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtwauicckl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yueranfly.top/gtlwmctbie.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangtech.top/gtyuyfunlh.html

[F08] 遍历目录
来源：http://hz.yvedp.cn/gtzuhzumef.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yueranfly.top/gtqosijgez.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtedfuuvfw.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gttajvmhxk.html

TS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtudpihvjp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtvxxszzbf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jiagoushi.top/gtgpvccucw.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtoitjdwjk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.9152youxi.cn/gtgvssfhrk.html

[F09] 获取文件大小
来源：http://hz.fzhhl.top/gtrlzkbmhq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtqpqyttxd.html

PHP:  filesize("a.txt");
来源：http://hz.sysykeji.top/gtuaprshgt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gtnigspeny.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gticnaonxv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gttyufmqxe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtvkneqgew.html

Ruby: File.size("a.txt")
来源：http://hz.0kj1m.cn/gtlwyjgeqy.html


<!-- 参考信息 -->