代发 wailian999

================================================================================
来源：http://hz.yuxming.cn/gtrqozldqa.html

E. 字符串处理
来源：http://hz.fengsongda.top/gtaqxydulx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmmgdiztp.html

[E01] 拼接字符串
来源：http://hz.shzxlz.cn/gtwaqabspa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenzaomai.com/gtycwrurhn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangshuangyany.cn/gtgmriodim.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtvddanlqn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtgbiypyhp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gzhubu.top/gtsussyesg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtbmpngonj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nwbrower.top/gtohtnneoa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jyoumei.cn/gttvkkkamb.html

[E02] 重复字符串
来源：http://hz.cashguo.top/gtagosceij.html

Py:   "ab" * 3
来源：http://hz.pycfn.com/gtiiymymdf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ehwqpu.com/gtntjumdmt.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258888.top/gtwuhhysxj.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtwrvhrvrd.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtqumujuxn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gthzwfsoxj.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtunzugloo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenlongwang.top/gtwqgknvwf.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtkjgtkojt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinghuilouyu.cn/gtciswcyci.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daxiang520.top/gtqbjfkvuh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtybfciuog.html

TS:   s.slice(1, 4)
来源：http://hz.guowangkeji.top/gtvkcdksie.html

Java: s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtisdxuawg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtfjisqxmu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.kuanghao11.cn/gtofyqeize.html

C#:   s.Substring(1, 3)
来源：http://hz.xziqi.cn/gtmlmsgnfh.html

[E04] 查找子串位置
来源：http://hz.zhengqikj.top/gtunqgraic.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtktwrgotv.html

PHP:  strpos($s, "x");
来源：http://hz.sysykeji.top/gtlkqonmpf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgufenzy.top/gtuztqplzc.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtggfhgaex.html

Java: s.indexOf("x")
来源：http://hz.c1oappe.top/gthcenuuvd.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtjofdecws.html

Ruby: s.index("x")
来源：http://hz.zdqjudy.top/gtlztjwkrf.html

C#:   s.IndexOf("x")
来源：http://hz.yvedp.cn/gtwfqeiihh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtitffkzob.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangdashe.top/gtgotrsvbe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daria6918.cn/gtthdivtyd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtogwkomjz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.svipenyu.cn/gtywfgvfpv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtsvxaoljd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cqqwz.cn/gtkbejgcwu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhengqikj.top/gtdbzyznvo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guowangkeji.top/gtrkjfwgcf.html

[E06] 替换子串
来源：http://hz.shzxlz.cn/gtsrfoihqn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtbgsjgzig.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj202588.top/gthnflpaei.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtyvczcgqa.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtniqmlqqe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtuebxguuw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ybcxt.top/gtflffhirf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtxwzqgnym.html

C#:   s.Replace("a", "b")
来源：http://hz.smart0.xyz/gtqunqrpue.html

[E07] 按分隔符拆分
来源：http://hz.ywan-chungtsiang.top/gtnlmpvjsv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtmpgiufto.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenzaomai.com/gtppxdwqdl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtfcnwzune.html

TS:   s.split(",")
来源：http://hz.haohaochexian.top/gtlabqmxik.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtoeoaiume.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.316326.xyz/gtklgdbsto.html

Ruby: s.split(",");  s.split
来源：http://hz.ehwqpu.com/gtpihfdncx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fengsongda.top/gtrtmmzbtj.html

[E08] 数组按分隔符合并
来源：http://hz.hongshengwenyu.top/gtppcxpwrs.html

Py:   ",".join(items)
来源：http://hz.cucudq.cn/gtxhyiqzgk.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtghefqcsy.html

JS:   items.join(",")
来源：http://hz.tanke756.top/gtznmvuacw.html

TS:   items.join(",")
来源：http://hz.wangdashe.top/gttzkapnra.html

Java: String.join(",", items)
来源：http://hz.fzhhl.top/gttgamardw.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtytumajzl.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtzzdsdjmp.html

C#:   string.Join(",", items)
来源：http://hz.tanke756.top/gtfvcutmcd.html

[E09] 去除所有空白字符
来源：http://hz.zhiwuduotai.top/gtndjowkkb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtqclmhnpy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtineksjdu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtrrueptbj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtnfgnicvy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtrywuqete.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.quarkkingdee.top/gtybwrjzjp.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gtyfogjbnq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhiwuduotai.top/gtdqzgrzhl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtkbjfwdgv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtfbvhdhsv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jqgfzy.top/gtlyrdjzrq.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtjfwvkkzs.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtjzmbehyg.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtriumjprv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhijiandao.cn/gtnhuxgnrh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydzc1.top/gtjortdfwv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fzhhl.top/gtuyaltula.html

[E11] 反转字符串
来源：http://hz.zhixingplan.top/gtlcctdwyo.html

Py:   s[::-1]
来源：http://hz.pycfn.com/gtcihfzauc.html

PHP:  strrev($s);
来源：http://hz.redwolf501.top/gtzharqlix.html

JS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtofdnpuwu.html

TS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtfosadsue.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zycfv.cn/gtqfrfpdie.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhaomingkeji.xyz/gtzktonhle.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtcmokkmkd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtlzxcctgo.html

[E12] 统计某字符出现次数
来源：http://hz.zhixingplan.top/gtfgxerrwo.html

Py:   s.count("a")
来源：http://hz.chenzaomai.com/gtfnxgpndy.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtpytlsnpk.html

JS:   s.split("a").length - 1
来源：http://hz.xuetiantiany.cn/gtcmhieclb.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtvubdtbqw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhiwuduotai.top/gtzwodmbci.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gthiwyisvz.html

Ruby: s.count("a")
来源：http://hz.yj202588.top/gtcfftjajg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangdashe.top/gtmkzfgyiy.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtrcwvdreb.html

Py:   for ch in s: print(ch)
来源：http://hz.feifeiyinyue.top/gtptqixtle.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.haohaochexian.top/gtpzumevgu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtvwrjzqve.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtupdaktpy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.snrcjt.cn/gtcxmguqdb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shzxlz.cn/gtgenrdwkw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fengsongda.top/gtlfvjnneq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.andypj.xyz/gtqghunsng.html

[E14] URL 编码与 Base64
来源：http://hz.yueranfly.top/gtuekrjpml.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtomjhkqsu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shangyingyoupin.top/gtboiwfuwx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fzhhl.top/gtlslcdrgf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhoulong.xyz/gtpypvhqcl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xingfuxueyuan.xyz/gthpiztent.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fzhhl.top/gtbhvwfkph.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtvzeyorzg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtkvnevgvs.html

[E15] HTML 转义 / 反转义
来源：http://hz.svipenyu.cn/gtadpvnpby.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtkvpvatce.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.kuanghao11.cn/gtimosollv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cucudq.cn/gtkmqgtmnl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nwbrower.top/gtvbbcymze.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.mhx1999.top/gtiuqsenod.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhijiandao.cn/gtsvhlcopr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jyoumei.cn/gtntujqzur.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xingfuxueyuan.xyz/gtfostpklj.html

[E16] 数字千分位
来源：http://hz.zhengqikj.top/gtcjbgobep.html

Py:   f"{1234567:,}"
来源：http://hz.c1oappe.top/gtqgzkjrpf.html

PHP:  number_format(1234567);
来源：http://hz.yangfankeji.com/gtrmjeeray.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jianghu66.top/gtftbnpdtf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtiawnnwdx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hammf.cn/gtucuojjda.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gthcjzccwy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinyuanbaomall.cn/gtxtkxfjvp.html

C#:   1234567.ToString("N0")
来源：http://hz.zhoulong.xyz/gtfejyoqwm.html

[E17] 首字母大写
来源：http://hz.xylfe.cn/gtktrcxkfb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtuexwideo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtqfhingrs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gtocmlimle.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtxmialxgz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tianlin.xyz/gtzogcwfqz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gotoacloud.top/gtkuknmgzb.html

Ruby: s.capitalize
来源：http://hz.yvedp.cn/gtamrtoiev.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj202588.top/gtdadmixuw.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtvvuddmcm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daria6918.cn/gtguehcvag.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gtoivuaeqb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtctripmdv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtoytdjiiq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtfcgocvvn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.haohaochexian.top/gtnevyfaiq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fzhhl.top/gtpabojwhj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ybcxt.top/gtvkteimpk.html

[E19] 多行文本按行拆分
来源：http://hz.fengsongda.top/gtpleywinh.html

Py:   s.splitlines()
来源：http://hz.xylfe.cn/gtpqzbyyqg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hfpthk.cn/gtbvdfmdeg.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtgnuqbest.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtkhlxedbm.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gtatjiitcw.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangshuangyany.cn/gtbxpwscbs.html

Ruby: s.lines
来源：http://hz.zhixingplan.top/gtikffeolt.html

C#:   s.Split('\n')
来源：http://hz.hongshengwenyu.top/gtyqojefmj.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtnmgyoawl.html

Py:   if not s:
来源：http://hz.wangdashe.top/gtdyigtftd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gttzbtdnbp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuxming.cn/gtngalxoya.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtojmspcjt.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhengqikj.top/gteamqkpax.html

Go:   if s == "" {}
来源：http://hz.kuanghao11.cn/gtfdnqrwiz.html

Ruby: if s.empty?
来源：http://hz.iojbl.cn/gttuwtfgcy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxuanxn.top/gtfqbjuwey.html

[E21] 超长截断加省略号
来源：http://hz.meibo888.top/gtcqvnoeqn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.haohaochexian.top/gtnsenepka.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.quarkkingdee.top/gtiwiaegsa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtmmdmifmo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtlbznxmei.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtmyikbxnn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zycfv.cn/gtgrtpnegy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtericahtx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtlawqsdlf.html

[E22] 字节长度与字符长度
来源：http://hz.zhengqikj.top/gtnkljtnxx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hysaishi.cn/gtzbnovrov.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtlcpqaydv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtwloodsyu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtbqluxbww.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgufenzy.top/gtrzdhxnfo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hammf.cn/gtsfqpezdx.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigufen.top/gttqfwqpts.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yueranfly.top/gtxfmscqng.html

================================================================================
来源：http://hz.smart0.xyz/gtosuitxnj.html

F. 文件与目录
来源：http://hz.havefunace.top/gtxvpgtsro.html

================================================================================
来源：http://hz.fzhhl.top/gtpwqbyhqd.html

[F01] 读取整个文件
来源：http://hz.guowangkeji.top/gtpgbfytsk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sufxvd.cn/gtrtyjmfdm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenlongwang.top/gtimfiqkts.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.fengsongda.top/gtasmuxboj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtvsdjmhxx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtwzcswdmv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cqqwz.cn/gtwmxietqw.html

Ruby: File.read("a.txt")
来源：http://hz.chenzaomai.com/gtmoiqwtfi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.feifeiyinyue.top/gtlqzpwzrf.html

[F02] 逐行读取文件
来源：http://hz.yangfankeji.com/gtjgjqolen.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinyuanbaomall.cn/gttpdtvvjc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gtacqwwvxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtnryreodd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtamjjetvm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gttrbykiat.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ydzc1.top/gtanklrgcg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangkeji.top/gtxdmetjmz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cqqwz.cn/gtsbjwxhuk.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gtyyvfcckp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtfqffyppo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xinyue.icu/gtmttgsewy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtenxeucer.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtufddpskq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuxming.cn/gthykmpact.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gtvasnhsmv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pycfn.com/gtfdqbzjfw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hammf.cn/gtzrmbvcbr.html

[F04] 追加写入文件
来源：http://hz.ywan-chungtsiang.top/gtqtqzfmku.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgufenzy.top/gtivxbexpy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtgekojpbm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtbwpqyqss.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zdqjudy.top/gttnoirgyd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhengqikj.top/gtwfzicspt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xziqi.cn/gtaiyehfji.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gthvjfbula.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtrdvalbna.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnqzz.top/gtisuhbvgu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtxjbyxlbe.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtxzoagsfk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtfmibwifv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtifgtsyrx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtlmwchczb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.birdmap.top/gtlfgaqigg.html

Ruby: File.exist?("a.txt")
来源：http://hz.ppjwa.cn/gtfefejwwk.html

C#:   File.Exists("a.txt")
来源：http://hz.sysykeji.top/gtxppjtmgf.html

[F06] 删除文件
来源：http://hz.fengsongda.top/gtenpyohhe.html

Py:   os.remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtbwxeihzo.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gttwzevdlw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtwlsjquzo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtyjvotcso.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtqhfwbihz.html

Go:   os.Remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtxzdmhbra.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtvnjfjsmf.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gtnbefnnun.html

[F07] 创建目录（含多级）
来源：http://hz.snrcjt.cn/gthkohhnnz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.bjfxy.top/gtwnrigkba.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zycfv.cn/gtjkqanohc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtuvzmlwfz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtduofnsuq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtadtpbemb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtpfqhdcuy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangdashe.top/gtwlphcmdn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnxiangtu.top/gttztewhwo.html

[F08] 遍历目录
来源：http://hz.fzhhl.top/gttguoubuw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pengpengdd.cyou/gtsiorfddr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtzsfhyywk.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtdhkvoxuy.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtbjjbztvz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtxaafazrd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtqyuvllck.html

Ruby: Dir.children("dir")
来源：http://hz.yanxiufei.cn/gtrulnxnhy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tianlin.xyz/gtrveyuhlc.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gttshjsamb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuetiantiany.cn/gtatsnyjbm.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258.top/gtdxcchskd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtrujxaxjf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtnwweibsz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtnkvigwzd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtsbbornmi.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gttsjskubk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.feifeiyinyue.top/gtvgbmzpis.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtllntmgmm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtumjlcxez.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtubtmcsjk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtwsxpqufo.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gttusjbthm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gtlgnisfdc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jlsjyb.cn/gttfuuujdk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtfiyvnohp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtqnwsllzr.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtmtcxgyhs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtwxiqnytm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sysykeji.top/gtvryvzreb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtclohdrjf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtfhiktjqm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtfasfzlot.html


<!-- 参考信息 -->