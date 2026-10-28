代发 wailian999

[D23] reduce 累积计算
来源：http://hz.redwolf501.top/gttdszqdex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jyoumei.cn/gtaxyfevrl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.c1oappe.top/gtycgfgtro.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtfsbigrea.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtesjtwdwn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangshuangyany.cn/gtyoxvbcfv.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gtrqmqbnvh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhijiandao.cn/gtclzcyjbp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.iojbl.cn/gtalyuvkkp.html

[D24] 字典 / Map 基本操作
来源：http://hz.xylfe.cn/gtyickfzvw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nwbrower.top/gtvorujzyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sufxvd.cn/gtczhugtop.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guannengcc.top/gtmhbmrvgw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinqigfzy.top/gtsldczhyw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.smart0.xyz/gtblqvxkzj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxinkj.top/gtvnliwfcs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtggzvvaie.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aizwys.cn/gtylwtknzy.html

[D25] Set 集合去重与交并差
来源：http://hz.jiagoushi.top/gtcckhknop.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtzymhdlng.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangtech.top/gtazavrrzc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtjvfynmgn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cdnleiting.top/gtattjklvz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sweek.top/gtsvupurif.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sxryk.cn/gtdxmcvlpw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.smart0.xyz/gtvnmdqhrr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtorykvwnm.html

[D26] 数组转字符串
来源：http://hz.sweek.top/gtyfbbvbic.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhoulong.xyz/gtgofzdkps.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gthqzsroax.html

JS:   arr.join(", ")
来源：http://hz.cucudq.cn/gtprbinyzg.html

TS:   arr.join(", ")
来源：http://hz.xinyue.icu/gtqmbndlop.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtpouidoml.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenjidiqi.icu/gtwjzkipcn.html

Ruby: arr.join(", ")
来源：http://hz.sweek.top/gtdvwkucru.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtcdpeyhry.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmsmuclio.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtiqtksomk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxzwzjvcu.html

[E01] 拼接字符串
来源：http://hz.cdnleiting.top/gtofcdhpwl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yuxming.cn/gtvbdtnwtx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtyfsjmkng.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtebhmcedo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtcdesspft.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtmueclsoj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gtxbvxcjht.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.andypj.xyz/gttxdurxhx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gtsvyykdrf.html

[E02] 重复字符串
来源：http://hz.aibaodan.cn/gtpwvehkeg.html

Py:   "ab" * 3
来源：http://hz.pengpengdd.cyou/gtehvrykhc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yangfankeji.com/gtgxltmiaf.html

JS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtyczjkjuh.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtkqqoldru.html

Java: "ab".repeat(3)
来源：http://hz.yongpay.top/gthidvslzv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.smart0.xyz/gtjwjwsemp.html

Ruby: "ab" * 3
来源：http://hz.sufxvd.cn/gtqbptoype.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ydjk.org.cn/gtdebgxwcr.html

[E03] 截取子串
来源：http://hz.ydzc1.top/gtpttcskyk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.andypj.xyz/gtowpwzjad.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtbbhbdvxx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gtiaetwofr.html

TS:   s.slice(1, 4)
来源：http://hz.316326.xyz/gtfsmsonvq.html

Java: s.substring(1, 4)
来源：http://hz.ivvv.top/gtiwkcuzmq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.dashuyun.cn/gtbkgraahf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangshuangyany.cn/gtzqmehqxw.html

C#:   s.Substring(1, 3)
来源：http://hz.cdnleiting.top/gtjnyxzubc.html

[E04] 查找子串位置
来源：http://hz.shuidangran.top/gtesqwwtlw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sweek.top/gtscqisfem.html

PHP:  strpos($s, "x");
来源：http://hz.vqdsnc.cn/gtxdrvobbc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtmzuhsibr.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gttlbcqqta.html

Java: s.indexOf("x")
来源：http://hz.52xcode.cn/gtpraswyye.html

Go:   strings.Index(s, "x")
来源：http://hz.cheryme.top/gtvslncowc.html

Ruby: s.index("x")
来源：http://hz.bjfxy.top/gtorymdarp.html

C#:   s.IndexOf("x")
来源：http://hz.shangyingyoupin.top/gteanjhzvt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shangyingyoupin.top/gtystqmysn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cqqwz.cn/gtwuixqpum.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hywenlv.cn/gtlbxcsgtp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtvrhsymrh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yangfankeji.com/gtippoungd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gtaicciuto.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydzc1.top/gtelxzzudj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sysykeji.top/gtfyirfnwc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pengpengdd.cyou/gtvjspwasm.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtfbujdmah.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtltyzeict.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinqigufen.top/gtrxckbezx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtqtqsulya.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtjbseyfgk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtfoeujnwg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gtxmopapcg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gzhubu.top/gtfjxabdkq.html

C#:   s.Replace("a", "b")
来源：http://hz.daria6918.cn/gtlqpdkegp.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtnckqshsj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gthcbjzjnf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gtnuajlrok.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.guowangkeji.top/gtpgqwhlfi.html

TS:   s.split(",")
来源：http://hz.zhiwuduotai.top/gttmhoujdl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gogol.net.cn/gtyvhegbui.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cheryme.top/gtmobfwxqh.html

Ruby: s.split(",");  s.split
来源：http://hz.shzxlz.cn/gtntoporad.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtjikijnhp.html

[E08] 数组按分隔符合并
来源：http://hz.andypj.xyz/gtslljwlah.html

Py:   ",".join(items)
来源：http://hz.zhengqikj.top/gttchmbrfz.html

PHP:  implode(",", $items);
来源：http://hz.ppjwa.cn/gtvzqaigle.html

JS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtrvpdmrfg.html

TS:   items.join(",")
来源：http://hz.hnqzz.top/gtmnzfqviu.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gthvhpdwea.html

Go:   strings.Join(items, ",")
来源：http://hz.andypj.xyz/gtbeoskfqu.html

Ruby: items.join(",")
来源：http://hz.yanxiufei.cn/gtlssxakiv.html

C#:   string.Join(",", items)
来源：http://hz.jqgufenzy.top/gtynxajnwb.html

[E09] 去除所有空白字符
来源：http://hz.aibaodan.cn/gtyhtdrfdp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.andypj.xyz/gtvilzujjm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtasdjvmtm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtwmegxwqm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangdashe.top/gtzfcasovn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtmrwypdsm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj202588.top/gtyvwkoxvh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tanke756.top/gtgvphauuo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhoulong.xyz/gtajbupqry.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yonumen.top/gtngbgubyi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtqgyllsrj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shuidangran.top/gtzsbycqsu.html

JS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtalbngwdo.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtsflbswia.html

Java: String.format("%03d", 7)
来源：http://hz.zhixingplan.top/gtpkdoazhn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gturasoxtb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtyzwuaxse.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jyoumei.cn/gtmeyarmgo.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gthvjfucpc.html

Py:   s[::-1]
来源：http://hz.jianghu66.top/gtbbyhuecy.html

PHP:  strrev($s);
来源：http://hz.sweek.top/gtbhgpkwoc.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtvovhcibn.html

TS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtrxoocpvd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.quarkkingdee.top/gtebgqedgl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shuidangran.top/gtsamxqlpp.html

Ruby: s.reverse
来源：http://hz.zhaomingkeji.xyz/gttpbdqpvt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtqynvsdtf.html

[E12] 统计某字符出现次数
来源：http://hz.cdnleiting.top/gtcsqpgicd.html

Py:   s.count("a")
来源：http://hz.jinghuilouyu.cn/gtnnxjbmeh.html

PHP:  substr_count($s, "a");
来源：http://hz.shanyushiyangkeji.top/gthmiqixao.html

JS:   s.split("a").length - 1
来源：http://hz.zhongyouzk.top/gtmycpmyfl.html

TS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtunenzojw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtmkziovim.html

Go:   strings.Count(s, "a")
来源：http://hz.snrcjt.cn/gtleomgplr.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtrzddhzcl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtdpwalxwh.html

[E13] 逐字符遍历
来源：http://hz.tianlin.xyz/gtmypjtvke.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtkvxyrwfv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.c1oappe.top/gtwqukiwek.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtybnepvbh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenlongwang.top/gtwqhupyug.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtnxugntpr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinghuilouyu.cn/gtrujifucw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gtiojwyhft.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtqgijcqks.html

[E14] URL 编码与 Base64
来源：http://hz.yangfankeji.com/gtzkbcrjky.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtcumwpiwb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jyoumei.cn/gtwunwtxrq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.0kj1m.cn/gtqajioryr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.haohaochexian.top/gtykfxgfls.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnxiangtu.top/gtesuvvmoo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtgnhbivpz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gogol.net.cn/gtgcigjytk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guowangkeji.top/gtzacermcl.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtfqvasqcc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cucudq.cn/gtvtpvjnuz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yanxiufei.cn/gtytnbpgyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cqqwz.cn/gtdufgekig.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cdnleiting.top/gtuixcvyxj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.havefunace.top/gtvhojoplr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hysaishi.cn/gtncjrcjvc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gtyzrgrirc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigfzy.top/gtraysljjp.html

[E16] 数字千分位
来源：http://hz.hammf.cn/gtiopceqzg.html

Py:   f"{1234567:,}"
来源：http://hz.feifeiyinyue.top/gtidscfaoo.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtelhcmtui.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtjqkglxsr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtimdrjgmw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnxiangtu.top/gtqokdgmgk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.havefunace.top/gtikpjgrzz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.0kj1m.cn/gtlvzojmue.html

C#:   1234567.ToString("N0")
来源：http://hz.tianlin.xyz/gtuzigxpjl.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gttcyoprst.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtiyqvmdfk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtelalufac.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtdnepmdin.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtszgkntdp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhaomingkeji.xyz/gtyfswgyfo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtaliqsuno.html

Ruby: s.capitalize
来源：http://hz.jianghu66.top/gteqwqusin.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtzvmequnm.html

[E18] 模板占位符替换
来源：http://hz.bjfxy.top/gterrfyhfy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tianlin.xyz/gtpyierevv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dashuyun.cn/gtqtjxecqy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtgjzukgci.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtjzgmhafq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.quarkkingdee.top/gtkovetgsh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shuidangran.top/gtiezcsimq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cdnleiting.top/gtfoyvgmvk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shanyushiyangtech.top/gtgitoyyxd.html

[E19] 多行文本按行拆分
来源：http://hz.tanke756.top/gtumpsdjvm.html

Py:   s.splitlines()
来源：http://hz.hywenlv.cn/gtgyknnqmx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guowangkeji.top/gtnapnqidr.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtkiffijtc.html

TS:   s.split(/\r?\n/)
来源：http://hz.daria6918.cn/gtlvqkfwco.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtpofdzkru.html

Go:   strings.Split(s, "\n")
来源：http://hz.gaohongyu789.top/gtdinbxbpt.html

Ruby: s.lines
来源：http://hz.wangdashe.top/gtdraajwrv.html

C#:   s.Split('\n')
来源：http://hz.dianchejie.cn/gtdruiozrg.html

[E20] 判断字符串是否为空
来源：http://hz.jinghuilouyu.cn/gtcllqidpl.html

Py:   if not s:
来源：http://hz.daxiang520.top/gtmcocjuvx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zdqjudy.top/gturxuynwh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gthnkvolbx.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtdglbpalv.html

Java: if (s.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtclgrcmdk.html

Go:   if s == "" {}
来源：http://hz.zhijiandao.cn/gtdzegtivv.html

Ruby: if s.empty?
来源：http://hz.smart0.xyz/gtbfcswsls.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtxfytzopy.html

[E21] 超长截断加省略号
来源：http://hz.zhiwuduotai.top/gtitwdfbys.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aizwys.cn/gtgbeyzuoz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtkhpghbhy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtgdpzzsrj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtzkrwgyjw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtdvphrfdg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtplnpjyrw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.snrcjt.cn/gtjzrokyix.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yueranfly.top/gtsipomnsj.html

[E22] 字节长度与字符长度
来源：http://hz.jqgfzy.top/gtfwzscbto.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gogol.net.cn/gtwfvtkafb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gteohdjyzq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtocanuxii.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtynyygxhc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinyuanbaomall.cn/gtnyhsxqey.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.feifeiyinyue.top/gtnkvnvnub.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtjemnnmmv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtxsikmxua.html

================================================================================
来源：http://hz.cqqwz.cn/gtwnzhinar.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gtqjzfcxwu.html

================================================================================
来源：http://hz.hysaishi.cn/gtucbfiqco.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtsbazmkvx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jyoumei.cn/gtauhhmlkd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guannengcc.top/gtxqkvhqur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cucudq.cn/gtangkpqxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dashuyun.cn/gtpltlhvqh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtuqvpwxhx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtwuxtxsoi.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtyvmoetsa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cucudq.cn/gtvoksjesr.html

[F02] 逐行读取文件
来源：http://hz.bjfxy.top/gtatgrpold.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtbrxhmrow.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtijhligdh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtmhwjjyhp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtfalzwrmt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtltlpatey.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtkorwgdvt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtnfpfekdq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gtsuxbechk.html

[F03] 写入文件（覆盖）
来源：http://hz.xylfe.cn/gttnjsillp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xylfe.cn/gtivfqqtik.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gogol.net.cn/gteeyuzivc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtbuxhuvlb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtjlnkwfre.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtcauwoize.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtzpbuolzo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtflqxoujq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtmblgcpqy.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtbkxgvyol.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtfrtxasgc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.wangdashe.top/gtdjeqdfqo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtpyjdkgku.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtzcvhdhkn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shzxlz.cn/gtlfpvssqb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.birdmap.top/gtkudrmgwx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtgpsvfhiq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtixnkzuzr.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gtudwegdgc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxuanxn.top/gtpbmxjals.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gttccydzcn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtukufoaec.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtyipubaqu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtcjwxxrul.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gtdbwuayya.html

Ruby: File.exist?("a.txt")
来源：http://hz.c1oappe.top/gtgebbokcp.html

C#:   File.Exists("a.txt")
来源：http://hz.yanxiufei.cn/gtarzkpqjw.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gtifmoteid.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtsejlirnv.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtcfpqvwri.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtbigmlvsp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtvzlylgcj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtdtajmtsd.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gteezlcbvz.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtnffjxscl.html

C#:   File.Delete("a.txt");
来源：http://hz.cheryme.top/gtxzryjvmg.html

[F07] 创建目录（含多级）
来源：http://hz.haohaochexian.top/gtehsqwrzu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tianlin.xyz/gtwwndzqha.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtlfqcwvst.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtsirlmxcb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtgwaxtmky.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258.top/gtarvcccqu.html


<!-- 参考信息 -->