代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.kuanghao11.cn/gtmvqqcrkm.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj202588.top/gtiqgcjsqh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtoagdjqkb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ppjwa.cn/gtmkljrnln.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xingfuxueyuan.xyz/gtgqvttolm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cheryme.top/gtiydbxmvc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xziqi.cn/gtuhpapgos.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.svipenyu.cn/gtncpousxj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhixingplan.top/gtbnmrrqff.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtcijewgdz.html

[D25] Set 集合去重与交并差
来源：http://hz.sysykeji.top/gtmrzvkoby.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangtech.top/gtxqxgnwzn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gttqjfuskw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ydzc1.top/gtbpgzqolj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sxryk.cn/gteleqknpb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinyuanbaomall.cn/gtidlebcmp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yongpay.top/gtcdcslywg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xziqi.cn/gtjycmiwne.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gteiylitiy.html

[D26] 数组转字符串
来源：http://hz.gzhubu.top/gtrwffcxtn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gtnvftzpmf.html

PHP:  implode(", ", $arr);
来源：http://hz.xuetiantiany.cn/gtvvqvaemz.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtlryjauyw.html

TS:   arr.join(", ")
来源：http://hz.pycfn.com/gtfxxognti.html

Java: String.join(", ", list)
来源：http://hz.guannengcc.top/gtceflhasj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gthltuzngv.html

Ruby: arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtulbacfum.html

C#:   string.Join(", ", list)
来源：http://hz.ydzc1.top/gtrqmsyhzj.html

================================================================================
来源：http://hz.xylfe.cn/gtzphcdlok.html

E. 字符串处理
来源：http://hz.birdmap.top/gtwwrneqby.html

================================================================================
来源：http://hz.xinyue.icu/gtyyojalbz.html

[E01] 拼接字符串
来源：http://hz.feifeiyinyue.top/gtmkpjnzdt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtgacfdjpp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tanke756.top/gtrqfzxblf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtraiwrpbu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtgkkxerla.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fengsongda.top/gthhhlxdxh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinghuilouyu.cn/gttlvolgze.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shzxlz.cn/gtdmpaodlv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtmdpvjpch.html

[E02] 重复字符串
来源：http://hz.yuxming.cn/gthaxgxqrv.html

Py:   "ab" * 3
来源：http://hz.hfpthk.cn/gtyngldgpt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhengqikj.top/gttcijtsvb.html

JS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtalnjfdzc.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtwgknijtq.html

Java: "ab".repeat(3)
来源：http://hz.daria6918.cn/gtqofsownm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cheryme.top/gtujpxakca.html

Ruby: "ab" * 3
来源：http://hz.birdmap.top/gtkupfzzax.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.daxiang520.top/gtzqtgxgcu.html

[E03] 截取子串
来源：http://hz.yongpay.top/gtgkfrtdsg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenjidiqi.icu/gtdsxebsbw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.haohaochexian.top/gttqiqyzvj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtsqbjsgmi.html

TS:   s.slice(1, 4)
来源：http://hz.guannengcc.top/gtytjghvog.html

Java: s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gtjzbwhyat.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gtzblzaxre.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tianlin.xyz/gtiwgqnwqa.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gtufaedolg.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtqncqxdkj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gaohongyu789.top/gtavmnojzi.html

PHP:  strpos($s, "x");
来源：http://hz.xuanzx.com/gtlsrsqgij.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ivvv.top/gtmyomzdjx.html

TS:   s.indexOf("x")
来源：http://hz.birdmap.top/gtlhbaguzo.html

Java: s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtotazlhee.html

Go:   strings.Index(s, "x")
来源：http://hz.gogol.net.cn/gtkipelnni.html

Ruby: s.index("x")
来源：http://hz.yongpay.top/gthozbobvv.html

C#:   s.IndexOf("x")
来源：http://hz.yanxiufei.cn/gtmjkmuaqn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.iojbl.cn/gtyukandvi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtnawucpzn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgfzy.top/gtsczdwfgw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtbrjpvhbt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cqqwz.cn/gtrhlmwnhq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtqniyodpb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.svipenyu.cn/gtjsjnjaam.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yvedp.cn/gtgkfickmf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.haohaochexian.top/gtlpqsngdu.html

[E06] 替换子串
来源：http://hz.tianlin.xyz/gtumhmxbne.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yvedp.cn/gteyrwypbw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jyoumei.cn/gtvfipimde.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtanebqwxl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtwafjmbav.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtnkuqtrkt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guowangkeji.top/gtsyzlextd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cqqwz.cn/gtkmvuidck.html

C#:   s.Replace("a", "b")
来源：http://hz.yongpay.top/gthabtedeu.html

[E07] 按分隔符拆分
来源：http://hz.yonumen.top/gtkdxbhdwt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangshuangyany.cn/gtyefgxsdh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.mhx1999.top/gtrxxvflwp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtjacqtblf.html

TS:   s.split(",")
来源：http://hz.zhongyouzk.top/gtdgybvlod.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.redwolf501.top/gtdxasdmdd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fengsongda.top/gtibfomebt.html

Ruby: s.split(",");  s.split
来源：http://hz.ybcxt.top/gtzrignkfm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zdqjudy.top/gtazcbenmz.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtttoiyjzh.html

Py:   ",".join(items)
来源：http://hz.sweek.top/gtfgetexhl.html

PHP:  implode(",", $items);
来源：http://hz.xingfuxueyuan.xyz/gtjfqbdkic.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gthzslhdyn.html

TS:   items.join(",")
来源：http://hz.cdnleiting.top/gtkkmxxthp.html

Java: String.join(",", items)
来源：http://hz.tanke756.top/gtshumenvk.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigfzy.top/gtqxouzdml.html

Ruby: items.join(",")
来源：http://hz.yj202588.top/gtlyddxcfh.html

C#:   string.Join(",", items)
来源：http://hz.gaohongyu789.top/gtumlvarmg.html

[E09] 去除所有空白字符
来源：http://hz.meibo888.top/gtdskfutqo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gaohongyu789.top/gtgxqjqtvm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jianghu66.top/gttbmddvtm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtwqpycdtv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtmsyrclos.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shzxlz.cn/gthfurdvfh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.quarkkingdee.top/gtnrqmtidq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zycfv.cn/gtejptsfir.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sxryk.cn/gtjbvqdzjw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gogol.net.cn/gtchydznpb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuanzhike.top/gtdstglcuo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dashuyun.cn/gtzgwfldgl.html

JS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtfczbwhrm.html

TS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gthkzilcua.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtmuyczvlh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtfwulynsq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gzhubu.top/gthzhivyky.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daria6918.cn/gtorxjbdeq.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtggjbiubi.html

Py:   s[::-1]
来源：http://hz.dianchejie.cn/gtsuvlkcuk.html

PHP:  strrev($s);
来源：http://hz.hnxiangtu.top/gtpbmrzsoa.html

JS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtpqcchasc.html

TS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtpvzzfaxw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtcksihwid.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.quarkkingdee.top/gtdgswrxip.html

Ruby: s.reverse
来源：http://hz.fengsongda.top/gtbflssbrw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtbudtykmz.html

[E12] 统计某字符出现次数
来源：http://hz.wangdashe.top/gtvgtkfddy.html

Py:   s.count("a")
来源：http://hz.ivvv.top/gtsrrkphuj.html

PHP:  substr_count($s, "a");
来源：http://hz.zhongyouzk.top/gtumfivdvw.html

JS:   s.split("a").length - 1
来源：http://hz.xuetiantiany.cn/gtmgebnlfu.html

TS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtacruzmng.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gtapnjsyfg.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gtwbqcbyki.html

Ruby: s.count("a")
来源：http://hz.nwbrower.top/gteyikuyqr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtvudzgrer.html

[E13] 逐字符遍历
来源：http://hz.gogol.net.cn/gteemuhzkq.html

Py:   for ch in s: print(ch)
来源：http://hz.chenzaomai.com/gtrsivwnan.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtbthocnmk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtjfguvyhu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtqzbvskob.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtkdsvvetk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhixingplan.top/gtuyksgixn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.iojbl.cn/gtwuabdrvr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtcklcnjcl.html

[E14] URL 编码与 Base64
来源：http://hz.yj202588.top/gtgwzuglbl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ywan-chungtsiang.top/gtrkjtadfv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jlsjyb.cn/gtwenqkfka.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.kuanghao11.cn/gtcnnqbaml.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhijiandao.cn/gtlherdrdl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtgnsbmeat.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yonumen.top/gtatqajtuj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sxryk.cn/gtztecadnx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.316326.xyz/gtmrnvzvbv.html

[E15] HTML 转义 / 反转义
来源：http://hz.yvedp.cn/gtolkzexlp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xylfe.cn/gtqebvbcfk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhijiandao.cn/gtjibgupon.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cucudq.cn/gtjdxbqgke.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.bjfxy.top/gtcpjpcthw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtpbshgkbt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuetiantiany.cn/gtimamxgch.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.9152youxi.cn/gtvctfhulr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.c1oappe.top/gtqduzbcey.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtzwypwtfp.html

Py:   f"{1234567:,}"
来源：http://hz.jyoumei.cn/gtccosjoyz.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtavskgiof.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtgjkcnbak.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtphsqjdxs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xylfe.cn/gtdhgflyue.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.9152youxi.cn/gtptprhpwl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gtqacakeqh.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtbbxnpkjr.html

[E17] 首字母大写
来源：http://hz.316326.xyz/gthumrvhud.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangdashe.top/gtdtxzcuey.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daxiang520.top/gtbcmagsak.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtbjbmwuca.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fengsongda.top/gtaiwoavxf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gttenwoptf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fzhhl.top/gtetqjeusi.html

Ruby: s.capitalize
来源：http://hz.pengpengdd.cyou/gtkvoyigbe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.bjfxy.top/gtfxmvxqjw.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gtlhgiyjlt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuxming.cn/gtlfeoyrcn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtragzmmiz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtfnnormrs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtzuvpiqrk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtkpmlflsd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtcihcntbd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tian-w.cn/gtqnakkebo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtrahmoaqz.html

[E19] 多行文本按行拆分
来源：http://hz.yuxming.cn/gtjtlfhbzi.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtyqljeocw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aizwys.cn/gthldinlmm.html

JS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtdefwpubc.html

TS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtmrhbirlv.html

Java: s.lines().toList()
来源：http://hz.feifeiyinyue.top/gtxgwvtgxt.html

Go:   strings.Split(s, "\n")
来源：http://hz.xingfuxueyuan.xyz/gtqyloqtsu.html

Ruby: s.lines
来源：http://hz.chenjidiqi.icu/gtphdiuzmh.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtiiiqrtrf.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtkgtjwrup.html

Py:   if not s:
来源：http://hz.pengpengdd.cyou/gtmsuzcqnw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhixingplan.top/gtumvamwin.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.mhx1999.top/gthsrahobn.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtxaswmanf.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtniwqzxel.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtvllbiprk.html

Ruby: if s.empty?
来源：http://hz.pycfn.com/gtiqndpdia.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gtmofavxed.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtlvcruvzg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtjfirqvsd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gttwjdxbto.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gttosywypj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtpqbffzlr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtkgvajlie.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydjk.org.cn/gtjcysztcg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nwbrower.top/gtvsssbcke.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gttzxfgwuj.html

[E22] 字节长度与字符长度
来源：http://hz.ivvv.top/gtnrpuvqbc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtqzhensbk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nwbrower.top/gtcpxvhthl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gttwmiwden.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtaculihse.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinyuanbaomall.cn/gtfbwtkxws.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtujvvbpyv.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenjidiqi.icu/gtdkspnntd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gtkgkwqtss.html

================================================================================
来源：http://hz.fzhhl.top/gtssufclpy.html

F. 文件与目录
来源：http://hz.zdqjudy.top/gtwonqavat.html

================================================================================
来源：http://hz.chenlongwang.top/gtvmxgeqwl.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtyfaaenmo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgfzy.top/gtpzdcenjx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gtvmbtcupu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.redwolf501.top/gtqrzxstuj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtmuvworxc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtacahatba.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ivvv.top/gtynfgtqxy.html

Ruby: File.read("a.txt")
来源：http://hz.havefunace.top/gtydluybri.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tianlin.xyz/gtqjfnypqt.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gtjlhmiksb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gtmksmpgzp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhaomingkeji.xyz/gtdsyqilyy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtnksqplrq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gthumxwujk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtroaqhmuf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtzllibojw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shuidangran.top/gtljnlnkdk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.9152youxi.cn/gtdbftavgu.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtpptplkgl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigfzy.top/gtujzgygql.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yvedp.cn/gtkwaodrdi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtldskguzw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtykoanjih.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnqzz.top/gtfyczvgch.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtwfvrwipm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnxiangtu.top/gtgyexlzfy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtmymwfgho.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtphajfswk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtawetkhzv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shuidangran.top/gtnxdgxhwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtddcfmhuf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtuetyotmx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258.top/gtovkuzfwy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtnrgxpgio.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtsdhckqoc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtiiwhcxxc.html

[F05] 判断文件或目录是否存在
来源：http://hz.0kj1m.cn/gtgaqiumoi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.smart0.xyz/gtzgqicvqi.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gttrwmxycw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gthziljqjk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtafwrshbe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtvmatffvq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtpncguysr.html

Ruby: File.exist?("a.txt")
来源：http://hz.jqgfzy.top/gtdjykgqpa.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtopazwquy.html

[F06] 删除文件
来源：http://hz.daria6918.cn/gtmgdsdifn.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gthgtvrtwm.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangtech.top/gtacmyoglz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtzijlpojh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gttimsdnqm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtnairqraa.html

Go:   os.Remove("a.txt")
来源：http://hz.yj20258888.top/gtvmoqoijm.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtyanmubso.html

C#:   File.Delete("a.txt");
来源：http://hz.hnxiangtu.top/gtxnruaopa.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtacdqirjp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gtaczuwxpp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gtevmoehxj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtqpxqqlcy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtbmbsqnit.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxinkj.top/gtqccdpncd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gtcuxdrcvj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtfftimthj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.smart0.xyz/gtzfdjoeow.html

[F08] 遍历目录
来源：http://hz.birdmap.top/gtxvvikwaf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gthglraacw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yangfankeji.com/gtrtwajjsx.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtkbdvlnnl.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtukzhqizv.html


<!-- 参考信息 -->