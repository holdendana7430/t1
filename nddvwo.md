代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtckhjqfdf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258888.top/gtcyafpvxg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daria6918.cn/gtpaujfhas.html

C#:   new List<int>(list);
来源：http://hz.jyoumei.cn/gtivukkzhl.html

[D23] reduce 累积计算
来源：http://hz.wangshuangyany.cn/gtrugeczus.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhoulong.xyz/gtepvgrygi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cdnleiting.top/gtgydqfmrl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtlhazqpug.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtzrckjiaq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhengqikj.top/gtpmhnnhjq.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtfximvzhp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhixingplan.top/gtxgqziphy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinyuanbaomall.cn/gtrqaodeyj.html

[D24] 字典 / Map 基本操作
来源：http://hz.aizwys.cn/gtjrjeqepg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydjk.org.cn/gtyackiwhz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtghdnliax.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xziqi.cn/gtlmsrplpn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtlnyantsc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.haohaochexian.top/gtjzedauuy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtubufmrxr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtxmlhhhil.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtyulohvfz.html

[D25] Set 集合去重与交并差
来源：http://hz.316326.xyz/gtqumxujad.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhixingplan.top/gtxhaujmuv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtphwgejzl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jqgfzy.top/gtrqczkxxw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.daxiang520.top/gtlesjrtrr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.mhx1999.top/gtgxkkabai.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gttgpsfqek.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xziqi.cn/gttvhcjqxk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnqzz.top/gtxsunobyr.html

[D26] 数组转字符串
来源：http://hz.xuetiantiany.cn/gtsfygykdh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yangfankeji.com/gtjoztkrui.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangtech.top/gtdkzbhbey.html

JS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtcdkolmjf.html

TS:   arr.join(", ")
来源：http://hz.nwbrower.top/gttkjfxgnu.html

Java: String.join(", ", list)
来源：http://hz.xuetiantiany.cn/gtbsafajss.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtjkmgrxaz.html

Ruby: arr.join(", ")
来源：http://hz.mhx1999.top/gtffdrezvv.html

C#:   string.Join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtcbpxtisp.html

================================================================================
来源：http://hz.ivvv.top/gtjvupakro.html

E. 字符串处理
来源：http://hz.hfpthk.cn/gtpgahmaib.html

================================================================================
来源：http://hz.ydzc1.top/gtxslkevsi.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gthrwalaaq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.redwolf501.top/gtycyxfnde.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258.top/gtzgumzxay.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtownsvlwc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtdclpclow.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yueranfly.top/gtajugbaal.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xziqi.cn/gtailynove.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtwdbeplnw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tian-w.cn/gtpxcpjszb.html

[E02] 重复字符串
来源：http://hz.jyoumei.cn/gtqvunatlt.html

Py:   "ab" * 3
来源：http://hz.cheryme.top/gtdbgutlrj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shangyingyoupin.top/gtcjansjvt.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gtlevgqzxh.html

TS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtfhqyvjhs.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtmmvwqelo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhijiandao.cn/gthiaefgwg.html

Ruby: "ab" * 3
来源：http://hz.andypj.xyz/gtsvyuwuiu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hfpthk.cn/gtkfhopobf.html

[E03] 截取子串
来源：http://hz.jlsjyb.cn/gtxtjzubxu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.haohaochexian.top/gtgwgdgpzt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gthnranzsv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtofyrojkh.html

TS:   s.slice(1, 4)
来源：http://hz.sufxvd.cn/gtpcqrygij.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtrlpdhjpi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.9152youxi.cn/gtwuntzqcj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hongshengwenyu.top/gtnqbavzgp.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gtanqncpea.html

[E04] 查找子串位置
来源：http://hz.jinyuanbaomall.cn/gtqrlxvsyf.html

Py:   s.find("x");  s.index("x")
来源：http://hz.9152youxi.cn/gtpnhseqoa.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gtrqxbrofb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jyoumei.cn/gttduozyaa.html

TS:   s.indexOf("x")
来源：http://hz.ppjwa.cn/gtemlxudnb.html

Java: s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtkecspqua.html

Go:   strings.Index(s, "x")
来源：http://hz.shangyingyoupin.top/gtvxkuwmzb.html

Ruby: s.index("x")
来源：http://hz.aizwys.cn/gtivraoubq.html

C#:   s.IndexOf("x")
来源：http://hz.cashguo.top/gtirccfued.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hywenlv.cn/gtasggudzn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cashguo.top/gtozwdiazg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gttwpqmndf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gttabctqkq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ivvv.top/gtnmithqqu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtrwgibgwr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.wangshuangyany.cn/gtzgeqjifa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.0kj1m.cn/gtmfhafhva.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hongshengwenyu.top/gthuzfisih.html

[E06] 替换子串
来源：http://hz.jianghu66.top/gtxyiaapvw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangshuangyany.cn/gtsfazbgzx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.c1oappe.top/gtqqpoxwke.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtdqbskmxq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtyhhkhevq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtaybxznvn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sufxvd.cn/gtuvywctdr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shzxlz.cn/gtgrbavovv.html

C#:   s.Replace("a", "b")
来源：http://hz.haohaochexian.top/gthlovjlkc.html

[E07] 按分隔符拆分
来源：http://hz.hnqzz.top/gtxfisdlfx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhiwuduotai.top/gtfjrcncyx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgufenzy.top/gtnppovdsv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.52xcode.cn/gtglrmrytd.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtghfnhkft.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yuxming.cn/gtyoyeebvh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gtromkxnoi.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangkeji.top/gtdcxhzrqc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.316326.xyz/gtbldzxahq.html

[E08] 数组按分隔符合并
来源：http://hz.sweek.top/gtzjzaccse.html

Py:   ",".join(items)
来源：http://hz.hnxiangtu.top/gtsvtqzzuc.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtbykhhtst.html

JS:   items.join(",")
来源：http://hz.yongpay.top/gtteheqkrz.html

TS:   items.join(",")
来源：http://hz.zhaomingkeji.xyz/gtynokeqyz.html

Java: String.join(",", items)
来源：http://hz.yvedp.cn/gtiumfjavl.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtnoqeltfk.html

Ruby: items.join(",")
来源：http://hz.quarkkingdee.top/gtcqysdzzb.html

C#:   string.Join(",", items)
来源：http://hz.yj202588.top/gtttxduvve.html

[E09] 去除所有空白字符
来源：http://hz.xingfuxueyuan.xyz/gtastsuedn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xziqi.cn/gtkzfmbuns.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxuanxn.top/gtpplwvgvh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtxwjxrxhj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtumzlqvyj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hfpthk.cn/gtuupxcspn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cashguo.top/gtggyyruir.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.52xcode.cn/gtlnaiqkhj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hammf.cn/gtlfzxivop.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtfdhiuyyi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shangyingyoupin.top/gtqqhutugq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenjidiqi.icu/gtmgunkqxi.html

JS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtdwxmucwu.html

TS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtjeoalobl.html

Java: String.format("%03d", 7)
来源：http://hz.yueranfly.top/gtlvqkpbxv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xylfe.cn/gtpicuptyd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dianchejie.cn/gtunmbdgtf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtztvcvmzt.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gtsoywomif.html

Py:   s[::-1]
来源：http://hz.ybcxt.top/gtdcgmcnmr.html

PHP:  strrev($s);
来源：http://hz.zhongyouzk.top/gtlndrfbfa.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtvnexlmln.html

TS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtnhogglna.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tianlin.xyz/gtidlolchr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangtech.top/gtrfwzflzn.html

Ruby: s.reverse
来源：http://hz.hammf.cn/gtgiavzsbo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtskkryoeu.html

[E12] 统计某字符出现次数
来源：http://hz.cqqwz.cn/gtzrrzazlg.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtmswkiotj.html

PHP:  substr_count($s, "a");
来源：http://hz.jinghuilouyu.cn/gtegrgqzwz.html

JS:   s.split("a").length - 1
来源：http://hz.shzxlz.cn/gttbrvgeis.html

TS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtwxpykeqo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pycfn.com/gteofvlbiv.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gttxjcejtw.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtwtffudlo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuetiantiany.cn/gtgdvxeknp.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtbfkwnpux.html

Py:   for ch in s: print(ch)
来源：http://hz.nwbrower.top/gtxwflggrr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gtkjfllydy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtkkaaykop.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtvynawado.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtugnpamuy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.quarkkingdee.top/gtpxieszhr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tian-w.cn/gtrjupcgsi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guowangkeji.top/gteurwtwao.html

[E14] URL 编码与 Base64
来源：http://hz.hnqzz.top/gtkymspzbr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cheryme.top/gtbvzhszvn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shangyingyoupin.top/gtlzuxofui.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtzruexhsp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hfpthk.cn/gtcjpwsaku.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gtnnxxqaej.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtdypuglbr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtwpasapfp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yonumen.top/gtlbpxadad.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuxming.cn/gthqycdhhs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtllmwesjm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangdashe.top/gtuhkxavgw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cheryme.top/gtgxotonds.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangkeji.top/gthfunesow.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sufxvd.cn/gtlrpvnuhz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ehwqpu.com/gtugfddjrf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daxiang520.top/gtaqistjhm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhiwuduotai.top/gtpkletnkq.html

[E16] 数字千分位
来源：http://hz.ivvv.top/gtdsrkonas.html

Py:   f"{1234567:,}"
来源：http://hz.chenzaomai.com/gtqxvspfwd.html

PHP:  number_format(1234567);
来源：http://hz.cucudq.cn/gtwiyqplrk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gtroozpgzh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtgfkzvsdh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.iojbl.cn/gthonhlony.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtslzibnqa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.meibo888.top/gtilzqztqt.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gtrictjeet.html

[E17] 首字母大写
来源：http://hz.wangdashe.top/gtbxkzqixq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xziqi.cn/gttqlmmwqk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtwdwrbgcc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gttajlcclt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtiahfrubs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zdqjudy.top/gttzxtndit.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aizwys.cn/gttbjoansq.html

Ruby: s.capitalize
来源：http://hz.redwolf501.top/gtlvrdfcxr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtsngkhjra.html

[E18] 模板占位符替换
来源：http://hz.zycfv.cn/gtmebfkbbi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.0kj1m.cn/gtnuzfkdoz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nwbrower.top/gtarkeibhs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gthbwdjxny.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtbpsoalzz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.meibo888.top/gtwilastro.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gttfyttflc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shzxlz.cn/gtbojhajzn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xziqi.cn/gtbfsqhese.html

[E19] 多行文本按行拆分
来源：http://hz.shuidangran.top/gtwhvbndfl.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtzzpaougn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnqzz.top/gtljmnnoqv.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtkyzarshv.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtrhdbegyp.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtcmzicghs.html

Go:   strings.Split(s, "\n")
来源：http://hz.yvedp.cn/gtfzhmynsz.html

Ruby: s.lines
来源：http://hz.xinyue.icu/gtstazkprd.html

C#:   s.Split('\n')
来源：http://hz.hongshengwenyu.top/gtafctygdf.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gttqawfhmw.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gttqbrcnuu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtuxwhdixu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gotoacloud.top/gtgiyhdtup.html

TS:   if (s === "") {}
来源：http://hz.jqgufenzy.top/gtncptqdwc.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtakwxoyxc.html

Go:   if s == "" {}
来源：http://hz.pengpengdd.cyou/gtvbzwxmsu.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtmojtufyy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guowangkeji.top/gtynrxjkhw.html

[E21] 超长截断加省略号
来源：http://hz.tian-w.cn/gtjskkwqdf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuxming.cn/gthkfxcifa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtdmyvxbvm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtdibzttzu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtzzpuvaeb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtfhdnpohr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.kuanghao11.cn/gtpnecwxzn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guannengcc.top/gtohaiikid.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sxryk.cn/gtvpsvcdql.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gthzdeqrdb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tanke756.top/gtzyqkdpgx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtxwdmbvjf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtmruoxgrm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtuwztghul.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tian-w.cn/gtexjvfgkk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.bjfxy.top/gtyjfxrpxk.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtazrklqzc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gtyvsruyap.html

================================================================================
来源：http://hz.hysaishi.cn/gtsdcgdcvw.html

F. 文件与目录
来源：http://hz.bjfxy.top/gticvnmxtu.html

================================================================================
来源：http://hz.ydzc1.top/gtyzyotdtl.html

[F01] 读取整个文件
来源：http://hz.snrcjt.cn/gttpcqdcwj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.smart0.xyz/gtdaxwyfte.html

PHP:  file_get_contents("a.txt");
来源：http://hz.kuanghao11.cn/gtzlowzbnn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangtech.top/gtbuhhtggl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hongshengwenyu.top/gtcumbdmay.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtusvhqmcq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gtrbdatdcy.html

Ruby: File.read("a.txt")
来源：http://hz.zhoulong.xyz/gtzhymcxfg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtvxjwnjbd.html

[F02] 逐行读取文件
来源：http://hz.yj20258888.top/gthnblsilx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gtsnoqduek.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hysaishi.cn/gtkcouujmt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtgntqxotk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtkbcndppl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtlvrwawfa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.quarkkingdee.top/gthaipbisd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangtech.top/gtwvtqwqkt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinghuilouyu.cn/gttqteinyw.html

[F03] 写入文件（覆盖）
来源：http://hz.havefunace.top/gtxpsmatix.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenlongwang.top/gtedsalxnj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtsygbtgpk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtopemtzjn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtojseoyfi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.smart0.xyz/gtictylkyg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gthgnvbrga.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jiagoushi.top/gtstjbtfrx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yongpay.top/gtziwocyxp.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gttoasjbqs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.snrcjt.cn/gtjzhnfncl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtjohksanz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtnpyoklng.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gthaolpfal.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ppjwa.cn/gtggerepym.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gtdcxkdejt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jiagoushi.top/gtstykgohc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zdqjudy.top/gtukdumeap.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gtjmydkgsj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.c1oappe.top/gtuouxebsu.html

PHP:  file_exists("a.txt");
来源：http://hz.shangyingyoupin.top/gtosthirey.html

JS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtdguemmdm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtdmduyeuu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtzaklchcq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ehwqpu.com/gtpsxrfxfw.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtamdlcdan.html

C#:   File.Exists("a.txt")
来源：http://hz.hammf.cn/gtgerkvuqs.html

[F06] 删除文件
来源：http://hz.xuetiantiany.cn/gtwrzifmgn.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigfzy.top/gtlcwkjgib.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtjqsmxync.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtvdckhkoa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtvtydfktj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtbcialcvw.html

Go:   os.Remove("a.txt")
来源：http://hz.bjfxy.top/gtyebfsnyo.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gthpjwsfhe.html

C#:   File.Delete("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtnxnrfxen.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtbzgotvxs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gterantgib.html


<!-- 参考信息 -->