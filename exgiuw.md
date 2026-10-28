代发 wailian999

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gtnvbeomvc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtkxvvowql.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangdashe.top/gtxjklmlms.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtwyetvoee.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtgkiuhuuu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yangfankeji.com/gtclsqrlpj.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtdfpriwdl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.meibo888.top/gtbjemizch.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydjk.org.cn/gtgqxgswrn.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuetiantiany.cn/gtssypnwnf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangtech.top/gtaodauhpi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtxbsazgfr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gteiyobkgs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtalxzwbss.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtongyeuxu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtcyrtcdfp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shangyingyoupin.top/gtlahwudnz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtayutcswe.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtbnrsqxog.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sweek.top/gtvutzgpkq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zycfv.cn/gtrxjmqzmc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zdqjudy.top/gtrpxeozdh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gtyvzfpxcj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtichdkyeo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tanke756.top/gtopehrhjz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.quarkkingdee.top/gtugftkhzk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.haohaochexian.top/gtepuegbxa.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtbzapikvn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangshuangyany.cn/gtuvhavaxb.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtxjidtphx.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtihmzskxh.html

TS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtiiawnegd.html

Java: String.join(", ", list)
来源：http://hz.hnxiangtu.top/gtixgeadrn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.wangdashe.top/gtyqrgoghb.html

Ruby: arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtznbhguxg.html

C#:   string.Join(", ", list)
来源：http://hz.c1oappe.top/gtdvkvypjg.html

================================================================================
来源：http://hz.snrcjt.cn/gtghlvtwtw.html

E. 字符串处理
来源：http://hz.jinghuilouyu.cn/gtyhsjfdng.html

================================================================================
来源：http://hz.jinqigufen.top/gtyqvmtgsg.html

[E01] 拼接字符串
来源：http://hz.sxryk.cn/gtneelzcai.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj202588.top/gtpqavsouj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.0kj1m.cn/gtjrbwsutq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gthcusvbzf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtkysnzhfn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xingfuxueyuan.xyz/gtgueikwng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.c1oappe.top/gtqrylrywi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangshuangyany.cn/gtxffvjoel.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tianlin.xyz/gtikyekyre.html

[E02] 重复字符串
来源：http://hz.jinghuilouyu.cn/gtroeksbev.html

Py:   "ab" * 3
来源：http://hz.ybcxt.top/gtsgzgldop.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cashguo.top/gteqqavxup.html

JS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtpbihqcjc.html

TS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtbiutofqc.html

Java: "ab".repeat(3)
来源：http://hz.tanke756.top/gtbbncqdoe.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ydjk.org.cn/gtnzrnyouj.html

Ruby: "ab" * 3
来源：http://hz.aizwys.cn/gtpxeyfjlt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hysaishi.cn/gtifphmhcd.html

[E03] 截取子串
来源：http://hz.pengpengdd.cyou/gtmualbovy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.0kj1m.cn/gtcdtzhjdk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtllemhand.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gtrogllaiv.html

TS:   s.slice(1, 4)
来源：http://hz.hnxiangtu.top/gtlztyjjhg.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtiqcatkel.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ywan-chungtsiang.top/gtcfqvftko.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.andypj.xyz/gtffgfdpgv.html

C#:   s.Substring(1, 3)
来源：http://hz.pycfn.com/gtbodicawv.html

[E04] 查找子串位置
来源：http://hz.hammf.cn/gtinucqlqp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zdqjudy.top/gtcdvwrivj.html

PHP:  strpos($s, "x");
来源：http://hz.zhixingplan.top/gteayrlwnw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.bjfxy.top/gtkgcbhlib.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtqptsdiqh.html

Java: s.indexOf("x")
来源：http://hz.birdmap.top/gtzaqyrmpi.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtvhtckpju.html

Ruby: s.index("x")
来源：http://hz.hnxiangtu.top/gtjgyzrsbf.html

C#:   s.IndexOf("x")
来源：http://hz.zdqjudy.top/gtephibesa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenjidiqi.icu/gtrvewplup.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.bjfxy.top/gtjeasbfev.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gaohongyu789.top/gtvijzmpth.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtvyfxglqz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtatuojtio.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtwzpjbrdx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sufxvd.cn/gtywacvhsc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangshuangyany.cn/gtzpultcid.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtxoofpuhw.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtlgwibnos.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ydjk.org.cn/gtwgsepssh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhiwuduotai.top/gtqnwcnmdu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtwaacomsa.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtxcjlwltx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtnhaqtkbr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.316326.xyz/gthrjjjqiu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ybcxt.top/gtuiugqfyx.html

C#:   s.Replace("a", "b")
来源：http://hz.cqqwz.cn/gtxlahhfhh.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtldbucixg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gzhubu.top/gtdbjogesd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtymmwtyli.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtzcexotjc.html

TS:   s.split(",")
来源：http://hz.jqgufenzy.top/gtfrunerli.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.kuanghao11.cn/gtxsrzzlac.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258888.top/gtxxxdgyrn.html

Ruby: s.split(",");  s.split
来源：http://hz.shzxlz.cn/gtkddbnpyo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pengpengdd.cyou/gtuawybcam.html

[E08] 数组按分隔符合并
来源：http://hz.hnxiangtu.top/gtqwmrsrrd.html

Py:   ",".join(items)
来源：http://hz.ydjk.org.cn/gtctqkgixr.html

PHP:  implode(",", $items);
来源：http://hz.hfpthk.cn/gtaojdutcp.html

JS:   items.join(",")
来源：http://hz.fengsongda.top/gtwcczibjm.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtmunzmyho.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gtalfxikas.html

Go:   strings.Join(items, ",")
来源：http://hz.ywan-chungtsiang.top/gturljlpmg.html

Ruby: items.join(",")
来源：http://hz.chenjidiqi.icu/gtqsgksfxg.html

C#:   string.Join(",", items)
来源：http://hz.yangfankeji.com/gtfcmjgxkc.html

[E09] 去除所有空白字符
来源：http://hz.hysaishi.cn/gtzeawwbeb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtqdoexxsg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.fzhhl.top/gtkdanltnj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtchyeybzx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtickjcpqs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtlozlpbjk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtjsjodcxc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnxiangtu.top/gtclznbjug.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhaomingkeji.xyz/gtfbryoebh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.wangshuangyany.cn/gtexdbumzr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinghuilouyu.cn/gtvrceprid.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shuidangran.top/gttgubwxqo.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtlmycotmj.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtizvwrvvt.html

Java: String.format("%03d", 7)
来源：http://hz.andypj.xyz/gtyvnajadt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtzbaetsmd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtcwsmicnk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ivvv.top/gtgbuwlkqj.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gtvgjwjdqs.html

Py:   s[::-1]
来源：http://hz.wangdashe.top/gtbvazzxed.html

PHP:  strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtpekwjqyy.html

JS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtsjnxbulj.html

TS:   [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtwondoyat.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258888.top/gtyczusiqj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.9152youxi.cn/gtumjazmcu.html

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtiivzodud.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtvollhrpj.html

[E12] 统计某字符出现次数
来源：http://hz.hammf.cn/gtzljttfms.html

Py:   s.count("a")
来源：http://hz.nanxinkj.top/gttcipbccq.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxuanxn.top/gtdedyrbks.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtaxybcghx.html

TS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gttvnembfg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigufen.top/gtujitphhv.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gtrploqjkn.html

Ruby: s.count("a")
来源：http://hz.birdmap.top/gtgbslslpm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gthfypvvon.html

[E13] 逐字符遍历
来源：http://hz.birdmap.top/gtzqkxzcuk.html

Py:   for ch in s: print(ch)
来源：http://hz.sxryk.cn/gtsjjsqqgc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sufxvd.cn/gtublxwauu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtfovravjy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtjznxinwz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydjk.org.cn/gtutktjolg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ybcxt.top/gtvtnqnjqu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gtpqqljzmu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhoulong.xyz/gtflfffkjp.html

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtismehgej.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gtnkjyyxhl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgufenzy.top/gtpnvkrlkk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gtmejqgsvw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gtcpfvxsqw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.iojbl.cn/gtcnscdfko.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shzxlz.cn/gttgzsiqpq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ydzc1.top/gtymyayibx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangshuangyany.cn/gttgwyoptg.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtqbttplze.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtjmgffbvv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj202588.top/gtvybfumsq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.vqdsnc.cn/gteauafmgl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtfvwnecad.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gotoacloud.top/gttbafrway.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hongshengwenyu.top/gtcfmznuua.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gogol.net.cn/gtovesfnem.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dianchejie.cn/gtufivyxst.html

[E16] 数字千分位
来源：http://hz.jqgufenzy.top/gtbrtzngqm.html

Py:   f"{1234567:,}"
来源：http://hz.chenzaomai.com/gtekcrbxmc.html

PHP:  number_format(1234567);
来源：http://hz.jqgfzy.top/gtamsjsiap.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtftdcmzyg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtgtesgxpx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zycfv.cn/gtqhbincap.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtvhdtskev.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhengqikj.top/gthfchkxtf.html

C#:   1234567.ToString("N0")
来源：http://hz.yongpay.top/gtpoeibyrv.html

[E17] 首字母大写
来源：http://hz.yuxming.cn/gtxndfdhgu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhoulong.xyz/gtdhnmhuoh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtrhjuqhnn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gthfqzhgqu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtiysrrqln.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hnqzz.top/gtafvbqvcj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gtlhrtamiv.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtcsshnvhz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.bjfxy.top/gtphkibqfp.html

[E18] 模板占位符替换
来源：http://hz.cqqwz.cn/gtppquarwo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shanyushiyangkeji.top/gtcymnjong.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.andypj.xyz/gtlhlhqmyr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtdsdwtpgd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.mhx1999.top/gtlrokgevs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtaqqtliss.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guowangkeji.top/gtntxpptyh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.meibo888.top/gtljlllqmm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nwbrower.top/gtuhdnzgnj.html

[E19] 多行文本按行拆分
来源：http://hz.jiagoushi.top/gtkieezlso.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtnwxntjij.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtdsfbjhoy.html

JS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtggdfqtqp.html

TS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtipmpiqgh.html

Java: s.lines().toList()
来源：http://hz.guannengcc.top/gtfnvptzti.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangkeji.top/gtnwhytklh.html

Ruby: s.lines
来源：http://hz.fengsongda.top/gtobonyeou.html

C#:   s.Split('\n')
来源：http://hz.xylfe.cn/gtwtqfsbqv.html

[E20] 判断字符串是否为空
来源：http://hz.xuanzx.com/gtsjsnowgz.html

Py:   if not s:
来源：http://hz.pycfn.com/gtjhuqfgfk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xylfe.cn/gtqzgqaane.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.316326.xyz/gtwqssxlsz.html

TS:   if (s === "") {}
来源：http://hz.bjfxy.top/gtbirvqbah.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinghuilouyu.cn/gtzofxjcha.html

Go:   if s == "" {}
来源：http://hz.smart0.xyz/gttfbznodl.html

Ruby: if s.empty?
来源：http://hz.ivvv.top/gtgglmzhsh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtovjtvdyp.html

[E21] 超长截断加省略号
来源：http://hz.cqqwz.cn/gtrkuilzro.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuanzhike.top/gtteogjmde.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cqqwz.cn/gtdaposqtx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtprnbqzfn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gttjhesyjw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtumzucmqg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zycfv.cn/gtlnafhbim.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtqcjsrmew.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtwfafyepj.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gtscxnlzzt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ywan-chungtsiang.top/gtgipsldpa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtwuevwcqf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtplqjcymi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtgvyuybco.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hywenlv.cn/gtydgzjdsy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hongshengwenyu.top/gttesoryvm.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtoncuvhcl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guowangkeji.top/gtgyotamhx.html

================================================================================
来源：http://hz.snrcjt.cn/gtbffoyfjo.html

F. 文件与目录
来源：http://hz.316326.xyz/gthrsrrzsa.html

================================================================================
来源：http://hz.havefunace.top/gtwwgnrbmw.html

[F01] 读取整个文件
来源：http://hz.feifeiyinyue.top/gtkabljwql.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shangyingyoupin.top/gtnvwjofpg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aizwys.cn/gttiyikbjo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dianchejie.cn/gtrtorlzfq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydjk.org.cn/gtrwzkfrii.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gteawjxdoj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hywenlv.cn/gtutsjvzej.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtrzjfhcic.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tanke756.top/gtregbtxnu.html

[F02] 逐行读取文件
来源：http://hz.ehwqpu.com/gtrppnryuz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yueranfly.top/gtmicsmgcw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gtbqtcagqz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtnhmoaruo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtgrkdmqoq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtsmolqbjy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jlsjyb.cn/gtpxlvieme.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.daria6918.cn/gtfivuvoyp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gtlavoyehc.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtohbpzzao.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cucudq.cn/gtbczmqjka.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtxxcnlvlk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtdfuaxahy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtfdcmuakf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cucudq.cn/gtjcqaphuq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.havefunace.top/gtjrsfdvdc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtkpdpzysw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gttnoudfwo.html

[F04] 追加写入文件
来源：http://hz.jyoumei.cn/gtxzkluvuw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtpxltizzv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gtwlxhnwqr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtcgkeafgo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guowangkeji.top/gtxqizgfxq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dashuyun.cn/gtlenggdbb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtlyhldjkg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gtxugrxigi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinyuanbaomall.cn/gttebbyvsl.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhijiandao.cn/gtrxcgcfts.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinyuanbaomall.cn/gttuenmcwk.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtehpiiasz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtbtjheehl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gttmjhooiw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtvqmjrdxq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yangfankeji.com/gtdwdxlqgc.html

Ruby: File.exist?("a.txt")
来源：http://hz.cdnleiting.top/gtusvsgdjs.html

C#:   File.Exists("a.txt")
来源：http://hz.birdmap.top/gtetibijui.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtpprbxcsa.html

Py:   os.remove("a.txt")
来源：http://hz.0kj1m.cn/gtievquqde.html

PHP:  unlink("a.txt");
来源：http://hz.xuanzx.com/gtwpwoplfl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtaymjrvhr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtsbameqns.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtunfwckwg.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtnewidmix.html

Ruby: File.delete("a.txt")
来源：http://hz.gotoacloud.top/gtozwhhrcg.html

C#:   File.Delete("a.txt");
来源：http://hz.quarkkingdee.top/gtgmegvgph.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtsgnvoglh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dashuyun.cn/gtwczjtsxc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtublygrqk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtaslmpori.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtuzkergen.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gtttbmnigu.html


<!-- 参考信息 -->