代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gttigxejqk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cashguo.top/gtewqgowvu.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtsjblwney.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gtoucglbbi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gthqxwydrx.html

[D24] 字典 / Map 基本操作
来源：http://hz.yongpay.top/gtjkxgsgqq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xylfe.cn/gtabrvuwbq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hywenlv.cn/gtmmsqdkug.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinghuilouyu.cn/gtlkmtkczk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuetiantiany.cn/gtklswevoc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nwbrower.top/gtodnzjlli.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.52xcode.cn/gtezvtvtsm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydjk.org.cn/gtfvabmved.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenzaomai.com/gtgzeytxnm.html

[D25] Set 集合去重与交并差
来源：http://hz.zhongyouzk.top/gtmdnwrelp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtsotabxvg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuetiantiany.cn/gtcgjhytum.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gthzhdxxvs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cucudq.cn/gtjggjykei.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fengsongda.top/gtatusmhjz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtzoqvicmi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shangyingyoupin.top/gtudusgfqq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tanke756.top/gtaggbnldg.html

[D26] 数组转字符串
来源：http://hz.c1oappe.top/gttzozylhm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gotoacloud.top/gtjeonsqkz.html

PHP:  implode(", ", $arr);
来源：http://hz.yuxming.cn/gtfxoobccl.html

JS:   arr.join(", ")
来源：http://hz.shzxlz.cn/gtyjixiova.html

TS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtevgiwddz.html

Java: String.join(", ", list)
来源：http://hz.hammf.cn/gteonyfirt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtcsbvmzrz.html

Ruby: arr.join(", ")
来源：http://hz.hnxiangtu.top/gtcbhvtfmv.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtkzvqmkgx.html

================================================================================
来源：http://hz.zhongyouzk.top/gthwvzcwmt.html

E. 字符串处理
来源：http://hz.zhoulong.xyz/gtkgyhzrcl.html

================================================================================
来源：http://hz.sweek.top/gtjkpjipts.html

[E01] 拼接字符串
来源：http://hz.ppjwa.cn/gtmskxwozj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shangyingyoupin.top/gtaaadmzrd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zycfv.cn/gtulqdlwew.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cheryme.top/gtlngdmfml.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtosgtmsqa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hysaishi.cn/gthycildax.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuanzx.com/gtltjlkufx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.316326.xyz/gtpvyamccs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtbwpjqkuz.html

[E02] 重复字符串
来源：http://hz.jyoumei.cn/gtmvhnskdz.html

Py:   "ab" * 3
来源：http://hz.xylfe.cn/gtarvzpbyy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.mhx1999.top/gtvldquuxs.html

JS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gttxyfuztv.html

TS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gttbeosvxt.html

Java: "ab".repeat(3)
来源：http://hz.nwbrower.top/gtfjlwzbtf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhongyouzk.top/gtftpacxvd.html

Ruby: "ab" * 3
来源：http://hz.havefunace.top/gtzjpboafo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yangfankeji.com/gtqtftgvob.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gtroybddex.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.haohaochexian.top/gtcdwhdcup.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtfyawzppv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fzhhl.top/gtakdwtpol.html

TS:   s.slice(1, 4)
来源：http://hz.hysaishi.cn/gtjeeqjldm.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtujhhcsgf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fzhhl.top/gtfaqcdyvo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zycfv.cn/gtbsohgqdb.html

C#:   s.Substring(1, 3)
来源：http://hz.xingfuxueyuan.xyz/gtutperjao.html

[E04] 查找子串位置
来源：http://hz.iojbl.cn/gtarhkfmvx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cqqwz.cn/gtanzymxok.html

PHP:  strpos($s, "x");
来源：http://hz.aibaodan.cn/gtiombptfg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sweek.top/gttikrrrqq.html

TS:   s.indexOf("x")
来源：http://hz.aizwys.cn/gtnslsrckx.html

Java: s.indexOf("x")
来源：http://hz.hammf.cn/gtlxbiycgc.html

Go:   strings.Index(s, "x")
来源：http://hz.ivvv.top/gtlcohtziy.html

Ruby: s.index("x")
来源：http://hz.haohaochexian.top/gtojomsgnm.html

C#:   s.IndexOf("x")
来源：http://hz.kuanghao11.cn/gtatkzzkun.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yongpay.top/gtcnlituml.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenjidiqi.icu/gtkpuuawhk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.redwolf501.top/gthglhvnza.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.feifeiyinyue.top/gtugxfvvjq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fzhhl.top/gtakjsfkdd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtugtpunin.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnqzz.top/gtwhgdwbco.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.havefunace.top/gtedbeojmw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtgfoyhuov.html

[E06] 替换子串
来源：http://hz.guowangkeji.top/gtmmbafrap.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenlongwang.top/gtkmdvutjt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.quarkkingdee.top/gtgmmyrrto.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtpyuqloby.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtudyvafbz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gttvywjqin.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daria6918.cn/gtfgxdxvig.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtjzbpzvio.html

C#:   s.Replace("a", "b")
来源：http://hz.daria6918.cn/gtqoiiodmh.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gtbvfxrnhz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhijiandao.cn/gtiqjqtcej.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sxryk.cn/gtxslhydvv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gogol.net.cn/gtlhdicufg.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtqlnjbqin.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.dashuyun.cn/gtrpjjgjeh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ehwqpu.com/gtaptezddz.html

Ruby: s.split(",");  s.split
来源：http://hz.daxiang520.top/gtezsaiabo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.kuanghao11.cn/gtbiznkykg.html

[E08] 数组按分隔符合并
来源：http://hz.havefunace.top/gtyeyehurv.html

Py:   ",".join(items)
来源：http://hz.zycfv.cn/gtcxtvhurz.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gtqwvlbccl.html

JS:   items.join(",")
来源：http://hz.c1oappe.top/gtiygmzrix.html

TS:   items.join(",")
来源：http://hz.havefunace.top/gtwhgbkrnh.html

Java: String.join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtgxzqptcd.html

Go:   strings.Join(items, ",")
来源：http://hz.shuidangran.top/gtisrxjpuf.html

Ruby: items.join(",")
来源：http://hz.ydjk.org.cn/gttbyugvdw.html

C#:   string.Join(",", items)
来源：http://hz.jinqigfzy.top/gtvectqxwm.html

[E09] 去除所有空白字符
来源：http://hz.snrcjt.cn/gtejiajcjg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtmnlqphet.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cashguo.top/gthxqhcgce.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgufenzy.top/gtfudkiomr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtkmbxsaip.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtisdohzch.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shzxlz.cn/gtqbbzxtlh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangdashe.top/gtloudtmhy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinghuilouyu.cn/gtnwbxxesx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtmtxbybxl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jqgfzy.top/gtymfqzmia.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gtvkqjvrbr.html

JS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtkeywkwrc.html

TS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtbfvbtyxf.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtjmdwiwcr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuanzx.com/gtnkwmicnw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenzaomai.com/gtwgrezblw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cheryme.top/gteizxcmwj.html

[E11] 反转字符串
来源：http://hz.52xcode.cn/gtdhxyaqin.html

Py:   s[::-1]
来源：http://hz.daria6918.cn/gtjmpzkbop.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtlidubjdj.html

JS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtzrxdbmdc.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtighgyrra.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yueranfly.top/gtmzpksnvm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtpksldogw.html

Ruby: s.reverse
来源：http://hz.zhiwuduotai.top/gtnzaegepb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtabwbnbsi.html

[E12] 统计某字符出现次数
来源：http://hz.gogol.net.cn/gtlxuotmca.html

Py:   s.count("a")
来源：http://hz.yuxming.cn/gtsnlqwhvb.html

PHP:  substr_count($s, "a");
来源：http://hz.xylfe.cn/gttvxgdfaa.html

JS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtzakdolpm.html

TS:   s.split("a").length - 1
来源：http://hz.jinghuilouyu.cn/gtulxeaqqk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.smart0.xyz/gtrmvqojxh.html

Go:   strings.Count(s, "a")
来源：http://hz.guannengcc.top/gtbivjutrf.html

Ruby: s.count("a")
来源：http://hz.gaohongyu789.top/gtaxeahuvz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sxryk.cn/gtrnrtlodp.html

[E13] 逐字符遍历
来源：http://hz.sweek.top/gtvbpwwdhg.html

Py:   for ch in s: print(ch)
来源：http://hz.bjfxy.top/gtpdsrdvwh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xuetiantiany.cn/gtcchysivg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtciusoxcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtgyiuyhfa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shangyingyoupin.top/gtyziibhtr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.svipenyu.cn/gtoakgcqmq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hfpthk.cn/gtgjjdusoq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aizwys.cn/gtopujiycw.html

[E14] URL 编码与 Base64
来源：http://hz.sxryk.cn/gtndyvggee.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jyoumei.cn/gteuyyzmzc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenzaomai.com/gtofludswr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuanzx.com/gtprhnouko.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fengsongda.top/gtwplpbyka.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtazlnahwe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtisigexon.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtioookgba.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258888.top/gtlgamcnmr.html

[E15] HTML 转义 / 反转义
来源：http://hz.yvedp.cn/gtsoxuydgs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gtvqmwbxwx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtbbdimdjr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xziqi.cn/gtrwobisih.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hysaishi.cn/gtecnmuvdm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuanzx.com/gtewkyylee.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtqkdrhbuf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yangfankeji.com/gtmescunge.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtvkolirpe.html

[E16] 数字千分位
来源：http://hz.gaohongyu789.top/gtgtyvkepv.html

Py:   f"{1234567:,}"
来源：http://hz.c1oappe.top/gtvojkghft.html

PHP:  number_format(1234567);
来源：http://hz.haohaochexian.top/gtaxkjdaoe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtqusrffzc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtqxjzqfuw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hongshengwenyu.top/gtyuyfwnve.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigufen.top/gtcjuszlsz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shangyingyoupin.top/gttlpfrlxz.html

C#:   1234567.ToString("N0")
来源：http://hz.snrcjt.cn/gtbmrlmuzb.html

[E17] 首字母大写
来源：http://hz.hongshengwenyu.top/gtawcqhztc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuanzhike.top/gtecelfepb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtrysnfbvd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtlgumdomp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtilywrkdm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtbxdyfvir.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtfzgjooiq.html

Ruby: s.capitalize
来源：http://hz.yuanzhike.top/gtwzmphqkx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtvqkghfot.html

[E18] 模板占位符替换
来源：http://hz.sweek.top/gtvqhqsmvd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.meibo888.top/gtqkjbyvya.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gtyyfffajz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtkmflqnnl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtutmanlup.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.feifeiyinyue.top/gtrpdgcdna.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cashguo.top/gtnoijkzpf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtgfycstrw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.bjfxy.top/gtckcmewks.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtdivlzhqq.html

Py:   s.splitlines()
来源：http://hz.jyoumei.cn/gtlyupoyeq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtkntzvpzh.html

JS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtdvoorxvc.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtiufgmpgx.html

Java: s.lines().toList()
来源：http://hz.aizwys.cn/gtaurmsfxx.html

Go:   strings.Split(s, "\n")
来源：http://hz.zycfv.cn/gtnwainlwn.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtfeeqekqa.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gtausknwld.html

[E20] 判断字符串是否为空
来源：http://hz.svipenyu.cn/gtkujmcndz.html

Py:   if not s:
来源：http://hz.shuidangran.top/gtqgvuazhl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.smart0.xyz/gtcbbhkrwa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sxryk.cn/gtkkpczpsi.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtujqtatvy.html

Java: if (s.isEmpty()) {}
来源：http://hz.sxryk.cn/gtklucokwv.html

Go:   if s == "" {}
来源：http://hz.zhaomingkeji.xyz/gtzmebxihq.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtdmjdqxdy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtfbewiepj.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtaweknsur.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtwkqfxaqp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtqddlbili.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtoubpcjff.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtclekeuwe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gthzpnormj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtzmwaxzix.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtydgnakht.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtaqnmymfx.html

[E22] 字节长度与字符长度
来源：http://hz.hysaishi.cn/gtkfpbtvvm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtknkhxnko.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gteggezgcy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gthxjzvqiw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtpozxkajp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jqgufenzy.top/gtetfygwfu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtrmvjfbyl.html

Ruby: s.bytesize;  s.length
来源：http://hz.guowangkeji.top/gtisfhiokv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtguwxbmwx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtjyvwkyar.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtkvcruycs.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvzrjihir.html

[F01] 读取整个文件
来源：http://hz.sysykeji.top/gtxlzwvyym.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtlebkunpp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuxming.cn/gtsefnsrap.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtshrjsqyl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gaohongyu789.top/gtjntyvtfr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtewneursl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jiagoushi.top/gtcpsyscdb.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtokiyjdkm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtfuevekrf.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtqwrhcazd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yueranfly.top/gtadfyfdlb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.vqdsnc.cn/gthlqirhdo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtcyejzipd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtbtpcnoep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtzpxodcpd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtgsjlaznz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gtsxkwiubo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gttqnfrcnr.html

[F03] 写入文件（覆盖）
来源：http://hz.birdmap.top/gtirukidzy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtwsaysgnd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtpvdzfjky.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtwfepfiss.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gthcibdxcx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sysykeji.top/gtvigbkcur.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinghuilouyu.cn/gtldapznoq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.andypj.xyz/gtzxwauvbg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtswgzjjiq.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gthognhxtv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258888.top/gtfopauzjx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuanzx.com/gtiyrstprr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gthgikrhvc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtqjubkhvk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zdqjudy.top/gttnycrhkz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shangyingyoupin.top/gtwuzizjrm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gterlrvjhy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cqqwz.cn/gtnucttxlx.html

[F05] 判断文件或目录是否存在
来源：http://hz.gogol.net.cn/gtefvduzkd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daria6918.cn/gtcudrqvaq.html

PHP:  file_exists("a.txt");
来源：http://hz.bjfxy.top/gtjvbaodql.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtjznuxiqa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gttwgcjchf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtojycjxrz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gttmolxzdc.html

Ruby: File.exist?("a.txt")
来源：http://hz.cdnleiting.top/gtkdsrdbsw.html

C#:   File.Exists("a.txt")
来源：http://hz.daxiang520.top/gtfnocjtgo.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtrvorstqc.html

Py:   os.remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtmblibguw.html

PHP:  unlink("a.txt");
来源：http://hz.aizwys.cn/gtrmsdefsl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtvxzeoemq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtbebflqsm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtktpnwhjs.html

Go:   os.Remove("a.txt")
来源：http://hz.zhongyouzk.top/gthhwlbzts.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtfveixuux.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtyuxkdmoz.html

[F07] 创建目录（含多级）
来源：http://hz.nanxinkj.top/gtavekoocu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtsnmftxea.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtrbtvyjmd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtytcamuxe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtiazncpcd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtgtjlsvbd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.52xcode.cn/gtftokxwfy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258.top/gtthwfwhey.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cheryme.top/gthjxeqmhc.html

[F08] 遍历目录
来源：http://hz.cashguo.top/gtwkehicuf.html


<!-- 参考信息 -->