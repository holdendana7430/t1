代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhoulong.xyz/gtuatandmu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtincxviyz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shangyingyoupin.top/gtecylrxiz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gogol.net.cn/gtvbvehmgp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.smart0.xyz/gtpsxoeord.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yueranfly.top/gtrlwvvknq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daria6918.cn/gtihnzmunx.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtixgmzujc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenzaomai.com/gtwryuiyhu.html

PHP:  implode(", ", $arr);
来源：http://hz.hnxiangtu.top/gtezktmugr.html

JS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtygtyexso.html

TS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtpnnvskti.html

Java: String.join(", ", list)
来源：http://hz.yanxiufei.cn/gtqafncmlk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxinkj.top/gtwglasvbj.html

Ruby: arr.join(", ")
来源：http://hz.svipenyu.cn/gtfpgpzzds.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtzapqgwps.html

================================================================================
来源：http://hz.shuidangran.top/gtsrnsghxz.html

E. 字符串处理
来源：http://hz.hammf.cn/gtcmlqdaij.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqauooqeb.html

[E01] 拼接字符串
来源：http://hz.hfpthk.cn/gtbbtvecsi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangkeji.top/gtypvayhvi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gaohongyu789.top/gtqqnlpldi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gttnqezvjw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtbrguifpv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.c1oappe.top/gtzdbkllql.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gttvmyhchx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gtitlsmqnz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenjidiqi.icu/gtnqlwohpx.html

[E02] 重复字符串
来源：http://hz.jqgfzy.top/gtfnbnhblv.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gttasuxhnd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pengpengdd.cyou/gtniiohdmp.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtnyljslis.html

TS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtabhfftgn.html

Java: "ab".repeat(3)
来源：http://hz.sysykeji.top/gtdpbtrvjy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.vqdsnc.cn/gtxxqjkvce.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtfwnhsyns.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sufxvd.cn/gthipxqtoo.html

[E03] 截取子串
来源：http://hz.fengsongda.top/gtxxonskaw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dianchejie.cn/gtujysfmmn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gtkieshglh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtwqsqridz.html

TS:   s.slice(1, 4)
来源：http://hz.ivvv.top/gtxgnkxkvl.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtiufxibdn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhengqikj.top/gtcflkivgz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aibaodan.cn/gtggdvscsu.html

C#:   s.Substring(1, 3)
来源：http://hz.xuanzx.com/gtosjbqykb.html

[E04] 查找子串位置
来源：http://hz.dianchejie.cn/gtvcivdxla.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ivvv.top/gttcakzotm.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtwocglrbg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtkrzekfxf.html

TS:   s.indexOf("x")
来源：http://hz.tian-w.cn/gtwqqcxhad.html

Java: s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtpbywuhdh.html

Go:   strings.Index(s, "x")
来源：http://hz.0kj1m.cn/gthasecwoi.html

Ruby: s.index("x")
来源：http://hz.gzhubu.top/gtrqrqwuum.html

C#:   s.IndexOf("x")
来源：http://hz.guannengcc.top/gtqccdqveb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtutswimso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gotoacloud.top/gtxdkautoa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guowangkeji.top/gtcapyagie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ywan-chungtsiang.top/gtrhbjhsot.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtvzbwndnf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtclviaemn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.wangdashe.top/gtylkobugt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jiagoushi.top/gtgovqrgxv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xinyue.icu/gttstaimbc.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtlzkgisxm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtfkoirakw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.kuanghao11.cn/gtozqlaibj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtlrzxhcsq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtozjsdncd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtwdzcnnwz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtwfbftphx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guowangkeji.top/gtclmrnnid.html

C#:   s.Replace("a", "b")
来源：http://hz.jiagoushi.top/gtlbndsttx.html

[E07] 按分隔符拆分
来源：http://hz.hnxiangtu.top/gtstnrvxqh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hysaishi.cn/gtstzkywgj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtkhdecsdd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuxming.cn/gtzlinjani.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtybggmhcc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.feifeiyinyue.top/gtxiintpyl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtqxxkiheg.html

Ruby: s.split(",");  s.split
来源：http://hz.jyoumei.cn/gtnvkatiic.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zycfv.cn/gtclimutzh.html

[E08] 数组按分隔符合并
来源：http://hz.yueranfly.top/gtbfjuopjl.html

Py:   ",".join(items)
来源：http://hz.jinqigfzy.top/gtnrgzstmd.html

PHP:  implode(",", $items);
来源：http://hz.zhiwuduotai.top/gtzwbgtkgf.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtcifrnlgn.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gttpwljgvn.html

Java: String.join(",", items)
来源：http://hz.xziqi.cn/gtflygowsp.html

Go:   strings.Join(items, ",")
来源：http://hz.52xcode.cn/gtuzzfiedz.html

Ruby: items.join(",")
来源：http://hz.daria6918.cn/gtcfnyikqn.html

C#:   string.Join(",", items)
来源：http://hz.xuanzx.com/gtftmjxdwh.html

[E09] 去除所有空白字符
来源：http://hz.xingfuxueyuan.xyz/gtdkzgfhym.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhiwuduotai.top/gtutedrtbs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtycxsjpwx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtisojszme.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtlsubcvvh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guowangkeji.top/gthnoevvyw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yueranfly.top/gtkxisqfte.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtemddaznn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gtaxoxwfyx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shanyushiyangkeji.top/gtvdhymxge.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuetiantiany.cn/gtikdxuplh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xuanzx.com/gtgcwscvjl.html

JS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtpdsdnyiz.html

TS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtvjmbjgyd.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtzmhensyn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sysykeji.top/gtaftmezpm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtbbvpxtkz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sweek.top/gtjguatdjr.html

[E11] 反转字符串
来源：http://hz.jinqigfzy.top/gtkdbmwvht.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtleqecskf.html

PHP:  strrev($s);
来源：http://hz.cucudq.cn/gtzcwjyczt.html

JS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtyofiyhkp.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gteflnpxfm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hywenlv.cn/gtuppvxmix.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gttcpvkgfm.html

Ruby: s.reverse
来源：http://hz.yonumen.top/gtchoofjeg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gteundntnx.html

[E12] 统计某字符出现次数
来源：http://hz.snrcjt.cn/gtsawvngbl.html

Py:   s.count("a")
来源：http://hz.zhaomingkeji.xyz/gttvhiqccc.html

PHP:  substr_count($s, "a");
来源：http://hz.kuanghao11.cn/gtotkbnmtp.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtefaeoaed.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtpnsfklou.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtdeikzhyz.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtvjsmjzry.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gtertipige.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenzaomai.com/gteathaxqe.html

[E13] 逐字符遍历
来源：http://hz.jqgfzy.top/gtyuhxjnsx.html

Py:   for ch in s: print(ch)
来源：http://hz.aizwys.cn/gtokobvlwq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtprojkpgv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtwhpcujbo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.snrcjt.cn/gtcfulypjj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtjaggcgdz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shuidangran.top/gtrqogwxuq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtrghytkcj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangtech.top/gtbsfcuhty.html

[E14] URL 编码与 Base64
来源：http://hz.yuanzhike.top/gtwrdwcerz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtcotmjwte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cheryme.top/gttipcpylq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jiagoushi.top/gtlvdbmcvi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.0kj1m.cn/gtdvdmtxuu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daria6918.cn/gtmkxgwofx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fzhhl.top/gtsbsyiixg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yongpay.top/gtffkhuhav.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gtcpkeileu.html

[E15] HTML 转义 / 反转义
来源：http://hz.cheryme.top/gtcnwvafbj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gogol.net.cn/gtdyqkfyuk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinyuanbaomall.cn/gtcygxvykh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtlocxxlar.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pycfn.com/gtkjhxlsso.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tanke756.top/gtmwnanbzj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtzezdbsbu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtyhizyipq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gzhubu.top/gtlkglgzdl.html

[E16] 数字千分位
来源：http://hz.shuidangran.top/gtafikyaic.html

Py:   f"{1234567:,}"
来源：http://hz.9152youxi.cn/gtmnfaawqw.html

PHP:  number_format(1234567);
来源：http://hz.zhengqikj.top/gtsjiymtsi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gthuhzmpoa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtcztxjqlm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhongyouzk.top/gtagrjvolx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gtxadrrove.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ivvv.top/gtzwpoisic.html

C#:   1234567.ToString("N0")
来源：http://hz.hnqzz.top/gtnywrlsna.html

[E17] 首字母大写
来源：http://hz.52xcode.cn/gtxxmaaubi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.c1oappe.top/gtpngqoyep.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gtoetrvwcu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gteaccvxjv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtrdnjrkdr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gtbfsqyioc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shangyingyoupin.top/gtnklbdoyy.html

Ruby: s.capitalize
来源：http://hz.gotoacloud.top/gtxgsjkdmr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jiagoushi.top/gtnkbnbror.html

[E18] 模板占位符替换
来源：http://hz.jianghu66.top/gtvwzkzwgc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtnugbztjb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigfzy.top/gtivviposx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtxqmauryr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtfcrjctfq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zycfv.cn/gtzneiyovj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jiagoushi.top/gtapaebnoh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhengqikj.top/gtalhwzjub.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cheryme.top/gtnwizojic.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gtnkunhqxe.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtgeylostj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gtrbnttnec.html

JS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtdutiehde.html

TS:   s.split(/\r?\n/)
来源：http://hz.vqdsnc.cn/gtibsgxrjb.html

Java: s.lines().toList()
来源：http://hz.haohaochexian.top/gtztkesrty.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtmxnjlqfk.html

Ruby: s.lines
来源：http://hz.jianghu66.top/gtfxcyqroz.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gtkwcxzgpt.html

[E20] 判断字符串是否为空
来源：http://hz.aibaodan.cn/gtueyyvzxy.html

Py:   if not s:
来源：http://hz.gotoacloud.top/gtdrfqvxsw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pengpengdd.cyou/gtywxsbagp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258888.top/gtwliwndjw.html

TS:   if (s === "") {}
来源：http://hz.hnxiangtu.top/gtfrsykpic.html

Java: if (s.isEmpty()) {}
来源：http://hz.nanxinkj.top/gttjkbdwmt.html

Go:   if s == "" {}
来源：http://hz.guowangkeji.top/gtexupviho.html

Ruby: if s.empty?
来源：http://hz.yuxming.cn/gtmbqqmedf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gthzvnnhwi.html

[E21] 超长截断加省略号
来源：http://hz.ywan-chungtsiang.top/gtfxeygfqc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guannengcc.top/gtiqcxrtow.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.havefunace.top/gtvxlecxac.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtodcosqyx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtcimxhvah.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258.top/gttkxrrgnd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtqfswwfar.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.0kj1m.cn/gtywgpslek.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gthtnylgza.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtroxzfquf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtacqhkcsw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtxxwxbdpe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtmdpcmavk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gttwdgptxp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.andypj.xyz/gtuonxlfmc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gtfpchkcez.html

Ruby: s.bytesize;  s.length
来源：http://hz.tianlin.xyz/gtcqrfhuxs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shuidangran.top/gtparqyemu.html

================================================================================
来源：http://hz.iojbl.cn/gtgjqnzoie.html

F. 文件与目录
来源：http://hz.fengsongda.top/gtpnxxvkhs.html

================================================================================
来源：http://hz.sxryk.cn/gtkrfabfpu.html

[F01] 读取整个文件
来源：http://hz.wangshuangyany.cn/gtnsbzlfiv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangshuangyany.cn/gtzyagppmb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.9152youxi.cn/gtajushtps.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtkkunnzml.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fzhhl.top/gtwitubtxp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtiezvbhbb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xinyue.icu/gtzdojtggi.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gtpzunkiar.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.bjfxy.top/gtjtmocexq.html

[F02] 逐行读取文件
来源：http://hz.cdnleiting.top/gtbvcrkvgc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtlamlrxal.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydjk.org.cn/gtxbhotbqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtuktciblp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtfwnumefa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtqkauztvx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenjidiqi.icu/gtuzhtynqm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhijiandao.cn/gtbkxgdwrs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.9152youxi.cn/gtgmwzmfeg.html

[F03] 写入文件（覆盖）
来源：http://hz.ehwqpu.com/gtrbgefcvw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gogol.net.cn/gtbjghfwwp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gtqcextpvs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtempktlvy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gttamwqokl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yongpay.top/gtekovipcb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtjgyedzhd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtpforjrlc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yonumen.top/gtnolxfnwu.html

[F04] 追加写入文件
来源：http://hz.wangdashe.top/gthirmonqx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tianlin.xyz/gtmqbbllzg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydjk.org.cn/gtmkhummrx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gthwsvckpq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cucudq.cn/gtuezxjqfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.havefunace.top/gthosfwgea.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ywan-chungtsiang.top/gtzpttwgzz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ybcxt.top/gtrtazbexa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ppjwa.cn/gtyjcxubkq.html

[F05] 判断文件或目录是否存在
来源：http://hz.yanxiufei.cn/gtxjanuevu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xziqi.cn/gtuahtrlnb.html

PHP:  file_exists("a.txt");
来源：http://hz.bjfxy.top/gtuptionio.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtijixibib.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtcodazsst.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gttcecosec.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtsoyxwrsp.html

Ruby: File.exist?("a.txt")
来源：http://hz.ppjwa.cn/gtopkmgtwx.html

C#:   File.Exists("a.txt")
来源：http://hz.yonumen.top/gtxukefbze.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gttqtetxil.html

Py:   os.remove("a.txt")
来源：http://hz.xylfe.cn/gtouctnugw.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258.top/gtfudehmev.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtbxnlicod.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtshvukbsz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtiobscntm.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtcdnhsuft.html

Ruby: File.delete("a.txt")
来源：http://hz.zycfv.cn/gtkysxchri.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtgqziovum.html

[F07] 创建目录（含多级）
来源：http://hz.sweek.top/gtcfvxtdav.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yongpay.top/gtviwgjwyg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fengsongda.top/gtgiiwhloa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtgiqjorlk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtzyhbmknz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tian-w.cn/gtsiprpjvl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gogol.net.cn/gtrnfojfbl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yangfankeji.com/gtteeyeqny.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtwgqjwdfy.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtbgawmogu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgfzy.top/gtmgirfcai.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigufen.top/gtdfamxcgi.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtzfjqwcxt.html

TS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtptovujsn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtfwwgbqaj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guowangkeji.top/gtirdbimiy.html

Ruby: Dir.children("dir")
来源：http://hz.guowangkeji.top/gthekwaudn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sysykeji.top/gtcveitill.html

[F09] 获取文件大小
来源：http://hz.52xcode.cn/gtmfgcebjm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhiwuduotai.top/gtqduyaawv.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtxigmbqgo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtpwdstgix.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtikqclwlb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtjwswhfmx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xingfuxueyuan.xyz/gtowdbbbuu.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gthlhszmuo.html


<!-- 参考信息 -->