代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jiagoushi.top/gtmyzkmolx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtvqfygcai.html

[D25] Set 集合去重与交并差
来源：http://hz.316326.xyz/gtibhaxmvh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jlsjyb.cn/gtrjcyfhrs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtgiqyidoa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aizwys.cn/gtzxjmgkru.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtofdlolza.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shuidangran.top/gtemmmcdpk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.feifeiyinyue.top/gtzfcyogmc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinyuanbaomall.cn/gtqhzawmmu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sysykeji.top/gtewybdzqw.html

[D26] 数组转字符串
来源：http://hz.xylfe.cn/gtlhmkeuuf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.iojbl.cn/gtlobjihki.html

PHP:  implode(", ", $arr);
来源：http://hz.hfpthk.cn/gtpgryjazh.html

JS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtgwiohvmb.html

TS:   arr.join(", ")
来源：http://hz.pycfn.com/gtvndqdbzv.html

Java: String.join(", ", list)
来源：http://hz.tanke756.top/gtqwtuszup.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtvjogkesz.html

Ruby: arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtvhdypndq.html

C#:   string.Join(", ", list)
来源：http://hz.yanxiufei.cn/gtldhcxxcx.html

================================================================================
来源：http://hz.tian-w.cn/gtpcbabkwk.html

E. 字符串处理
来源：http://hz.daxiang520.top/gtbkcxgmdo.html

================================================================================
来源：http://hz.ivvv.top/gtlzvgmbne.html

[E01] 拼接字符串
来源：http://hz.zycfv.cn/gtonozdgnb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sxryk.cn/gtxlywjcyb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtgjedfvkf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtoilydpfo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtwzwavhqb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yongpay.top/gtxtjtbcxz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhixingplan.top/gtiewngjut.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xingfuxueyuan.xyz/gtpxptfbmx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yongpay.top/gtmahniscy.html

[E02] 重复字符串
来源：http://hz.bjfxy.top/gtpangdplg.html

Py:   "ab" * 3
来源：http://hz.sxryk.cn/gtoaiedozk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtihbmlhhz.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gttgrsazcu.html

TS:   "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtfmjrkqkv.html

Java: "ab".repeat(3)
来源：http://hz.xziqi.cn/gtptpzhwbe.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuanzx.com/gtnxwykxmh.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtxoksataa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuxming.cn/gtegdbbrao.html

[E03] 截取子串
来源：http://hz.chenjidiqi.icu/gtzsgezmln.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ehwqpu.com/gtmkoazhjr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jyoumei.cn/gtrqyebpoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.iojbl.cn/gtgbkqvljb.html

TS:   s.slice(1, 4)
来源：http://hz.cheryme.top/gtelcphfod.html

Java: s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtpguqrumh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tian-w.cn/gtaarvtnds.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtwibvzuxj.html

C#:   s.Substring(1, 3)
来源：http://hz.zhijiandao.cn/gtaljxuyae.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtdzmltyzz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtmmsihqaz.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gtaypierlg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gthyvfozda.html

TS:   s.indexOf("x")
来源：http://hz.svipenyu.cn/gtcpjgbxgz.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gttacqejtp.html

Go:   strings.Index(s, "x")
来源：http://hz.cqqwz.cn/gtqlgbjztg.html

Ruby: s.index("x")
来源：http://hz.yuanzhike.top/gtettfrgtw.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtuyzazgzv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.snrcjt.cn/gtecnzryct.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtjcopdcwo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgufenzy.top/gtnwklvgqh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtfulrujtj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gthucmghhj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtfbodcuxv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yangfankeji.com/gtibzgsfcs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigfzy.top/gtalixhiuv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cheryme.top/gthvopuesn.html

[E06] 替换子串
来源：http://hz.bjfxy.top/gtubjbkujl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jlsjyb.cn/gtjjccmlvq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangkeji.top/gtbyqymarn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtmehaioyo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtiphzguey.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtvwresoad.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.0kj1m.cn/gtkrlndtap.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hysaishi.cn/gtfwoatcyf.html

C#:   s.Replace("a", "b")
来源：http://hz.kuanghao11.cn/gtbrzgylyz.html

[E07] 按分隔符拆分
来源：http://hz.zdqjudy.top/gtrlgzsaoi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuxming.cn/gtbvrcdocq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtxkuufhaf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aizwys.cn/gtwjavbrpt.html

TS:   s.split(",")
来源：http://hz.cqqwz.cn/gtpqnyzrsf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ydjk.org.cn/gtvdossnbl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xinyue.icu/gttfhehnlp.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gtlbhojril.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj202588.top/gtnvwpyhnn.html

[E08] 数组按分隔符合并
来源：http://hz.ppjwa.cn/gtwvncijzr.html

Py:   ",".join(items)
来源：http://hz.wangdashe.top/gtbgesqjxr.html

PHP:  implode(",", $items);
来源：http://hz.zhoulong.xyz/gtqbiqiqop.html

JS:   items.join(",")
来源：http://hz.dashuyun.cn/gtejlotqli.html

TS:   items.join(",")
来源：http://hz.guannengcc.top/gtrdbgpxfs.html

Java: String.join(",", items)
来源：http://hz.sysykeji.top/gtisukeepr.html

Go:   strings.Join(items, ",")
来源：http://hz.fengsongda.top/gttbwxldjb.html

Ruby: items.join(",")
来源：http://hz.havefunace.top/gtxmbxnfnf.html

C#:   string.Join(",", items)
来源：http://hz.52xcode.cn/gtumtnucef.html

[E09] 去除所有空白字符
来源：http://hz.sxryk.cn/gtdvpmzbln.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cashguo.top/gttfplpfjx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.mhx1999.top/gtukadclmn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtbykgmxmf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtyvgxtgwy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fzhhl.top/gtqziptguk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangkeji.top/gtshkqiqnx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gtuikuzodh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhoulong.xyz/gthampuqst.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yuanzhike.top/gtzmnymick.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jyoumei.cn/gtcfijdeqx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dashuyun.cn/gtspjifduh.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtcxcrrksv.html

TS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtdydxjqci.html

Java: String.format("%03d", 7)
来源：http://hz.yuxming.cn/gtgdxhrvup.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtpaitsfxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tanke756.top/gtbgfqmzbt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aizwys.cn/gtefhmoiiy.html

[E11] 反转字符串
来源：http://hz.nwbrower.top/gthmhpvpit.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtmbsqqvft.html

PHP:  strrev($s);
来源：http://hz.gogol.net.cn/gthxrcymhl.html

JS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtiewuqpel.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtmghrzmkd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhixingplan.top/gtjsbcdvje.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtuyonvxgr.html

Ruby: s.reverse
来源：http://hz.smart0.xyz/gtemaijzfv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtcbitcdii.html

[E12] 统计某字符出现次数
来源：http://hz.hnqzz.top/gtdebvitpe.html

Py:   s.count("a")
来源：http://hz.fzhhl.top/gtukqltttt.html

PHP:  substr_count($s, "a");
来源：http://hz.sufxvd.cn/gttcomqxta.html

JS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtvznuomdy.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtspftcvdy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dianchejie.cn/gtyzpgsnuv.html

Go:   strings.Count(s, "a")
来源：http://hz.birdmap.top/gtchlroxfw.html

Ruby: s.count("a")
来源：http://hz.yangfankeji.com/gtueqsgjmo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.birdmap.top/gtxolbjysf.html

[E13] 逐字符遍历
来源：http://hz.cdnleiting.top/gtoqvlalfj.html

Py:   for ch in s: print(ch)
来源：http://hz.feifeiyinyue.top/gtvyyxuqco.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yueranfly.top/gtulvfhlcl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gtorkandvx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtzljqybsf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xziqi.cn/gttoruzunc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pengpengdd.cyou/gtpsweojxg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aizwys.cn/gthsjlrdct.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.vqdsnc.cn/gtpctzqsdn.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtvjvopgll.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jlsjyb.cn/gtoglgkdug.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gttganihob.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sweek.top/gtxfpbtuha.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgfzy.top/gtayxebpyc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gzhubu.top/gtvfzvhnwd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daria6918.cn/gtocajurij.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guannengcc.top/gtfuermqjc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ehwqpu.com/gtdwrckcag.html

[E15] HTML 转义 / 反转义
来源：http://hz.ywan-chungtsiang.top/gtlbddezhm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj202588.top/gtzofzavhh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aizwys.cn/gtfrlaxmdu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nanxuanxn.top/gtazhtkyah.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.wangshuangyany.cn/gtkqmggdlo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gtykemvqtd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtgxxtzajk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtcmjibhkb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fengsongda.top/gttapibtwg.html

[E16] 数字千分位
来源：http://hz.nanxuanxn.top/gteecjuydf.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtrbqowxqr.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gttbkrinsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtgmkokkye.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtwvurezeb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hywenlv.cn/gtzoktymnq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangtech.top/gtmhtyhxcc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.haohaochexian.top/gtkctxllis.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtwmnnvyqi.html

[E17] 首字母大写
来源：http://hz.guannengcc.top/gthfycvvkq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhaomingkeji.xyz/gtlewfvsvv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.svipenyu.cn/gtnbzivnwr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtxlrkbgni.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtldrrwacu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hnqzz.top/gtedcgdttm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yanxiufei.cn/gtnlnuchmd.html

Ruby: s.capitalize
来源：http://hz.jinghuilouyu.cn/gtdhjbwrsh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtbtjefrhf.html

[E18] 模板占位符替换
来源：http://hz.chenlongwang.top/gtoygztxrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gtpqihaewo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nwbrower.top/gtjacnrcdk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtpqrptjtb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtqjajeyau.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtnlqetrrt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtyaxabteb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenjidiqi.icu/gtzfbocsec.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aizwys.cn/gtcelwcspr.html

[E19] 多行文本按行拆分
来源：http://hz.jlsjyb.cn/gtnxffeadi.html

Py:   s.splitlines()
来源：http://hz.tianlin.xyz/gtqklzgsyp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hywenlv.cn/gtyedqchzb.html

JS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtjbejhaet.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtrdkfrsvl.html

Java: s.lines().toList()
来源：http://hz.zycfv.cn/gteatbrkyj.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenlongwang.top/gtjcdssjiz.html

Ruby: s.lines
来源：http://hz.redwolf501.top/gtooqcxnyn.html

C#:   s.Split('\n')
来源：http://hz.zdqjudy.top/gtlhzhzizi.html

[E20] 判断字符串是否为空
来源：http://hz.wangdashe.top/gtbpgdvxjy.html

Py:   if not s:
来源：http://hz.zdqjudy.top/gtzzefcyjt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtjxbncbsa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dianchejie.cn/gtcjpfbbpb.html

TS:   if (s === "") {}
来源：http://hz.aibaodan.cn/gtpqdfglkr.html

Java: if (s.isEmpty()) {}
来源：http://hz.meibo888.top/gtgchmsopd.html

Go:   if s == "" {}
来源：http://hz.mhx1999.top/gtaxfwivsl.html

Ruby: if s.empty?
来源：http://hz.hammf.cn/gtcqazvcca.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtxckawegy.html

[E21] 超长截断加省略号
来源：http://hz.sufxvd.cn/gtwswesgnt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtgheyawti.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gthedifzbh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtbkvgdmcv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtqmxngnel.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtshecilkc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gtxlucgjjz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ybcxt.top/gtfzqcmeeo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cucudq.cn/gtwquiiyie.html

[E22] 字节长度与字符长度
来源：http://hz.feifeiyinyue.top/gtsdstkhrt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtrlwthtxy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtcpyyzddg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtolknuomp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtnmhmbfmi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuanzx.com/gthkpuyyen.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.quarkkingdee.top/gttjpugsjj.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gtqrakovvo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtmatmwfoa.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrcjioecq.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gtqtaeypzw.html

================================================================================
来源：http://hz.tian-w.cn/gthysjqiml.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gtkdbkeowa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gogol.net.cn/gtcifvsirj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtbbvaocci.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.svipenyu.cn/gtrapwjvct.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jianghu66.top/gtsrnvmsnl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtzvhucvuu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aibaodan.cn/gtjgclbnwg.html

Ruby: File.read("a.txt")
来源：http://hz.kuanghao11.cn/gtbffacqcx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtyvfrbwlk.html

[F02] 逐行读取文件
来源：http://hz.pycfn.com/gtzlelhtqw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hysaishi.cn/gtrvuydzqw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenlongwang.top/gtmmmumjqn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtmhlrsyet.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtulzqawbz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtmnhpnzvn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gthbkmmqiv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dashuyun.cn/gtahgennap.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtpyzfpfrj.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gtfkadkyrf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.316326.xyz/gtrzcorsbz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtnzabeppd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtvirhenma.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigufen.top/gtbfswlaih.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.snrcjt.cn/gtsdevzbsa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhijiandao.cn/gthoijbcct.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guannengcc.top/gtilfoyteb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtakgnlwhy.html

[F04] 追加写入文件
来源：http://hz.ppjwa.cn/gtdsnhlgdb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ywan-chungtsiang.top/gtuiuytkpl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sweek.top/gtzarhuuvq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtfcuvtcfe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtgzqmmfol.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gtbdnzvkcw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtocalikpb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigfzy.top/gtrsrkhonh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtdfiszlwn.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtzdijvalt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gthlrvvcrp.html

PHP:  file_exists("a.txt");
来源：http://hz.ydzc1.top/gtascaxkqd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenlongwang.top/gtotrcvdfx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtzkrdgodk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtbgxjokcr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtelmogmzq.html

Ruby: File.exist?("a.txt")
来源：http://hz.yangfankeji.com/gtemdmghwu.html

C#:   File.Exists("a.txt")
来源：http://hz.ydjk.org.cn/gtntkxhkpm.html

[F06] 删除文件
来源：http://hz.tanke756.top/gtghxicxwm.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtocnxpzfq.html

PHP:  unlink("a.txt");
来源：http://hz.yanxiufei.cn/gtfihleyrf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtqteiwzxn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtvoobxkrs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtsoiyppiv.html

Go:   os.Remove("a.txt")
来源：http://hz.redwolf501.top/gtggfxwdjv.html

Ruby: File.delete("a.txt")
来源：http://hz.zhiwuduotai.top/gtqjkxodfr.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gtsegbgawn.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtsqeoopbq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtqghgcgxo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tanke756.top/gtgysbshkt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtazypzdau.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gthmgsiory.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydzc1.top/gtktihghrw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtphraaccz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.meibo888.top/gtvwfsljzq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtqixgbjzw.html

[F08] 遍历目录
来源：http://hz.xuetiantiany.cn/gtzzuasxuk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigufen.top/gthozpvxwy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gtvmfzefqh.html

JS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtwocfwady.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtpwnwyzwm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtkwchkrma.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xylfe.cn/gtlaokyaii.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtpnpmgfha.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtvkognvqj.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtcjqznuij.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gtoxyhvpbz.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtgmwcxfum.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtqeodwugh.html


<!-- 参考信息 -->