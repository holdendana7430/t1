代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtjielwwjm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtzcasgswp.html

Go:   // 手写循环
来源：http://hz.dianchejie.cn/gtvcltlmza.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuetiantiany.cn/gtskkbqyzp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigfzy.top/gtleucqpuu.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtjpqbkcpl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sysykeji.top/gtxplnloag.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yanxiufei.cn/gtemeiquey.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtkgyhjewx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cheryme.top/gtmwuuehrh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtmksbsuxe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guannengcc.top/gtbzdsklgc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guannengcc.top/gtdnrvtdfk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gttbhhitjb.html

[D25] Set 集合去重与交并差
来源：http://hz.xuetiantiany.cn/gtfhxkbkjm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxinkj.top/gtwdhmxjfp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shangyingyoupin.top/gtxdgjxewo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jianghu66.top/gtnbbhsiaj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tanke756.top/gtrhcbhfup.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dianchejie.cn/gtedrsgqfb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gtjrogrbnt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtrlbbbiwo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangtech.top/gtoupnahyj.html

[D26] 数组转字符串
来源：http://hz.jinqigfzy.top/gtazggujbx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtxebbbhcs.html

PHP:  implode(", ", $arr);
来源：http://hz.xinyue.icu/gtsuqpwhxr.html

JS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtefxkdfyh.html

TS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtessdbyrc.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gtkmzzhiti.html

Go:   strings.Join(strs, ", ")
来源：http://hz.andypj.xyz/gtpejcntms.html

Ruby: arr.join(", ")
来源：http://hz.daxiang520.top/gtmitxeryj.html

C#:   string.Join(", ", list)
来源：http://hz.9152youxi.cn/gtnoxtyxis.html

================================================================================
来源：http://hz.zhixingplan.top/gtrqmfvvdf.html

E. 字符串处理
来源：http://hz.52xcode.cn/gtoyzuvimo.html

================================================================================
来源：http://hz.shzxlz.cn/gtxbdzmsdu.html

[E01] 拼接字符串
来源：http://hz.hfpthk.cn/gtrqzrpvwr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daria6918.cn/gtpgiobxtp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtyybizahr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtfupqaipv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtqfuztevl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sysykeji.top/gtoiohnlnd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.guowangkeji.top/gtwiqikvzp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yonumen.top/gtekjyphrx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtvwmlzfmt.html

[E02] 重复字符串
来源：http://hz.ybcxt.top/gtvqrbehbs.html

Py:   "ab" * 3
来源：http://hz.ivvv.top/gtzaiagpyu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gtaqnlwwye.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtcnndofio.html

TS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gttyjszoej.html

Java: "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtwnnrhvcv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.haohaochexian.top/gtcdtpfapy.html

Ruby: "ab" * 3
来源：http://hz.zhijiandao.cn/gtywxhkzjc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daxiang520.top/gtlgfflkjg.html

[E03] 截取子串
来源：http://hz.zhengqikj.top/gtfcbshojc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.9152youxi.cn/gtghcpgphb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tianlin.xyz/gtebouvqxa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yongpay.top/gtfhixpbsj.html

TS:   s.slice(1, 4)
来源：http://hz.yueranfly.top/gtnldehzmv.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtlcgphujh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.birdmap.top/gtnmxlalsl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhiwuduotai.top/gtcrkvzfqo.html

C#:   s.Substring(1, 3)
来源：http://hz.hammf.cn/gtpochsrdp.html

[E04] 查找子串位置
来源：http://hz.c1oappe.top/gtffyewqch.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xuetiantiany.cn/gtxzqxacke.html

PHP:  strpos($s, "x");
来源：http://hz.fzhhl.top/gtnztvkdyn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yanxiufei.cn/gtzxiolyqp.html

TS:   s.indexOf("x")
来源：http://hz.guowangkeji.top/gtcrjfgguf.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtbqtwgbnl.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gtksyqlsgm.html

Ruby: s.index("x")
来源：http://hz.dashuyun.cn/gtibydwnkm.html

C#:   s.IndexOf("x")
来源：http://hz.pycfn.com/gtjzknmjzo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.feifeiyinyue.top/gtevnvynex.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tanke756.top/gtdcuhgskh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgufenzy.top/gtznlrvwto.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tian-w.cn/gthpkexsbj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.birdmap.top/gtzpdebcag.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtkictjeak.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gtfmfanofy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ywan-chungtsiang.top/gtleivurij.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxinkj.top/gtlcerfmhi.html

[E06] 替换子串
来源：http://hz.jianghu66.top/gtmbxkakbf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nwbrower.top/gtbgqgtspm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.daxiang520.top/gtcmhmorcl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtxihvtufe.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtzajfmvki.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtkjeviocw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtsnyzxdaf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aibaodan.cn/gticpmleap.html

C#:   s.Replace("a", "b")
来源：http://hz.jlsjyb.cn/gtradkdzrf.html

[E07] 按分隔符拆分
来源：http://hz.cashguo.top/gtnosqshur.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigfzy.top/gtvvjcbnrq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gtnoprdxgz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinqigfzy.top/gtxhpqzlan.html

TS:   s.split(",")
来源：http://hz.hammf.cn/gtvlczwfcc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.birdmap.top/gtxwgghtlh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gttvaspcqk.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtcaydosvj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jyoumei.cn/gtswwektba.html

[E08] 数组按分隔符合并
来源：http://hz.sufxvd.cn/gtsqdzbows.html

Py:   ",".join(items)
来源：http://hz.chenlongwang.top/gtftalvxyz.html

PHP:  implode(",", $items);
来源：http://hz.daria6918.cn/gteuywqbdw.html

JS:   items.join(",")
来源：http://hz.hfpthk.cn/gticdgkbif.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtdyqenqje.html

Java: String.join(",", items)
来源：http://hz.dashuyun.cn/gtjmyxelvw.html

Go:   strings.Join(items, ",")
来源：http://hz.cucudq.cn/gtkrdkdrhj.html

Ruby: items.join(",")
来源：http://hz.snrcjt.cn/gtzrkeskdf.html

C#:   string.Join(",", items)
来源：http://hz.zhongyouzk.top/gtihfnshbc.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtmbpkdyea.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yangfankeji.com/gtrymxearh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhengqikj.top/gttpxdgbee.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hnqzz.top/gtktdwdhfd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtlaaddsbz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cashguo.top/gtsvboxfmw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtwkvkwvgk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtqhryqhki.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuanzx.com/gteranwxou.html

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtrmtboaij.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtvqdwywrn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.0kj1m.cn/gtbgprmeaq.html

JS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtmyapnrwt.html

TS:   "7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtkhygvmjb.html

Java: String.format("%03d", 7)
来源：http://hz.zycfv.cn/gtjwppdskm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhijiandao.cn/gtvrelgues.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gtbiigupwa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnqzz.top/gtocnuirpd.html

[E11] 反转字符串
来源：http://hz.wangshuangyany.cn/gtaggagwom.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gttfbudmgv.html

PHP:  strrev($s);
来源：http://hz.0kj1m.cn/gtnlonkzbc.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtxvljpvsg.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtuieuuznw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhijiandao.cn/gtrcoyfakz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.vqdsnc.cn/gttrqraaqx.html

Ruby: s.reverse
来源：http://hz.ybcxt.top/gtuegunesm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtdhzcgbdj.html

[E12] 统计某字符出现次数
来源：http://hz.nanxuanxn.top/gtyxjsafhu.html

Py:   s.count("a")
来源：http://hz.aibaodan.cn/gtlptqmeny.html

PHP:  substr_count($s, "a");
来源：http://hz.nwbrower.top/gtgzfumcpn.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtccthqiak.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtlnrllwyx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dashuyun.cn/gtsewjdqot.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtugrdjgns.html

Ruby: s.count("a")
来源：http://hz.hnxiangtu.top/gtefdzohai.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jiagoushi.top/gtdvbhtfhg.html

[E13] 逐字符遍历
来源：http://hz.shzxlz.cn/gtapyqouyx.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtkfwxpunv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gttwmaiqla.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtbppijswe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtgijqkmcn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigufen.top/gtaoeghxvt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hongshengwenyu.top/gtrrzvjwxi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dianchejie.cn/gtfcmnwsbw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtumvxvqow.html

[E14] URL 编码与 Base64
来源：http://hz.iojbl.cn/gtefphmheg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhaomingkeji.xyz/gtoszedkyo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jlsjyb.cn/gtdddygwvb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cqqwz.cn/gtrhpwxaqz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gogol.net.cn/gtbkfwfync.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtwnbismuy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gtpmdhfvwp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yanxiufei.cn/gtbdkjkeop.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gaohongyu789.top/gtthjynops.html

[E15] HTML 转义 / 反转义
来源：http://hz.yongpay.top/gtpsfzffer.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yonumen.top/gtuveologf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhongyouzk.top/gtayijflpy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.quarkkingdee.top/gtxjohwico.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtpkksoeoz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtbccvwgbh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shzxlz.cn/gthejuyers.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinyuanbaomall.cn/gtjrdaigyg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sxryk.cn/gtqhuuwimt.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtixwxjoqs.html

Py:   f"{1234567:,}"
来源：http://hz.guowangkeji.top/gtlyeudmlc.html

PHP:  number_format(1234567);
来源：http://hz.fzhhl.top/gtghikwwuk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtqmjsblsc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtokqzvmqq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtqlqycybo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtteaottze.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangkeji.top/gtpukwdtdr.html

C#:   1234567.ToString("N0")
来源：http://hz.cashguo.top/gtdsekergm.html

[E17] 首字母大写
来源：http://hz.snrcjt.cn/gtmsrulkyr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shzxlz.cn/gtqactznkr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sufxvd.cn/gtetfuczlx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtzfmjvjsm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtkyeuwdyn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sxryk.cn/gtkcsbszgu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gaohongyu789.top/gteveotlmj.html

Ruby: s.capitalize
来源：http://hz.cucudq.cn/gtvoiqptod.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gtbmjebchh.html

[E18] 模板占位符替换
来源：http://hz.dianchejie.cn/gtledohtax.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtxpcwpjpz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gzhubu.top/gtqlzlluew.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtbwdpyuhf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtiyyidfsp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.0kj1m.cn/gtzdltxmeq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.svipenyu.cn/gtdejlsoty.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gtqywpnjal.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuxming.cn/gtjclucenb.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtucdygwqv.html

Py:   s.splitlines()
来源：http://hz.yongpay.top/gtxenenftg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.smart0.xyz/gtpiqorhba.html

JS:   s.split(/\r?\n/)
来源：http://hz.ehwqpu.com/gttsrphffu.html

TS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gthckfwlqs.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtlkgsymbv.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtlwnqnnlg.html

Ruby: s.lines
来源：http://hz.wangshuangyany.cn/gtihlfzhpc.html

C#:   s.Split('\n')
来源：http://hz.xylfe.cn/gteevyospg.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gthfznvckz.html

Py:   if not s:
来源：http://hz.svipenyu.cn/gthlshakpd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pengpengdd.cyou/gtpzlxcthv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xinyue.icu/gtllkyyhdr.html

TS:   if (s === "") {}
来源：http://hz.gotoacloud.top/gtihrqlctq.html

Java: if (s.isEmpty()) {}
来源：http://hz.jqgfzy.top/gtffsocvpk.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtnoolynrz.html

Ruby: if s.empty?
来源：http://hz.svipenyu.cn/gtkfylbjes.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhijiandao.cn/gtozlcwpkj.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtrkzahxpb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.bjfxy.top/gtvgfqfcnr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.andypj.xyz/gtxdfmjbrs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtiixywvdu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtqxafdowq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtnrwwwajv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yueranfly.top/gtfgryxnte.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtxhqujjgl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtaqjghebh.html

[E22] 字节长度与字符长度
来源：http://hz.aibaodan.cn/gtuxqisqgg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shuidangran.top/gtyepxcfad.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtiuektanw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtnohnotdm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtluxxdoll.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtztjmrvbq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gthjhjerik.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gtmcliuizi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgufenzy.top/gtapoonosv.html

================================================================================
来源：http://hz.ybcxt.top/gtpgssodfq.html

F. 文件与目录
来源：http://hz.jqgufenzy.top/gtuydtcwgm.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqqnttkbf.html

[F01] 读取整个文件
来源：http://hz.bjfxy.top/gtbctihngf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtozsckhnt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cashguo.top/gtzmbcywaf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtpzytltnr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtlvovbygq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtlzhmggxf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.kuanghao11.cn/gtpittgxac.html

Ruby: File.read("a.txt")
来源：http://hz.havefunace.top/gtotsyitbg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gteltsfpbp.html

[F02] 逐行读取文件
来源：http://hz.shuidangran.top/gtfkfepluk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtbdzdpysp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shzxlz.cn/gtuongczxp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtrcblaubg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtsoxhzzwy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtvppkhaei.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cheryme.top/gtzvnqavdj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtdbniucym.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.meibo888.top/gtzmhsxsxn.html

[F03] 写入文件（覆盖）
来源：http://hz.zhongyouzk.top/gtgnrjllzo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cucudq.cn/gtcosrzdzb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtujramqsz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gteqlzisii.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtdlmoxarr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgfzy.top/gtzefxiiqf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtcpujoeps.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gttjghnqsz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtwpqacldx.html

[F04] 追加写入文件
来源：http://hz.gogol.net.cn/gtghbuccxf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.havefunace.top/gtugvxenha.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cqqwz.cn/gtbworfamj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtkoonkumh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtunobazcd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.0kj1m.cn/gtsgkcffkm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fengsongda.top/gthkihmspc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cashguo.top/gtcvmqtwqe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yanxiufei.cn/gtvlhkgavy.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gtzgpswvck.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtegktttim.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtkangdgui.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtzktyezfl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtbfflknre.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtpgpfsmay.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtiofhcwwl.html

Ruby: File.exist?("a.txt")
来源：http://hz.shzxlz.cn/gtjcuetjof.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtvmpewutl.html

[F06] 删除文件
来源：http://hz.nwbrower.top/gtrwkkxmym.html

Py:   os.remove("a.txt")
来源：http://hz.mhx1999.top/gtqwqjubjl.html

PHP:  unlink("a.txt");
来源：http://hz.meibo888.top/gtkoknzyhe.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtqifvgzog.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.andypj.xyz/gtafswlokw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtcumgpadk.html

Go:   os.Remove("a.txt")
来源：http://hz.cheryme.top/gtrflaezhg.html

Ruby: File.delete("a.txt")
来源：http://hz.jlsjyb.cn/gtrcjvpauu.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangtech.top/gtzsbbgcnq.html

[F07] 创建目录（含多级）
来源：http://hz.tanke756.top/gtklgsbddj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtcajcpcqn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtgicqxdwy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtraykathk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtfratsmke.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jlsjyb.cn/gtedqryrtg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtrggrmefd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pengpengdd.cyou/gtpoyhxbmd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gthmayiuhs.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtsztrmkec.html


<!-- 参考信息 -->