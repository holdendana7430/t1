代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtpixvccse.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pycfn.com/gtegdaaasw.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtsuaxquqo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtzexafxqg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinghuilouyu.cn/gtyugaqmpe.html

[D24] 字典 / Map 基本操作
来源：http://hz.shanyushiyangkeji.top/gtfxmrdfkc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shangyingyoupin.top/gtcrnrfmyn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.9152youxi.cn/gtdvvtjrlp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daxiang520.top/gtkhskjrdf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gzhubu.top/gtbhgbmxeo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnxiangtu.top/gtqumukhcf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhaomingkeji.xyz/gtyabghrjl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtjfvkdozo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.haohaochexian.top/gtzoptdgqn.html

[D25] Set 集合去重与交并差
来源：http://hz.zhoulong.xyz/gtseipqxbs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gtrwdhkcvz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydzc1.top/gtzwtmpsjf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtoticpvcy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nwbrower.top/gtpcetztsw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtoqutniim.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yueranfly.top/gtguvweovz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cashguo.top/gtclxflvxo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tian-w.cn/gthnjffvxc.html

[D26] 数组转字符串
来源：http://hz.zhaomingkeji.xyz/gtbbnqwtgx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gtynaphbnp.html

PHP:  implode(", ", $arr);
来源：http://hz.yuanzhike.top/gtwduarcyh.html

JS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtoypgkqmv.html

TS:   arr.join(", ")
来源：http://hz.aizwys.cn/gtrablkmmw.html

Java: String.join(", ", list)
来源：http://hz.cheryme.top/gtbwbcbeiy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shuidangran.top/gtbdhlxyan.html

Ruby: arr.join(", ")
来源：http://hz.yueranfly.top/gtwqvhjfkd.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtwanguueh.html

================================================================================
来源：http://hz.bjfxy.top/gtbiqrdpup.html

E. 字符串处理
来源：http://hz.yonumen.top/gtjkriacnq.html

================================================================================
来源：http://hz.tanke756.top/gtbrolkgyf.html

[E01] 拼接字符串
来源：http://hz.c1oappe.top/gtkelywwbp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj202588.top/gtmcprsloh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtgigccztx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gtqxieaccy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtcjvomrkd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.iojbl.cn/gtcmddfslx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sysykeji.top/gtvuqbvufj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenzaomai.com/gtaoxfwrog.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtyetdspwz.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtqhpubuzu.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gtctkhzlgz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jqgfzy.top/gtmfmoaisb.html

JS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtgnjwlmtm.html

TS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gteaqbtjmv.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtdhxjbdmb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gtwuutynas.html

Ruby: "ab" * 3
来源：http://hz.dianchejie.cn/gtambguqva.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtkcwxqvqg.html

[E03] 截取子串
来源：http://hz.guowangkeji.top/gtjsnmgwzd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pycfn.com/gtjypwdbxu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xingfuxueyuan.xyz/gtxldgrgbx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tian-w.cn/gtigwnhttg.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtnbgchiqa.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gtimbprjxo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guannengcc.top/gtoplookle.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgufenzy.top/gtwzqmqjvk.html

C#:   s.Substring(1, 3)
来源：http://hz.xuanzx.com/gtnweilqbv.html

[E04] 查找子串位置
来源：http://hz.gogol.net.cn/gtjrmlixuq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zdqjudy.top/gtvseuxxel.html

PHP:  strpos($s, "x");
来源：http://hz.9152youxi.cn/gtklllpysb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yongpay.top/gtxnwvctee.html

TS:   s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtstkkjjef.html

Java: s.indexOf("x")
来源：http://hz.nwbrower.top/gtdmcttzak.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gthpsbwexx.html

Ruby: s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gthoucywai.html

C#:   s.IndexOf("x")
来源：http://hz.gzhubu.top/gtzhetqzuk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xinyue.icu/gttwdrwrfv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhongyouzk.top/gtmfrocaeb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangshuangyany.cn/gtxdcheyzu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydjk.org.cn/gtbozhgpgd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pengpengdd.cyou/gtigqktqgo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtpsdqaaqf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nwbrower.top/gtjvjltpvl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shzxlz.cn/gtkpzxvzhl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtnrwfpoeo.html

[E06] 替换子串
来源：http://hz.yuxming.cn/gtetoyilhr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxuanxn.top/gtjsalfirh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.wangdashe.top/gtgddbyuun.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtkxcqanuz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtrxjbjalp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gttsygsxxs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtnezeuhor.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gtllxlblrd.html

C#:   s.Replace("a", "b")
来源：http://hz.haohaochexian.top/gtbfctcjzm.html

[E07] 按分隔符拆分
来源：http://hz.gogol.net.cn/gtdqlccwsk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.aizwys.cn/gtiqlkcovf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.havefunace.top/gtjpbeacwm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tian-w.cn/gtxtkcbidu.html

TS:   s.split(",")
来源：http://hz.52xcode.cn/gtgqheazpx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fzhhl.top/gtscywumfi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydzc1.top/gtneewrjyp.html

Ruby: s.split(",");  s.split
来源：http://hz.smart0.xyz/gtsrvvsybf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.redwolf501.top/gttxtbhwro.html

[E08] 数组按分隔符合并
来源：http://hz.fzhhl.top/gtzxhjzcpe.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtlcncrsal.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtevlikvoh.html

JS:   items.join(",")
来源：http://hz.tianlin.xyz/gtfsimksaf.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtucyxbmgw.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gtnfokbulr.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtfftjsthj.html

Ruby: items.join(",")
来源：http://hz.smart0.xyz/gtbezfenrr.html

C#:   string.Join(",", items)
来源：http://hz.nanxinkj.top/gtxmfoffyi.html

[E09] 去除所有空白字符
来源：http://hz.andypj.xyz/gtzikptrbe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtombzrwlg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xinyue.icu/gtyoaaefvl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtgqpwneis.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtskoiaslq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yongpay.top/gttsayztqy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenjidiqi.icu/gtcwsaqqwq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aibaodan.cn/gtaihvehzl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.snrcjt.cn/gtlhxoekut.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jlsjyb.cn/gtdnhuqgsh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinghuilouyu.cn/gtedfankyy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenzaomai.com/gtwacjlovv.html

JS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtgpvorloj.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtnwgkdknd.html

Java: String.format("%03d", 7)
来源：http://hz.chenlongwang.top/gtfdsmzknv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guannengcc.top/gtpxtcuyuz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gtfegtvyfw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtptscjdxo.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtsfocuopl.html

Py:   s[::-1]
来源：http://hz.hysaishi.cn/gtuivwphja.html

PHP:  strrev($s);
来源：http://hz.jinghuilouyu.cn/gtypcruwgo.html

JS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtluidasoi.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtodvopekh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shzxlz.cn/gtpmwcuckr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guowangkeji.top/gtscffuhie.html

Ruby: s.reverse
来源：http://hz.hongshengwenyu.top/gtifttyyks.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtgrlwegso.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtqedjullw.html

Py:   s.count("a")
来源：http://hz.yongpay.top/gtyvnjspbv.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gtxexczueh.html

JS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtiiknegax.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtjwahvpiv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.fengsongda.top/gtecjllyrg.html

Go:   strings.Count(s, "a")
来源：http://hz.yongpay.top/gtfrgulyai.html

Ruby: s.count("a")
来源：http://hz.yangfankeji.com/gtijajfvxx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenjidiqi.icu/gtdkitgqmf.html

[E13] 逐字符遍历
来源：http://hz.ybcxt.top/gtlkupvdko.html

Py:   for ch in s: print(ch)
来源：http://hz.ydjk.org.cn/gtxctumded.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.meibo888.top/gtsnavaqrk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtghmsqlsk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtireermfc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sufxvd.cn/gtddlzxnuf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtvkxfoexw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxinkj.top/gtktsiigzr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shzxlz.cn/gtcqhicwkt.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gttwzktjzo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sweek.top/gtwwbuydhr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gaohongyu789.top/gtsqpyuhzf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtucnjktgf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtgrkoucrq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtnpbuiirm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtsyqoaeez.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yuxming.cn/gtrxchjgtq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pycfn.com/gtoyowsxvk.html

[E15] HTML 转义 / 反转义
来源：http://hz.andypj.xyz/gtbjfyfkvf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ehwqpu.com/gtkvrtabou.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gthjuptpbs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gtuiktsjym.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tianlin.xyz/gtmhfnyzkn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sysykeji.top/gttmqdbcqc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtqceiokmc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtmvnrlfmy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.52xcode.cn/gtgbpmqdgz.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtobnmcugj.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtungnblox.html

PHP:  number_format(1234567);
来源：http://hz.hnxiangtu.top/gturkhwpws.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtosbtulhr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtokxctimg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangkeji.top/gtatmbcamb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtwfmhddtw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cucudq.cn/gthzpasjbw.html

C#:   1234567.ToString("N0")
来源：http://hz.ydjk.org.cn/gtzekpxuim.html

[E17] 首字母大写
来源：http://hz.shangyingyoupin.top/gtzsvubxry.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shzxlz.cn/gtmdyyunmf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.vqdsnc.cn/gtavcivtoh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtzbtcaofh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtzsaserht.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.smart0.xyz/gtshjzalpl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnxiangtu.top/gtnwicgzww.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtuxggfmib.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhixingplan.top/gtnwfpxeii.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtyjlrrarw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhaomingkeji.xyz/gtlpefgbwm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zdqjudy.top/gtfubuqtxs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtglbhatvo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.daxiang520.top/gtvshkrfzn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gzhubu.top/gtjiifllwp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yvedp.cn/gtjvsqgkfn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgfzy.top/gtsoujluzb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yangfankeji.com/gtgketfvyy.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtstabmisf.html

Py:   s.splitlines()
来源：http://hz.fengsongda.top/gtvhpedgsh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgufenzy.top/gtasbvoine.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gthftvjucu.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gthsnanhyt.html

Java: s.lines().toList()
来源：http://hz.meibo888.top/gteisbzhdi.html

Go:   strings.Split(s, "\n")
来源：http://hz.dashuyun.cn/gtsoatjvap.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtiltfpdym.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtrgfxesyv.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtlmcmedse.html

Py:   if not s:
来源：http://hz.meibo888.top/gtorsdhcvn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhaomingkeji.xyz/gtmkcxzopi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtrnxowrqy.html

TS:   if (s === "") {}
来源：http://hz.cdnleiting.top/gtsfhmczpo.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtxwhbablj.html

Go:   if s == "" {}
来源：http://hz.yuanzhike.top/gtzancxjls.html

Ruby: if s.empty?
来源：http://hz.zhongyouzk.top/gtrsgsodsa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.meibo888.top/gtdtfotyax.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gtqldldsfv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.redwolf501.top/gtcuzpoiaf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.redwolf501.top/gtafzlajqy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtbryersjq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtacmdrukt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtrnshozay.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.feifeiyinyue.top/gthzkmdbbr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtxawxlgqg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.316326.xyz/gtkepuklrc.html

[E22] 字节长度与字符长度
来源：http://hz.feifeiyinyue.top/gtgibqnipf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtiafaecdb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtpswvbchn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gttmnrfrmu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gtrkofrnml.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gthspswcan.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.bjfxy.top/gtqjrbehrs.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhiwuduotai.top/gtbwnarpor.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gteowsoibv.html

================================================================================
来源：http://hz.52xcode.cn/gttpdtgmve.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtihoqpzaj.html

================================================================================
来源：http://hz.yj202588.top/gtfrqtdocl.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtxrdpsuwl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.0kj1m.cn/gtovfurcfr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhixingplan.top/gtqlhqcwlf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gtzbcyljks.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gtaotwgjup.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtmbrcbneb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sweek.top/gtpydxpomh.html

Ruby: File.read("a.txt")
来源：http://hz.gzhubu.top/gtemxrnjre.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sysykeji.top/gtmhmvigqg.html

[F02] 逐行读取文件
来源：http://hz.nanxuanxn.top/gtltvleicj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtjwkxhrvx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangtech.top/gtigmpqilh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gttwodddiv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtwdlqrliv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sweek.top/gtbzdfdyxe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hammf.cn/gtgdoivclp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenjidiqi.icu/gtiqpdqhez.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgufenzy.top/gtlcqmqbnf.html

[F03] 写入文件（覆盖）
来源：http://hz.iojbl.cn/gtzqkdrnvr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guowangkeji.top/gtznwqlssh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xziqi.cn/gtxjnvnxmy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gtifppijug.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtgzbtbbux.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxuanxn.top/gtjkogaokv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.havefunace.top/gtbtkpxdgd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tanke756.top/gtgrhwjvgk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtzkyjoqmc.html

[F04] 追加写入文件
来源：http://hz.zdqjudy.top/gtagsbembm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtjbyaqoew.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtseavsivf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtjyxhzkrs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtckcknfhn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtjivthprw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gtjdjshgcg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtvthaujme.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtqcbujqql.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gtkjnnnjwe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtaguajqde.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gtkvcrpgnh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtkmojodgm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtoaghbugx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtlsmnbotr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtzrxchlyb.html

Ruby: File.exist?("a.txt")
来源：http://hz.nwbrower.top/gtmlrjupys.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gtwujiffuk.html

[F06] 删除文件
来源：http://hz.ywan-chungtsiang.top/gtpxvroikh.html

Py:   os.remove("a.txt")
来源：http://hz.zhoulong.xyz/gtfkgdjlcz.html

PHP:  unlink("a.txt");
来源：http://hz.nwbrower.top/gtjlviwkqd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gthkprumof.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtbfxofvtk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtfdrsbxql.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtbhldtbcz.html

Ruby: File.delete("a.txt")
来源：http://hz.kuanghao11.cn/gtuzfhatvi.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtkqtjvcwb.html

[F07] 创建目录（含多级）
来源：http://hz.gzhubu.top/gtzapsofxx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cdnleiting.top/gtznwwcysq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yueranfly.top/gttmdpujnv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtioksnfxz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.316326.xyz/gtbgtnmund.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtguxhawxg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gtxjltxhyg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guannengcc.top/gtexvcpied.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gtvuepcyba.html

[F08] 遍历目录
来源：http://hz.yuxming.cn/gtdxmbvbqv.html


<!-- 参考信息 -->