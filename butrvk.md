代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangshuangyany.cn/gtpgcvdopy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtozbwfgdo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenzaomai.com/gtjmcoaqxn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtiymfwwqk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.havefunace.top/gtbkvlzfub.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gteqaaucri.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtqcfxcqmx.html

[D26] 数组转字符串
来源：http://hz.jianghu66.top/gtnngojfml.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shuidangran.top/gtcvwroffx.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtjtgujhxg.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gttnrijizg.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtdoclqjkj.html

Java: String.join(", ", list)
来源：http://hz.dianchejie.cn/gtdgfwngbm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sufxvd.cn/gtdlysijwf.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gturqueava.html

C#:   string.Join(", ", list)
来源：http://hz.hnxiangtu.top/gtvncayixj.html

================================================================================
来源：http://hz.ydzc1.top/gtvtwxcmvw.html

E. 字符串处理
来源：http://hz.xingfuxueyuan.xyz/gtrcujvsjd.html

================================================================================
来源：http://hz.sufxvd.cn/gtxmjtmpmh.html

[E01] 拼接字符串
来源：http://hz.hnqzz.top/gtpdxtmasx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.mhx1999.top/gtmztccjtz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenzaomai.com/gtpxjeoofa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daxiang520.top/gtthyfugks.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtlojzbfjy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nwbrower.top/gtwxbtpvpj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ppjwa.cn/gtutkwlsdn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenzaomai.com/gtbweynqme.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtavledkxy.html

[E02] 重复字符串
来源：http://hz.zdqjudy.top/gtiruifqdk.html

Py:   "ab" * 3
来源：http://hz.jinghuilouyu.cn/gtliibaypc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yanxiufei.cn/gtdumpxflm.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtmxzaelch.html

TS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gttdbqzxtt.html

Java: "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtxqqyvbph.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnqzz.top/gtsehbwpwu.html

Ruby: "ab" * 3
来源：http://hz.sysykeji.top/gtebfujsph.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhengqikj.top/gtmiurrfgx.html

[E03] 截取子串
来源：http://hz.jqgfzy.top/gtukfkfwcn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinyuanbaomall.cn/gtgthtkgyy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.haohaochexian.top/gtvzgtnbpl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sweek.top/gtxfyurxnh.html

TS:   s.slice(1, 4)
来源：http://hz.zhongyouzk.top/gtzwkbczes.html

Java: s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtvgxbaefe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guannengcc.top/gtyahvwrwh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gtfourzqec.html

C#:   s.Substring(1, 3)
来源：http://hz.hammf.cn/gtsihmhazw.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gtzzlzdcvo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sufxvd.cn/gtmvbjboic.html

PHP:  strpos($s, "x");
来源：http://hz.quarkkingdee.top/gtwjrsgppt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenzaomai.com/gtvsuxkbav.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtbrukaxcv.html

Java: s.indexOf("x")
来源：http://hz.yuxming.cn/gtzugioktk.html

Go:   strings.Index(s, "x")
来源：http://hz.zhaomingkeji.xyz/gtubxmxvai.html

Ruby: s.index("x")
来源：http://hz.zhijiandao.cn/gtcdpyvftl.html

C#:   s.IndexOf("x")
来源：http://hz.cqqwz.cn/gtcqsrejyy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tian-w.cn/gtsbjmgmhx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cashguo.top/gtpasvcvkk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtlltyozlo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtzrgtkman.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ywan-chungtsiang.top/gttiyynuev.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zycfv.cn/gtagezoypm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hywenlv.cn/gtwffughml.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nwbrower.top/gttacovlgw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.9152youxi.cn/gttggglpid.html

[E06] 替换子串
来源：http://hz.zhixingplan.top/gttijmpnfe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.daria6918.cn/gtbwjgzbwr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dashuyun.cn/gtbvmcaayj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtdqieewrv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtyapdksdx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtmmxeyfms.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.0kj1m.cn/gtmygzpqyb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.wangdashe.top/gtshrnkltm.html

C#:   s.Replace("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtdbbowkfz.html

[E07] 按分隔符拆分
来源：http://hz.yangfankeji.com/gtfhauzrfd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.feifeiyinyue.top/gtxjnemyjg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuetiantiany.cn/gtvlsrmila.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.guowangkeji.top/gtptmolacs.html

TS:   s.split(",")
来源：http://hz.xuetiantiany.cn/gtarfdihdp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gtghakflei.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigfzy.top/gtjkgilprj.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigufen.top/gtaqgjwert.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtnvsmlfqr.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258888.top/gtznoysoif.html

Py:   ",".join(items)
来源：http://hz.shzxlz.cn/gtlpswahzx.html

PHP:  implode(",", $items);
来源：http://hz.jinqigufen.top/gtftidljmu.html

JS:   items.join(",")
来源：http://hz.jiagoushi.top/gtlbcupazz.html

TS:   items.join(",")
来源：http://hz.yvedp.cn/gtshanfdxl.html

Java: String.join(",", items)
来源：http://hz.birdmap.top/gttzpwnggz.html

Go:   strings.Join(items, ",")
来源：http://hz.jlsjyb.cn/gtxlqypsjo.html

Ruby: items.join(",")
来源：http://hz.shzxlz.cn/gtypptnrzy.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gtsabacfdx.html

[E09] 去除所有空白字符
来源：http://hz.cashguo.top/gtzbffddke.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtnabtaati.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtbzzwizbb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtynrnupvx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtksjfmwxj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangshuangyany.cn/gtdpwmxxow.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ivvv.top/gtogrmxtcb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuanzhike.top/gtlvjplpse.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydzc1.top/gtmyaddkon.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gttovpgsaz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtuqnpgien.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xuanzx.com/gtgdkxuvwh.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtrpgeknfg.html

TS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtwiqaqyul.html

Java: String.format("%03d", 7)
来源：http://hz.meibo888.top/gtxsfsaowa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jlsjyb.cn/gtmvvuprfh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xuanzx.com/gtxvoaimel.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yanxiufei.cn/gtakybqyoj.html

[E11] 反转字符串
来源：http://hz.cashguo.top/gtobawzqsy.html

Py:   s[::-1]
来源：http://hz.yueranfly.top/gtlrmicvkw.html

PHP:  strrev($s);
来源：http://hz.tian-w.cn/gtdomyyume.html

JS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtsmdypdpf.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtlctncngt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.0kj1m.cn/gtstrxpkda.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtmiknfxsw.html

Ruby: s.reverse
来源：http://hz.yangfankeji.com/gtuhfdmgzw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtxbvwcomk.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtupxjcdlc.html

Py:   s.count("a")
来源：http://hz.guowangkeji.top/gtygodfsav.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtqvwucwuv.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gttwaupadz.html

TS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtsrhhtxof.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gtumvutcji.html

Go:   strings.Count(s, "a")
来源：http://hz.yvedp.cn/gtqodjciur.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtopetyeab.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinyuanbaomall.cn/gtrzqidnyl.html

[E13] 逐字符遍历
来源：http://hz.chenjidiqi.icu/gtneqcvwpg.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gtqrtpupux.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.vqdsnc.cn/gtqlmczbpt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtnmwlwcmd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtqcfnsjdx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinghuilouyu.cn/gttdxisbah.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.kuanghao11.cn/gtjerbosgr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtsjwzemdn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtfnloupdx.html

[E14] URL 编码与 Base64
来源：http://hz.hnxiangtu.top/gtajtoydcp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.meibo888.top/gtvrzgquft.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtosuavicu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jlsjyb.cn/gtllhxxnzg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aizwys.cn/gtfxhcrenh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ppjwa.cn/gtrarxgvvp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtdplpojeb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtadqzjfdh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtlfkcfuzy.html

[E15] HTML 转义 / 反转义
来源：http://hz.shzxlz.cn/gtigssmyqp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtvhblezwy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shangyingyoupin.top/gtpwfhhsif.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenzaomai.com/gtzsabsuhq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fengsongda.top/gtpzivgysb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hammf.cn/gtnnsfcrfz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.smart0.xyz/gtsmxqafyk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shuidangran.top/gtyeqffqaf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sxryk.cn/gtaabthlrm.html

[E16] 数字千分位
来源：http://hz.andypj.xyz/gtqgsoezsi.html

Py:   f"{1234567:,}"
来源：http://hz.pengpengdd.cyou/gtxvyrxnku.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gthegtputn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtsvsfphoc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtesztvtan.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sufxvd.cn/gtbimslxis.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sxryk.cn/gtrnuhwncl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aibaodan.cn/gtzzhjdhwh.html

C#:   1234567.ToString("N0")
来源：http://hz.yuxming.cn/gtrziiomij.html

[E17] 首字母大写
来源：http://hz.wangshuangyany.cn/gtnuneusbk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.52xcode.cn/gtieecwdsb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhaomingkeji.xyz/gtzeyrknqf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtxecmcuxa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtjxqfqrsy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.mhx1999.top/gtemdoxbrf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258.top/gtvqjwrrsw.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtykzabdoz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangkeji.top/gtwvkkuhuv.html

[E18] 模板占位符替换
来源：http://hz.ywan-chungtsiang.top/gtahgbltfd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenlongwang.top/gtobhovyxl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtuxxaaksi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtvowvtjuc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtppymienq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhongyouzk.top/gtipjcthhz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.feifeiyinyue.top/gtvzkoyvdp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.iojbl.cn/gtitqvhwvh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.birdmap.top/gthkzneibp.html

[E19] 多行文本按行拆分
来源：http://hz.hongshengwenyu.top/gtgrpjpzvh.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gtwuwicfhf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.kuanghao11.cn/gtcvpmrxey.html

JS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtwmphtosg.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtnmasktqi.html

Java: s.lines().toList()
来源：http://hz.jianghu66.top/gtpncqufcw.html

Go:   strings.Split(s, "\n")
来源：http://hz.yueranfly.top/gtpmitcdpp.html

Ruby: s.lines
来源：http://hz.andypj.xyz/gtphvhcfsa.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gtztdqihhq.html

[E20] 判断字符串是否为空
来源：http://hz.quarkkingdee.top/gthbotrdfm.html

Py:   if not s:
来源：http://hz.nwbrower.top/gtuazkriqk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cucudq.cn/gtkkfxhydk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gtlohjqczn.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtstieynce.html

Java: if (s.isEmpty()) {}
来源：http://hz.pycfn.com/gtfhxkxale.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtlmbggzbf.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtcygmxlsn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guowangkeji.top/gtxfxqalmk.html

[E21] 超长截断加省略号
来源：http://hz.jyoumei.cn/gtssjfrrgq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.meibo888.top/gthmmjoqgb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtovpmqcqf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtjiedxapd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtwhpmldpj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtaflqdwdq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnqzz.top/gttdfffvhi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daxiang520.top/gtpzfkshzw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgfzy.top/gtgzwjbsxn.html

[E22] 字节长度与字符长度
来源：http://hz.yuxming.cn/gtvvlsycxz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fzhhl.top/gtssppulfv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtuckiuanh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtnmmcfgld.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cdnleiting.top/gtwtveisii.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gthraykvkn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtdlybgoel.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangshuangyany.cn/gtdazdxqsj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtvmjgimzj.html

================================================================================
来源：http://hz.mhx1999.top/gtrvmagnfz.html

F. 文件与目录
来源：http://hz.cheryme.top/gteqsmuujw.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqgjlfful.html

[F01] 读取整个文件
来源：http://hz.yangfankeji.com/gtbkxohrlm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gthcykryse.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtjbwxzrad.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxinkj.top/gtcqwbarxo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.kuanghao11.cn/gtbdymccix.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtbiaefhlz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtjsnfjdeu.html

Ruby: File.read("a.txt")
来源：http://hz.guowangkeji.top/gteqteiumx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cucudq.cn/gtkgxluiam.html

[F02] 逐行读取文件
来源：http://hz.xuanzx.com/gtrnhvjxrp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sufxvd.cn/gtiwftklwz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ybcxt.top/gtgqmyggzx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtslaxxklo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gthqjeymqc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtxkmhfaps.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtckdlpjem.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daria6918.cn/gtvhcbnbeg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgfzy.top/gtkxtmnels.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gtfqybxmaz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtjghsizgb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yongpay.top/gtkkvkdtrj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtrloowkbv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtjsssknqg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtwxwdwrvh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenjidiqi.icu/gtvrwzkhyn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtqoqwowmt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuanzx.com/gtomzcuwxy.html

[F04] 追加写入文件
来源：http://hz.zhiwuduotai.top/gtshykvltp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtxruxihhi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ivvv.top/gtawjxlqde.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtjozqkeih.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtnilbuhsb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtcaveejnv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtjbciirbv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuetiantiany.cn/gtrxznfdss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtpxogfzye.html

[F05] 判断文件或目录是否存在
来源：http://hz.mhx1999.top/gtifxxjopt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtpiyfsreg.html

PHP:  file_exists("a.txt");
来源：http://hz.chenlongwang.top/gtnghwdzxy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtpknknbiv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.svipenyu.cn/gtcyyqggmr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtlcbsavzn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.9152youxi.cn/gtalgmirwm.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gtcbhwyvkt.html

C#:   File.Exists("a.txt")
来源：http://hz.hfpthk.cn/gtzxhophot.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtjfthgeue.html

Py:   os.remove("a.txt")
来源：http://hz.jqgfzy.top/gtvwqtusyn.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gtliknllsz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtduxkamhp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtixebgecw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtqjdjhvvz.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtyncelqoy.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigfzy.top/gttccdrxnp.html

C#:   File.Delete("a.txt");
来源：http://hz.smart0.xyz/gthewpsbvw.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtlhljkfke.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtprwwhozf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtjoikgneh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtofumakds.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtrcpezsiy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shzxlz.cn/gthaezxwex.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gthsbvdpob.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtmuypfstj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shuidangran.top/gtqtreboam.html

[F08] 遍历目录
来源：http://hz.jlsjyb.cn/gtmhucwrun.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtywiuvonk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cheryme.top/gtaorrskgg.html

JS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtidwfzvme.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtxuyvfdzo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shangyingyoupin.top/gtddntkoap.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.birdmap.top/gtecjaljyt.html

Ruby: Dir.children("dir")
来源：http://hz.hywenlv.cn/gtkmeledwt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hammf.cn/gtxgmvprjc.html

[F09] 获取文件大小
来源：http://hz.zdqjudy.top/gtotploslx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gtbjakkqbb.html

PHP:  filesize("a.txt");
来源：http://hz.tianlin.xyz/gtpkycbcic.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtidnnpmnc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtozvwqlpa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtlayqiexl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guannengcc.top/gtrriscpny.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtvdjqefpi.html


<!-- 参考信息 -->