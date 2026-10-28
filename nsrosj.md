代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://hz.snrcjt.cn/gtmyjkunun.html

PHP:  implode(", ", $arr);
来源：http://hz.cheryme.top/gtznylhvlh.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtomgvprxb.html

TS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtnzspczcp.html

Java: String.join(", ", list)
来源：http://hz.gzhubu.top/gtomoybvnt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sweek.top/gtqvwifgia.html

Ruby: arr.join(", ")
来源：http://hz.cdnleiting.top/gtlllewfpa.html

C#:   string.Join(", ", list)
来源：http://hz.fengsongda.top/gtvvhnzuwb.html

================================================================================
来源：http://hz.jqgfzy.top/gtnrpvzicb.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gtznemcbbx.html

================================================================================
来源：http://hz.aizwys.cn/gtzjmomsxa.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtbxovacku.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtxbwsuimi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tianlin.xyz/gtnyradxof.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gteycydljp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtffymmtqd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xuanzx.com/gtsfsqlfwk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xingfuxueyuan.xyz/gtnoixfdjh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cdnleiting.top/gtwtfqustt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.bjfxy.top/gtaxsvhpiy.html

[E02] 重复字符串
来源：http://hz.haohaochexian.top/gtytlqpufj.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtqvbxuclv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258888.top/gtiwbeglbn.html

JS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtabompbqg.html

TS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtwyeywrap.html

Java: "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtuoggvdak.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sysykeji.top/gtwrzhiesj.html

Ruby: "ab" * 3
来源：http://hz.ybcxt.top/gtrrtnrcnl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yueranfly.top/gtesrlhtcx.html

[E03] 截取子串
来源：http://hz.shzxlz.cn/gtqofsrhdn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnxiangtu.top/gthsjhuygk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.52xcode.cn/gtxilhxwgj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yueranfly.top/gtlgqdgxze.html

TS:   s.slice(1, 4)
来源：http://hz.0kj1m.cn/gtheeqsxvt.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtjsdlunui.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.feifeiyinyue.top/gtfciblzfa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgufenzy.top/gtvwxiebgd.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgufenzy.top/gtjwrpxyrj.html

[E04] 查找子串位置
来源：http://hz.chenlongwang.top/gtfohyknck.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sysykeji.top/gtqodhfalh.html

PHP:  strpos($s, "x");
来源：http://hz.jlsjyb.cn/gtrjtduabl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgufenzy.top/gtvgjehngl.html

TS:   s.indexOf("x")
来源：http://hz.yongpay.top/gtnidbibtb.html

Java: s.indexOf("x")
来源：http://hz.bjfxy.top/gtudkwjzhr.html

Go:   strings.Index(s, "x")
来源：http://hz.daria6918.cn/gtwnkrxnar.html

Ruby: s.index("x")
来源：http://hz.ydjk.org.cn/gtbijcamkb.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gteaovstsa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shanyushiyangtech.top/gtdlupgxxk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xinyue.icu/gtisbxpqsl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhixingplan.top/gtqgcvupcb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtpvpqlhqd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.haohaochexian.top/gtjlygxgkd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gthudkdlzk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cucudq.cn/gtsvohdwqn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.haohaochexian.top/gtgedbkwea.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.52xcode.cn/gtmryoboxj.html

[E06] 替换子串
来源：http://hz.daxiang520.top/gtaofmxjzq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ivvv.top/gtoqzqwlad.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guowangkeji.top/gtnqoircfh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtzxitsati.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtrtrmehkj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtjedyfjms.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jianghu66.top/gtikclvill.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.redwolf501.top/gtjkccrbrd.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtguoxegen.html

[E07] 按分隔符拆分
来源：http://hz.jlsjyb.cn/gtwsektogr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yonumen.top/gtdvbibxeh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gtsvlpfjpu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.redwolf501.top/gtpacsngbe.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtbkczvadx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhongyouzk.top/gtbmmtbcdc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigfzy.top/gtcxbykbru.html

Ruby: s.split(",");  s.split
来源：http://hz.meibo888.top/gtowyclyii.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daria6918.cn/gtznetfafl.html

[E08] 数组按分隔符合并
来源：http://hz.jqgfzy.top/gtbgzyzdet.html

Py:   ",".join(items)
来源：http://hz.ydzc1.top/gtemphptdn.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtqbjvrrjc.html

JS:   items.join(",")
来源：http://hz.zdqjudy.top/gtebwhmvkr.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtksgykcai.html

Java: String.join(",", items)
来源：http://hz.gogol.net.cn/gtwklqogve.html

Go:   strings.Join(items, ",")
来源：http://hz.sufxvd.cn/gtfjijxfwv.html

Ruby: items.join(",")
来源：http://hz.daria6918.cn/gtwyitimsw.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gtzsbcshzq.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gtmjahdiar.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gaohongyu789.top/gtrhmvsiyj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtcdxltdtk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtuzikdzar.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtcdlmfrnx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.c1oappe.top/gtkvsjdhsn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtyhpzsujt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydzc1.top/gtqllwioyf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xylfe.cn/gtdgzzzrqa.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtdqxqjpxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gotoacloud.top/gtkseffirl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xuetiantiany.cn/gttlkkocyi.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtkbgelkxx.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gttapdwvow.html

Java: String.format("%03d", 7)
来源：http://hz.dianchejie.cn/gtmammgjpb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtcgvnaqtc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.redwolf501.top/gtihumwzmj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guannengcc.top/gtnvhmobjv.html

[E11] 反转字符串
来源：http://hz.hammf.cn/gtaiaqjnaa.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtbmcquhfv.html

PHP:  strrev($s);
来源：http://hz.shanyushiyangtech.top/gtocmwyhme.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtvqgnaedo.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtqkgphbhm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtsonhhtpz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangtech.top/gtilncpksx.html

Ruby: s.reverse
来源：http://hz.hfpthk.cn/gtevhekfdi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtllooszuq.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gtyjnplfpj.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtmopzynmu.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtilvlqkpp.html

JS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtthdsduwk.html

TS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtihmlytpe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hysaishi.cn/gtaxbjzcst.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258888.top/gtrlaprknv.html

Ruby: s.count("a")
来源：http://hz.9152youxi.cn/gtobgvhbmx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aizwys.cn/gtfavqcgmy.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtkjcmyppz.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtesbwkxmk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtnrxczrqd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gtpmsnwxdr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtypedatdk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhiwuduotai.top/gtigfoyzbl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtogtwavhc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gtxnzlofsi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.feifeiyinyue.top/gtvhedhumb.html

[E14] URL 编码与 Base64
来源：http://hz.nanxinkj.top/gtsbvwfvpp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxuanxn.top/gthodxryif.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yanxiufei.cn/gtdbrorcxs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtamhisnpy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.snrcjt.cn/gtlotbcueo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cucudq.cn/gtmgpqysnw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.smart0.xyz/gtnclpiiln.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.vqdsnc.cn/gtlfejzxkt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zycfv.cn/gtqbqwkcda.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuetiantiany.cn/gtziwgjntt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sufxvd.cn/gtnxoezqdb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jiagoushi.top/gtdakqxdft.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenzaomai.com/gthtdmqhnx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangtech.top/gterqhzyjl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gtynwzhith.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hfpthk.cn/gtfewudujg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gtsufqadkx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gtxqwsdisv.html

[E16] 数字千分位
来源：http://hz.vqdsnc.cn/gtzitixjiu.html

Py:   f"{1234567:,}"
来源：http://hz.hfpthk.cn/gtuzdjdrlc.html

PHP:  number_format(1234567);
来源：http://hz.zhengqikj.top/gtlccfsurl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jianghu66.top/gtlrtgcuwm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtrnuukmqk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shuidangran.top/gtzszcvpkv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtppaxxslm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtnrmtsmyq.html

C#:   1234567.ToString("N0")
来源：http://hz.jiagoushi.top/gtbtizpvam.html

[E17] 首字母大写
来源：http://hz.meibo888.top/gtlxirwojb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gthndhuxlu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtmogpkcov.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtrhdhpiop.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtzoeppmdz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.fzhhl.top/gtshvqidxr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gteiboekqb.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtzyhzysyb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sysykeji.top/gturmauswa.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtwmzmkcia.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sxryk.cn/gtxvohabka.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ivvv.top/gtxevyaida.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtlmkqdsig.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtezzjgrsz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtzbtzvzyr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtqeczcdcy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtbhuywxvu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.haohaochexian.top/gtgscamfvy.html

[E19] 多行文本按行拆分
来源：http://hz.wangdashe.top/gtoxrhbzbp.html

Py:   s.splitlines()
来源：http://hz.gzhubu.top/gtlyolvmbi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hfpthk.cn/gtlzxublea.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtdyghrqdk.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtaylocprb.html

Java: s.lines().toList()
来源：http://hz.vqdsnc.cn/gtjolqdypy.html

Go:   strings.Split(s, "\n")
来源：http://hz.yuxming.cn/gtunasusya.html

Ruby: s.lines
来源：http://hz.daxiang520.top/gtmruzajfg.html

C#:   s.Split('\n')
来源：http://hz.jqgufenzy.top/gtyurwaaxi.html

[E20] 判断字符串是否为空
来源：http://hz.hnqzz.top/gtuilktkzi.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtbvhrbnwa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhixingplan.top/gtswrpyjpl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtfcjilpft.html

TS:   if (s === "") {}
来源：http://hz.cucudq.cn/gtmnmhcwgz.html

Java: if (s.isEmpty()) {}
来源：http://hz.pycfn.com/gtfgauncnp.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtmaixctxr.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtktqiqopu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gthtnefnsb.html

[E21] 超长截断加省略号
来源：http://hz.aizwys.cn/gttvkdrkld.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxuanxn.top/gtehksuboe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.quarkkingdee.top/gtpnhezsaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtrhcmtpla.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtvqsrvddu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtwamhncnk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtwdciyyvm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cashguo.top/gtiruzkbkq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinqigufen.top/gtjokowprt.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtnhrrxprn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tianlin.xyz/gtwcoxyamf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtfrjplrci.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtgduawbvr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gtmpawclzg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.9152youxi.cn/gtzikcumoa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ehwqpu.com/gtiamnubzv.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gttrtqevpt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhengqikj.top/gtjrpfnoad.html

================================================================================
来源：http://hz.snrcjt.cn/gtroothqlo.html

F. 文件与目录
来源：http://hz.zhoulong.xyz/gtktcfywbf.html

================================================================================
来源：http://hz.zhixingplan.top/gtwvluuqjg.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtbbfjybee.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnqzz.top/gtklwiwpos.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hywenlv.cn/gteulvcccf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuxming.cn/gtpakhwpko.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtddfeecdq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtecjkzedk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtahwefgap.html

Ruby: File.read("a.txt")
来源：http://hz.aibaodan.cn/gtfquskbnw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pengpengdd.cyou/gtuangvvxm.html

[F02] 逐行读取文件
来源：http://hz.tanke756.top/gtopcqqioa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuanzhike.top/gtvjgmcmat.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtmbwvplqi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtlubcghrk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtqljdpyxm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtvmbiosxg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtzqwledoy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ehwqpu.com/gtrijiubpx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtuwgjdmww.html

[F03] 写入文件（覆盖）
来源：http://hz.bjfxy.top/gtezdvpirk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangshuangyany.cn/gtmvdhmfgf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtpaozybrj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cqqwz.cn/gtokpqlchi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtyucgiinb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtngnajimj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnxiangtu.top/gtdyduvkdi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gtlgyyadrq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jianghu66.top/gtsxqgzxmg.html

[F04] 追加写入文件
来源：http://hz.jqgfzy.top/gtkosrwigy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gzhubu.top/gthlzptjdj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gthkuuciey.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtcwocsvde.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtrlecdrsr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.redwolf501.top/gtbutnkhbg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yueranfly.top/gtkyzhffsw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zdqjudy.top/gtnzchubxh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258888.top/gtbdlsaxdj.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtaaelxxid.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sweek.top/gtwlfzvjpn.html

PHP:  file_exists("a.txt");
来源：http://hz.hywenlv.cn/gtwyrslilu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtwxzohhhi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.svipenyu.cn/gtyfilgvxy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtbpnarvca.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtynyxvixb.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtohwtmkdg.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtcrankhxm.html

[F06] 删除文件
来源：http://hz.yj20258888.top/gtkksfzlld.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtvubyrkqx.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gteoaulcsl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtwgilyyhc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtufrelhjy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtggfomwpg.html

Go:   os.Remove("a.txt")
来源：http://hz.iojbl.cn/gtkesrslms.html

Ruby: File.delete("a.txt")
来源：http://hz.shuidangran.top/gtazllehty.html

C#:   File.Delete("a.txt");
来源：http://hz.c1oappe.top/gtrueryyiv.html

[F07] 创建目录（含多级）
来源：http://hz.ehwqpu.com/gtvkazimzk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtbjukbkip.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258888.top/gtryfpgmis.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtxqnasobh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtxtlxrysf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtxngkpnzs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtcgrolnem.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.snrcjt.cn/gtdintsgug.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.andypj.xyz/gtfnitnlgo.html

[F08] 遍历目录
来源：http://hz.ydjk.org.cn/gtkrdjbrau.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zdqjudy.top/gtwqreogkl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ppjwa.cn/gtbtbtozxh.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtjxqyvolf.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtvfvmincv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtuqatpgaf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hysaishi.cn/gthmjzfrrv.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtbasuikei.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtwvznygtp.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtxpyguxxv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnqzz.top/gtdgdugjqd.html

PHP:  filesize("a.txt");
来源：http://hz.hnxiangtu.top/gtdthwzsjj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtnwkbudxf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gttcujzpem.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtwfsirreg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aibaodan.cn/gtygijenyj.html

Ruby: File.size("a.txt")
来源：http://hz.ehwqpu.com/gteqjurwku.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangdashe.top/gtntfrzkgw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtunswdsas.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtkdhgakvf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuxming.cn/gtdogexanb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtnxsfqurz.html

TS:   path.extname("a.txt")
来源：http://hz.haohaochexian.top/gtvftiacid.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nwbrower.top/gtduhfdgnd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtlukbrndi.html


<!-- 参考信息 -->