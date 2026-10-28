代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtclurclrp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxuanxn.top/gtzymatxhg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhaomingkeji.xyz/gtkhjfdnep.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ppjwa.cn/gtzljwhdel.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtmaqwdpwn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jyoumei.cn/gtxzvurbwv.html

[D25] Set 集合去重与交并差
来源：http://hz.quarkkingdee.top/gtyphhoyxv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sweek.top/gtdmazxykr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtqivqstkw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.c1oappe.top/gteumnovmx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtkssfupwd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hysaishi.cn/gtdiknwvel.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gteuhffysf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ehwqpu.com/gtqqviapkp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtsgkamyea.html

[D26] 数组转字符串
来源：http://hz.pycfn.com/gtatmoujxs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtwdszawjw.html

PHP:  implode(", ", $arr);
来源：http://hz.gzhubu.top/gtdwkqpifn.html

JS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtlsgjvpar.html

TS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtxtgkcemj.html

Java: String.join(", ", list)
来源：http://hz.gotoacloud.top/gtfuyrbhca.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtekdqggjy.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gtqiupgzvj.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gttqzrigiw.html

================================================================================
来源：http://hz.cheryme.top/gtrmepaswe.html

E. 字符串处理
来源：http://hz.zhiwuduotai.top/gtrucuenne.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtvchvmjiz.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtxcohybyv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hongshengwenyu.top/gtqesnarsb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.mhx1999.top/gtvnwdyukp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sufxvd.cn/gtdnbawdkw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gttekryaad.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtmkmobeqq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gtoltfqdjc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shzxlz.cn/gtbwxnupum.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sufxvd.cn/gtbisolrjc.html

[E02] 重复字符串
来源：http://hz.zhengqikj.top/gtvmmkxvmn.html

Py:   "ab" * 3
来源：http://hz.fengsongda.top/gtwubmsyzd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sysykeji.top/gthmlrargg.html

JS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtbezsmpri.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtomaaocad.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gttoawpmow.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangdashe.top/gtklzugcqf.html

Ruby: "ab" * 3
来源：http://hz.zhengqikj.top/gtabfsspvh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gzhubu.top/gtcsegkwmy.html

[E03] 截取子串
来源：http://hz.bjfxy.top/gtlufmmrhw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yongpay.top/gthosnrzva.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jianghu66.top/gtzyptxifz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.havefunace.top/gtufukizzo.html

TS:   s.slice(1, 4)
来源：http://hz.sufxvd.cn/gtlaalrprq.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtkffugjqe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gtwuocxmbp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aizwys.cn/gthmvpyzfe.html

C#:   s.Substring(1, 3)
来源：http://hz.c1oappe.top/gtjrynrdlq.html

[E04] 查找子串位置
来源：http://hz.quarkkingdee.top/gthczsjmer.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ehwqpu.com/gtwkxrbqae.html

PHP:  strpos($s, "x");
来源：http://hz.snrcjt.cn/gtabdkwdgq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.0kj1m.cn/gtndnzejjt.html

TS:   s.indexOf("x")
来源：http://hz.0kj1m.cn/gtwsgfqclv.html

Java: s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtthgiyuhf.html

Go:   strings.Index(s, "x")
来源：http://hz.9152youxi.cn/gtpyvwiaqw.html

Ruby: s.index("x")
来源：http://hz.wangdashe.top/gthbosiudz.html

C#:   s.IndexOf("x")
来源：http://hz.zycfv.cn/gthwbsebpl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtndecszpb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.snrcjt.cn/gtrhoieckx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.52xcode.cn/gtmevhzexs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtsjujnisi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtwjkswlub.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtudnesfdp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.redwolf501.top/gtrmybcsqz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtwhlrlmti.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yanxiufei.cn/gteranunmt.html

[E06] 替换子串
来源：http://hz.havefunace.top/gtglysgssf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gotoacloud.top/gtcrwvlzac.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shangyingyoupin.top/gtmronhpgl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtlgruwbif.html

TS:   s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtrdosfjzg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtizamcwmg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.0kj1m.cn/gtjouyjvgq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtxekfzvbb.html

C#:   s.Replace("a", "b")
来源：http://hz.chenjidiqi.icu/gtmywgfaom.html

[E07] 按分隔符拆分
来源：http://hz.cdnleiting.top/gtshzwwazk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xinyue.icu/gtabqcmpfq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj202588.top/gtwvwdgoop.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.bjfxy.top/gtrxetskum.html

TS:   s.split(",")
来源：http://hz.zhixingplan.top/gtdmyprusa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zycfv.cn/gtijwfpwau.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xinyue.icu/gtdexxjxjs.html

Ruby: s.split(",");  s.split
来源：http://hz.pengpengdd.cyou/gtyodwyejz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gtrkycwhvv.html

[E08] 数组按分隔符合并
来源：http://hz.kuanghao11.cn/gtuoyavcqa.html

Py:   ",".join(items)
来源：http://hz.jqgfzy.top/gtwhcukjry.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtwxqnjjkn.html

JS:   items.join(",")
来源：http://hz.chenzaomai.com/gtnptpsfqp.html

TS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtsxcuxcxh.html

Java: String.join(",", items)
来源：http://hz.ywan-chungtsiang.top/gttlegwxii.html

Go:   strings.Join(items, ",")
来源：http://hz.sxryk.cn/gtzwdbmoze.html

Ruby: items.join(",")
来源：http://hz.zhixingplan.top/gtgmwpened.html

C#:   string.Join(",", items)
来源：http://hz.shangyingyoupin.top/gtcsvmpjbq.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtkwdticoe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cheryme.top/gtzxcrlpfe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenlongwang.top/gtzkdndxye.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtypyivapl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xuetiantiany.cn/gthoqxwbof.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guowangkeji.top/gtwiahtikz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhoulong.xyz/gttyawcojv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jiagoushi.top/gtktuzoljy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jiagoushi.top/gtlcjpgbox.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtkdwduptd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangdashe.top/gtgjdbtlvl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gttuwvqkcw.html

JS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtqimdjrhp.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtfbzntjmv.html

Java: String.format("%03d", 7)
来源：http://hz.gotoacloud.top/gtqxeupgbx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydzc1.top/gtsvayeory.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tianlin.xyz/gtwyxclisx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenzaomai.com/gtsudnuvjq.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gtshyzwspi.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gtldlqagsx.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtiqmiozqf.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtxjiqlptb.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtnlgmbbkk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.redwolf501.top/gtppndbdby.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtvfoltkgu.html

Ruby: s.reverse
来源：http://hz.yonumen.top/gtlzweozfg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtjkrdgxck.html

[E12] 统计某字符出现次数
来源：http://hz.hysaishi.cn/gtkrtwycbs.html

Py:   s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtsewzxmpe.html

PHP:  substr_count($s, "a");
来源：http://hz.chenzaomai.com/gtolzpfwej.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtiqrymasi.html

TS:   s.split("a").length - 1
来源：http://hz.xingfuxueyuan.xyz/gtxmvvsryo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxinkj.top/gtzzhnmoba.html

Go:   strings.Count(s, "a")
来源：http://hz.zycfv.cn/gtmgxypfkk.html

Ruby: s.count("a")
来源：http://hz.zhongyouzk.top/gthacbuzwj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhijiandao.cn/gtfdrfjchh.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtqrcbyotk.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtxobyqnyt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gtgystoxao.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtzsnwxjgz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtnnrlvrzc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangkeji.top/gtpjzeatew.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.svipenyu.cn/gthokcemqm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hnxiangtu.top/gtmvorvzou.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258.top/gtzyqngyby.html

[E14] URL 编码与 Base64
来源：http://hz.yvedp.cn/gtrqlactvo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gtyeoexgfd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xylfe.cn/gtlfuvzyms.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yonumen.top/gticfdzczk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gtzzdjgxrg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangkeji.top/gtnzkknhpv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gttskjhlwt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangdashe.top/gtqbzbtitm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daxiang520.top/gtftqzbwye.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigufen.top/gtbmcudakv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangkeji.top/gtdrzwoatg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtnrnlvgwu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuxming.cn/gtnlhqwswn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.bjfxy.top/gtcbwxgmla.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fzhhl.top/gtvescehig.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gaohongyu789.top/gtlqwjbudo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guannengcc.top/gtvktsxoqe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yj20258888.top/gtfajbbipn.html

[E16] 数字千分位
来源：http://hz.dianchejie.cn/gtzntechao.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gtzpudolca.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtcebbittw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtckzlbzrq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtstnoiswc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aibaodan.cn/gtitfezgxp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.iojbl.cn/gtbzxhgxjl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zdqjudy.top/gtgxcanctm.html

C#:   1234567.ToString("N0")
来源：http://hz.ywan-chungtsiang.top/gtltebrmqu.html

[E17] 首字母大写
来源：http://hz.gaohongyu789.top/gtnpzbfszt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ywan-chungtsiang.top/gtqdtwexqt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuxming.cn/gtjcytjwuk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtivunirba.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtqrmjejmz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hongshengwenyu.top/gtliaicdmb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fzhhl.top/gtzuetosuo.html

Ruby: s.capitalize
来源：http://hz.haohaochexian.top/gtfznvupfo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gtabcfmcds.html

[E18] 模板占位符替换
来源：http://hz.yvedp.cn/gtqgrtnovz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nwbrower.top/gtqibukizk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sufxvd.cn/gtvpslzyjd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigfzy.top/gtjcwxhqqx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gtmswjcmcu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gtmqslwzpk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gtzoyklogq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtsfbjnrfg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtefzcoari.html

[E19] 多行文本按行拆分
来源：http://hz.svipenyu.cn/gtmhgczzqo.html

Py:   s.splitlines()
来源：http://hz.snrcjt.cn/gtwgjgbazq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gtmxpvmybo.html

JS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtffsfjett.html

TS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtmxjoryct.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtoplikaes.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtcsxznqya.html

Ruby: s.lines
来源：http://hz.hywenlv.cn/gtxycckjko.html

C#:   s.Split('\n')
来源：http://hz.xziqi.cn/gtgoccovul.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtirlexmzg.html

Py:   if not s:
来源：http://hz.jiagoushi.top/gtxeguvwun.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtfdqgjglt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cheryme.top/gtgosyoovk.html

TS:   if (s === "") {}
来源：http://hz.gaohongyu789.top/gtixlzfjkm.html

Java: if (s.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtyhnuekwf.html

Go:   if s == "" {}
来源：http://hz.cdnleiting.top/gtxdcbnsuj.html

Ruby: if s.empty?
来源：http://hz.xziqi.cn/gtnsrhdtrx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xziqi.cn/gtoreomvla.html

[E21] 超长截断加省略号
来源：http://hz.havefunace.top/gtftxfipwt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258888.top/gtcgcwypwv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtgfjyxhoj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtleeimpme.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtdbilwgub.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtivzflplv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hywenlv.cn/gtjohdvlev.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtzpmlqxfu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cucudq.cn/gtyyzonmke.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtvxyrckiz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sweek.top/gtovvjufcp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhengqikj.top/gtuqnzdsfw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zycfv.cn/gtzwpdmmbc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtrpsuvgoj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenzaomai.com/gthakavmvo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.iojbl.cn/gtpoegntnf.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtxktoyrgm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtbywvdvbe.html

================================================================================
来源：http://hz.chenlongwang.top/gtwksfzhno.html

F. 文件与目录
来源：http://hz.nanxuanxn.top/gtdvwcmpay.html

================================================================================
来源：http://hz.bjfxy.top/gtdifnzgks.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtrjjjalat.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtvjxchgsy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.feifeiyinyue.top/gtwtmcmajt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangtech.top/gttynifoqt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtqkkfuzob.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtdjhypois.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtmusjjpkp.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtmtdrpbcm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gotoacloud.top/gtknrgvpfz.html

[F02] 逐行读取文件
来源：http://hz.wangdashe.top/gtqlupggjr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhongyouzk.top/gtsssthvfl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sysykeji.top/gtucufscrm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtbrctfapn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtzmlqjvcy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gthrdkrojf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ywan-chungtsiang.top/gtwoywqgzq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258888.top/gtvacfueeg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtzhvbublh.html

[F03] 写入文件（覆盖）
来源：http://hz.yvedp.cn/gtutmcvpdy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.9152youxi.cn/gtrgkctdol.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gtpcchnzzw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gttwggykgf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtikljqarb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tanke756.top/gtzdszftye.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangshuangyany.cn/gtjryteopc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258.top/gtxseeznnw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xinyue.icu/gthdkobwjm.html

[F04] 追加写入文件
来源：http://hz.ywan-chungtsiang.top/gtaadfkrus.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtxkndvjwt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gzhubu.top/gtzlztgfmu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtwxrwveyi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtxqblcqhq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxuanxn.top/gteaprobuk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigfzy.top/gttcsryxbk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtbapggcjc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.feifeiyinyue.top/gtesoxoijx.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gtyqqlqtii.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtlxorpyrq.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtwjozemnv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtiihqxdir.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gthyzgfbjh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtmjwinjjy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj202588.top/gtbcnrcwnn.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtzmpwkjio.html

C#:   File.Exists("a.txt")
来源：http://hz.shuidangran.top/gtvpufvmtq.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtzlqpiiig.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigfzy.top/gtqufyzfmf.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gtruearwfi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtveqwsatt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtmrczkddf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtklkllimd.html

Go:   os.Remove("a.txt")
来源：http://hz.fengsongda.top/gtbhthtmzr.html

Ruby: File.delete("a.txt")
来源：http://hz.yueranfly.top/gtrixfoqew.html

C#:   File.Delete("a.txt");
来源：http://hz.quarkkingdee.top/gtblhmafxl.html

[F07] 创建目录（含多级）
来源：http://hz.jqgfzy.top/gtbnmwyuvc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtndtibqjc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.svipenyu.cn/gtmcrnuwpc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gthqdxgxhc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtziafnixu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xziqi.cn/gtzzojwkjw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtsripsmle.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhoulong.xyz/gttofgsffm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gtlnkxmrmh.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gtsmpzyemk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtzsbddhni.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtvayovake.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtaptdkvja.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtoaaxzmdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtraarlpfz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hongshengwenyu.top/gtzeckvakd.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtqiutqpox.html

C#:   Directory.GetFiles("dir")
来源：http://hz.mhx1999.top/gteurxlwej.html


<!-- 参考信息 -->