代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtjbguiiel.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shzxlz.cn/gtntbouthw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.quarkkingdee.top/gtedopsfwb.html

C#:   new List<int>(list);
来源：http://hz.chenlongwang.top/gtkzvljdnk.html

[D23] reduce 累积计算
来源：http://hz.ybcxt.top/gtxmpopirg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shuidangran.top/gtemkoytcw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtmuiybsif.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtisneqdig.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtgnzhofdb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gtkylqujov.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtqpcfjart.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangtech.top/gtofmvljjo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hfpthk.cn/gtncvcgeej.html

[D24] 字典 / Map 基本操作
来源：http://hz.fzhhl.top/gtjvqhvkxi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtxiifikej.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtvmwdswyi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sweek.top/gttzewbvla.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj202588.top/gtvoapbvgf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtzlrrnmav.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cqqwz.cn/gtdbmjoliz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zdqjudy.top/gtsigjjshp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhongyouzk.top/gtvsmuywqw.html

[D25] Set 集合去重与交并差
来源：http://hz.hfpthk.cn/gtnefvpkko.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.c1oappe.top/gthrgcsxto.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtqwuzocps.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nwbrower.top/gtlqlpbzgf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gtkjjuhnye.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj20258888.top/gtqyoyxprb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nwbrower.top/gtaamshbwb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.andypj.xyz/gtfvcegdtk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xinyue.icu/gtcagymflu.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtqpwlbqzp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hywenlv.cn/gtsqahtixk.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtmdvwmxhp.html

JS:   arr.join(", ")
来源：http://hz.316326.xyz/gtspqyaxyg.html

TS:   arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtehqoraic.html

Java: String.join(", ", list)
来源：http://hz.nwbrower.top/gtcnkrstjo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sysykeji.top/gtojohangv.html

Ruby: arr.join(", ")
来源：http://hz.smart0.xyz/gtkzsmdtea.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtavkkxxdy.html

================================================================================
来源：http://hz.xinyue.icu/gtlymfdrwh.html

E. 字符串处理
来源：http://hz.tian-w.cn/gthlcgqgxq.html

================================================================================
来源：http://hz.meibo888.top/gtrwhvblha.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtsxdfnekw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgufenzy.top/gtvgbjtlex.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhongyouzk.top/gthmmxlasu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtbyglweis.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gteiwhwnao.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuanzhike.top/gtcscvhcro.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtqxftansq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtzjflcdbe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxinkj.top/gtuufzkkdw.html

[E02] 重复字符串
来源：http://hz.meibo888.top/gtwtutunch.html

Py:   "ab" * 3
来源：http://hz.sufxvd.cn/gtwuchqkew.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtaielinrf.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtryysgsiq.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gthtsmnamd.html

Java: "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtbilxahln.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gaohongyu789.top/gttofcerdl.html

Ruby: "ab" * 3
来源：http://hz.chenzaomai.com/gtzuzhxiyv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.vqdsnc.cn/gtbcdnbuyi.html

[E03] 截取子串
来源：http://hz.quarkkingdee.top/gtidxmrijk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xziqi.cn/gtdlekrfgb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shuidangran.top/gtkiqjysld.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hammf.cn/gtvdkfbgdo.html

TS:   s.slice(1, 4)
来源：http://hz.jlsjyb.cn/gtdtfgxnny.html

Java: s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtnskwhgkz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinqigufen.top/gtvwjlfrai.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sufxvd.cn/gtfhbvsgmm.html

C#:   s.Substring(1, 3)
来源：http://hz.ivvv.top/gtusyypgnx.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gthiwfzmkb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hammf.cn/gtgjcsmfux.html

PHP:  strpos($s, "x");
来源：http://hz.hnxiangtu.top/gttdexakni.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cheryme.top/gtjwqaoryv.html

TS:   s.indexOf("x")
来源：http://hz.sufxvd.cn/gtnfhgrulh.html

Java: s.indexOf("x")
来源：http://hz.ivvv.top/gtparbdvqw.html

Go:   strings.Index(s, "x")
来源：http://hz.0kj1m.cn/gtjsrbpfeb.html

Ruby: s.index("x")
来源：http://hz.mhx1999.top/gtretjodna.html

C#:   s.IndexOf("x")
来源：http://hz.ehwqpu.com/gttyfwqrok.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenzaomai.com/gtvgcccfxh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.meibo888.top/gtfovyeuln.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gttubemliq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtcaneuqvm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.0kj1m.cn/gtnunemkwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtgrwjjevs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.pengpengdd.cyou/gtwmtlbfeg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xuanzx.com/gtmlzrpsxx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sweek.top/gthykndent.html

[E06] 替换子串
来源：http://hz.hnxiangtu.top/gtdsltixhy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dashuyun.cn/gtpcgpgxbr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sysykeji.top/gtorjqaksc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtllkbizfd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtjxtmltme.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtpudwlozs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yongpay.top/gttwpnpymr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cashguo.top/gtohhdfygj.html

C#:   s.Replace("a", "b")
来源：http://hz.nanxinkj.top/gtpfkhhyah.html

[E07] 按分隔符拆分
来源：http://hz.birdmap.top/gtkbyzrmuc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.9152youxi.cn/gtjqhtiuqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ehwqpu.com/gtaqlnaqmh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hysaishi.cn/gtlmahjvxg.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtykjdqbph.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.vqdsnc.cn/gtksqrgpyz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.iojbl.cn/gtczwoqcqi.html

Ruby: s.split(",");  s.split
来源：http://hz.feifeiyinyue.top/gtsgkxnbbb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jyoumei.cn/gtebjbumxh.html

[E08] 数组按分隔符合并
来源：http://hz.hongshengwenyu.top/gteowcndtj.html

Py:   ",".join(items)
来源：http://hz.cqqwz.cn/gtnfbizvyh.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtkgwdniyp.html

JS:   items.join(",")
来源：http://hz.hnqzz.top/gtepqmhqts.html

TS:   items.join(",")
来源：http://hz.c1oappe.top/gtpxrbeyhx.html

Java: String.join(",", items)
来源：http://hz.yuanzhike.top/gtuguliske.html

Go:   strings.Join(items, ",")
来源：http://hz.pengpengdd.cyou/gtoklykjxc.html

Ruby: items.join(",")
来源：http://hz.smart0.xyz/gtiqvmwkcz.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtpamezhnt.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gtpgfsctio.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtgcqdvglm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jiagoushi.top/gtegprfwrh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtxrneyzbw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtugytfczl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.aibaodan.cn/gtletngfmc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtazjtkzvv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yangfankeji.com/gtewoxlktd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cqqwz.cn/gtvlgsdiwt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenzaomai.com/gtuctcowak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yongpay.top/gtotsmcxwl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.andypj.xyz/gtdvooqfiw.html

JS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtshmowega.html

TS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtbpredsrz.html

Java: String.format("%03d", 7)
来源：http://hz.daxiang520.top/gtgjnynmpm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtmuizpzih.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtktgrdxpr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aizwys.cn/gtzydhfcgk.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtkakyxeop.html

Py:   s[::-1]
来源：http://hz.guowangkeji.top/gtcbnylqwu.html

PHP:  strrev($s);
来源：http://hz.ydzc1.top/gtuoszzlcf.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtbvuabzpv.html

TS:   [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtvpmwdjrg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtqdumcfux.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.c1oappe.top/gtmljnyuqt.html

Ruby: s.reverse
来源：http://hz.zhoulong.xyz/gtdapjxmub.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtvseynchq.html

[E12] 统计某字符出现次数
来源：http://hz.sweek.top/gtymkvofrn.html

Py:   s.count("a")
来源：http://hz.zhaomingkeji.xyz/gtxwttssxt.html

PHP:  substr_count($s, "a");
来源：http://hz.birdmap.top/gtqlsdhsco.html

JS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtvveionfy.html

TS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtmxkwaywr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gthvykwvps.html

Go:   strings.Count(s, "a")
来源：http://hz.jianghu66.top/gtomcidxio.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtbbczzuwx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtfuuyhsci.html

[E13] 逐字符遍历
来源：http://hz.zhaomingkeji.xyz/gtovxkrtfp.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtvwxhhbpd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daxiang520.top/gtbxonsksc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gtasxizsts.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtmopmgnat.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sxryk.cn/gtdendsggz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xylfe.cn/gtqlpxtwnt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxuanxn.top/gthbvtemlb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnxiangtu.top/gtbporlhxm.html

[E14] URL 编码与 Base64
来源：http://hz.cucudq.cn/gtmqjvsfzm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258888.top/gtrapktroz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuanzx.com/gtxxpqavfk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.quarkkingdee.top/gtteyxgrla.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhaomingkeji.xyz/gtrbchjkgz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnxiangtu.top/gtfsqlfgdg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sysykeji.top/gtybpawvws.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtalapxrvi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shzxlz.cn/gtxnbfsbpl.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gttjcwdujh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhijiandao.cn/gtznoevvja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtbhmephsg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xingfuxueyuan.xyz/gtbixteirc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hongshengwenyu.top/gtgbtzowdy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.havefunace.top/gtfalqmlbg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhengqikj.top/gtdwshxsdh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinghuilouyu.cn/gttbwkrmgj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tian-w.cn/gtrpqrxxmu.html

[E16] 数字千分位
来源：http://hz.tanke756.top/gteykazzzs.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gteausytze.html

PHP:  number_format(1234567);
来源：http://hz.52xcode.cn/gtsrrgradl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtzpmomemc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jianghu66.top/gttdlldpql.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxinkj.top/gttlyeehri.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zdqjudy.top/gtctucedrh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tianlin.xyz/gtakbwumkr.html

C#:   1234567.ToString("N0")
来源：http://hz.mhx1999.top/gtduwgytsu.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gthxkwkrbc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ydzc1.top/gtsldtvkpn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.haohaochexian.top/gtwfgvaozb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtlvmkpepi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtrvlobttt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gthwhsjofy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydjk.org.cn/gtpawrnyts.html

Ruby: s.capitalize
来源：http://hz.hfpthk.cn/gtbaxdvyqp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtfaiwznfn.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtkknhfcul.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtcqkgddie.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cucudq.cn/gtwsgrvexl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ybcxt.top/gtjkwrijil.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtstagjfyx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gthczgberw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhoulong.xyz/gtbzehddwm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gtkyumgwen.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigfzy.top/gtlshmedgb.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258.top/gtchxbmdna.html

Py:   s.splitlines()
来源：http://hz.yueranfly.top/gtwqfzturb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigfzy.top/gtkkaujfrl.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtrndqsltj.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtffxextmj.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gthhhapbly.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenlongwang.top/gtkkfdwptm.html

Ruby: s.lines
来源：http://hz.birdmap.top/gtvqcoovkc.html

C#:   s.Split('\n')
来源：http://hz.daxiang520.top/gtttlwoqvx.html

[E20] 判断字符串是否为空
来源：http://hz.gzhubu.top/gtjaosegdq.html

Py:   if not s:
来源：http://hz.sxryk.cn/gtvnmiyghv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtpphpdzok.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hysaishi.cn/gtulvmqnbe.html

TS:   if (s === "") {}
来源：http://hz.gzhubu.top/gtfxbrvjzr.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtmzjqwxhc.html

Go:   if s == "" {}
来源：http://hz.hywenlv.cn/gtkbfmdgmh.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtkxdrgdyv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangtech.top/gtobqkzibg.html

[E21] 超长截断加省略号
来源：http://hz.yonumen.top/gtzzeulyje.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shuidangran.top/gtympsmokq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yvedp.cn/gtwlcssfpu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtydgohsej.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtcjpmrpex.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtzxunepnj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pengpengdd.cyou/gtaqqwxddi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.meibo888.top/gtjkkdomti.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtshvfzwcx.html

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtqgwyxbto.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nwbrower.top/gtyuppokqs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtfbkmwhku.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtkuimucrp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtbvvbfrpy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuanzx.com/gticpqsnqi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fzhhl.top/gtdhefpusc.html

Ruby: s.bytesize;  s.length
来源：http://hz.cucudq.cn/gtilgtmjxc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cqqwz.cn/gtblynwiqq.html

================================================================================
来源：http://hz.yj202588.top/gtzjzmgptv.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtyuunsgvs.html

================================================================================
来源：http://hz.316326.xyz/gtapjnilqp.html

[F01] 读取整个文件
来源：http://hz.shuidangran.top/gtvmlcvway.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.vqdsnc.cn/gtjzxedyrq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.smart0.xyz/gtmhgecoxn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtvkphuimp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtjxzewlsj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtvjnqabak.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtmztrlqnj.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtuslrcfer.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhengqikj.top/gtxoqlowzq.html

[F02] 逐行读取文件
来源：http://hz.jinyuanbaomall.cn/gtivfzxtpy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gtntxussea.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj20258888.top/gtpmnnbacx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gtxesfghyw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtcbnbctuc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtmlpwvxtl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.9152youxi.cn/gtnztijurk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sysykeji.top/gtcdavndbs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yueranfly.top/gtbhqnrifz.html

[F03] 写入文件（覆盖）
来源：http://hz.smart0.xyz/gtcurrhend.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangshuangyany.cn/gtecuoblgn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtgfmuicgs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtypwihusu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtjdujzsyl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gzhubu.top/gtjmgwsjit.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtgooiggwc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hysaishi.cn/gtmiytzzxx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtqrtimwcp.html

[F04] 追加写入文件
来源：http://hz.xuanzx.com/gtyovetmaj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.havefunace.top/gtcisgtnbw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtpggqovpg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gteuazqkeb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtzgdrueex.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gtovwdzrjw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.redwolf501.top/gttuomphwu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtaattaohg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtbeihpkgp.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtsdidjbcp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yanxiufei.cn/gtagmsbayh.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtdhwebiri.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtfbmjzmwd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtdnrfghjm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtheuryhhv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.daxiang520.top/gtnwjdnhjx.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gtlwqxtckz.html

C#:   File.Exists("a.txt")
来源：http://hz.cqqwz.cn/gtgudvwouw.html

[F06] 删除文件
来源：http://hz.yj20258.top/gtzdrsbrmj.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtfcacvgyg.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtcoislqpi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtllskcdkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtmducueda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gtqaelqwtc.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtskcocjsd.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtchrpbguv.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtyjgcokgf.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangtech.top/gtjwtgjnlu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gthuokxfrv.html


<!-- 参考信息 -->