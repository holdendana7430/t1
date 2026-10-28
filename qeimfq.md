代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuanzx.com/gtfiwxingb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.vqdsnc.cn/gtokqvljsr.html

[D25] Set 集合去重与交并差
来源：http://hz.cheryme.top/gtrmfgdmfn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.quarkkingdee.top/gtnunkxygz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtvyaetxlu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xinyue.icu/gtjdvwinze.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xinyue.icu/gtimzcuqqp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtbfjoodgs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gtfnugleig.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtbfapqttd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangkeji.top/gtxyjnxgox.html

[D26] 数组转字符串
来源：http://hz.xinyue.icu/gtarcclatn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtabsqvdwc.html

PHP:  implode(", ", $arr);
来源：http://hz.0kj1m.cn/gtoooejsfh.html

JS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gthyfmfjsz.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtazynnqek.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gtrnxjvlkd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtruzhxixr.html

Ruby: arr.join(", ")
来源：http://hz.zhongyouzk.top/gtftlfcxqx.html

C#:   string.Join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtznvofpcb.html

================================================================================
来源：http://hz.fengsongda.top/gtoyarzcir.html

E. 字符串处理
来源：http://hz.hnxiangtu.top/gtqadorbko.html

================================================================================
来源：http://hz.cucudq.cn/gtuynjsxvv.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtppzkbhjb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.birdmap.top/gtgjamkxso.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gaohongyu789.top/gtbgyqfhwe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtraffshsh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.redwolf501.top/gtdbxocgju.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuxming.cn/gtzpqjxusz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.mhx1999.top/gtyhzdvgcr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhixingplan.top/gteqhjsfsk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.52xcode.cn/gtjqwhszvz.html

[E02] 重复字符串
来源：http://hz.guowangkeji.top/gtkltxaxwi.html

Py:   "ab" * 3
来源：http://hz.9152youxi.cn/gtlkaksbua.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtvrqbtbjk.html

JS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtnadakqdc.html

TS:   "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtyhhfhbkj.html

Java: "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtnionqhru.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.haohaochexian.top/gtgqgejqng.html

Ruby: "ab" * 3
来源：http://hz.9152youxi.cn/gtmfpjlvrj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.quarkkingdee.top/gtlmzneske.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtzcducmhx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtbpnmxrje.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtjcrisvjq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtwsixcpvm.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtfcumiodo.html

Java: s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtirspqcdx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.pengpengdd.cyou/gtedtmgmzq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.haohaochexian.top/gtcwnnltji.html

C#:   s.Substring(1, 3)
来源：http://hz.jinghuilouyu.cn/gtxssnvter.html

[E04] 查找子串位置
来源：http://hz.quarkkingdee.top/gtfafhxdbm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuanzhike.top/gtjijvgsls.html

PHP:  strpos($s, "x");
来源：http://hz.pengpengdd.cyou/gtnxhrdqhw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yangfankeji.com/gtghofvjky.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtdyghbasg.html

Java: s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtpqvdqrgm.html

Go:   strings.Index(s, "x")
来源：http://hz.ehwqpu.com/gtvfakfyoz.html

Ruby: s.index("x")
来源：http://hz.iojbl.cn/gtvaulyibc.html

C#:   s.IndexOf("x")
来源：http://hz.yj20258.top/gtessiqnuj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtbjvvvftg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.kuanghao11.cn/gtefehzape.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sxryk.cn/gtpzewuwuw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtvmswgtnv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.316326.xyz/gtkvuxjrtz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtobqjsatd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gttkkdknbd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aizwys.cn/gtyjbcvapa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtkqxawngf.html

[E06] 替换子串
来源：http://hz.havefunace.top/gtnajpiedg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cdnleiting.top/gtmrhzcxgt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pycfn.com/gtxfqacyhi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtfibfbgxm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtctlafjjj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtpskpxlru.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fengsongda.top/gtyjwkntru.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gotoacloud.top/gtiykpvchp.html

C#:   s.Replace("a", "b")
来源：http://hz.chenzaomai.com/gtdionaehe.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtonedofzl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hfpthk.cn/gtwgdnnnef.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgfzy.top/gtmktcbxnl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gtljujgwwc.html

TS:   s.split(",")
来源：http://hz.sysykeji.top/gtteyueobb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgfzy.top/gthioaksmk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.dianchejie.cn/gtkiyuwexp.html

Ruby: s.split(",");  s.split
来源：http://hz.jinyuanbaomall.cn/gtoghoudrf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.smart0.xyz/gtwjexoltj.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtrvwpblzz.html

Py:   ",".join(items)
来源：http://hz.zhengqikj.top/gtthwpzflj.html

PHP:  implode(",", $items);
来源：http://hz.haohaochexian.top/gtwauamngk.html

JS:   items.join(",")
来源：http://hz.0kj1m.cn/gtmztqdjfk.html

TS:   items.join(",")
来源：http://hz.ybcxt.top/gtqvupepdr.html

Java: String.join(",", items)
来源：http://hz.birdmap.top/gtqkphggka.html

Go:   strings.Join(items, ",")
来源：http://hz.yanxiufei.cn/gtezxuwkso.html

Ruby: items.join(",")
来源：http://hz.nanxuanxn.top/gtpbytsitd.html

C#:   string.Join(",", items)
来源：http://hz.pycfn.com/gtjiyyqanh.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gtieopktpw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gtmuueyupb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258.top/gtnwukbiae.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtxaurjesq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtsurrnsem.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aibaodan.cn/gtghdlhkit.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hfpthk.cn/gtfmhauqbl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gthoucgbuj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guannengcc.top/gttwrcfzko.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gogol.net.cn/gtdqeawmxs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shzxlz.cn/gtegmhcjdk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jqgufenzy.top/gtfywvsohp.html

JS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtlfqqnaui.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gttokjkyij.html

Java: String.format("%03d", 7)
来源：http://hz.dashuyun.cn/gtddxuxwkv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtlxsxkkjq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.mhx1999.top/gtyicqxhhz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.birdmap.top/gtmhvfxvbh.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtkfzordip.html

Py:   s[::-1]
来源：http://hz.daria6918.cn/gtpzjsgjkl.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gttiiuwvpn.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtcuoagwey.html

TS:   [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtyyqkpcmy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangshuangyany.cn/gtxirrukcq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jyoumei.cn/gtvbkaqxew.html

Ruby: s.reverse
来源：http://hz.tianlin.xyz/gtpsntdhzx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtxwygirdb.html

[E12] 统计某字符出现次数
来源：http://hz.jlsjyb.cn/gtyphodhcf.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtpkdfzlcw.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gthklzxcne.html

JS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gtkxlrgslx.html

TS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtdccaqfgs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtprzndyms.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gthxbncqps.html

Ruby: s.count("a")
来源：http://hz.ybcxt.top/gtfotjsufv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gtlczrdhjg.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtnnufcrte.html

Py:   for ch in s: print(ch)
来源：http://hz.yueranfly.top/gtkwwinmgq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shangyingyoupin.top/gtbeslpbme.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yongpay.top/gtwpzraqdh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.andypj.xyz/gtxngrlzgv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydzc1.top/gtcogindzm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigufen.top/gtylguggfw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtnfibxlif.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zycfv.cn/gtuxbpwjat.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtofsjfwdg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gtsxyffxwc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.snrcjt.cn/gtuiteagfi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sweek.top/gtwcqqcnjb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jyoumei.cn/gtxkmyelaq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtmqgozwxm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.havefunace.top/gthxdknahr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jqgfzy.top/gtffvnuqnx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.birdmap.top/gtymclaggx.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtarbtjwzf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shangyingyoupin.top/gtsjkbxszx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sweek.top/gtnbupimtm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gtwprthapg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gtvgbolnuv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnxiangtu.top/gtitdrdqlw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hywenlv.cn/gtsfagiuxv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxinkj.top/gthivrppoo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hfpthk.cn/gtlzgdrivx.html

[E16] 数字千分位
来源：http://hz.nwbrower.top/gtxrpjygjj.html

Py:   f"{1234567:,}"
来源：http://hz.andypj.xyz/gtxwpstfko.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtknnsychm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gthubhtaco.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gthmgzyfkh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangshuangyany.cn/gtfcpnprkg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cucudq.cn/gtfrzmcecm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtumlbocht.html

C#:   1234567.ToString("N0")
来源：http://hz.guannengcc.top/gtuaqpwbak.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtyiclezvx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.quarkkingdee.top/gtbcvsilbc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.kuanghao11.cn/gttmxnjbvb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtlyybqkys.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtioojtrgh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hnqzz.top/gtoydapwrt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtzhztxjil.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gtfkroorgz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.havefunace.top/gthiycwdrl.html

[E18] 模板占位符替换
来源：http://hz.jinghuilouyu.cn/gtsuoozzuk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.meibo888.top/gtpihojzqe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.c1oappe.top/gtbioldqtt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtazbyrpwp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigfzy.top/gtmovekorf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zdqjudy.top/gtdogagnyg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cashguo.top/gtivduirhx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ivvv.top/gtlurhgaxi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtrmhhxcty.html

[E19] 多行文本按行拆分
来源：http://hz.fengsongda.top/gtufmvrcxe.html

Py:   s.splitlines()
来源：http://hz.jqgfzy.top/gtcfuqblqh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtaguahhqg.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtraeeeqdg.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtctfedsnz.html

Java: s.lines().toList()
来源：http://hz.iojbl.cn/gteswyetgh.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258888.top/gtjdfmigvc.html

Ruby: s.lines
来源：http://hz.jqgufenzy.top/gtsuzmbhif.html

C#:   s.Split('\n')
来源：http://hz.gzhubu.top/gtpovdcerz.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gtxnwsgvyv.html

Py:   if not s:
来源：http://hz.pengpengdd.cyou/gtrbytgrgj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtidgftkoi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daria6918.cn/gtefyyqegq.html

TS:   if (s === "") {}
来源：http://hz.yueranfly.top/gtupbdlown.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtcupxeyqv.html

Go:   if s == "" {}
来源：http://hz.ppjwa.cn/gtubqhzpoy.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtajazrjjz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigufen.top/gtyeyqfelv.html

[E21] 超长截断加省略号
来源：http://hz.chenjidiqi.icu/gtiskqxfww.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cqqwz.cn/gtgnbryhar.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jianghu66.top/gtyioeqqnn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtznrztbqs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.birdmap.top/gtvyzdccdf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtdaqvggpm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtifjfjmow.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gtacufdzzu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtqmbzsxkx.html

[E22] 字节长度与字符长度
来源：http://hz.zhoulong.xyz/gtsahksbov.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangshuangyany.cn/gtnttdtess.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gttortzuhk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtncizdfnx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtnvcphkiq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.haohaochexian.top/gtyjhivpjq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtjwwkezsp.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhixingplan.top/gtxyjimdhf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtsvucowui.html

================================================================================
来源：http://hz.zhixingplan.top/gtuigzsxio.html

F. 文件与目录
来源：http://hz.yvedp.cn/gtekrbigkd.html

================================================================================
来源：http://hz.tianlin.xyz/gtktoxvgje.html

[F01] 读取整个文件
来源：http://hz.9152youxi.cn/gtsqnecdyr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtahkczpog.html

PHP:  file_get_contents("a.txt");
来源：http://hz.c1oappe.top/gtumdetccm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhaomingkeji.xyz/gtyphxkujj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtnghkrdsy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtcnbbnfvb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.0kj1m.cn/gtpyeiqfyp.html

Ruby: File.read("a.txt")
来源：http://hz.yonumen.top/gtustlymxu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aizwys.cn/gtwjzytoya.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtqibwfyfx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtvwxvxgkv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.bjfxy.top/gtvupauzut.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtjsvzalyb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtuepgtlrp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtpbjdsbyu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtwtdirvjh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gttpeotxdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xylfe.cn/gtflolyqix.html

[F03] 写入文件（覆盖）
来源：http://hz.snrcjt.cn/gtcsumubtc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258888.top/gtwmvvphtv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tanke756.top/gtuszmzvms.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtsxzycfht.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gttkzzuist.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gtfgmjhdvd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtsmxjjvqp.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yonumen.top/gtlmzwttze.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guannengcc.top/gtilfhogcn.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtzkbonirm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.mhx1999.top/gtpkiirozl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258888.top/gtqnhqsusy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gteuapopht.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtmngmkvur.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guannengcc.top/gttwufdmgd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jianghu66.top/gtnewcqxnl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shzxlz.cn/gtresyfpdq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtzqunpkjd.html

[F05] 判断文件或目录是否存在
来源：http://hz.fengsongda.top/gtvkdjpfhn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gtnouffljm.html

PHP:  file_exists("a.txt");
来源：http://hz.sweek.top/gtsipgzwfc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtbxdkvsog.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtemgparrz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtdgmmntfl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pycfn.com/gtrdlmjgfc.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtrvwkxpaw.html

C#:   File.Exists("a.txt")
来源：http://hz.c1oappe.top/gtnswdwnis.html

[F06] 删除文件
来源：http://hz.tanke756.top/gtoskqmkjf.html

Py:   os.remove("a.txt")
来源：http://hz.chenlongwang.top/gtepzmloun.html

PHP:  unlink("a.txt");
来源：http://hz.gotoacloud.top/gtyqlfsyjy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtwbxemftg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtrjeoysts.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtyqnycprl.html

Go:   os.Remove("a.txt")
来源：http://hz.cheryme.top/gtxxdiwyhi.html

Ruby: File.delete("a.txt")
来源：http://hz.tanke756.top/gtrtzjehqk.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtjaqlxoyi.html

[F07] 创建目录（含多级）
来源：http://hz.zhengqikj.top/gtkndrxvba.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtzqtyfxdv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gtiuottobb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtinaueazb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gteqpsffeg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hammf.cn/gttuvutqww.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtivxiaknt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigufen.top/gtzrgtxrye.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinyuanbaomall.cn/gtojfgbhdj.html

[F08] 遍历目录
来源：http://hz.haohaochexian.top/gtlpzuwqts.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.52xcode.cn/gtnlltxfkm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yueranfly.top/gtgxxpcuvr.html

JS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtcdofllcx.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtufhfkezp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gthksalteq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.svipenyu.cn/gtegfbzwrq.html

Ruby: Dir.children("dir")
来源：http://hz.cdnleiting.top/gtcmjugqul.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daria6918.cn/gtsgmtsywl.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtrxtxfgvt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.52xcode.cn/gtjdiwlwdc.html

PHP:  filesize("a.txt");
来源：http://hz.zdqjudy.top/gtwwqyexek.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtrsfrcoml.html


<!-- 参考信息 -->