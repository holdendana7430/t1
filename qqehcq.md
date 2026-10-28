代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinghuilouyu.cn/gtzdaddpbi.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtfxmephto.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guannengcc.top/gtekxtubgx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gttcvamwba.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtpenemtdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuanzx.com/gtjogjxrtm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhiwuduotai.top/gtjildewob.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.smart0.xyz/gtxmmfnolx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtruwyvmdm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shuidangran.top/gtvulglsmx.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtthnxfzrg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258.top/gtcadqauao.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtmsuqxxvr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangkeji.top/gtbvqobhwv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuanzhike.top/gtkzthanuk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtbizkjxac.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtxxqcgukv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.svipenyu.cn/gtzkkekhjg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtiqcstfrb.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gtbrrpwzrp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258.top/gtusvhxfxe.html

PHP:  implode(", ", $arr);
来源：http://hz.jlsjyb.cn/gtqtapguys.html

JS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtvjfromap.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtxrkiuvmt.html

Java: String.join(", ", list)
来源：http://hz.chenjidiqi.icu/gttragueqz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xylfe.cn/gtodvrilqm.html

Ruby: arr.join(", ")
来源：http://hz.yvedp.cn/gtkeaxmluv.html

C#:   string.Join(", ", list)
来源：http://hz.yongpay.top/gtzewrqygm.html

================================================================================
来源：http://hz.ivvv.top/gtssapymln.html

E. 字符串处理
来源：http://hz.xuanzx.com/gtroppuooq.html

================================================================================
来源：http://hz.hywenlv.cn/gtsonstdbr.html

[E01] 拼接字符串
来源：http://hz.tianlin.xyz/gtoufcwael.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtpblbxtnh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnxiangtu.top/gtdzhvxxwz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cheryme.top/gtzucjvynr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangdashe.top/gtrfdmsihl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tanke756.top/gtllznojrv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtnpxwagpc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zycfv.cn/gtpjbssezz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gtywpofczd.html

[E02] 重复字符串
来源：http://hz.xuetiantiany.cn/gttobyddxz.html

Py:   "ab" * 3
来源：http://hz.yangfankeji.com/gtovqrpoar.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nwbrower.top/gtevkjpoam.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtbgyhoytw.html

TS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtcidquqot.html

Java: "ab".repeat(3)
来源：http://hz.52xcode.cn/gtmsnqfopx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fengsongda.top/gtcxnltkzz.html

Ruby: "ab" * 3
来源：http://hz.ppjwa.cn/gtriwbqoxt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tian-w.cn/gtdmfzzupy.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gtdqkeblyf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gtmvttwdff.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gtiwzwaepv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gtfgcxfizy.html

TS:   s.slice(1, 4)
来源：http://hz.xuetiantiany.cn/gtjbkezchd.html

Java: s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtkuvlnbws.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gttqfelsjw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dashuyun.cn/gtlvhvtuna.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtbddovvfe.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gttyaxfivh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gttjnebkeg.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtahkrkdwc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gaohongyu789.top/gtdltkldmb.html

TS:   s.indexOf("x")
来源：http://hz.hnqzz.top/gtxhludbap.html

Java: s.indexOf("x")
来源：http://hz.jqgfzy.top/gtsvtetsmp.html

Go:   strings.Index(s, "x")
来源：http://hz.cheryme.top/gtuqgbhcie.html

Ruby: s.index("x")
来源：http://hz.dianchejie.cn/gtdkjvtpbr.html

C#:   s.IndexOf("x")
来源：http://hz.sufxvd.cn/gtyihifypt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pengpengdd.cyou/gtvlmvywek.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xylfe.cn/gtxgfnfzze.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hammf.cn/gtuiziedus.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtqnsahhfl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinqigufen.top/gtgxibumwf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fzhhl.top/gthfrjayfw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sxryk.cn/gtsduukngs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cheryme.top/gtrdnpyyvz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnxiangtu.top/gthyxgemgx.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtzjacgidm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtlinzvygm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenzaomai.com/gtxsvrmowz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtlfcfivpz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtvrndtoek.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtrneqzohk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtzjfkmget.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtneabsepv.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtwnyuxkfh.html

[E07] 按分隔符拆分
来源：http://hz.yueranfly.top/gtpdqnzyrj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jyoumei.cn/gtovlbchdi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhiwuduotai.top/gtrthhhdsd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.meibo888.top/gtcnmofshi.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtvkeddhaf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtzfghpgtu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xuanzx.com/gttbsnwpan.html

Ruby: s.split(",");  s.split
来源：http://hz.gotoacloud.top/gtodnsodvg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.iojbl.cn/gtoaxgmusw.html

[E08] 数组按分隔符合并
来源：http://hz.hnxiangtu.top/gtmluikmkc.html

Py:   ",".join(items)
来源：http://hz.xingfuxueyuan.xyz/gtxogampuv.html

PHP:  implode(",", $items);
来源：http://hz.yuanzhike.top/gtaimdwlfa.html

JS:   items.join(",")
来源：http://hz.xuanzx.com/gtnsujdejr.html

TS:   items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtjtrzytyw.html

Java: String.join(",", items)
来源：http://hz.bjfxy.top/gtdehfbbpl.html

Go:   strings.Join(items, ",")
来源：http://hz.zhiwuduotai.top/gtjafuwhjd.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtkfwxerqq.html

C#:   string.Join(",", items)
来源：http://hz.guannengcc.top/gtkjeyvazi.html

[E09] 去除所有空白字符
来源：http://hz.yongpay.top/gtxokfrpml.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxinkj.top/gtscstxywn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.0kj1m.cn/gtbykshodx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtahqzuzkn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinghuilouyu.cn/gtgsutmzqx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ehwqpu.com/gtjytxtsfu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj202588.top/gtfhvcdrkr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangdashe.top/gtnaweumtn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daxiang520.top/gtzcolklwe.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhixingplan.top/gtnawzgovn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtctzyeeik.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtggrzyxxa.html

JS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtegchaczj.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtlbiufyut.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gttqrnbqkf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtvjiwfien.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gtnvpdgdom.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenzaomai.com/gtiufsvdph.html

[E11] 反转字符串
来源：http://hz.sweek.top/gtgzxcaefp.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtkhnjswzl.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtjkvdxcbx.html

JS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtbjktvzlb.html

TS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtdjdzeqml.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cucudq.cn/gtvoimbkti.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenlongwang.top/gtdepizbvv.html

Ruby: s.reverse
来源：http://hz.hywenlv.cn/gtynyogozp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtwdfbqtsx.html

[E12] 统计某字符出现次数
来源：http://hz.smart0.xyz/gtdnzerxaz.html

Py:   s.count("a")
来源：http://hz.chenzaomai.com/gteztwhhgm.html

PHP:  substr_count($s, "a");
来源：http://hz.yangfankeji.com/gtztrehugs.html

JS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtiypzegkc.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtumaipkbc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hywenlv.cn/gtgyauivdg.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258888.top/gtozprifoz.html

Ruby: s.count("a")
来源：http://hz.svipenyu.cn/gtrwaymbly.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xylfe.cn/gtxpxupfqc.html

[E13] 逐字符遍历
来源：http://hz.jianghu66.top/gtexkufctm.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gtjjyqumfe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hongshengwenyu.top/gtxrkpixti.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.c1oappe.top/gtrnnnfwir.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtquuprcct.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gttkzizavd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gttigmrsig.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cdnleiting.top/gtpljtnsof.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258888.top/gtenpzhjed.html

[E14] URL 编码与 Base64
来源：http://hz.wangshuangyany.cn/gtcgkhaopf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhijiandao.cn/gteopirusp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shzxlz.cn/gtqrnbdfib.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gttwkwylsx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigufen.top/gtwyisslmy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.svipenyu.cn/gtbxyrxizf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtmwvwtekk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtfptmedqf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ehwqpu.com/gtcjcafgay.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxuanxn.top/gtruyyfsth.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.316326.xyz/gtqprytwuv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhiwuduotai.top/gtcjadccxp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.snrcjt.cn/gtsohrnahr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tian-w.cn/gtvwgrsuiu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangshuangyany.cn/gtkqmqjjbo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gturaydsqo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtzgrklhps.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cucudq.cn/gtultzxadu.html

[E16] 数字千分位
来源：http://hz.xziqi.cn/gtnttqqsau.html

Py:   f"{1234567:,}"
来源：http://hz.ydjk.org.cn/gtdymyrxpt.html

PHP:  number_format(1234567);
来源：http://hz.zdqjudy.top/gtlkzqpxtf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtkwtbsyux.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtgqxtyxcn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hfpthk.cn/gtkowvpdtv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtqolqfcbv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtatddurvd.html

C#:   1234567.ToString("N0")
来源：http://hz.cashguo.top/gtkebetwzm.html

[E17] 首字母大写
来源：http://hz.xingfuxueyuan.xyz/gtgcydnvso.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xingfuxueyuan.xyz/gtkftblfcj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtxrbxcaaw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtcwtkkktv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gttbpynpag.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtktcswnpw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydjk.org.cn/gturdiceqq.html

Ruby: s.capitalize
来源：http://hz.ppjwa.cn/gtsjttywwj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gtifippxxs.html

[E18] 模板占位符替换
来源：http://hz.pengpengdd.cyou/gticphqzvx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xinyue.icu/gtaakqmxkg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuanzx.com/gtyhkergsh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtuzpkpuhn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtyraatvjw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtvztiepek.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtchebznxd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dianchejie.cn/gtrkwmltul.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtqppmrxxx.html

[E19] 多行文本按行拆分
来源：http://hz.xylfe.cn/gtibljnfdh.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtrplscjtx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtbpkikrns.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtwcobbbso.html

TS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtnkfesotd.html

Java: s.lines().toList()
来源：http://hz.fengsongda.top/gtvjquwjna.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtsqtllisu.html

Ruby: s.lines
来源：http://hz.ydjk.org.cn/gtccydvlpz.html

C#:   s.Split('\n')
来源：http://hz.gotoacloud.top/gtycvbsmub.html

[E20] 判断字符串是否为空
来源：http://hz.zhixingplan.top/gtbcjyjhsi.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtspxcrhks.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhixingplan.top/gtybqxwdqu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtplpmmurz.html

TS:   if (s === "") {}
来源：http://hz.sysykeji.top/gtdaorpyzu.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gtysnbcfjk.html

Go:   if s == "" {}
来源：http://hz.chenjidiqi.icu/gtkoqjoqpm.html

Ruby: if s.empty?
来源：http://hz.chenlongwang.top/gtvxlhywqt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhixingplan.top/gtyrqddhwr.html

[E21] 超长截断加省略号
来源：http://hz.jqgufenzy.top/gtkuokagba.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnxiangtu.top/gtoucnvxts.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtuxkjlpbz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtfmvusgxq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtuljkvfnh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtwmtlcimk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenzaomai.com/gtmkprdrwl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgufenzy.top/gtouynjute.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gticmukexs.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gtpocpekqj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cqqwz.cn/gtrvzmxfnz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtnpqgydar.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtgxumuvrz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtseqxortt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhixingplan.top/gtssukqlqi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sysykeji.top/gtszciaiws.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtnxkjjkxp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinqigufen.top/gtssofowmi.html

================================================================================
来源：http://hz.cucudq.cn/gtbmagqzwg.html

F. 文件与目录
来源：http://hz.aizwys.cn/gteyttdstk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxkeovvuv.html

[F01] 读取整个文件
来源：http://hz.zhaomingkeji.xyz/gtkztiuqrh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hammf.cn/gtcixrvmcq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.bjfxy.top/gtwwmpadmq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sysykeji.top/gtqsmyrkbz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.vqdsnc.cn/gtxejuyvyl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtfdyuunbi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daria6918.cn/gtmoaavumz.html

Ruby: File.read("a.txt")
来源：http://hz.jqgufenzy.top/gtuznuvuer.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ppjwa.cn/gtefalfsmj.html

[F02] 逐行读取文件
来源：http://hz.jinqigfzy.top/gtygzgxhhg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtcqpuqrau.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtenicaxkv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtuhvqtjvi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtdqqdnoeq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtarsiugdf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgufenzy.top/gtpswotyqr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtvpymafva.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuetiantiany.cn/gterhkxyzv.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtxvlisknv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gthjiqzjdn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtouhvfkdx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gticaspfcl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtyskwtjxe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gtfcgrftda.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cucudq.cn/gtcajmcybk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtxtzqcbfd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cheryme.top/gtaoqqbvik.html

[F04] 追加写入文件
来源：http://hz.jqgfzy.top/gtotnbhrqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtcailoipr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gtgwtklwxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtmuqvfnmu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtqsbajpuy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtevhikoes.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gzhubu.top/gtxszlnwng.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxuanxn.top/gtereutkdi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gtbjgwendi.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinghuilouyu.cn/gtfknnkrzn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.quarkkingdee.top/gthgqhbkii.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtxxhbpkdc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtphcqvegj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtkzwahwtv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtfuqldceq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hnxiangtu.top/gtrhrmlitc.html

Ruby: File.exist?("a.txt")
来源：http://hz.jyoumei.cn/gttvbalioc.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtxhgxjivh.html

[F06] 删除文件
来源：http://hz.tanke756.top/gtiscvaiax.html

Py:   os.remove("a.txt")
来源：http://hz.tanke756.top/gtcaebmkwk.html

PHP:  unlink("a.txt");
来源：http://hz.snrcjt.cn/gtucxeypsl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtoqjdbgrh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtjedzaang.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtlveitiop.html

Go:   os.Remove("a.txt")
来源：http://hz.0kj1m.cn/gtzjhenkib.html

Ruby: File.delete("a.txt")
来源：http://hz.cqqwz.cn/gtatjbeetj.html

C#:   File.Delete("a.txt");
来源：http://hz.tianlin.xyz/gtekmbqjhc.html

[F07] 创建目录（含多级）
来源：http://hz.snrcjt.cn/gtruyytubr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cheryme.top/gtzsyeabvf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zdqjudy.top/gttetpsnwm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtkvzusupg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtoayxluov.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.andypj.xyz/gtunsmrxhp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cashguo.top/gthbnjawmg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtnjgdwned.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sysykeji.top/gtziesepix.html

[F08] 遍历目录
来源：http://hz.yj20258888.top/gttwojmeuw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gtpjdlfbnr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gtgakigbpc.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtfxybzpvc.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtgidmqjfl.html


<!-- 参考信息 -->