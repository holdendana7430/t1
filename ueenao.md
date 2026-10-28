代发 wailian999

[D23] reduce 累积计算
来源：http://hz.haohaochexian.top/gtemqtdvza.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xingfuxueyuan.xyz/gtdztmflbt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tanke756.top/gtgxqjupiv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtqkzaquch.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gteomeccuz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtyddxgxtv.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtmpqmnovn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhaomingkeji.xyz/gtrsvmplgv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtaadianyi.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenjidiqi.icu/gtopuzvfns.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fengsongda.top/gtlrebncer.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.mhx1999.top/gtuesgncec.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cdnleiting.top/gtcgqemwvo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pengpengdd.cyou/gtduglrict.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tianlin.xyz/gtsgozblsn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dashuyun.cn/gttrlihxze.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xylfe.cn/gtkjyfifuk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.feifeiyinyue.top/gtekgecefv.html

[D25] Set 集合去重与交并差
来源：http://hz.dashuyun.cn/gtxzxmglix.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pycfn.com/gtvrgtpdll.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guannengcc.top/gtnlerlgly.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ybcxt.top/gtawuxqclj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuetiantiany.cn/gtyfzeliyd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gzhubu.top/gtidhaksfj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dashuyun.cn/gtnvkvrnsw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.fzhhl.top/gtubuufemy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.birdmap.top/gtdkpoymiv.html

[D26] 数组转字符串
来源：http://hz.jqgfzy.top/gtxrnpaxsq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtywqliklh.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gthefpzpco.html

JS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gteeuajaqc.html

TS:   arr.join(", ")
来源：http://hz.yueranfly.top/gtbnyrrejl.html

Java: String.join(", ", list)
来源：http://hz.yonumen.top/gtjfnfunei.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtqxrmjoej.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtzyuprkeh.html

C#:   string.Join(", ", list)
来源：http://hz.kuanghao11.cn/gtuuhzgesl.html

================================================================================
来源：http://hz.bjfxy.top/gtyslvjtmw.html

E. 字符串处理
来源：http://hz.chenlongwang.top/gtgntywxbt.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzmykvbar.html

[E01] 拼接字符串
来源：http://hz.daxiang520.top/gtvjzxryri.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fzhhl.top/gtxlhwpafi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxuanxn.top/gtqdzdfmuj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtogbdokug.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtysopimyh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.kuanghao11.cn/gtdyvjefxs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hysaishi.cn/gtpjvivqiv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtnyiysemn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.quarkkingdee.top/gtcmkmndhl.html

[E02] 重复字符串
来源：http://hz.jlsjyb.cn/gtsiklrlhh.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtjiiwxcgy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhiwuduotai.top/gtdghhlbos.html

JS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtpzxpteqs.html

TS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtroadwpfe.html

Java: "ab".repeat(3)
来源：http://hz.shuidangran.top/gtallltwaq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtjsgnfuul.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtcfioowez.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tanke756.top/gtoqsrezao.html

[E03] 截取子串
来源：http://hz.yuxming.cn/gtqzvvnfly.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zdqjudy.top/gtaqxhvael.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtopnkqtnl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ybcxt.top/gtccgrtohx.html

TS:   s.slice(1, 4)
来源：http://hz.yangfankeji.com/gtpeqblive.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtvddcqogd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gtkhqgbcef.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangkeji.top/gtrvlrkslj.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gtcrwrpyxf.html

[E04] 查找子串位置
来源：http://hz.kuanghao11.cn/gtogzofgie.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xziqi.cn/gtdnkotrfo.html

PHP:  strpos($s, "x");
来源：http://hz.zhoulong.xyz/gtzsvurwwa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.snrcjt.cn/gtkuymwqmw.html

TS:   s.indexOf("x")
来源：http://hz.pengpengdd.cyou/gtqjizicbr.html

Java: s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtctfuihze.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gtrfgjleau.html

Ruby: s.index("x")
来源：http://hz.zhoulong.xyz/gtfyzhmlqu.html

C#:   s.IndexOf("x")
来源：http://hz.hongshengwenyu.top/gtfrwebwty.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pengpengdd.cyou/gtrkyjwrsx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhaomingkeji.xyz/gtufzoerit.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gtzigscdnh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cdnleiting.top/gtavgnedwx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shangyingyoupin.top/gtihomgsyx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtwnmpblzt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xylfe.cn/gtbqowfwwn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhongyouzk.top/gtdtgcqmch.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgufenzy.top/gtzwgylvhm.html

[E06] 替换子串
来源：http://hz.pycfn.com/gtgknugqyo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shanyushiyangkeji.top/gtpdyqcywm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.bjfxy.top/gtgaxwzhpn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtyhkrfwvf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtdatuohjo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gttbcjwjam.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xylfe.cn/gtsxddmgtv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.smart0.xyz/gtzvmyxqjw.html

C#:   s.Replace("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtlmdpyisc.html

[E07] 按分隔符拆分
来源：http://hz.mhx1999.top/gturnltchl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtyreyvhwj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gtgnonaxrv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xinyue.icu/gthiegmgdv.html

TS:   s.split(",")
来源：http://hz.shangyingyoupin.top/gtepyhgtoh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.haohaochexian.top/gtsmbfhaoh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtirpyqknu.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtqddrztei.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gtjqtzkyzr.html

[E08] 数组按分隔符合并
来源：http://hz.hfpthk.cn/gtbfinrypi.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtlinjcteu.html

PHP:  implode(",", $items);
来源：http://hz.fzhhl.top/gteibthjvn.html

JS:   items.join(",")
来源：http://hz.bjfxy.top/gtwoxolvmm.html

TS:   items.join(",")
来源：http://hz.bjfxy.top/gtdegenudz.html

Java: String.join(",", items)
来源：http://hz.52xcode.cn/gtwhvnpyoz.html

Go:   strings.Join(items, ",")
来源：http://hz.hammf.cn/gtozdwuual.html

Ruby: items.join(",")
来源：http://hz.shzxlz.cn/gtwevzdmdz.html

C#:   string.Join(",", items)
来源：http://hz.meibo888.top/gtmdxlafzu.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtlktuvnln.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shzxlz.cn/gtchvfxlxj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pycfn.com/gtdpskceie.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtnyflgdzu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.mhx1999.top/gtrhewhkni.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtxqdlmyxk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.snrcjt.cn/gtalzbcaqa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ybcxt.top/gtlkhytbfq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258.top/gtvzxyagyv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.haohaochexian.top/gtrzavjstv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenlongwang.top/gtmopdnmqb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sufxvd.cn/gtleymifyy.html

JS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtpockgmgv.html

TS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtlogjpeds.html

Java: String.format("%03d", 7)
来源：http://hz.jiagoushi.top/gtfvkwlnhk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtaerutccz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtypsrgfyr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnqzz.top/gtfofxmipx.html

[E11] 反转字符串
来源：http://hz.aizwys.cn/gtihsinjzx.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtnbuywvah.html

PHP:  strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtmppxrygg.html

JS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtwakonrpy.html

TS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtqijygeor.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gotoacloud.top/gtmmvsmiis.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gtxxiejabo.html

Ruby: s.reverse
来源：http://hz.yj20258.top/gtfjwgmcty.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtgugtoncg.html

[E12] 统计某字符出现次数
来源：http://hz.cdnleiting.top/gtvdkzmrjx.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtmfgatefs.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtmwhrvdqg.html

JS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtppsbjtlm.html

TS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtcktmozof.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gttwcnbjcf.html

Go:   strings.Count(s, "a")
来源：http://hz.hnxiangtu.top/gtfvplqiva.html

Ruby: s.count("a")
来源：http://hz.hnxiangtu.top/gtluioogwx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gtqffyjaml.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtlnbroyom.html

Py:   for ch in s: print(ch)
来源：http://hz.xingfuxueyuan.xyz/gtrjovyhif.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gtmgtvdjsj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fzhhl.top/gtiylcmpdr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtpjiaydkr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hfpthk.cn/gtocodkhrs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tian-w.cn/gtszqnoswq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gtbnsgrmms.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yongpay.top/gtiygzchmo.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtodthznjj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.redwolf501.top/gtpzthynpg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.316326.xyz/gtmgrdahfx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jiagoushi.top/gtyiwfwuyi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tianlin.xyz/gtqoukyitq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.feifeiyinyue.top/gtkvjswobj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.svipenyu.cn/gtbtejbgfp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtdslzbbiz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangtech.top/gtzmatqnci.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtproafpxg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnqzz.top/gtijbqpput.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtsssrmawb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pengpengdd.cyou/gtxvlvcjxa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.9152youxi.cn/gtmgwxlksi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtnzapdcwz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.smart0.xyz/gtpmdywktp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tianlin.xyz/gtmyxsktvo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gtfwdsicla.html

[E16] 数字千分位
来源：http://hz.meibo888.top/gtnvhnlwxg.html

Py:   f"{1234567:,}"
来源：http://hz.quarkkingdee.top/gtssmciqib.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtumpxaima.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtpvwatdya.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jianghu66.top/gtdimhrvso.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cheryme.top/gthtwwuggh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtisdoispx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.redwolf501.top/gttoyjcdwq.html

C#:   1234567.ToString("N0")
来源：http://hz.shangyingyoupin.top/gtfptrizri.html

[E17] 首字母大写
来源：http://hz.ppjwa.cn/gtvuwyuqjr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zycfv.cn/gtixtosazv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cdnleiting.top/gtocfsltle.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtupheantg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangdashe.top/gtkcrznetw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gthsiicuyr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gtknzkqxrh.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtorfqdene.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtvhzurufm.html

[E18] 模板占位符替换
来源：http://hz.52xcode.cn/gtfkprvhhu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gtsanckutr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhaomingkeji.xyz/gtasvnoftq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtxibqtjcc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtazebtvso.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yongpay.top/gtopgdzswt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sysykeji.top/gtstoqvthd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ywan-chungtsiang.top/gtnkxygxvb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shzxlz.cn/gtxasecrxu.html

[E19] 多行文本按行拆分
来源：http://hz.redwolf501.top/gtsmvbuxsd.html

Py:   s.splitlines()
来源：http://hz.cqqwz.cn/gtpuaftsdw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yongpay.top/gtyyfvpvso.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtjwwpsife.html

TS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtjedwnuoj.html

Java: s.lines().toList()
来源：http://hz.ybcxt.top/gtxlyaavtq.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhiwuduotai.top/gtruzhbrwn.html

Ruby: s.lines
来源：http://hz.hfpthk.cn/gtutgjmbpf.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gthztthjce.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtojsnmlaf.html

Py:   if not s:
来源：http://hz.ywan-chungtsiang.top/gtfimzslrg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuanzx.com/gtbiyhamke.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zycfv.cn/gtqzghsqwp.html

TS:   if (s === "") {}
来源：http://hz.dianchejie.cn/gtgjaeopte.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtqyhmakda.html

Go:   if s == "" {}
来源：http://hz.meibo888.top/gthbuwebkr.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtzevotoas.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtohbjgryv.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtmnlezpkh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgufenzy.top/gtgmuopnjm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigfzy.top/gtirvhkdki.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtaufjjjfx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtftutofte.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtriukibfu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ivvv.top/gteazgikah.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gtigkdxrkw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aizwys.cn/gtfciwqmuf.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtcjtiesrf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtiyjafyne.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtyiepeaqd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtjrcfqxsv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtdknesnlj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ybcxt.top/gtxkisdgzw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ehwqpu.com/gtmaywohzn.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangkeji.top/gtecmvotae.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sysykeji.top/gtdvanzaps.html

================================================================================
来源：http://hz.yvedp.cn/gtrjnzmjej.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtrlrrvrsg.html

================================================================================
来源：http://hz.xuanzx.com/gtvnaejyyf.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtlwjdavev.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ppjwa.cn/gtmicdinrw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.smart0.xyz/gtojlqpsbr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtgdkjvtxn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtpbkxcrmx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtskymnmqi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenzaomai.com/gtbvwrmqty.html

Ruby: File.read("a.txt")
来源：http://hz.chenzaomai.com/gtibhyjrls.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.52xcode.cn/gtngfyzstv.html

[F02] 逐行读取文件
来源：http://hz.yuxming.cn/gtrufxmnyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258.top/gtsgcanvny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sysykeji.top/gtbhlantbk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jyoumei.cn/gtiicmulbs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtzettiuqk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtcbayostc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtvryaooqx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.9152youxi.cn/gtnyxbzoqe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhijiandao.cn/gtedzvdhcp.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtxoniqnzb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinghuilouyu.cn/gtekzhlmrp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtcvgvgtjd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tanke756.top/gtkkroriss.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtkmqymzvf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinghuilouyu.cn/gtmhdbqhyp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gtktjlfdrc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sweek.top/gtsrgxbfwr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtinukiobf.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gtsnwmjowp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtnhvzycjy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtslsupflz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtduwvzwdj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtzenmusbu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtbyfjqkin.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.bjfxy.top/gtbvzcepia.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aizwys.cn/gtddnsvecm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtaegzulmj.html

[F05] 判断文件或目录是否存在
来源：http://hz.yvedp.cn/gtunettbwc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.c1oappe.top/gtjdhxchvg.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtdblkcgfr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtdtkllrpq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtmyqqmxnc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtddaybrzp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ehwqpu.com/gtoalgoewk.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtmismdvdu.html

C#:   File.Exists("a.txt")
来源：http://hz.iojbl.cn/gtsclpthek.html

[F06] 删除文件
来源：http://hz.hywenlv.cn/gtsnptlwpk.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtwgthryet.html

PHP:  unlink("a.txt");
来源：http://hz.bjfxy.top/gtobajmocr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtsmdtzxgw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtnxdvvwvv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gthumdklii.html

Go:   os.Remove("a.txt")
来源：http://hz.cashguo.top/gtvtwjcurk.html

Ruby: File.delete("a.txt")
来源：http://hz.hfpthk.cn/gtpjevvmoi.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtdicqwukx.html

[F07] 创建目录（含多级）
来源：http://hz.guannengcc.top/gtsagqytrd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtfxsmwkur.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtfcrmakcd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtnirbwhfm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtzntpabmk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dianchejie.cn/gtcxjtljeu.html


<!-- 参考信息 -->