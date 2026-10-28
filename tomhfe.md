代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gthjyxnyib.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtpubxzraw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.daria6918.cn/gtpxsacgee.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtirunauyk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daria6918.cn/gtbxqeqhgg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.havefunace.top/gtvnnchuak.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnqzz.top/gtgnbdindm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.316326.xyz/gtfgqzwnve.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtpshfjxei.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj202588.top/gtognogagb.html

[D25] Set 集合去重与交并差
来源：http://hz.hnqzz.top/gthwnhzjqi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.aibaodan.cn/gtcxvgxvge.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtblruupvm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ybcxt.top/gtcwrjonym.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangdashe.top/gtsxtgiore.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtdvxwwffe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gtcgtrmkmh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sxryk.cn/gtpowwnook.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtfdpmuudc.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtcbojjbsi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pengpengdd.cyou/gtmfpfkter.html

PHP:  implode(", ", $arr);
来源：http://hz.havefunace.top/gtoidadzcf.html

JS:   arr.join(", ")
来源：http://hz.cheryme.top/gtrpxpjxti.html

TS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gtzpvapnki.html

Java: String.join(", ", list)
来源：http://hz.zhiwuduotai.top/gtrnmlzaoa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtqlfchtty.html

Ruby: arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtjirbjqnx.html

C#:   string.Join(", ", list)
来源：http://hz.yuanzhike.top/gthazgnbem.html

================================================================================
来源：http://hz.hysaishi.cn/gtuihjxthv.html

E. 字符串处理
来源：http://hz.zycfv.cn/gtgyionwnm.html

================================================================================
来源：http://hz.ehwqpu.com/gtxydnfupe.html

[E01] 拼接字符串
来源：http://hz.vqdsnc.cn/gtutuadhng.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zdqjudy.top/gthcvwtgkb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtbvamfcgp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtorobncra.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtlgkcvdkw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xinyue.icu/gtmzduziyz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aizwys.cn/gttqrojszg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.52xcode.cn/gtlsboplmw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gogol.net.cn/gtgdaxapwo.html

[E02] 重复字符串
来源：http://hz.chenzaomai.com/gtyxrjcant.html

Py:   "ab" * 3
来源：http://hz.gzhubu.top/gtgzcescca.html

PHP:  str_repeat("ab", 3);
来源：http://hz.bjfxy.top/gthkxtqnbk.html

JS:   "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtgnuazweb.html

TS:   "ab".repeat(3)
来源：http://hz.cqqwz.cn/gtsyheezqo.html

Java: "ab".repeat(3)
来源：http://hz.cheryme.top/gtlbrthizp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258.top/gtbdhrpzkk.html

Ruby: "ab" * 3
来源：http://hz.wangshuangyany.cn/gtxcobolvn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangshuangyany.cn/gtkefggzgv.html

[E03] 截取子串
来源：http://hz.iojbl.cn/gtutqkqdxv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtuhzwifma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgfzy.top/gtznmgseeq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gtyagwuuvu.html

TS:   s.slice(1, 4)
来源：http://hz.yuanzhike.top/gtlfiobfnf.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gthignyhpb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gtpoboerzb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangshuangyany.cn/gthuubtdvx.html

C#:   s.Substring(1, 3)
来源：http://hz.daria6918.cn/gteezcajdo.html

[E04] 查找子串位置
来源：http://hz.52xcode.cn/gtxzkkyakl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxuanxn.top/gtinjocwgw.html

PHP:  strpos($s, "x");
来源：http://hz.cashguo.top/gteymhhvuf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtizmuzhau.html

TS:   s.indexOf("x")
来源：http://hz.yj202588.top/gtgoneavft.html

Java: s.indexOf("x")
来源：http://hz.ivvv.top/gtdnpoqxfy.html

Go:   strings.Index(s, "x")
来源：http://hz.hongshengwenyu.top/gtplgzrcpg.html

Ruby: s.index("x")
来源：http://hz.zhixingplan.top/gtrcrkjuze.html

C#:   s.IndexOf("x")
来源：http://hz.iojbl.cn/gtbajdgmom.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tianlin.xyz/gtxgoimrya.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtzvqxtmmx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtfijjappz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtkjsifwgl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fzhhl.top/gthhyerkfb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fzhhl.top/gtcttgbmul.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuetiantiany.cn/gtezjrinvf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.feifeiyinyue.top/gtetzctnaw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangshuangyany.cn/gthhqhfpni.html

[E06] 替换子串
来源：http://hz.fzhhl.top/gtmggtzqej.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jyoumei.cn/gtyziopsyv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.snrcjt.cn/gtkcdxsomx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtfjafcran.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtxqklohqn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtgrqkparn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgufenzy.top/gtilnnbeqo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guowangkeji.top/gtfgjjvvls.html

C#:   s.Replace("a", "b")
来源：http://hz.fengsongda.top/gtomvntmhq.html

[E07] 按分隔符拆分
来源：http://hz.ivvv.top/gtnlslbxpb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cashguo.top/gttahnphdh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhiwuduotai.top/gtgniyslnp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydzc1.top/gtagehooqv.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtyyzbufsz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtpzhbihyd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jiagoushi.top/gtrzvlilxz.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtapntsgco.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtnajvxyaw.html

[E08] 数组按分隔符合并
来源：http://hz.ehwqpu.com/gtfeayhdpx.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtdzwnmbjn.html

PHP:  implode(",", $items);
来源：http://hz.dashuyun.cn/gtkbjukorb.html

JS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtqwzkhyic.html

TS:   items.join(",")
来源：http://hz.zhongyouzk.top/gthrnpfcls.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtjhmpvzkp.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtmuwfjasb.html

Ruby: items.join(",")
来源：http://hz.jinqigufen.top/gtiyoowzlf.html

C#:   string.Join(",", items)
来源：http://hz.ppjwa.cn/gtzrhapxym.html

[E09] 去除所有空白字符
来源：http://hz.yvedp.cn/gtbmdrkkxv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xinyue.icu/gtpqghwurm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gtxhtgotac.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtbzuwebkr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtxorjafey.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daxiang520.top/gtkzsmjweb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtxhlsxxwc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fzhhl.top/gtrzzlyvgq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnqzz.top/gtpgwapemu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.52xcode.cn/gtwzbjykhf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenlongwang.top/gtxguflmky.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtkhtjwozq.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gtxafvwbxi.html

TS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtgahdidnx.html

Java: String.format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtrrbsyatq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cdnleiting.top/gtlxptnvrr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fzhhl.top/gtvposqvit.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.c1oappe.top/gttwnywtkv.html

[E11] 反转字符串
来源：http://hz.fengsongda.top/gtimsgjrvr.html

Py:   s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtzcexyanr.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gtydypjsza.html

JS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtzthhscff.html

TS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtbncssmta.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yueranfly.top/gtixropmhs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxuanxn.top/gteodunkij.html

Ruby: s.reverse
来源：http://hz.tianlin.xyz/gtlegktmaq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtcfykeswc.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtcvwhjmgq.html

Py:   s.count("a")
来源：http://hz.aibaodan.cn/gtwrzrotpp.html

PHP:  substr_count($s, "a");
来源：http://hz.zhoulong.xyz/gttrzglvbu.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtkixkckng.html

TS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtsohrsvfx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtodnfbglb.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtdanqvble.html

Ruby: s.count("a")
来源：http://hz.hysaishi.cn/gtjtqbjjln.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gtrctdzxvc.html

[E13] 逐字符遍历
来源：http://hz.wangdashe.top/gttjvdthos.html

Py:   for ch in s: print(ch)
来源：http://hz.chenzaomai.com/gtvpnzhegz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnxiangtu.top/gtwsacuorn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtenlqdldt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gthketkhei.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gaohongyu789.top/gtawcdcgan.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aibaodan.cn/gtjqgnwrzq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtstudaidq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtpyocfjtw.html

[E14] URL 编码与 Base64
来源：http://hz.havefunace.top/gtilznumbm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangtech.top/gtbbmgqmgn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnqzz.top/gtktzsvzlr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258.top/gtojaucoys.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cucudq.cn/gthhqjbnnm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtnmhhwjrb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aizwys.cn/gtldhnhlln.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.andypj.xyz/gtywzityte.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aibaodan.cn/gtwhjgqxud.html

[E15] HTML 转义 / 反转义
来源：http://hz.jqgfzy.top/gteqrwdlvk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.havefunace.top/gtrkaycmol.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtqcepfxlo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigfzy.top/gtshjppsav.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yueranfly.top/gtcfzhjxhb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigfzy.top/gtjpqwelnl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuetiantiany.cn/gttioondwg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtymayjvrw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.feifeiyinyue.top/gtriaenxnb.html

[E16] 数字千分位
来源：http://hz.yuanzhike.top/gtjpvkdtnl.html

Py:   f"{1234567:,}"
来源：http://hz.tianlin.xyz/gtwjighanp.html

PHP:  number_format(1234567);
来源：http://hz.jinqigufen.top/gtpmjeiuei.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gteivkhrqx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtualtiijd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ybcxt.top/gtagipzuuf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daria6918.cn/gthtaotupl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.9152youxi.cn/gtzqfxtlsi.html

C#:   1234567.ToString("N0")
来源：http://hz.0kj1m.cn/gtsqjbdbfi.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtiyvsqyax.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ydzc1.top/gtemxjaqhd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtzldzdhxe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gttlgehnrj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtnstxgytr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nanxuanxn.top/gtmjjrghps.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gtqrdchqoq.html

Ruby: s.capitalize
来源：http://hz.cheryme.top/gtrbmwylie.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtfxnszedw.html

[E18] 模板占位符替换
来源：http://hz.pycfn.com/gtrymkagyw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shangyingyoupin.top/gtaljytxss.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtgbzayfgz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtixbnqxka.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtgxohhexf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtaincswzn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xylfe.cn/gtcgjmunme.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hfpthk.cn/gtwwwzbgxi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigufen.top/gtmxfedzxd.html

[E19] 多行文本按行拆分
来源：http://hz.birdmap.top/gtebcdijfc.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gtajvjrhyu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.nanxuanxn.top/gtyabnpiiz.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtytrthmke.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtelragbej.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtqqctgxbc.html

Go:   strings.Split(s, "\n")
来源：http://hz.snrcjt.cn/gtslmkdxam.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtzctmgwaf.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtjvpcxzra.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtaoniumcc.html

Py:   if not s:
来源：http://hz.yongpay.top/gtqwgufdhh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hywenlv.cn/gtqzyzymnt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.meibo888.top/gtivexsljh.html

TS:   if (s === "") {}
来源：http://hz.shangyingyoupin.top/gtqqzhxveu.html

Java: if (s.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtrkaywtjc.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtbzqfiwqd.html

Ruby: if s.empty?
来源：http://hz.ybcxt.top/gtrxmtbwxc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtkqmrlfka.html

[E21] 超长截断加省略号
来源：http://hz.fengsongda.top/gtgpkoidle.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtvpypfdck.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtdbtdxrwm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtcuibeqbr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtwwjzilrc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtisjmjgng.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fzhhl.top/gtrwuasjwm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jyoumei.cn/gtrgisxprr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenzaomai.com/gthpwxitng.html

[E22] 字节长度与字符长度
来源：http://hz.zycfv.cn/gtjzjhxrnd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangtech.top/gtbwctiwxc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtiemkzkev.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtistnunvf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtqesrlmbx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.havefunace.top/gthcxkwygk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hammf.cn/gtstrnmsvj.html

Ruby: s.bytesize;  s.length
来源：http://hz.yonumen.top/gttpoggqea.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hongshengwenyu.top/gtdjwqnbcz.html

================================================================================
来源：http://hz.tian-w.cn/gtgfnsdump.html

F. 文件与目录
来源：http://hz.jqgfzy.top/gtglubitdn.html

================================================================================
来源：http://hz.aibaodan.cn/gtyasnryos.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gttrzdhrkq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.birdmap.top/gtjwsbhxpl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenlongwang.top/gtnfiguwll.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtcqrvgzvd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtaoejfraq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtafmbrtyh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj202588.top/gthicualax.html

Ruby: File.read("a.txt")
来源：http://hz.hnqzz.top/gtkwqxowul.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cdnleiting.top/gtxgsxliuz.html

[F02] 逐行读取文件
来源：http://hz.chenjidiqi.icu/gtwpikumjp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.svipenyu.cn/gtcavjncbq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gtbyucglkj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtucfixddb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtguktuydk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtznortxvg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gzhubu.top/gttbcasers.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.0kj1m.cn/gtpnjgybdp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.snrcjt.cn/gtzyowhppz.html

[F03] 写入文件（覆盖）
来源：http://hz.redwolf501.top/gtdnphtawf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.iojbl.cn/gthpsisnjw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtpdzjasri.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtsszioxcq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtsplavdcg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yueranfly.top/gtutrbkbzz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtbmsozftw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtyzxdbasq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtxhbfvenv.html

[F04] 追加写入文件
来源：http://hz.zdqjudy.top/gtcstbxzhh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gtmxmuqrlc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.kuanghao11.cn/gtwlejmelh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgufenzy.top/gtephanxhr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangshuangyany.cn/gtxdboeozx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtxpqbjwle.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cashguo.top/gtrxlhpdss.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtyjijixtb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtjmjeodvp.html

[F05] 判断文件或目录是否存在
来源：http://hz.shuidangran.top/gtfypuvjib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pycfn.com/gtlypbzjvw.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtqxbjldsx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtgzjopxuc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gthysctdkc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtjmnzfodb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinyuanbaomall.cn/gtuqnjkhqe.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenjidiqi.icu/gtwmdaddqi.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtdsbfgrtl.html

[F06] 删除文件
来源：http://hz.jlsjyb.cn/gtcmwykble.html

Py:   os.remove("a.txt")
来源：http://hz.c1oappe.top/gtsyktelkc.html

PHP:  unlink("a.txt");
来源：http://hz.xuanzx.com/gtbvmiifsx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtnfwnmjxy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtnuorqhag.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtmrjewdoe.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtqwccbvsf.html

Ruby: File.delete("a.txt")
来源：http://hz.ivvv.top/gtwmjxqxtq.html

C#:   File.Delete("a.txt");
来源：http://hz.xinyue.icu/gtrbrpddnw.html

[F07] 创建目录（含多级）
来源：http://hz.hammf.cn/gtjvtonxla.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtkulypnpx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cdnleiting.top/gtrtdzvioo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtpnpuzydb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtpyyqfbzf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.vqdsnc.cn/gtwsorzsmh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtndjssihd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtdovdkhgg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shangyingyoupin.top/gtpkelfqoz.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtckpzhkih.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hongshengwenyu.top/gtwprddgfc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hywenlv.cn/gtebfjjxdm.html

JS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtizgxnvxe.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtdqrxpixq.html


<!-- 参考信息 -->