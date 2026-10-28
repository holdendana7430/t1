代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinyuanbaomall.cn/gtnngecmgl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxinkj.top/gtvegczhjd.html

[D25] Set 集合去重与交并差
来源：http://hz.zhengqikj.top/gtpslqyqyb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtpjbueyru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cashguo.top/gtygvfsaya.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhongyouzk.top/gtktzeourh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenzaomai.com/gttahfvuqp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jyoumei.cn/gtmrmatkfk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinghuilouyu.cn/gttwrvazhi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zdqjudy.top/gthjomxdgs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhaomingkeji.xyz/gtdyacwmeg.html

[D26] 数组转字符串
来源：http://hz.vqdsnc.cn/gthixaoage.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ppjwa.cn/gtqlmjgxlf.html

PHP:  implode(", ", $arr);
来源：http://hz.xziqi.cn/gtvfwyqstr.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtdntwgvrq.html

TS:   arr.join(", ")
来源：http://hz.yj20258.top/gtgkejrizp.html

Java: String.join(", ", list)
来源：http://hz.xinyue.icu/gtztgbghxk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigufen.top/gtnkkdrqqa.html

Ruby: arr.join(", ")
来源：http://hz.zycfv.cn/gtbqxtamfz.html

C#:   string.Join(", ", list)
来源：http://hz.xuanzx.com/gtktkhodxc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdtcuzcvk.html

E. 字符串处理
来源：http://hz.pycfn.com/gtljkgugnt.html

================================================================================
来源：http://hz.yonumen.top/gtxulznloh.html

[E01] 拼接字符串
来源：http://hz.chenzaomai.com/gtodbtyrub.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gthfxuhfon.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gtfleiqjae.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtzkbokmqf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtgonqjcmw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tian-w.cn/gtmnzgwpoo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hywenlv.cn/gtpoqcddwi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinghuilouyu.cn/gtazbguidc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangtech.top/gtytmvaluu.html

[E02] 重复字符串
来源：http://hz.tianlin.xyz/gtjubwculk.html

Py:   "ab" * 3
来源：http://hz.hnqzz.top/gtleidjwoh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtjnsbefvi.html

JS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtgbepqthz.html

TS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtclahycpa.html

Java: "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtbjvqpaok.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhaomingkeji.xyz/gtkluocnve.html

Ruby: "ab" * 3
来源：http://hz.guannengcc.top/gtlkyaxjxi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daxiang520.top/gtbfccvnzu.html

[E03] 截取子串
来源：http://hz.hysaishi.cn/gtosxgfwtr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xylfe.cn/gtsaopopjr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtehyudaew.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xziqi.cn/gtxxmqwlmx.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gteylubxkr.html

Java: s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtyokwezfg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cashguo.top/gttaqmzwfq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yonumen.top/gthesagrxd.html

C#:   s.Substring(1, 3)
来源：http://hz.quarkkingdee.top/gtgkwpzmhd.html

[E04] 查找子串位置
来源：http://hz.redwolf501.top/gtwypojqzi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuanzhike.top/gtyrfjvwpn.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gtyzosptcn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtfxccqgml.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtbndtlmwf.html

Java: s.indexOf("x")
来源：http://hz.cdnleiting.top/gtlcddbuvt.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gttigjiuck.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtvvzgkujj.html

C#:   s.IndexOf("x")
来源：http://hz.bjfxy.top/gtphfagpdc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sufxvd.cn/gtdjgdqgko.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgufenzy.top/gtwwkigwkp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydzc1.top/gtyurbgqjn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtrybnhghq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.haohaochexian.top/gtpaovwxfi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtoyrzgfqt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gtkerudoqx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinqigufen.top/gtlcbzezho.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtqztibsrz.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtjpyabxyn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.svipenyu.cn/gtpthzifaq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258888.top/gtqcowfptw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtjzfhhenx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtxobeltkv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtiwdzqmvh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sxryk.cn/gtnkbsyybf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxinkj.top/gtkvafhzft.html

C#:   s.Replace("a", "b")
来源：http://hz.pycfn.com/gtjnkitnjj.html

[E07] 按分隔符拆分
来源：http://hz.xylfe.cn/gtywucsinj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shuidangran.top/gtkkiojrqd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.quarkkingdee.top/gtvhusnrpy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nwbrower.top/gtmztiyluk.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtjgbppbmx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgufenzy.top/gtxbyobixi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtadrhvadh.html

Ruby: s.split(",");  s.split
来源：http://hz.zhijiandao.cn/gtnfkwdopt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cucudq.cn/gtluqgzhek.html

[E08] 数组按分隔符合并
来源：http://hz.pengpengdd.cyou/gtkhuchqch.html

Py:   ",".join(items)
来源：http://hz.tianlin.xyz/gtmoojaljq.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtjeztqoux.html

JS:   items.join(",")
来源：http://hz.316326.xyz/gtjnkadpdy.html

TS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtpbgoxdhx.html

Java: String.join(",", items)
来源：http://hz.nanxinkj.top/gtyyjdbzft.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangkeji.top/gtbnimykqg.html

Ruby: items.join(",")
来源：http://hz.fengsongda.top/gtuhmiwfuq.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtwfwyghim.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gteqcsuygq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daria6918.cn/gtegbsldac.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhoulong.xyz/gtpmfpjdtr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtodefdczl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtotigcoqz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.snrcjt.cn/gtnfdznlmy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtjeingiha.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258888.top/gtsuqcfyfs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuetiantiany.cn/gtakbaufsl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yvedp.cn/gtqrpcylwu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gotoacloud.top/gtmsmbsptw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangdashe.top/gtiguxjlmy.html

JS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtpcfkvrtn.html

TS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtrcmbyrnd.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtjorfmuck.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.feifeiyinyue.top/gthlmwtywe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hfpthk.cn/gtsdraednz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtrzdweqal.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gtoajalhhk.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtxpezhjug.html

PHP:  strrev($s);
来源：http://hz.cqqwz.cn/gtyxnducre.html

JS:   [...s].reverse().join("")
来源：http://hz.tian-w.cn/gticsixqyt.html

TS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtrqmvgdvk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnxiangtu.top/gtvpciiayh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ehwqpu.com/gtxenogyqm.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtjdubjqyo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtqmqklgcf.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtgjmehfjt.html

Py:   s.count("a")
来源：http://hz.sysykeji.top/gtvqbqebgq.html

PHP:  substr_count($s, "a");
来源：http://hz.andypj.xyz/gthzmwxwza.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtascdaedq.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtqgtqldic.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aizwys.cn/gtuylgnbdb.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtcrcxqmbw.html

Ruby: s.count("a")
来源：http://hz.jinghuilouyu.cn/gtvihjcvwq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gtusvughug.html

[E13] 逐字符遍历
来源：http://hz.ydjk.org.cn/gtzvoyfqmv.html

Py:   for ch in s: print(ch)
来源：http://hz.ydzc1.top/gtsdqzextx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtclgbnekr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtopvlkqpu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gttupmwupw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.smart0.xyz/gtpvyqhhxy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gotoacloud.top/gtmiuakhco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zycfv.cn/gtmxdfsigi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yonumen.top/gtcvakldmx.html

[E14] URL 编码与 Base64
来源：http://hz.tian-w.cn/gtoqcgkzrt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.meibo888.top/gtiwlrapnh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtxwkdjwbb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sysykeji.top/gtdwqkbdsh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhongyouzk.top/gtptgtowfc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.vqdsnc.cn/gteiivjrui.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydjk.org.cn/gtpbcrnswt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gtnltvhoor.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtibsiozyo.html

[E15] HTML 转义 / 反转义
来源：http://hz.shzxlz.cn/gteteyxlzv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xziqi.cn/gtiwfyvxcl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhijiandao.cn/gtdbvvvtzj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.quarkkingdee.top/gtkfjldkdi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.andypj.xyz/gtlmkzwssb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuanzx.com/gtvlqdrtal.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yvedp.cn/gtnuyuvttt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtgzwcjlcz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydjk.org.cn/gtanggnbmv.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtufuantir.html

Py:   f"{1234567:,}"
来源：http://hz.316326.xyz/gtsatwqcso.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtxqbhkuey.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtumagcwcv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtwdiilyrh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtpaxotgya.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gthsxcyjdd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.0kj1m.cn/gtcrnaynmp.html

C#:   1234567.ToString("N0")
来源：http://hz.zhongyouzk.top/gtspegstsq.html

[E17] 首字母大写
来源：http://hz.wangdashe.top/gtunlolpzx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xylfe.cn/gtxrniukvp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xuanzx.com/gtzohlxcez.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtallkzork.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gthmujzejz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gtniciytnd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gtqztkskdx.html

Ruby: s.capitalize
来源：http://hz.hnxiangtu.top/gtiidhpkii.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtwxwrnyou.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtuhranvoy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guowangkeji.top/gtcvbxevjo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yangfankeji.com/gtufgvnbso.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtomehmete.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtjkthxobn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gthuxsschr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhiwuduotai.top/gtyypdozrs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenzaomai.com/gttphxhbhn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.c1oappe.top/gtfpiwtbvc.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtudokycyj.html

Py:   s.splitlines()
来源：http://hz.jianghu66.top/gtqzqhdqcn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtsotcegay.html

JS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtbjxpgdce.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtgivdfrys.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtxnyudcjn.html

Go:   strings.Split(s, "\n")
来源：http://hz.aibaodan.cn/gtwnaqooru.html

Ruby: s.lines
来源：http://hz.zhongyouzk.top/gtzwqvrjjn.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtalwjllci.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtyemdtenf.html

Py:   if not s:
来源：http://hz.nanxinkj.top/gtgyjbprli.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zycfv.cn/gtjqjttecd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dianchejie.cn/gtjdgaxqpz.html

TS:   if (s === "") {}
来源：http://hz.fengsongda.top/gtbllgdwca.html

Java: if (s.isEmpty()) {}
来源：http://hz.pycfn.com/gtygtglpcb.html

Go:   if s == "" {}
来源：http://hz.smart0.xyz/gtxtfgpsuy.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtuzbwhous.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtlcclqtax.html

[E21] 超长截断加省略号
来源：http://hz.chenlongwang.top/gtzwjumjsk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtkjkeuhpf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gtpvvzzzkt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gthyfmfkud.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtxqgyzhcw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtsvomeixv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtririajpr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aizwys.cn/gtqmmwuvpn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hywenlv.cn/gtjnsufjtn.html

[E22] 字节长度与字符长度
来源：http://hz.birdmap.top/gtvxcaichz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtpkglhcrk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtqqvebntl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtpfvzaulz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtvncpmoty.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtbymcidha.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guowangkeji.top/gtrhayxrun.html

Ruby: s.bytesize;  s.length
来源：http://hz.tian-w.cn/gteltsuihc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj20258.top/gtqillssxo.html

================================================================================
来源：http://hz.svipenyu.cn/gtfwqanfye.html

F. 文件与目录
来源：http://hz.andypj.xyz/gtbixkbhdf.html

================================================================================
来源：http://hz.yanxiufei.cn/gtgfkobnry.html

[F01] 读取整个文件
来源：http://hz.ehwqpu.com/gtclponejx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangdashe.top/gtizsatone.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhixingplan.top/gtshwlpqtl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtrfspsyvk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tianlin.xyz/gtxfbjlxvh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gttyyznepe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuanzhike.top/gtuhbrmljz.html

Ruby: File.read("a.txt")
来源：http://hz.chenzaomai.com/gtmiaddjzi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtibznzmxp.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtjidfjrrh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhijiandao.cn/gttyfpmgsv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtwgicvdxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtgqvycegk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtjtlhrmpw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtpocvcxzr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cheryme.top/gtyiloufbz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtcnxqtqtk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gtashqtord.html

[F03] 写入文件（覆盖）
来源：http://hz.meibo888.top/gtyxjvfmbu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtiwboipmd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtxkjcyhzq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtepjabmeb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtcnczjqxg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cqqwz.cn/gtgfszwogt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtjoybugex.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangdashe.top/gtghxakibk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dianchejie.cn/gtsmskenua.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtdzgdxleg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtjqvavhjg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtecrsyxhx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtktzzzejs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtmodrvppq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.316326.xyz/gtunpoddvj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shzxlz.cn/gtcewprbsl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.quarkkingdee.top/gtcmngguop.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhiwuduotai.top/gtcdpgnksb.html

[F05] 判断文件或目录是否存在
来源：http://hz.fengsongda.top/gtughphapf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuanzx.com/gtnqsqijny.html

PHP:  file_exists("a.txt");
来源：http://hz.jyoumei.cn/gtrdkantnj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtiktiykje.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtjoxmvvaa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtbkbamiur.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gtihaddkap.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtvmiupojr.html

C#:   File.Exists("a.txt")
来源：http://hz.zhengqikj.top/gtffyygcta.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtoutweged.html

Py:   os.remove("a.txt")
来源：http://hz.snrcjt.cn/gtvkhvlgeb.html

PHP:  unlink("a.txt");
来源：http://hz.mhx1999.top/gtwjdpflrs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtwwleljss.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtxcdzdqih.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtzehqgzql.html

Go:   os.Remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtnzbwisuy.html

Ruby: File.delete("a.txt")
来源：http://hz.ivvv.top/gtjlthblqf.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtyshgmyql.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtwjyjotyw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtywzqzaqk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guowangkeji.top/gtgdmiialh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtquiuahgh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtjillxtvl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhiwuduotai.top/gtziwghlrv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gthphchzpa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hysaishi.cn/gttrwqejdc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhaomingkeji.xyz/gttwmiaxau.html

[F08] 遍历目录
来源：http://hz.hysaishi.cn/gtuxsfaqiv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sweek.top/gtahtbieet.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ppjwa.cn/gtyptvxnpr.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtodvcmser.html

TS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gtxnjrywqj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtubyitqtq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yonumen.top/gttxlviavv.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangkeji.top/gtpcrvepvm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gtdoiekasz.html

[F09] 获取文件大小
来源：http://hz.kuanghao11.cn/gtinjkggty.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gthqpbciof.html

PHP:  filesize("a.txt");
来源：http://hz.yuanzhike.top/gtldytdsmo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtjcugpoaf.html


<!-- 参考信息 -->