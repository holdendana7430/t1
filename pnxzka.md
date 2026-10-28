代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gtfevactuk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangdashe.top/gtcuuyhxpm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.andypj.xyz/gtrtabvijv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxuanxn.top/gtiqyjpkhc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnqzz.top/gthneoqhvu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhaomingkeji.xyz/gtqrqqgrfz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cqqwz.cn/gtelsyqcpx.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtdpltewav.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jlsjyb.cn/gtattqeyoh.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gterquxpic.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtrpdfubyz.html

TS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtaydogufo.html

Java: String.join(", ", list)
来源：http://hz.daxiang520.top/gtyfteaciu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtnwehfcat.html

Ruby: arr.join(", ")
来源：http://hz.pycfn.com/gtlahpbyim.html

C#:   string.Join(", ", list)
来源：http://hz.jqgufenzy.top/gttovwlhjh.html

================================================================================
来源：http://hz.tanke756.top/gtrmxkolen.html

E. 字符串处理
来源：http://hz.ybcxt.top/gttrfiajwa.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtujcbxtum.html

[E01] 拼接字符串
来源：http://hz.jiagoushi.top/gtndznxbet.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ivvv.top/gtzrtgtrvy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yangfankeji.com/gtgvzbntkv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gthonatorz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hfpthk.cn/gtileujyip.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dianchejie.cn/gtspeqneli.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ehwqpu.com/gtklfrbtgd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.smart0.xyz/gtnurdwhdi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtwduxuuvi.html

[E02] 重复字符串
来源：http://hz.sxryk.cn/gtsnhemudj.html

Py:   "ab" * 3
来源：http://hz.guowangkeji.top/gtfcwfvdnx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hfpthk.cn/gtzlmncyyl.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtfsjibmlz.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtmnaddozs.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtcpupdzxx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.dianchejie.cn/gtmzlkbrzw.html

Ruby: "ab" * 3
来源：http://hz.ybcxt.top/gtsnicfzuk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.316326.xyz/gtbajfozag.html

[E03] 截取子串
来源：http://hz.sxryk.cn/gtbxbzjhrk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.birdmap.top/gtpxccegph.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.havefunace.top/gtkpqkhmco.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtlwcagkya.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtqszyeztv.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtufhguvpz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.svipenyu.cn/gtoqohmrkn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhengqikj.top/gtgadittbf.html

C#:   s.Substring(1, 3)
来源：http://hz.hnqzz.top/gtjrpsikcg.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gtrcvlzpfz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shzxlz.cn/gtddgntcqn.html

PHP:  strpos($s, "x");
来源：http://hz.vqdsnc.cn/gtvlczurfm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.vqdsnc.cn/gtcfbgnhjp.html

TS:   s.indexOf("x")
来源：http://hz.gotoacloud.top/gtdvomvlyd.html

Java: s.indexOf("x")
来源：http://hz.jiagoushi.top/gtqlghwofs.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtaelwbroh.html

Ruby: s.index("x")
来源：http://hz.fzhhl.top/gtnrnsrihw.html

C#:   s.IndexOf("x")
来源：http://hz.zhixingplan.top/gtiaptsmqa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guannengcc.top/gtggmeqxoz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jianghu66.top/gtptvsskqt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hnqzz.top/gtsxtwrrlu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtjzkqbycx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtxpjpwcbw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtzszgqlwd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tianlin.xyz/gtbjkiflqj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nwbrower.top/gtzcicmbxw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gttwfecrjo.html

[E06] 替换子串
来源：http://hz.jinyuanbaomall.cn/gtkijbeomh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sysykeji.top/gtzpaobecv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.quarkkingdee.top/gtxamutykv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtancwzjxt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtbhaadgwi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtjcfbsndg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhijiandao.cn/gtskuuomgb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gtkpduyfjs.html

C#:   s.Replace("a", "b")
来源：http://hz.shanyushiyangtech.top/gtkclzmfxj.html

[E07] 按分隔符拆分
来源：http://hz.fzhhl.top/gtkjhkxspv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ybcxt.top/gtehuhxcsa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yonumen.top/gtbzpfxvxc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.dashuyun.cn/gtctpeywfj.html

TS:   s.split(",")
来源：http://hz.gaohongyu789.top/gtuluvttqq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtsxirdqqk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.mhx1999.top/gttklvwfbg.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258888.top/gtxsdalfyw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aibaodan.cn/gtvclwtqdx.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtolsbhrvo.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gtzgxtjbqj.html

PHP:  implode(",", $items);
来源：http://hz.pengpengdd.cyou/gtumufxuai.html

JS:   items.join(",")
来源：http://hz.jyoumei.cn/gtjbuxvuyb.html

TS:   items.join(",")
来源：http://hz.xuanzx.com/gtljzsnguk.html

Java: String.join(",", items)
来源：http://hz.hysaishi.cn/gtadyhfsri.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gtkgoovpld.html

Ruby: items.join(",")
来源：http://hz.0kj1m.cn/gtwymlqkdu.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtostmtgpm.html

[E09] 去除所有空白字符
来源：http://hz.xinyue.icu/gtjqssztwo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhiwuduotai.top/gtjmtckisc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gtvuyiuyhz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gthnxstcjo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtlqbnathp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangtech.top/gtnrhjuowd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtlcktuuwr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtirxorrvb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtgxbosucw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtqgiavyhz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jlsjyb.cn/gtudxvclag.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cashguo.top/gtjoipbops.html

JS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtgtkvybwk.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtczzzsmaq.html

Java: String.format("%03d", 7)
来源：http://hz.ybcxt.top/gtksxaaqqa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yangfankeji.com/gtkynbaqjv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtjdvggzvz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gtnvhofylo.html

[E11] 反转字符串
来源：http://hz.xziqi.cn/gtrwandlnd.html

Py:   s[::-1]
来源：http://hz.redwolf501.top/gtntziokhk.html

PHP:  strrev($s);
来源：http://hz.ydzc1.top/gttpgbsyjx.html

JS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtbrxenpwt.html

TS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtkltblwfc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.c1oappe.top/gtmtofxzgx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yonumen.top/gtqpejdprc.html

Ruby: s.reverse
来源：http://hz.tianlin.xyz/gtfqtedgqw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtugrccasw.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtvvutyabc.html

Py:   s.count("a")
来源：http://hz.zhiwuduotai.top/gtrpqumbwf.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtccuxbdfe.html

JS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtpnojdfky.html

TS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtuqnbuads.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daxiang520.top/gtjkcwrzbz.html

Go:   strings.Count(s, "a")
来源：http://hz.yuanzhike.top/gtfkswzvuh.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtcwesefbz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtufvlbdda.html

[E13] 逐字符遍历
来源：http://hz.jinyuanbaomall.cn/gtodkkgvxr.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtsojlkjic.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.smart0.xyz/gtfirbfpqx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtoilixgoi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtajzdlfsl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.bjfxy.top/gthiktzwov.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.haohaochexian.top/gtjclmzhqa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.meibo888.top/gtusbalklb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.9152youxi.cn/gtijbpvrss.html

[E14] URL 编码与 Base64
来源：http://hz.jqgfzy.top/gtfnlbvovb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.52xcode.cn/gtxijuwxrl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fzhhl.top/gthludeozk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtsjanlhmk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.nanxuanxn.top/gtlsvvznaj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.meibo888.top/gtmsvsvvhn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangshuangyany.cn/gthungyejx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuanzhike.top/gtnlbnvsxa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinqigufen.top/gtmzjuolkt.html

[E15] HTML 转义 / 反转义
来源：http://hz.zycfv.cn/gtsbqusygl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cashguo.top/gtwyvefrul.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtsymirgnz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cqqwz.cn/gttathlysj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenjidiqi.icu/gtcmwtvfaj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.c1oappe.top/gtjvnceufi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cucudq.cn/gtrioqnaie.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtujsbanle.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guowangkeji.top/gtdlxnqusu.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gttsltflga.html

Py:   f"{1234567:,}"
来源：http://hz.ybcxt.top/gtbgcqcihb.html

PHP:  number_format(1234567);
来源：http://hz.birdmap.top/gtedihuzlq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtbvlrbyjs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtqzvytaup.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtdsujbmkf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cqqwz.cn/gtgztzthgr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xylfe.cn/gtqzxezjcy.html

C#:   1234567.ToString("N0")
来源：http://hz.zhongyouzk.top/gtpfauggwr.html

[E17] 首字母大写
来源：http://hz.dashuyun.cn/gtiqafxgjs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fzhhl.top/gtrqffrgkp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtaysyatxk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtbxbtcrxr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtuauxdovl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydzc1.top/gthfdxcokd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.vqdsnc.cn/gtijhzilen.html

Ruby: s.capitalize
来源：http://hz.vqdsnc.cn/gthovebinm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.9152youxi.cn/gtosbnogwg.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtsxgirdyf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shangyingyoupin.top/gtucrnqtut.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuetiantiany.cn/gtefdznmvh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtziblxiaz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtwjduxhxu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258888.top/gtksnqjcqv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtbjgzquuc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gtzxinywdm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtmfphvikc.html

[E19] 多行文本按行拆分
来源：http://hz.daria6918.cn/gtndjunsmd.html

Py:   s.splitlines()
来源：http://hz.jinqigufen.top/gtrikplxfz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.feifeiyinyue.top/gttbutplwn.html

JS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtnnpcrvot.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtsmetksss.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gtiywctqrh.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtdkokwimw.html

Ruby: s.lines
来源：http://hz.andypj.xyz/gtnkzehnjq.html

C#:   s.Split('\n')
来源：http://hz.feifeiyinyue.top/gtcqfuteqd.html

[E20] 判断字符串是否为空
来源：http://hz.feifeiyinyue.top/gtuckfvodx.html

Py:   if not s:
来源：http://hz.zycfv.cn/gtigygjhpc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtvdawixai.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxuanxn.top/gtllizrqwc.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtmzsicaec.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangshuangyany.cn/gtxecnoaqb.html

Go:   if s == "" {}
来源：http://hz.yonumen.top/gtlelkwcqo.html

Ruby: if s.empty?
来源：http://hz.xziqi.cn/gtabbyqmvk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.quarkkingdee.top/gtnviuinye.html

[E21] 超长截断加省略号
来源：http://hz.kuanghao11.cn/gtcdmoqxcg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhengqikj.top/gtbgfsicvu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.snrcjt.cn/gtcyrstcrj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtompszyrs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtdirnqcoz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtghmkrhiu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yangfankeji.com/gtorszpjzu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtehedtjtr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dianchejie.cn/gtxkuixkoh.html

[E22] 字节长度与字符长度
来源：http://hz.gotoacloud.top/gtnduwadpo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ivvv.top/gtxceqqzev.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtresgennx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gttjovbmzx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtuejxbdgw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tanke756.top/gtpffjwxzc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yvedp.cn/gtsuhzpldq.html

Ruby: s.bytesize;  s.length
来源：http://hz.tian-w.cn/gtsuvxcevl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tanke756.top/gtpdptvuih.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtsdwpjmgg.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtfetvgrwu.html

================================================================================
来源：http://hz.zycfv.cn/gtiakmaile.html

[F01] 读取整个文件
来源：http://hz.hammf.cn/gtinpavrxf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxuanxn.top/gtwzdzjzxg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtjxlfahfq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtfjyqfaml.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.haohaochexian.top/gttbnielzm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtynuqahrs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hongshengwenyu.top/gttofkcjdk.html

Ruby: File.read("a.txt")
来源：http://hz.andypj.xyz/gtmhfusdzl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.haohaochexian.top/gtxskngmwq.html

[F02] 逐行读取文件
来源：http://hz.vqdsnc.cn/gtomseqneg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtaadljutm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gthctbuenp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtzxjupwnc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.mhx1999.top/gtguonpamx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtsysntxbi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangtech.top/gtgxxrdxku.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtgjgyoogk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gogol.net.cn/gtiganvxst.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtfarqvjxh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shuidangran.top/gtkwgjamry.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtveyjapid.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtwqopvukb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtyfrstnyn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cucudq.cn/gtllovpwtr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gtitpaznwm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinyuanbaomall.cn/gtvtiltouy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtvxtdxhqq.html

[F04] 追加写入文件
来源：http://hz.xuetiantiany.cn/gtipdbzibh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnqzz.top/gtpfdtuxoc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.52xcode.cn/gtbdliazto.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtasoostsw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtpirmqxrz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pycfn.com/gttvfaklhg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgfzy.top/gtvgdqdqaj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhengqikj.top/gtjjxhlkoa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.daria6918.cn/gtscuufiwp.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtxokrcqlu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.snrcjt.cn/gthvbdydgy.html

PHP:  file_exists("a.txt");
来源：http://hz.yanxiufei.cn/gteafaegij.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtrcgqgrus.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtuvrbbgjo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtnqccgmjl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhaomingkeji.xyz/gtrcbutotb.html

Ruby: File.exist?("a.txt")
来源：http://hz.pengpengdd.cyou/gtwwtdzprr.html

C#:   File.Exists("a.txt")
来源：http://hz.chenjidiqi.icu/gthibolysj.html

[F06] 删除文件
来源：http://hz.smart0.xyz/gtuitlnbgj.html

Py:   os.remove("a.txt")
来源：http://hz.dashuyun.cn/gtbaeudmjh.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtfmmpttan.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtpdfhsuqi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtearhjejs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtwzjkfwnd.html

Go:   os.Remove("a.txt")
来源：http://hz.ivvv.top/gtaxuatfsz.html

Ruby: File.delete("a.txt")
来源：http://hz.zhengqikj.top/gtrgohzbxh.html

C#:   File.Delete("a.txt");
来源：http://hz.jianghu66.top/gtmqgxzaar.html

[F07] 创建目录（含多级）
来源：http://hz.zhaomingkeji.xyz/gtlmjqferg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtvqdujqkz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yanxiufei.cn/gtazxmenmh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtsufrfaxj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtccfznunv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zdqjudy.top/gteaendlcq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.52xcode.cn/gtriwuybya.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtcebmkpxs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtjwflmpqs.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gtcrqlnwbz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guowangkeji.top/gtamtjcmfz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.quarkkingdee.top/gtbsuexzso.html

JS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gthnjtqlbg.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtvtbdwekb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtprdxvize.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.feifeiyinyue.top/gtqborgeiq.html

Ruby: Dir.children("dir")
来源：http://hz.xuanzx.com/gtrbyjhkot.html

C#:   Directory.GetFiles("dir")
来源：http://hz.birdmap.top/gtnckctqmz.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtdjhryzcv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtjanxgcda.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtjgygjzyv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtwtervipv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtizxqcuvc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gttvggduzh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtcxzzbrny.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtnqsabxrp.html


<!-- 参考信息 -->