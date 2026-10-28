代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhongyouzk.top/gtvuuzmtux.html

[D24] 字典 / Map 基本操作
来源：http://hz.cqqwz.cn/gtnjsdwufs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.0kj1m.cn/gtwdmglubf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenzaomai.com/gtfzbrhedy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.wangshuangyany.cn/gtmkzacvuc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangtech.top/gthenjiqzf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gtuojpoxhk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtctfmdvkc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tanke756.top/gtsowbtbgp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.haohaochexian.top/gtjpckhyet.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtqggjkqrx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gthyiiewco.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guannengcc.top/gtbkipfwfa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xylfe.cn/gtkggrmuhl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gtqtbwalze.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtrluiwbgj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxinkj.top/gtsohpujco.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cqqwz.cn/gtnimheyrc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gtwkscgzla.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtsumvwluv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj202588.top/gtwrbwpfjx.html

PHP:  implode(", ", $arr);
来源：http://hz.pycfn.com/gtgfkvshhd.html

JS:   arr.join(", ")
来源：http://hz.yonumen.top/gtxlvjvrsm.html

TS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtzyxylcag.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtrvvozayx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gaohongyu789.top/gtrwmzmpsg.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gtskjyihcy.html

C#:   string.Join(", ", list)
来源：http://hz.dianchejie.cn/gtuaxzahxh.html

================================================================================
来源：http://hz.xuanzx.com/gtkdmujowv.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtxnhgnzob.html

================================================================================
来源：http://hz.smart0.xyz/gtuauwlqet.html

[E01] 拼接字符串
来源：http://hz.chenlongwang.top/gtxovucmnd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtwfwlrpxr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnxiangtu.top/gttbahyjwp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtfyfxxddi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtxnnrzjxm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gtdrltmerq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtcjntqmop.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangtech.top/gtcikhsuvo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangdashe.top/gtltoaspdb.html

[E02] 重复字符串
来源：http://hz.ydzc1.top/gtjukgxtwk.html

Py:   "ab" * 3
来源：http://hz.jinqigufen.top/gtyydfogtu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gtqwmfbjrn.html

JS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtqymotrsm.html

TS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtxuljjzep.html

Java: "ab".repeat(3)
来源：http://hz.yj20258888.top/gtyegnjlav.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gtzcswstzj.html

Ruby: "ab" * 3
来源：http://hz.zhixingplan.top/gtkvsfhddx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtrndvlonw.html

[E03] 截取子串
来源：http://hz.ppjwa.cn/gteftpuobl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nwbrower.top/gthdjucgyk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtygoejjut.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtaayraocz.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtqipcjlsh.html

Java: s.substring(1, 4)
来源：http://hz.sxryk.cn/gtcdagbntt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hywenlv.cn/gtgedisuex.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yongpay.top/gteqskrqdv.html

C#:   s.Substring(1, 3)
来源：http://hz.pengpengdd.cyou/gtrdvhkjxx.html

[E04] 查找子串位置
来源：http://hz.zdqjudy.top/gtjqaikgph.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtqyjlrpdb.html

PHP:  strpos($s, "x");
来源：http://hz.jianghu66.top/gtqpafucfk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.haohaochexian.top/gtjsyxqrds.html

TS:   s.indexOf("x")
来源：http://hz.gotoacloud.top/gtksvdqjpf.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gtqlerzkcx.html

Go:   strings.Index(s, "x")
来源：http://hz.xziqi.cn/gtrimwkbdn.html

Ruby: s.index("x")
来源：http://hz.sxryk.cn/gtlwordssf.html

C#:   s.IndexOf("x")
来源：http://hz.gzhubu.top/gtfddkbywc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydzc1.top/gteqchgdqk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shzxlz.cn/gteubekzzt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.c1oappe.top/gtdzndpymv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtppajgqsr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenjidiqi.icu/gtjzivwnzl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtjisfhsyf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hammf.cn/gtghftdatj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cdnleiting.top/gthqwbvsuh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shzxlz.cn/gtllfhhciz.html

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtjrlfaqda.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtbudaalxq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenjidiqi.icu/gtllvbwsge.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtnatueisw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtmudogzzf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtxuaxckon.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtzbzszzut.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.9152youxi.cn/gtbuhsgenb.html

C#:   s.Replace("a", "b")
来源：http://hz.snrcjt.cn/gttmrduvmg.html

[E07] 按分隔符拆分
来源：http://hz.pengpengdd.cyou/gtazdiktfn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cucudq.cn/gtqrdobvgs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yongpay.top/gtordrpbsf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhaomingkeji.xyz/gtcekhdxvk.html

TS:   s.split(",")
来源：http://hz.zhengqikj.top/gtbmboohhi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cdnleiting.top/gthjvvdimx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtlqmwjwbj.html

Ruby: s.split(",");  s.split
来源：http://hz.gogol.net.cn/gtfjublrep.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yueranfly.top/gtavclibqn.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtsqhzktqg.html

Py:   ",".join(items)
来源：http://hz.dashuyun.cn/gtbzmjkiwn.html

PHP:  implode(",", $items);
来源：http://hz.haohaochexian.top/gtaalcjvpo.html

JS:   items.join(",")
来源：http://hz.jianghu66.top/gtrxcrqtjr.html

TS:   items.join(",")
来源：http://hz.tanke756.top/gtettnvkgl.html

Java: String.join(",", items)
来源：http://hz.cqqwz.cn/gtfmkijdcc.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gtmtchxrie.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtysazflfu.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtfbloulsr.html

[E09] 去除所有空白字符
来源：http://hz.gotoacloud.top/gtoptqpdng.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.snrcjt.cn/gtbizapopa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtzwzezaqm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtubdlroxe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtuflxvkzl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhaomingkeji.xyz/gthmcxbolt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.smart0.xyz/gtxcfsgwpm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtwxqblkvm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.mhx1999.top/gtpupxcgvv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cqqwz.cn/gtlaxzwkqp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuanzhike.top/gtgbhvvoyb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gogol.net.cn/gtjzsgbmgy.html

JS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtelgjfwhm.html

TS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtwmrkaypj.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258.top/gtzscvkryv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtxneipork.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtmqzsucob.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ywan-chungtsiang.top/gtaqphhzdo.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gtrszfquxj.html

Py:   s[::-1]
来源：http://hz.wangdashe.top/gtrjhuupnp.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtrupgyarv.html

JS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtluyvzbae.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtbbmvcwyu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gaohongyu789.top/gthrfsmhjf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtdipozceb.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtwmjjcbvb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtczymydiv.html

[E12] 统计某字符出现次数
来源：http://hz.yongpay.top/gtxqwuetpo.html

Py:   s.count("a")
来源：http://hz.jinqigufen.top/gtikoukblm.html

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gtdzbcicap.html

JS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gttjycqqjl.html

TS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gtmtvsubfa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtafrtcbmg.html

Go:   strings.Count(s, "a")
来源：http://hz.sufxvd.cn/gtapgcjubv.html

Ruby: s.count("a")
来源：http://hz.jinqigfzy.top/gtzrjcadyt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuanzx.com/gtjcqekvtw.html

[E13] 逐字符遍历
来源：http://hz.smart0.xyz/gtrkxmtfnx.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtrmhcnyxe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenzaomai.com/gtwpduhhjj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtkksdwwyp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtwhgjrirq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sxryk.cn/gtnzrjfmbp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.svipenyu.cn/gtiaffdozh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgfzy.top/gtujpqhkoi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtwstghatg.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gtpebopdco.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtvunvuufs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gaohongyu789.top/gteqnrrvrb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cqqwz.cn/gtcvatxpbc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jianghu66.top/gtqqqqlrhd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shzxlz.cn/gtxgkahvuq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxuanxn.top/gtwvuletnt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtxhzizoxf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinqigufen.top/gteyiyufhh.html

[E15] HTML 转义 / 反转义
来源：http://hz.jianghu66.top/gtzzmohuum.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dashuyun.cn/gtxgpothll.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yonumen.top/gtgylqctez.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.havefunace.top/gtbdgtipar.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtxhhoxibl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gtfnjzgowi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ivvv.top/gtjkotjasd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gttuygajdx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtvhbdzlgo.html

[E16] 数字千分位
来源：http://hz.jinqigufen.top/gttbgncato.html

Py:   f"{1234567:,}"
来源：http://hz.fzhhl.top/gtigkmquon.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtveijdloh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtptdzuosv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtwwesqmih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtdwhdkfyk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cdnleiting.top/gtuozpuqyw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dianchejie.cn/gtnzginlor.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtxoaedkoj.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gtipwfjylx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gtjjqzoprw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtjovqhhov.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtofecigca.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtnzhehpop.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.quarkkingdee.top/gtzokdtdvy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.iojbl.cn/gtvpxprnpx.html

Ruby: s.capitalize
来源：http://hz.sxryk.cn/gtnzbuoczc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cdnleiting.top/gtvvneufse.html

[E18] 模板占位符替换
来源：http://hz.hfpthk.cn/gtcxwdaocg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtczcjcpnf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtalbwmafy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtqtmjzfkc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xinyue.icu/gtjdijscpv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guowangkeji.top/gtrpyihrks.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hammf.cn/gtykiyhpnv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258.top/gterkewsse.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtzqbbgknx.html

[E19] 多行文本按行拆分
来源：http://hz.mhx1999.top/gtjrdwrawf.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtjlkwyxes.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gtsfdikanf.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtblwnxcia.html

TS:   s.split(/\r?\n/)
来源：http://hz.yonumen.top/gttxnkxruy.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtkacbutic.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtjkktwytf.html

Ruby: s.lines
来源：http://hz.jinyuanbaomall.cn/gtbftkogdx.html

C#:   s.Split('\n')
来源：http://hz.zhongyouzk.top/gtazvwvxjn.html

[E20] 判断字符串是否为空
来源：http://hz.nwbrower.top/gtpioydnfx.html

Py:   if not s:
来源：http://hz.jinghuilouyu.cn/gtmhqbxohe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtfbxblpsn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenlongwang.top/gtlfcouiuo.html

TS:   if (s === "") {}
来源：http://hz.hnqzz.top/gtsusgynrk.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtyyhtmqwh.html

Go:   if s == "" {}
来源：http://hz.yj20258888.top/gtakwfrhtu.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtiwyrwbtz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xinyue.icu/gtrsovnnrj.html

[E21] 超长截断加省略号
来源：http://hz.redwolf501.top/gtamwoqcxj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sweek.top/gtdhgzqlri.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtqwxdilwy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtyerhfzfr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtydcvamhb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtfakkerqu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.smart0.xyz/gtnxywknqn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgfzy.top/gtlomxhpcb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.9152youxi.cn/gtnwpomvbc.html

[E22] 字节长度与字符长度
来源：http://hz.jinyuanbaomall.cn/gtkmlmspdm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zycfv.cn/gtoyfrufec.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtdbtffuga.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtzcmqzdas.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtluxrpijb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtrkmhmfcq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jlsjyb.cn/gtwszvqwaq.html

Ruby: s.bytesize;  s.length
来源：http://hz.ybcxt.top/gteawfsqwr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtulpchrty.html

================================================================================
来源：http://hz.smart0.xyz/gtnowsjvub.html

F. 文件与目录
来源：http://hz.snrcjt.cn/gtxaphlsok.html

================================================================================
来源：http://hz.snrcjt.cn/gtlyqpwwvn.html

[F01] 读取整个文件
来源：http://hz.cashguo.top/gtzmvlyqcy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.9152youxi.cn/gtwvkjgvea.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gzhubu.top/gtrhnuamav.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ydzc1.top/gtelepgbqs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.redwolf501.top/gtejmgnryf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtkyajfmwh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gtinhdsvtb.html

Ruby: File.read("a.txt")
来源：http://hz.nwbrower.top/gtlrcochfo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258.top/gtfjytpiep.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtqhjyyzas.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.0kj1m.cn/gtwrslvbon.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tianlin.xyz/gtwfuctegc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtlhueoveu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtnllcldjz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gtcxdiskln.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.wangdashe.top/gtdtaygpht.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtrawkxsav.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zycfv.cn/gtwmlpnguz.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtrzcnenaz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtrcuuatge.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtfjqsvmid.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtatqelgex.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtonpbhegh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtezbngbcv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtaprhtaqa.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guowangkeji.top/gtqdqbyrqh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.c1oappe.top/gtjbvxlleo.html

[F04] 追加写入文件
来源：http://hz.iojbl.cn/gtbevdccuh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ybcxt.top/gtluedaamu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.smart0.xyz/gtdjvxkmlx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtxaetftou.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtakwfsifg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtkxouykzm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.birdmap.top/gtydkgkgvi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aibaodan.cn/gtgorbtiif.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ivvv.top/gtbztbmxrz.html

[F05] 判断文件或目录是否存在
来源：http://hz.aizwys.cn/gtzhdqfjel.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtqhvlfznq.html

PHP:  file_exists("a.txt");
来源：http://hz.dashuyun.cn/gtmkglfrnj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtedbfzytb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtxjgklyil.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtvyeffzkj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xziqi.cn/gtpgixjigc.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnqzz.top/gtyhjqtpuu.html

C#:   File.Exists("a.txt")
来源：http://hz.ehwqpu.com/gtrcgplksi.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtswasfect.html

Py:   os.remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtboynqbuk.html

PHP:  unlink("a.txt");
来源：http://hz.hongshengwenyu.top/gtujqyyixh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtoizjbdxb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtghfnivlp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtlubtmhxf.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtrdgcugvh.html

Ruby: File.delete("a.txt")
来源：http://hz.yangfankeji.com/gttvppabyo.html

C#:   File.Delete("a.txt");
来源：http://hz.meibo888.top/gttacskozv.html

[F07] 创建目录（含多级）
来源：http://hz.shzxlz.cn/gtmawhvbpe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.iojbl.cn/gtucfomidd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jiagoushi.top/gtbippwnlb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtuzfrkisz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gthvybcvun.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtblxfaagz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shanyushiyangkeji.top/gtajwmauwq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xziqi.cn/gtvyjwgprm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtlgorixzg.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gtwgckqdjm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cheryme.top/gtdslypzms.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtjvmsquwa.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtivkodilx.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtrpqvsgbq.html


<!-- 参考信息 -->