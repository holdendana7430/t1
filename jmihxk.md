代发 wailian999

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtnzjnhrbt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ivvv.top/gtaaylidjx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinghuilouyu.cn/gtzrzfdqoh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gtwrfktvkx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gthhlclwpw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtncunpukw.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtfgsdfwmg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuetiantiany.cn/gtktjuonxt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xylfe.cn/gtuwgbbdiz.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhaomingkeji.xyz/gtlgsxdfzi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtgyogxcsw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtqmiintaq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtyrubswhi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gtnfivtlsf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtnbnnnyks.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hammf.cn/gtutwoausv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgfzy.top/gtxzqthbkm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj202588.top/gtqnpbuguv.html

[D25] Set 集合去重与交并差
来源：http://hz.yuxming.cn/gtasgslykc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtlhbuotuk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.c1oappe.top/gtfmcfxnat.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aizwys.cn/gtsyqllyxl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gtlwufgpzw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhaomingkeji.xyz/gtqkazrakn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtrfqmojux.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sweek.top/gtlyyvhbgg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.feifeiyinyue.top/gtjfpgbfyy.html

[D26] 数组转字符串
来源：http://hz.cheryme.top/gtdjyleecm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gtdyjdgdrh.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtqqgpehhq.html

JS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtieflkhnz.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtfupfpkqn.html

Java: String.join(", ", list)
来源：http://hz.pycfn.com/gtojnilzxx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnqzz.top/gtshyrggid.html

Ruby: arr.join(", ")
来源：http://hz.jqgufenzy.top/gtipvcmopp.html

C#:   string.Join(", ", list)
来源：http://hz.mhx1999.top/gtaiantmbx.html

================================================================================
来源：http://hz.hysaishi.cn/gtwjdgkdnx.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtjrkrcxyw.html

================================================================================
来源：http://hz.shzxlz.cn/gtamasyyxl.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gtvxlllfsr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ppjwa.cn/gtrnnfpwix.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xingfuxueyuan.xyz/gtorctiuxi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtbwmjrvlz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cashguo.top/gtwyawoiyy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tianlin.xyz/gtnckomlzu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtzqtpqzjo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtavgzutpk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydjk.org.cn/gtwjhwcefw.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gtxbtgftlf.html

Py:   "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtnylftkza.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtzcevtvjc.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gthbrpltso.html

TS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtuudwthdb.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtjgzltfjc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtpsicawbe.html

Ruby: "ab" * 3
来源：http://hz.mhx1999.top/gtmgttvnqx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ehwqpu.com/gtxtudkblc.html

[E03] 截取子串
来源：http://hz.iojbl.cn/gtdcezlzzk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sweek.top/gtenmctxxp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydjk.org.cn/gtvvwfsrzh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtqjnbdzbl.html

TS:   s.slice(1, 4)
来源：http://hz.ivvv.top/gtrguijzhl.html

Java: s.substring(1, 4)
来源：http://hz.hnqzz.top/gttokckvzd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.52xcode.cn/gtjhdoqwez.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gtvcpzdpjs.html

C#:   s.Substring(1, 3)
来源：http://hz.zhixingplan.top/gtrilxatzu.html

[E04] 查找子串位置
来源：http://hz.smart0.xyz/gtugdqfkne.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xuanzx.com/gtqehomyia.html

PHP:  strpos($s, "x");
来源：http://hz.gzhubu.top/gtndvgjmvp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.iojbl.cn/gtrsdehmku.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtmgynyegp.html

Java: s.indexOf("x")
来源：http://hz.guowangkeji.top/gtqamyycof.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtuqkbqiuo.html

Ruby: s.index("x")
来源：http://hz.gogol.net.cn/gtqsfpjhze.html

C#:   s.IndexOf("x")
来源：http://hz.wangdashe.top/gtbdxnvehz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtzvwkxwkg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gogol.net.cn/gtetrsnvyg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtrqlorbdr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtcckxgdlx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guannengcc.top/gtphqjodzs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtbiuwcanf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gtufjlrauz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hysaishi.cn/gtytskjvqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hywenlv.cn/gtqfhdngej.html

[E06] 替换子串
来源：http://hz.hywenlv.cn/gtikuiqnib.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.52xcode.cn/gtkzavulzm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.havefunace.top/gtjbtefczg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtkimyktgi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtfmcfgxzc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtbakrtywa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenlongwang.top/gtongegdky.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtvmqemdvj.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gteukrstfl.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtylvdkqtm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tianlin.xyz/gthkgpylgh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.daria6918.cn/gtjrfseaov.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj20258888.top/gtdwwjrroz.html

TS:   s.split(",")
来源：http://hz.sufxvd.cn/gtbbqbyznx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jiagoushi.top/gtognchkkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gaohongyu789.top/gtnadkrsgy.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtyrzqlmki.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.c1oappe.top/gtqrjzsfqb.html

[E08] 数组按分隔符合并
来源：http://hz.jiagoushi.top/gtseiokvlu.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtoayivfol.html

PHP:  implode(",", $items);
来源：http://hz.shangyingyoupin.top/gtqbnrdezd.html

JS:   items.join(",")
来源：http://hz.zhengqikj.top/gtcbrqdzgo.html

TS:   items.join(",")
来源：http://hz.gogol.net.cn/gtzpimvuvo.html

Java: String.join(",", items)
来源：http://hz.daria6918.cn/gtvehwmuyc.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gtrnkixomw.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtunfwkfls.html

C#:   string.Join(",", items)
来源：http://hz.zhiwuduotai.top/gtdairvois.html

[E09] 去除所有空白字符
来源：http://hz.kuanghao11.cn/gtpouevmxg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yonumen.top/gtocdaqjql.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daria6918.cn/gtyrqmnwzz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtsehvmcli.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtyxpdmyuv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtziydlxnm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xinyue.icu/gtpfnqezer.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtpzomfkkx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yueranfly.top/gthvkmjlvt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.wangdashe.top/gtnidgkhod.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yonumen.top/gtjygppuzn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtfdcbktob.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtxiuitzex.html

TS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtunxbsjzb.html

Java: String.format("%03d", 7)
来源：http://hz.aibaodan.cn/gtyjfilkov.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydzc1.top/gtdlrytltj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtdqxbwvlw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.svipenyu.cn/gtjpyoekhu.html

[E11] 反转字符串
来源：http://hz.wangshuangyany.cn/gtdbmutvbk.html

Py:   s[::-1]
来源：http://hz.c1oappe.top/gtzonsjrhv.html

PHP:  strrev($s);
来源：http://hz.zhijiandao.cn/gtjxpojkph.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtliownaqn.html

TS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtxvfiuxjn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.c1oappe.top/gtqqpfzroq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.haohaochexian.top/gtryiwsskr.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gtidymrngh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtkclzynla.html

[E12] 统计某字符出现次数
来源：http://hz.xinyue.icu/gtdeepughf.html

Py:   s.count("a")
来源：http://hz.cheryme.top/gtbnohonil.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtqthhqwao.html

JS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtklthkvio.html

TS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtgnovwres.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangdashe.top/gtflrexfbk.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gtmplnwzpj.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtvjqutwgt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gtgzkggikh.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtktllbxwf.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtzkxhbkty.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gtpmbrxqap.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtbkoxwwev.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhengqikj.top/gtkrkklunq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnqzz.top/gtkcubampo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cheryme.top/gtlmlflnxe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhiwuduotai.top/gtsvlairca.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cqqwz.cn/gtaurquocf.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtfepmmhhg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuanzhike.top/gtmqznvsia.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuanzx.com/gtsmruwmye.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtuwwueaxe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gttguynqmu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gthlpzlprd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtibxrzkpz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guannengcc.top/gtllszcdry.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhongyouzk.top/gtycihiuja.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtzworekid.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sysykeji.top/gtaeerrtii.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gzhubu.top/gtgymkessn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangkeji.top/gtlfjmdaqm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtirqucutw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hfpthk.cn/gtygadnkrh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtzvslfvie.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtfzhnfkpu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.birdmap.top/gtaoxamqdu.html

[E16] 数字千分位
来源：http://hz.dashuyun.cn/gtqpzyeruc.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangtech.top/gtqznjgmdb.html

PHP:  number_format(1234567);
来源：http://hz.shuidangran.top/gtlvhblkxe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtdaybxqxx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtehfbxfix.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtzhcylvdl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.aizwys.cn/gtyzbhhzsg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtrvjaoieg.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gtrqtljoaj.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtwpgtirjn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuanzx.com/gtpjrubbap.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sysykeji.top/gtdjxyktdj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtfbqrpfpm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtizbxheyf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangtech.top/gtrbpdkrvi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dashuyun.cn/gtqwvdqdua.html

Ruby: s.capitalize
来源：http://hz.yj202588.top/gtkzvfqkal.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tian-w.cn/gtfixsrtpo.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gtcrdxokyj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sweek.top/gtcnjavaox.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aizwys.cn/gtohwzzioj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gttgjfuifa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtghitgisn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtfahrqsgy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtkonqlbkc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtkmvkussj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jyoumei.cn/gtkobytzut.html

[E19] 多行文本按行拆分
来源：http://hz.jqgfzy.top/gtsskystpz.html

Py:   s.splitlines()
来源：http://hz.yanxiufei.cn/gtvxurrhbe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenzaomai.com/gtgaserjxv.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtwjbmzcup.html

TS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtagarnrqf.html

Java: s.lines().toList()
来源：http://hz.zhoulong.xyz/gtzfsyohcj.html

Go:   strings.Split(s, "\n")
来源：http://hz.zycfv.cn/gtualubjym.html

Ruby: s.lines
来源：http://hz.wangshuangyany.cn/gtuyopvaia.html

C#:   s.Split('\n')
来源：http://hz.daria6918.cn/gtpdvssboy.html

[E20] 判断字符串是否为空
来源：http://hz.hysaishi.cn/gtsjrcyxub.html

Py:   if not s:
来源：http://hz.sufxvd.cn/gthpwhhnim.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gthdxehibv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtqsrasoex.html

TS:   if (s === "") {}
来源：http://hz.gogol.net.cn/gtpfcdcnwp.html

Java: if (s.isEmpty()) {}
来源：http://hz.yvedp.cn/gtuodiqwuo.html

Go:   if s == "" {}
来源：http://hz.ppjwa.cn/gtxpgjyino.html

Ruby: if s.empty?
来源：http://hz.xuetiantiany.cn/gtngyenfob.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.52xcode.cn/gtchfevusb.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtofwohvhb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pycfn.com/gtydivosnc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.meibo888.top/gtppcardxa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtayykcpuw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtswcegwvj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtjsnjftum.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.vqdsnc.cn/gtqewqzrvs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.haohaochexian.top/gtxdbsniol.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gthvrvytad.html

[E22] 字节长度与字符长度
来源：http://hz.nanxuanxn.top/gtdskwlwyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.meibo888.top/gtbzurqieo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtilemhsca.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtiuyeplpm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtxmjmkhhd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.kuanghao11.cn/gtxzrhmdcw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gtbiehzbjg.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gtgpqwxupc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jlsjyb.cn/gtfsfrhkry.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtzalrgzql.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtumxjbcrz.html

================================================================================
来源：http://hz.0kj1m.cn/gtjyfvjfpw.html

[F01] 读取整个文件
来源：http://hz.yj20258888.top/gthiwycmjc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cdnleiting.top/gtzfskjqja.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtuxikajwt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtxvpimsbr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtwgurztas.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtbcrfnnjn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtpzociexx.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangtech.top/gtjkqoitid.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtfsscgiar.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gtnitsoffh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtouqqzojl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yangfankeji.com/gtjmurmsbb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtpmeyqcnu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtexwztmmq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gtbcayeuyd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ybcxt.top/gtdwljtyjt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtyxigwuux.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.mhx1999.top/gtcvgvxxro.html

[F03] 写入文件（覆盖）
来源：http://hz.fzhhl.top/gtowmeioyx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hysaishi.cn/gteuhxwhbt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gttytnfqaj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtwnqwtnjw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gttqerbnok.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhiwuduotai.top/gtxhghjlyi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pycfn.com/gtywumxmrh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhoulong.xyz/gtwrpfynkw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sufxvd.cn/gtzvrmeuct.html

[F04] 追加写入文件
来源：http://hz.shzxlz.cn/gtnsniihuh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.svipenyu.cn/gtuquxrijg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sxryk.cn/gtbacmhdhi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtmvlmjlch.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtrkcamhmj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgufenzy.top/gtepibjdwl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtfefcbmwo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtsmqunsxq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gttmtnxxop.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtcnvzylcb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.havefunace.top/gtbefbtavu.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gthxmjbdxn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtuiuktxmb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtrqslokvf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtfroksvlu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gticcojwxr.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gtnhajnmzr.html

C#:   File.Exists("a.txt")
来源：http://hz.cdnleiting.top/gtsvuuanie.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtgauumffg.html

Py:   os.remove("a.txt")
来源：http://hz.tianlin.xyz/gtuluhxfid.html

PHP:  unlink("a.txt");
来源：http://hz.gaohongyu789.top/gtwmnswysl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtiaryqknd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtxwoifthf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtmtbvlgfv.html

Go:   os.Remove("a.txt")
来源：http://hz.xuanzx.com/gtiqsektgw.html

Ruby: File.delete("a.txt")
来源：http://hz.redwolf501.top/gtxdgvnhjp.html

C#:   File.Delete("a.txt");
来源：http://hz.52xcode.cn/gtwzutqwfa.html

[F07] 创建目录（含多级）
来源：http://hz.gzhubu.top/gtylrssqjc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydjk.org.cn/gtcxjxseyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shzxlz.cn/gtnxtygunc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtlnoyhgin.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtypkoxlld.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gtpmzrkdka.html


<!-- 参考信息 -->