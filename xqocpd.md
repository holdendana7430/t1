代发 wailian999

[D23] reduce 累积计算
来源：http://hz.birdmap.top/gtrvbcicwn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.redwolf501.top/gtyszkijnu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dashuyun.cn/gtyezrswlq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtjswbidvr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtxaczhpsg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtdapmrcps.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtkyarocyu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.redwolf501.top/gtqkdbomyn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gotoacloud.top/gthlioarox.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtgqhhehxi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.0kj1m.cn/gtzxhcqnko.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ywan-chungtsiang.top/gtdixrauop.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgfzy.top/gtibdsvgnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.0kj1m.cn/gtosbpalvg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shuidangran.top/gtbhyriojs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtnhumqorb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhijiandao.cn/gteivdqzyx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yongpay.top/gthtjncrfr.html

[D25] Set 集合去重与交并差
来源：http://hz.cheryme.top/gtigmaofbl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtxwadwyrf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hysaishi.cn/gtehiphhof.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenzaomai.com/gtuyeqgtlb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigfzy.top/gtpbvdudrl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuxming.cn/gthkxebdzy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daria6918.cn/gtgnirhtsn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.316326.xyz/gtukimtjrh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtpcauckjf.html

[D26] 数组转字符串
来源：http://hz.fengsongda.top/gtobzxgdoc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xziqi.cn/gtzuwryweq.html

PHP:  implode(", ", $arr);
来源：http://hz.zhengqikj.top/gtudaffwps.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtjrhzlouv.html

TS:   arr.join(", ")
来源：http://hz.jlsjyb.cn/gtqkbylyts.html

Java: String.join(", ", list)
来源：http://hz.iojbl.cn/gthussiihi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yueranfly.top/gtkxjjhvcw.html

Ruby: arr.join(", ")
来源：http://hz.yj20258888.top/gthyabplxi.html

C#:   string.Join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtiqqzrdfe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtokbbtxpm.html

E. 字符串处理
来源：http://hz.wangdashe.top/gtfxqiayzu.html

================================================================================
来源：http://hz.daxiang520.top/gtpyqghwvn.html

[E01] 拼接字符串
来源：http://hz.yuxming.cn/gtigxxsipe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.haohaochexian.top/gtkkkjuwqu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtfaxmkirs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtnfeaeplu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtsjnrznue.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aibaodan.cn/gttkbdpivv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gotoacloud.top/gtvydjtrxq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yongpay.top/gtluwgszjt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gtvrmyafgn.html

[E02] 重复字符串
来源：http://hz.cheryme.top/gttkonygmi.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtzjbulqnt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gthbezclvj.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtjmkfweat.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtnvbtcjin.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtvalxfemr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtcldhuqec.html

Ruby: "ab" * 3
来源：http://hz.ehwqpu.com/gtikpmkdjh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shuidangran.top/gtdnmvozlw.html

[E03] 截取子串
来源：http://hz.zdqjudy.top/gtfdnbvuin.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pycfn.com/gtspjcdxaq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aibaodan.cn/gtbhxcqisk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xziqi.cn/gtvyeoxlxw.html

TS:   s.slice(1, 4)
来源：http://hz.jinqigfzy.top/gtmshivdee.html

Java: s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtwcmbbvrk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtxotsktkd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zdqjudy.top/gtftpxphwk.html

C#:   s.Substring(1, 3)
来源：http://hz.meibo888.top/gttwejefql.html

[E04] 查找子串位置
来源：http://hz.snrcjt.cn/gtmlniyixz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtogvdanbj.html

PHP:  strpos($s, "x");
来源：http://hz.hammf.cn/gtwtmhoibn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtbscboort.html

TS:   s.indexOf("x")
来源：http://hz.snrcjt.cn/gtgwldmyjg.html

Java: s.indexOf("x")
来源：http://hz.meibo888.top/gttjlvatda.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258888.top/gttawdthse.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtpffsgfis.html

C#:   s.IndexOf("x")
来源：http://hz.jinyuanbaomall.cn/gttuoaonyy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258888.top/gtzfzapbhf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gogol.net.cn/gtjeoctkok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtlauprlvw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtsgltpbpw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.52xcode.cn/gtxyzhynkd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtodpzgrfj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ybcxt.top/gttcxhwcmy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fengsongda.top/gtnwfxhjpx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gttxfngrtm.html

[E06] 替换子串
来源：http://hz.jiagoushi.top/gtriijlaoa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.c1oappe.top/gtxordoppk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hywenlv.cn/gtqlbykxky.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtnquynzkt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtnwmebetg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gthkkvkkxi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.52xcode.cn/gtqzbubtdh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtmuciwjaw.html

C#:   s.Replace("a", "b")
来源：http://hz.chenjidiqi.icu/gtknxakyti.html

[E07] 按分隔符拆分
来源：http://hz.iojbl.cn/gtpginodge.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xylfe.cn/gtgxvphpoo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtdesdcfoj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.mhx1999.top/gtzokiasnx.html

TS:   s.split(",")
来源：http://hz.jiagoushi.top/gtdrkkzqzr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgufenzy.top/gtksmqdclr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yvedp.cn/gtmkoevcbw.html

Ruby: s.split(",");  s.split
来源：http://hz.hysaishi.cn/gtgtllxvvg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtjfmgwmxr.html

[E08] 数组按分隔符合并
来源：http://hz.yanxiufei.cn/gtauqvdikq.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtntpztgkm.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtvopuwyur.html

JS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtnuwgsccn.html

TS:   items.join(",")
来源：http://hz.zycfv.cn/gtwoqkcatf.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtjeegonvr.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gtfgviigub.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gteocjlrtk.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtuclnuije.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtvdczyvkz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tian-w.cn/gthvylpoma.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhaomingkeji.xyz/gtdubvbdfl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtbmmptpcs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cqqwz.cn/gtlrfipxoa.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtsdmswxsv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258.top/gtwgldtbgs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinghuilouyu.cn/gtbjatjfwl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtkltmbxou.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yvedp.cn/gtqdrkohcq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gaohongyu789.top/gtilnppyfj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sxryk.cn/gtdkudohlk.html

JS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtqewulwvk.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gttdepkvzn.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtncsghtxf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.redwolf501.top/gtpikjrbgb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtlpqhrcbh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gogol.net.cn/gtykhduesj.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gtwheqqqfy.html

Py:   s[::-1]
来源：http://hz.zhixingplan.top/gtnmhrvyor.html

PHP:  strrev($s);
来源：http://hz.sufxvd.cn/gtcvixmvnb.html

JS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gttdyikbxj.html

TS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtjkvwwxbr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gaohongyu789.top/gtifanpjuy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtwvfrwtnx.html

Ruby: s.reverse
来源：http://hz.shuidangran.top/gtdlavlzyc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtewhssbek.html

[E12] 统计某字符出现次数
来源：http://hz.tian-w.cn/gtfahpdfdn.html

Py:   s.count("a")
来源：http://hz.tanke756.top/gtwoamdano.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtszqrpuxo.html

JS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtjoknpfmh.html

TS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gthpljjyii.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gzhubu.top/gtclmgxptb.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtkinstvwg.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gthxfeoofo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gtkiiplsrj.html

[E13] 逐字符遍历
来源：http://hz.jinghuilouyu.cn/gtwndwtkrj.html

Py:   for ch in s: print(ch)
来源：http://hz.jinqigfzy.top/gtfitiwzrb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tanke756.top/gtumqzquae.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtvppbfebp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtqkezighu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangdashe.top/gtbfqhzjka.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtqihfzplv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zycfv.cn/gtwhpdxlei.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtveevxaed.html

[E14] URL 编码与 Base64
来源：http://hz.xingfuxueyuan.xyz/gtkfvpuxdk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhaomingkeji.xyz/gtpvlpwoqm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gtgtnjbfsi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.vqdsnc.cn/gtkxutappj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.havefunace.top/gttvsqhadj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.iojbl.cn/gtrjkiralw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.quarkkingdee.top/gtakfrvssi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhixingplan.top/gtjdzcuwwr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtumgxohrm.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gtkjbvawhf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.52xcode.cn/gtyjwltgoj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daxiang520.top/gtjugvrrmm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gotoacloud.top/gtaesdmtkk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pycfn.com/gtooqkexog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gogol.net.cn/gthuvyvkpx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj202588.top/gtqqvrzsrn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gthmsnwlen.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.0kj1m.cn/gtaldaekgh.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtxhlmuono.html

Py:   f"{1234567:,}"
来源：http://hz.mhx1999.top/gtdovvrvts.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtgwqqgrwk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtynoimwsp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtugrpmxnp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xziqi.cn/gtxjdydwae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtudpwwjhu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gtzvyuekeu.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gtcxxjngfm.html

[E17] 首字母大写
来源：http://hz.jianghu66.top/gtrnjoizft.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenlongwang.top/gtlftmnvlg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gtwzcqmpaw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtgwduwaqc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gteneczcnp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cucudq.cn/gtbiakuhbe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hysaishi.cn/gthwhdofkt.html

Ruby: s.capitalize
来源：http://hz.c1oappe.top/gtyjtcektf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jianghu66.top/gtrddoynju.html

[E18] 模板占位符替换
来源：http://hz.ybcxt.top/gthmgzfugz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtzelfrdrw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jyoumei.cn/gtcvokspei.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtuaqnnvrh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtqsqxgeru.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtpikzknam.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aizwys.cn/gtyoakrsvj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daxiang520.top/gtrkbbrusr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cashguo.top/gtomihagnj.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtqvcuncdu.html

Py:   s.splitlines()
来源：http://hz.nanxuanxn.top/gtgpzshzys.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gtxjkeoqgx.html

JS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtdxgvhbxh.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gthletfezr.html

Java: s.lines().toList()
来源：http://hz.yj202588.top/gtaquhnbah.html

Go:   strings.Split(s, "\n")
来源：http://hz.fzhhl.top/gtjptxwkaz.html

Ruby: s.lines
来源：http://hz.aibaodan.cn/gtowqlzcld.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gtfmmlbnhu.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtdbcyupgt.html

Py:   if not s:
来源：http://hz.quarkkingdee.top/gtvxrdmegn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yuxming.cn/gtwqxuzigf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tian-w.cn/gtiywvoxso.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtwktvaghh.html

Java: if (s.isEmpty()) {}
来源：http://hz.andypj.xyz/gtshxfhgqf.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gtliexitrg.html

Ruby: if s.empty?
来源：http://hz.feifeiyinyue.top/gtqjtfewrx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gtdrrdalgu.html

[E21] 超长截断加省略号
来源：http://hz.shzxlz.cn/gtbxkuagkv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxuanxn.top/gttlmqvqve.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtdckayzdy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtelomfpzx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtxsjviizr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtwkpyprwu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.smart0.xyz/gtglivhwcr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jiagoushi.top/gtiglutvpo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guowangkeji.top/gtrxddeaol.html

[E22] 字节长度与字符长度
来源：http://hz.zdqjudy.top/gtuikifeov.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.andypj.xyz/gtkrkzwqvt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtkietnbxa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtbbkkjrws.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtxptahovl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gtvonqzhth.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuxming.cn/gtuyxjomgt.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenjidiqi.icu/gtdzgfjqgj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gtzylmqgqx.html

================================================================================
来源：http://hz.cashguo.top/gtanalkeny.html

F. 文件与目录
来源：http://hz.iojbl.cn/gtqysfteqj.html

================================================================================
来源：http://hz.xziqi.cn/gtscrnxpsy.html

[F01] 读取整个文件
来源：http://hz.ydjk.org.cn/gtnarnwvyj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtqurwnsfd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhongyouzk.top/gtmqmbiljv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jqgfzy.top/gthejddlhz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cucudq.cn/gttefmpkzi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtkwdmqhco.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gtekmebdkg.html

Ruby: File.read("a.txt")
来源：http://hz.c1oappe.top/gtjkzytpzw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.bjfxy.top/gtypzkqups.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtythayeof.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aizwys.cn/gtyooqjxxa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenjidiqi.icu/gtfcmmqihl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtmyekrlnd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gthldkqyrq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gttilttfso.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.haohaochexian.top/gtronmifbk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.quarkkingdee.top/gtzwydkast.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yangfankeji.com/gtohfozqba.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtascrvuwt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtsecgezhp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxinkj.top/gtfjirjkwd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtticuscaf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aizwys.cn/gtswsttqgw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gogol.net.cn/gtdctajair.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xuetiantiany.cn/gtufhqhslg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yonumen.top/gtvxfcjcoa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fengsongda.top/gthfxlzgsc.html

[F04] 追加写入文件
来源：http://hz.sxryk.cn/gtkgulijxy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtyfqjarvg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtbbaylscp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtdqfxgydm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtjianmzcn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gtsiqsizse.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pycfn.com/gtcogofubs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnqzz.top/gtldpaqgfu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtcgayokkx.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtrhnkhrzj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.birdmap.top/gtjtllevzf.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtbhwyvxyi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtczvbwwao.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtkbgiawgs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtopviqdee.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtmtzhdyzo.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gthcnbgfmw.html

C#:   File.Exists("a.txt")
来源：http://hz.jinghuilouyu.cn/gttkkbfqdu.html

[F06] 删除文件
来源：http://hz.yvedp.cn/gtpwwgegyo.html

Py:   os.remove("a.txt")
来源：http://hz.yangfankeji.com/gtrkygvnwd.html

PHP:  unlink("a.txt");
来源：http://hz.cqqwz.cn/gtzhgnqifg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtzzpfzzhg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtpysjbapk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtxkbxwurk.html

Go:   os.Remove("a.txt")
来源：http://hz.andypj.xyz/gtugszukga.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtnzrdhnkg.html

C#:   File.Delete("a.txt");
来源：http://hz.yvedp.cn/gtauhwthog.html

[F07] 创建目录（含多级）
来源：http://hz.svipenyu.cn/gtvktqvnpy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cheryme.top/gtzsnylmkk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtfckcoxkf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gttcdiuiev.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtzfaqfech.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnxiangtu.top/gtrmdkrdyr.html


<!-- 参考信息 -->