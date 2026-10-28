代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.316326.xyz/gtfbppljjb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.316326.xyz/gttuydkswp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tian-w.cn/gtrmoqxsyh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zdqjudy.top/gtejjpiuzn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sweek.top/gtodqjejuu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gtmuvmibuh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgfzy.top/gtdrygklpl.html

[D26] 数组转字符串
来源：http://hz.316326.xyz/gtdzcbqcyt.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtwxbbjmuj.html

PHP:  implode(", ", $arr);
来源：http://hz.zhijiandao.cn/gtqjjwxmjs.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtfvdqjnew.html

TS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtykeccuhj.html

Java: String.join(", ", list)
来源：http://hz.sufxvd.cn/gtmutbecll.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtzkvslwue.html

Ruby: arr.join(", ")
来源：http://hz.snrcjt.cn/gtowrkpcmy.html

C#:   string.Join(", ", list)
来源：http://hz.yvedp.cn/gttsmcvuix.html

================================================================================
来源：http://hz.bjfxy.top/gtlnhfqyie.html

E. 字符串处理
来源：http://hz.wangshuangyany.cn/gthlqhmcae.html

================================================================================
来源：http://hz.hysaishi.cn/gtidknrqfj.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gtxgseyehy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangshuangyany.cn/gtuzadcdbn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.316326.xyz/gtwfsjvnkz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gteyfeayrd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pycfn.com/gtmsffabyh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtmrfoysdh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.snrcjt.cn/gthbqhbtdy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daria6918.cn/gtexzyavtp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtutcziyle.html

[E02] 重复字符串
来源：http://hz.yangfankeji.com/gtomjzckaw.html

Py:   "ab" * 3
来源：http://hz.gzhubu.top/gtdsfiunyg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gtbmqtpgng.html

JS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtwnbqgrnt.html

TS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gtirxaiuaz.html

Java: "ab".repeat(3)
来源：http://hz.dashuyun.cn/gtkizpypys.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhongyouzk.top/gtcpeyijzo.html

Ruby: "ab" * 3
来源：http://hz.jinqigfzy.top/gtdtqbyqkp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuxming.cn/gttbqeirnr.html

[E03] 截取子串
来源：http://hz.ehwqpu.com/gtxfojxhaf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nanxinkj.top/gtubnsmrsz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.iojbl.cn/gtixrgsmbz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.bjfxy.top/gtlzvfiswf.html

TS:   s.slice(1, 4)
来源：http://hz.nwbrower.top/gtqczzdgbb.html

Java: s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtxwsdejaz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtdpfuxanw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ydzc1.top/gtxmurjoqc.html

C#:   s.Substring(1, 3)
来源：http://hz.zdqjudy.top/gtzfcmekkq.html

[E04] 查找子串位置
来源：http://hz.yanxiufei.cn/gtbvpyzere.html

Py:   s.find("x");  s.index("x")
来源：http://hz.kuanghao11.cn/gtkllqgggx.html

PHP:  strpos($s, "x");
来源：http://hz.cheryme.top/gtyxgvhncw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtsfuvencj.html

TS:   s.indexOf("x")
来源：http://hz.daxiang520.top/gteqibrksn.html

Java: s.indexOf("x")
来源：http://hz.yj20258888.top/gtrtmfehee.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gtgwcawqpu.html

Ruby: s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtrolgvxsp.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gtqmkiikhk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxuanxn.top/gtqkddfoev.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhongyouzk.top/gterujllnm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hysaishi.cn/gtzczswrnz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtxatwxgsg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hysaishi.cn/gtpubzwvvg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gtfxpfhstf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jqgufenzy.top/gtdpsyusuv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtozmxasfd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fzhhl.top/gtothhqqbj.html

[E06] 替换子串
来源：http://hz.redwolf501.top/gthfhbjcfh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhijiandao.cn/gtloqrpgbw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydjk.org.cn/gtfbzpyyif.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtesiatrkw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtnhepysdj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtfxkapvea.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxuanxn.top/gtwmyszwss.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.pycfn.com/gtpcehtbzh.html

C#:   s.Replace("a", "b")
来源：http://hz.iojbl.cn/gtdnorbtmw.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gtgbwsjgcy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gtzsguzhtv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxinkj.top/gtnszzganz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cqqwz.cn/gtjabuhsgr.html

TS:   s.split(",")
来源：http://hz.yvedp.cn/gtizkpzwdm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtnuewugeh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yueranfly.top/gtfowtwlfp.html

Ruby: s.split(",");  s.split
来源：http://hz.hywenlv.cn/gtotxcdgcc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgufenzy.top/gtqkbwsphs.html

[E08] 数组按分隔符合并
来源：http://hz.xziqi.cn/gtxhropfwl.html

Py:   ",".join(items)
来源：http://hz.jianghu66.top/gtfwcqjvqc.html

PHP:  implode(",", $items);
来源：http://hz.birdmap.top/gthcipmxti.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gtpbdfvmvw.html

TS:   items.join(",")
来源：http://hz.mhx1999.top/gtfmhtziou.html

Java: String.join(",", items)
来源：http://hz.ywan-chungtsiang.top/gtxaqhhqnt.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxuanxn.top/gtscawkjdk.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtgqnpbjmu.html

C#:   string.Join(",", items)
来源：http://hz.birdmap.top/gtileqngnu.html

[E09] 去除所有空白字符
来源：http://hz.aizwys.cn/gtyjkxpgyu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtgeibdlqd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhiwuduotai.top/gtjgbpgfgs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgufenzy.top/gtmjfddmvd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtnrsxlxvz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.andypj.xyz/gtllqtpthf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.mhx1999.top/gtuxviyssl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtznikyaho.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yonumen.top/gtbawgwone.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hywenlv.cn/gtjbhkmfth.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuetiantiany.cn/gtnknxrmtd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuanzhike.top/gtfbbghnrj.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtbnplllru.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtzdwmwjpv.html

Java: String.format("%03d", 7)
来源：http://hz.tanke756.top/gtrmdntogq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinqigfzy.top/gtkgispjbn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtgwpyrsqc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gtmsssinli.html

[E11] 反转字符串
来源：http://hz.jinqigfzy.top/gtwypjaode.html

Py:   s[::-1]
来源：http://hz.nwbrower.top/gtgtkqnslj.html

PHP:  strrev($s);
来源：http://hz.yanxiufei.cn/gtalgojulh.html

JS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtnpezlbmj.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtzdmsdogh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuanzx.com/gtpvxjgmou.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.316326.xyz/gtyqxpkiky.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gtyovhtdnh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtrhkobywk.html

[E12] 统计某字符出现次数
来源：http://hz.hysaishi.cn/gtkozqcjve.html

Py:   s.count("a")
来源：http://hz.xinyue.icu/gtslybhbpc.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtypmwhxdo.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gttozvsupd.html

TS:   s.split("a").length - 1
来源：http://hz.ppjwa.cn/gtfbnokbvf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xylfe.cn/gtxbxevkze.html

Go:   strings.Count(s, "a")
来源：http://hz.wangshuangyany.cn/gtfokwgmzf.html

Ruby: s.count("a")
来源：http://hz.yj20258.top/gtbhenaqfj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hfpthk.cn/gtzucsesup.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtdezofgng.html

Py:   for ch in s: print(ch)
来源：http://hz.ehwqpu.com/gtyxdifvlj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yueranfly.top/gtinsrxsdx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtyugxxjyu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtpdivsoun.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.andypj.xyz/gtevhhszzg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangkeji.top/gtcosdxvck.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cucudq.cn/gtxszpaojq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.quarkkingdee.top/gtdicpoqxa.html

[E14] URL 编码与 Base64
来源：http://hz.shzxlz.cn/gtcwaqnywz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jlsjyb.cn/gtzoaptvdk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigfzy.top/gtckyhkljr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jianghu66.top/gtfqxultpq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yonumen.top/gtdylugzvj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yuanzhike.top/gtnzgxwzte.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cucudq.cn/gtdvwmjogt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangkeji.top/gtzwlmqodx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gttccaojgk.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinghuilouyu.cn/gtvnoxzkgz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj202588.top/gtfiwejuvb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.andypj.xyz/gtntamnrkj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtuzizdorv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.iojbl.cn/gtuhugqbve.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.wangdashe.top/gtnllvpwzw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtjdtslcmg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cqqwz.cn/gtjdyjwqdm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guowangkeji.top/gtpcrbrblj.html

[E16] 数字千分位
来源：http://hz.snrcjt.cn/gtesxjsqca.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigfzy.top/gtsvuymhpu.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtmubpalpf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtyamcjnut.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtubsswkoi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sweek.top/gtzvahnmwx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenlongwang.top/gtzknenymv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sufxvd.cn/gtkwgraqvr.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtlvhvtxqr.html

[E17] 首字母大写
来源：http://hz.yanxiufei.cn/gtddtpamux.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hysaishi.cn/gtqahhgolj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtznoddzlu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtewvvgowk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtzhjfihpx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gtnonqayoj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yangfankeji.com/gtvsfmljzt.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtckgbzopk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtwbosgitl.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gtqoifrryz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtktikysnm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258888.top/gtcrvfrexw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gtlydjaaxx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtvdiiolmz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.aizwys.cn/gtfkwiwfgg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gttoyzbvsn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtdoshvyrg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.316326.xyz/gttforglrs.html

[E19] 多行文本按行拆分
来源：http://hz.tanke756.top/gtnwaxheoo.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtmbdwslck.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtyqsdapqc.html

JS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtwhzxwele.html

TS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtgcuartmd.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtlpiiwvwe.html

Go:   strings.Split(s, "\n")
来源：http://hz.guowangkeji.top/gtxvzslrhc.html

Ruby: s.lines
来源：http://hz.hysaishi.cn/gtwpcgvklh.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gturmsrogu.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gtudvljjev.html

Py:   if not s:
来源：http://hz.hysaishi.cn/gtieusdnqy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnxiangtu.top/gtumjwpuzr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinghuilouyu.cn/gtlmjmvczh.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtkwnwcuum.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtqgbtiknq.html

Go:   if s == "" {}
来源：http://hz.fzhhl.top/gtbvkjrbhn.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtbwtgmjrq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtbueceblv.html

[E21] 超长截断加省略号
来源：http://hz.dashuyun.cn/gtjwubjltv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.mhx1999.top/gtismtwchi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cdnleiting.top/gtzzncyafe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtpadyoazn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtbyjvximg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtpofsimtc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gtcnetxnmo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gaohongyu789.top/gttgdgjvyy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tian-w.cn/gtkldwsekb.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258888.top/gtkgbqbbpj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtkxyaoxsi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtmcwryvdh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtftkwuvew.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtxcjkqlzz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtadnwhrka.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtozqhvqsv.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gtqgoblgjy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gthohzjjwo.html

================================================================================
来源：http://hz.birdmap.top/gttaqtmcbx.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gttlhpidkw.html

================================================================================
来源：http://hz.aizwys.cn/gtzzpckypz.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gtfmmfkjdi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangdashe.top/gtlgnulwjz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtwlarqvbp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtsavxzmrz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenjidiqi.icu/gtybpykxic.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gthxkuuvpk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ydzc1.top/gtfqqmljiq.html

Ruby: File.read("a.txt")
来源：http://hz.yongpay.top/gtvwbvhosd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenlongwang.top/gtfeqffhxj.html

[F02] 逐行读取文件
来源：http://hz.havefunace.top/gtromehvpf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guannengcc.top/gtxeuydjwk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dianchejie.cn/gtiucvfvxx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtcvqnasju.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtzfgkxmgi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtqgzgijbt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gtoypfgrbj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangtech.top/gtuckumvqq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj202588.top/gtomxijafr.html

[F03] 写入文件（覆盖）
来源：http://hz.ybcxt.top/gtfnrvsitr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gttejbmozz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtntbxhsxq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtnyaetzpe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtwihggsgj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuxming.cn/gtilltdgdb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pengpengdd.cyou/gtbqynuayq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gttkuwybpn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtyrnvojxx.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtwusivkvx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gthajcycru.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtmjsypixn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gtgrgqhjkx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yanxiufei.cn/gtvitojbfy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hammf.cn/gtgerakgzm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtwlrvwsto.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.smart0.xyz/gthqazmsdt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtmwpnnmcj.html

[F05] 判断文件或目录是否存在
来源：http://hz.cheryme.top/gtttshycxl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtzvnepqfg.html

PHP:  file_exists("a.txt");
来源：http://hz.xziqi.cn/gtttxbztlf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtbcyufoon.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtppxztnns.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtnvhtagtd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sweek.top/gthoezrpbv.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtlvcoblxf.html

C#:   File.Exists("a.txt")
来源：http://hz.hfpthk.cn/gtcxrxthon.html

[F06] 删除文件
来源：http://hz.snrcjt.cn/gtslwdaxbi.html

Py:   os.remove("a.txt")
来源：http://hz.aizwys.cn/gtngpvwofx.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gtyzfxfhqi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gthgveettm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtccvhzzec.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtgpbqgnad.html

Go:   os.Remove("a.txt")
来源：http://hz.dashuyun.cn/gtucgbwrbp.html

Ruby: File.delete("a.txt")
来源：http://hz.zycfv.cn/gtbzocbnvv.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtyawbhmmx.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtkcsacxnv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgfzy.top/gtfowhteaf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtuquhzcix.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtlgbyusfl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtfvkugvwh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tian-w.cn/gtafprbtzi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.quarkkingdee.top/gtiyswqtct.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtehrslgyg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xuetiantiany.cn/gtbhznodun.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtcouuskxc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtzuhiitfk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gthgqhlgmv.html

JS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtutmynlmz.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtbiijwnip.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gttzuqpnpx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtsysbvoqb.html

Ruby: Dir.children("dir")
来源：http://hz.hammf.cn/gtyzldgmgx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtgadzljht.html

[F09] 获取文件大小
来源：http://hz.birdmap.top/gtudonixwv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtvnhocvaa.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtepdhsbut.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtdbiyudgq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtvlhstcvy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtbuaelfak.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sufxvd.cn/gtppjxlfxn.html

Ruby: File.size("a.txt")
来源：http://hz.zhixingplan.top/gtzwomazmk.html


<!-- 参考信息 -->