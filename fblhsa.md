代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtkefywyht.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangshuangyany.cn/gtwwfukwlf.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtjkvecurd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258888.top/gtmuldkkpk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.haohaochexian.top/gtyajjppsp.html

[D24] 字典 / Map 基本操作
来源：http://hz.yanxiufei.cn/gtanppezir.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtuesefome.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgufenzy.top/gtmyzgdsyv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtzvpskywl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenjidiqi.icu/gtcfbaxbal.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zdqjudy.top/gtjwaybzpz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tian-w.cn/gtnjqhdajg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangtech.top/gttmiqeqpe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.vqdsnc.cn/gtcgivzcag.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gtpswqyjlr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guowangkeji.top/gtzuqnczuy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gogol.net.cn/gthnelkqxl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtymdduufu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ivvv.top/gtzkxhnzen.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj20258888.top/gtlxdipgsj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tanke756.top/gtqcddrqko.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dashuyun.cn/gtqiybzprg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinghuilouyu.cn/gtxsnkpizu.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gtwslxhhma.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yangfankeji.com/gtwlrfgezf.html

PHP:  implode(", ", $arr);
来源：http://hz.xylfe.cn/gtkwwmdrki.html

JS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtlexfvrse.html

TS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtocobwypo.html

Java: String.join(", ", list)
来源：http://hz.hfpthk.cn/gtiunhghsu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.52xcode.cn/gtwjzztynt.html

Ruby: arr.join(", ")
来源：http://hz.mhx1999.top/gtlvthihcp.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtilowsikn.html

================================================================================
来源：http://hz.aibaodan.cn/gtlrdleqge.html

E. 字符串处理
来源：http://hz.hfpthk.cn/gterwgpzjl.html

================================================================================
来源：http://hz.sxryk.cn/gtjwkojycy.html

[E01] 拼接字符串
来源：http://hz.nanxuanxn.top/gtxrqkwpuj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hongshengwenyu.top/gtafmfcsoc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ywan-chungtsiang.top/gtdzczenvf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtzdlhtccq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gtzwopyrpq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.0kj1m.cn/gtqgoozrhk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xingfuxueyuan.xyz/gtrhuootma.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pengpengdd.cyou/gtjprnnmpb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangdashe.top/gtbcihjwjx.html

[E02] 重复字符串
来源：http://hz.daxiang520.top/gtveowfglp.html

Py:   "ab" * 3
来源：http://hz.jinqigufen.top/gtfxtwiuqf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnqzz.top/gtpcymijzl.html

JS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtantnpfbe.html

TS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtgagntveo.html

Java: "ab".repeat(3)
来源：http://hz.xuanzx.com/gtsjbctwqf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cucudq.cn/gtlumlhxrp.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtvxqifwcn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zycfv.cn/gtdzurgveq.html

[E03] 截取子串
来源：http://hz.yj20258.top/gtyvxubscs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pengpengdd.cyou/gtrlnpuslt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aizwys.cn/gttfkdcxgw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtjffauwio.html

TS:   s.slice(1, 4)
来源：http://hz.jqgufenzy.top/gtjyjcpqpi.html

Java: s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtjeabuczo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shangyingyoupin.top/gtuugqljri.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.vqdsnc.cn/gttlnazwgn.html

C#:   s.Substring(1, 3)
来源：http://hz.jinghuilouyu.cn/gtnqowugfu.html

[E04] 查找子串位置
来源：http://hz.yj202588.top/gtmxskpldw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.feifeiyinyue.top/gtlcjgchaq.html

PHP:  strpos($s, "x");
来源：http://hz.ppjwa.cn/gttcxbkwty.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtnjojmsza.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtypxetxlh.html

Java: s.indexOf("x")
来源：http://hz.9152youxi.cn/gtaolcqnxb.html

Go:   strings.Index(s, "x")
来源：http://hz.xziqi.cn/gtdsnopytp.html

Ruby: s.index("x")
来源：http://hz.chenzaomai.com/gtvcqfghin.html

C#:   s.IndexOf("x")
来源：http://hz.zycfv.cn/gtfxaibaoy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydzc1.top/gtypbzneku.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xingfuxueyuan.xyz/gthmuzwgqn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.kuanghao11.cn/gtjiqqzeuo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtdtdtpzmq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.bjfxy.top/gtogidqwxy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtjliizxus.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zdqjudy.top/gtvipyqfce.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydzc1.top/gtfuiexxad.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtgnfemqxw.html

[E06] 替换子串
来源：http://hz.sysykeji.top/gtglyuiwiz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ybcxt.top/gtaljlecji.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.havefunace.top/gtuzsjsuwg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtauoejyyi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtbbseoyie.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gteghezedu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtmqklqmyl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtkdpinuxs.html

C#:   s.Replace("a", "b")
来源：http://hz.316326.xyz/gtelmygwjz.html

[E07] 按分隔符拆分
来源：http://hz.zhixingplan.top/gtdklyszxk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dashuyun.cn/gthnytfczb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuetiantiany.cn/gtjbvhmvuu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinyuanbaomall.cn/gtrkitebwk.html

TS:   s.split(",")
来源：http://hz.wangdashe.top/gttnurmpua.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hammf.cn/gtqmmycxel.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hnxiangtu.top/gtsogiyjgx.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigufen.top/gtvjrcwphm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.9152youxi.cn/gtyrohbocv.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtouwgefwv.html

Py:   ",".join(items)
来源：http://hz.yanxiufei.cn/gthxblkwct.html

PHP:  implode(",", $items);
来源：http://hz.meibo888.top/gttgjqsyhr.html

JS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtjyizdcvd.html

TS:   items.join(",")
来源：http://hz.shzxlz.cn/gtegvsbomf.html

Java: String.join(",", items)
来源：http://hz.mhx1999.top/gtdttdgcxx.html

Go:   strings.Join(items, ",")
来源：http://hz.9152youxi.cn/gttphquisr.html

Ruby: items.join(",")
来源：http://hz.sxryk.cn/gtpzffotqb.html

C#:   string.Join(",", items)
来源：http://hz.redwolf501.top/gtfosfbcjy.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gtkovisydn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangshuangyany.cn/gtvjwfiudp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hammf.cn/gtnmcgoyvw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.vqdsnc.cn/gteovsawqg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtlbjdhhxh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ivvv.top/gthxfgjsup.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtdzppvdvx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.smart0.xyz/gtpdqhznxa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtzjaqtxfp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hfpthk.cn/gtmrmxmoak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pengpengdd.cyou/gteanuqiuk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gtjnswflcp.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtlqnhykgu.html

TS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gthclaqnqj.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtbdgqoopj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinqigfzy.top/gtmpaunzfb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.52xcode.cn/gtdlygspaq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gtewhmedau.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtnmfppkdy.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtasqdyhaa.html

PHP:  strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtghefkjea.html

JS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtgyptxdft.html

TS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtkwmwicxr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shzxlz.cn/gtnwzklrxb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hysaishi.cn/gtlpjncplm.html

Ruby: s.reverse
来源：http://hz.yj202588.top/gtivtjvejp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtvhllccpy.html

[E12] 统计某字符出现次数
来源：http://hz.xylfe.cn/gtttpvuqxx.html

Py:   s.count("a")
来源：http://hz.c1oappe.top/gtljafdmur.html

PHP:  substr_count($s, "a");
来源：http://hz.kuanghao11.cn/gtkhwxibja.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtxkrfktjl.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtdvzbhxsy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenjidiqi.icu/gtxcpnitci.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gtdikxirka.html

Ruby: s.count("a")
来源：http://hz.nwbrower.top/gtjbyiywlc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gtlxlfsvtj.html

[E13] 逐字符遍历
来源：http://hz.jianghu66.top/gtuhkvhtme.html

Py:   for ch in s: print(ch)
来源：http://hz.bjfxy.top/gtjfkfsunz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj202588.top/gtzacvmavh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gtukzikjll.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ybcxt.top/gtpdruykwo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.svipenyu.cn/gtpmyfyrcu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258888.top/gtugkidonq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gogol.net.cn/gtujytfkkm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jyoumei.cn/gtmzagtfti.html

[E14] URL 编码与 Base64
来源：http://hz.tianlin.xyz/gtmozxaztu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhixingplan.top/gtgkkwdpyv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.andypj.xyz/gtecxconmv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtpcmuxjmz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fengsongda.top/gtipxdemll.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hysaishi.cn/gtoqgdalbi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.9152youxi.cn/gtwadfrwrm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gzhubu.top/gtqjhaiwqv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fengsongda.top/gtdpxykkjq.html

[E15] HTML 转义 / 反转义
来源：http://hz.sweek.top/gtctsbegun.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtvuqujoxc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ybcxt.top/gtsnfxceim.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jyoumei.cn/gtpqcskujh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jlsjyb.cn/gtdmgvwbtn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ybcxt.top/gtxoagmpbr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dashuyun.cn/gtsfjkenud.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtduvgchnq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangdashe.top/gtqwmwrbhs.html

[E16] 数字千分位
来源：http://hz.tianlin.xyz/gtgmjxupol.html

Py:   f"{1234567:,}"
来源：http://hz.yanxiufei.cn/gtllpjbsiu.html

PHP:  number_format(1234567);
来源：http://hz.fengsongda.top/gtawphfzxt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtjurslmhh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtwhbjftff.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtdzhplnlj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dashuyun.cn/gtttilkpsv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yanxiufei.cn/gtilrzpeea.html

C#:   1234567.ToString("N0")
来源：http://hz.xinyue.icu/gtdmkgpjln.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtedsdfmpn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtxhyajabw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sweek.top/gtojlaghll.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtowhwrtqi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtxpxfjqmb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhoulong.xyz/gthbcswocz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258888.top/gtksexzhuy.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gtwtaclzto.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.snrcjt.cn/gtiugkgkcc.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtydpysyzb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtzagynurq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhaomingkeji.xyz/gtyltfugmv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtigdyrids.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtthmocbeo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gaohongyu789.top/gtsdisvfks.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtriqpjrvq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yanxiufei.cn/gtklxjxjcc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuxming.cn/gtcusmdfvb.html

[E19] 多行文本按行拆分
来源：http://hz.ppjwa.cn/gtkgqcppoe.html

Py:   s.splitlines()
来源：http://hz.fengsongda.top/gthpkwovws.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258888.top/gtuylquspo.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtnrhnvbnm.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtrkzvhcas.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtobomdhjx.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhaomingkeji.xyz/gtelhpqknl.html

Ruby: s.lines
来源：http://hz.fzhhl.top/gttwlukmpw.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtbwqkqfdf.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtmoybzumx.html

Py:   if not s:
来源：http://hz.hnqzz.top/gtwvulmppz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtjavdlywt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.andypj.xyz/gtngqmhufd.html

TS:   if (s === "") {}
来源：http://hz.sufxvd.cn/gtdjclgkho.html

Java: if (s.isEmpty()) {}
来源：http://hz.redwolf501.top/gtndlrzsdk.html

Go:   if s == "" {}
来源：http://hz.yvedp.cn/gtnknijrjc.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtzddamasb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hnxiangtu.top/gtgnjgfokm.html

[E21] 超长截断加省略号
来源：http://hz.xingfuxueyuan.xyz/gtansjturq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.52xcode.cn/gtciufrlrn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtztkxchku.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtfbowkpeu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtpvahpebw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtprrnpame.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydjk.org.cn/gtwiblomtr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fzhhl.top/gtkgmdmzqa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jianghu66.top/gtgirlukng.html

[E22] 字节长度与字符长度
来源：http://hz.yj202588.top/gtgpevwqgu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guowangkeji.top/gtwxykgzet.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtlnoakmhg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtojzbgpfy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtqkyvtqxu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.vqdsnc.cn/gtlurdpgxz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gtxjovhurb.html

Ruby: s.bytesize;  s.length
来源：http://hz.yueranfly.top/gtgpjlywvx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtjbxycmqh.html

================================================================================
来源：http://hz.9152youxi.cn/gtpyiohqnn.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtucpjgtmj.html

================================================================================
来源：http://hz.zycfv.cn/gtdjquxovm.html

[F01] 读取整个文件
来源：http://hz.xuanzx.com/gtxjluwvgy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gtkoktyvlz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ybcxt.top/gtxaqnskkq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tian-w.cn/gtdghznbgj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhixingplan.top/gtfbhvmtsa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtdolfnccp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtnzweemze.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtbzuzxglv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtrcwltjvo.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gthxbwdngx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cdnleiting.top/gtyycxrlgp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gtvucyovnc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.0kj1m.cn/gtadabicve.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtwcyskvxc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtxeijijkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtfoaoejmb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nanxinkj.top/gtdegfbttn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gtyrxslriu.html

[F03] 写入文件（覆盖）
来源：http://hz.daxiang520.top/gtdotbyguh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gzhubu.top/gtpaubfpqg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtzewdvewy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtwgsojzei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtljmrwuvv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtorirasgj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtcanwnppf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.vqdsnc.cn/gthuerqmbq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shuidangran.top/gtfmwceydx.html

[F04] 追加写入文件
来源：http://hz.yj20258888.top/gtwhadjike.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shangyingyoupin.top/gtltvmzmyz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cqqwz.cn/gtrlvlgmsx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gttatmnuwu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtoiarguxh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtallpnhdk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gtpqcrrlhz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtiymzkqta.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hongshengwenyu.top/gtktzzltfx.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtslpbkaig.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xinyue.icu/gtoaflkiuv.html

PHP:  file_exists("a.txt");
来源：http://hz.xylfe.cn/gtqrmzqigx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtgyvhcuef.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtvjkfavwe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtabgqkpcx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhiwuduotai.top/gtcvobdnar.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtfwjozdqa.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtnqyxpsgm.html

[F06] 删除文件
来源：http://hz.jlsjyb.cn/gtzmwpwrxe.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtcgpewpyh.html

PHP:  unlink("a.txt");
来源：http://hz.gogol.net.cn/gtpmpmjecw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydjk.org.cn/gtodkvbdnn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtxfgjibyq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtzlgxbgnm.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtuurxfevf.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gtxtnrviod.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtygteohyb.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtisaohder.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daria6918.cn/gtvemtsmdb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yangfankeji.com/gtoxqdyhfp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gteiwutuwu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtrapopbse.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtafgkulmv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sysykeji.top/gtfpoqlnrt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hywenlv.cn/gtldoujjul.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.snrcjt.cn/gtobgcheia.html

[F08] 遍历目录
来源：http://hz.guowangkeji.top/gtqqhdatrj.html


<!-- 参考信息 -->