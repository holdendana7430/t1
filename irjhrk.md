代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gotoacloud.top/gthybzpybg.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinghuilouyu.cn/gtanumqrln.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guowangkeji.top/gtvmkyxowc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gaohongyu789.top/gtzfgysxuk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhaomingkeji.xyz/gttpzrtzef.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cheryme.top/gtvkfsjrjk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.bjfxy.top/gtojtdfacz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xinyue.icu/gtxkxrxbmw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.c1oappe.top/gtdgbtydtq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aibaodan.cn/gtvthsywsc.html

[D25] Set 集合去重与交并差
来源：http://hz.cqqwz.cn/gthbafrzgw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gttvtdzwgo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtfhzvhoxc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gtyxhcakcv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zycfv.cn/gtkevzvgye.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtowvzcvyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangkeji.top/gtgcaqcnpm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtfznpptrl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xylfe.cn/gthhouuiiw.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtyhkofehw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nwbrower.top/gtvagpifgf.html

PHP:  implode(", ", $arr);
来源：http://hz.yueranfly.top/gtetwufxeh.html

JS:   arr.join(", ")
来源：http://hz.316326.xyz/gttfstirnp.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gteqhfhkgw.html

Java: String.join(", ", list)
来源：http://hz.quarkkingdee.top/gtffdelqhb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtigvqwwqe.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtkybuepqe.html

C#:   string.Join(", ", list)
来源：http://hz.wangshuangyany.cn/gtstemruqx.html

================================================================================
来源：http://hz.hywenlv.cn/gtwaifcrss.html

E. 字符串处理
来源：http://hz.daxiang520.top/gtrlljlzxq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbnwultic.html

[E01] 拼接字符串
来源：http://hz.yuxming.cn/gtctvesxvv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangdashe.top/gtlcjrnoll.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ybcxt.top/gtmgvucnjb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtswxqavvr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtcbnwsans.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydjk.org.cn/gtnfdmwowe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ydjk.org.cn/gtnvovzmma.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtqzjnbmcg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.smart0.xyz/gttxohgebs.html

[E02] 重复字符串
来源：http://hz.c1oappe.top/gtrrjrqick.html

Py:   "ab" * 3
来源：http://hz.yueranfly.top/gtwcolyffv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jlsjyb.cn/gtbntfbivj.html

JS:   "ab".repeat(3)
来源：http://hz.tian-w.cn/gttraqmidn.html

TS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtuytjxbyv.html

Java: "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gttmogzewx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtktophank.html

Ruby: "ab" * 3
来源：http://hz.jqgufenzy.top/gtraivpldu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shzxlz.cn/gtfxhlyebx.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtnsjanbel.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.guannengcc.top/gtqrzeiswt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenzaomai.com/gteywhrwlv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtironjqlu.html

TS:   s.slice(1, 4)
来源：http://hz.zdqjudy.top/gtomttjyao.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtglgdnigz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.0kj1m.cn/gtlhiebssv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.svipenyu.cn/gtrybtwukz.html

C#:   s.Substring(1, 3)
来源：http://hz.gzhubu.top/gtlsxaiphr.html

[E04] 查找子串位置
来源：http://hz.jianghu66.top/gtsohblnmb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj20258.top/gtwtlrzbyy.html

PHP:  strpos($s, "x");
来源：http://hz.yuanzhike.top/gthzuwdcnf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yangfankeji.com/gtqosnhxby.html

TS:   s.indexOf("x")
来源：http://hz.gogol.net.cn/gtjukiqrdq.html

Java: s.indexOf("x")
来源：http://hz.iojbl.cn/gtmidyzdsd.html

Go:   strings.Index(s, "x")
来源：http://hz.tanke756.top/gtohoymlqa.html

Ruby: s.index("x")
来源：http://hz.yonumen.top/gtszsfhjiu.html

C#:   s.IndexOf("x")
来源：http://hz.hammf.cn/gttbplnigx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ivvv.top/gtcfizrkeh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jiagoushi.top/gtqaoouucq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sxryk.cn/gtbosjzqos.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cashguo.top/gtwymtzrat.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtnbjpawzu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gttypmcpch.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.meibo888.top/gttlijdrzu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ppjwa.cn/gttrgvtvnz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtzxukvynx.html

[E06] 替换子串
来源：http://hz.yonumen.top/gthjtijlkn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.havefunace.top/gtwwtbakvv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jiagoushi.top/gtbmqcypip.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtjpaksjsm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtuzvkgbxs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtghslebbj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtloedrgdi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.wangdashe.top/gtxrykmrgf.html

C#:   s.Replace("a", "b")
来源：http://hz.haohaochexian.top/gtidbehreq.html

[E07] 按分隔符拆分
来源：http://hz.52xcode.cn/gtcmvbebzl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.52xcode.cn/gtbiirtygx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.quarkkingdee.top/gtohhrnyyy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jqgufenzy.top/gtevxufzca.html

TS:   s.split(",")
来源：http://hz.52xcode.cn/gtnlbzygaf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.9152youxi.cn/gtyefxybqg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hammf.cn/gtzatqzgqg.html

Ruby: s.split(",");  s.split
来源：http://hz.xylfe.cn/gtqxxkxpvi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.mhx1999.top/gtoshzferl.html

[E08] 数组按分隔符合并
来源：http://hz.fzhhl.top/gtngbwkkqy.html

Py:   ",".join(items)
来源：http://hz.chenzaomai.com/gtxyuiswmk.html

PHP:  implode(",", $items);
来源：http://hz.zhijiandao.cn/gtjrwzcbeu.html

JS:   items.join(",")
来源：http://hz.xziqi.cn/gtvxyndoap.html

TS:   items.join(",")
来源：http://hz.yueranfly.top/gtdumokycl.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gtmepsdvyk.html

Go:   strings.Join(items, ",")
来源：http://hz.zhoulong.xyz/gtmulwjlpr.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gtlxixevkz.html

C#:   string.Join(",", items)
来源：http://hz.tanke756.top/gtbspeqwrk.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtirohklqp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gtglsjalgz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.dianchejie.cn/gtfgncsnab.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtzpanujiv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhaomingkeji.xyz/gtjiiekfvf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sufxvd.cn/gtzauiycdh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hnxiangtu.top/gtzafelxmd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aibaodan.cn/gtjnekhomg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tian-w.cn/gtzoaszsya.html

[E10] 左侧补零 / 定长填充
来源：http://hz.mhx1999.top/gtcfjhcmwt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtlkamptdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ybcxt.top/gtyxlofthg.html

JS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtfsbeaard.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtubvepdvr.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gtafpkvqpt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cheryme.top/gtxgrclkjg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daxiang520.top/gtpkrywszs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangtech.top/gtrjmrqumf.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtkinjaryk.html

Py:   s[::-1]
来源：http://hz.fzhhl.top/gtmxpfffjg.html

PHP:  strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtamskrmja.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtigvxxyay.html

TS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtbjiusjqq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cheryme.top/gtewnsievt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinyuanbaomall.cn/gtlwggxufs.html

Ruby: s.reverse
来源：http://hz.xuanzx.com/gtazoctnds.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtfoljysud.html

[E12] 统计某字符出现次数
来源：http://hz.chenlongwang.top/gtklnzhdap.html

Py:   s.count("a")
来源：http://hz.jqgufenzy.top/gtrtzvakqs.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtxeyweafu.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gttojekblc.html

TS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtujoplyxx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtynieszlm.html

Go:   strings.Count(s, "a")
来源：http://hz.gogol.net.cn/gtltqbtvzj.html

Ruby: s.count("a")
来源：http://hz.tianlin.xyz/gtglhixtyc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tian-w.cn/gtbqipkzbz.html

[E13] 逐字符遍历
来源：http://hz.yvedp.cn/gtqzdnhgby.html

Py:   for ch in s: print(ch)
来源：http://hz.meibo888.top/gtkftdfkrz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenzaomai.com/gtmbcufmel.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtgljewtzv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtzyhlyzio.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenlongwang.top/gtfbqdpcvz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yongpay.top/gtgyohtyuw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yueranfly.top/gtkpgkfgpn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.iojbl.cn/gtscitcxqb.html

[E14] URL 编码与 Base64
来源：http://hz.chenzaomai.com/gtaxpuvogd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtqavqtycx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj202588.top/gtbpuamrtg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtpecdhucr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daxiang520.top/gtclsihhow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtloxodaot.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigfzy.top/gtixuqekzb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtqummzegu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yongpay.top/gtbppericm.html

[E15] HTML 转义 / 反转义
来源：http://hz.yonumen.top/gtbwdbrhbq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnxiangtu.top/gtdqvjjnna.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.svipenyu.cn/gtultymxzy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gtsxqipydj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cheryme.top/gtlymnrjsf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenlongwang.top/gtpfjsqqjm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtwioryjye.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtslcqopng.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xingfuxueyuan.xyz/gtuyxylkng.html

[E16] 数字千分位
来源：http://hz.haohaochexian.top/gtcyjgoiyl.html

Py:   f"{1234567:,}"
来源：http://hz.jqgfzy.top/gtjspgyttp.html

PHP:  number_format(1234567);
来源：http://hz.cdnleiting.top/gtqygqyvtd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtbkfenmml.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtqazkppsq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sysykeji.top/gtzpqmlyfm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtforksizx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aizwys.cn/gtpvvfusax.html

C#:   1234567.ToString("N0")
来源：http://hz.gzhubu.top/gtdiyopmig.html

[E17] 首字母大写
来源：http://hz.zhengqikj.top/gtckgpztwm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gtvzcqlkwy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangshuangyany.cn/gttcnfgrry.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtryzpglbr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gtvmrditql.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.birdmap.top/gtitshivoa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydjk.org.cn/gtechigrgq.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtutdprxse.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtukyssprr.html

[E18] 模板占位符替换
来源：http://hz.redwolf501.top/gtuecabpfs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yvedp.cn/gtsfpcinpm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgufenzy.top/gtokamiotf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtdvgcbpmr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtstjacexq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuxming.cn/gtflyeeozh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtjsxwhelj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ywan-chungtsiang.top/gtjtktlnta.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtqhdheojf.html

[E19] 多行文本按行拆分
来源：http://hz.jlsjyb.cn/gtfdxslrrd.html

Py:   s.splitlines()
来源：http://hz.smart0.xyz/gtlwairpdf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtxrinambw.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gteguwjjmh.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtusgmidgl.html

Java: s.lines().toList()
来源：http://hz.zhiwuduotai.top/gtfciyuacf.html

Go:   strings.Split(s, "\n")
来源：http://hz.meibo888.top/gteqyqiddk.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gthzhbemrj.html

C#:   s.Split('\n')
来源：http://hz.meibo888.top/gtemvpvpim.html

[E20] 判断字符串是否为空
来源：http://hz.yonumen.top/gtqfeojyjn.html

Py:   if not s:
来源：http://hz.zycfv.cn/gttnuatjjm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtmcuvmdas.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zdqjudy.top/gtvahxypcc.html

TS:   if (s === "") {}
来源：http://hz.aibaodan.cn/gtuowfnviv.html

Java: if (s.isEmpty()) {}
来源：http://hz.haohaochexian.top/gtlaabskar.html

Go:   if s == "" {}
来源：http://hz.yuanzhike.top/gtoppskztd.html

Ruby: if s.empty?
来源：http://hz.yanxiufei.cn/gttyhgxuyr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xziqi.cn/gteffhdrzq.html

[E21] 超长截断加省略号
来源：http://hz.dianchejie.cn/gttluuzylo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtdpksbbdb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuanzhike.top/gtzoyaered.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtqjrzptxi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtqqxsodjp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtlkwfygnp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtbhthotac.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gotoacloud.top/gtoydeomvs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gtcuokfxyk.html

[E22] 字节长度与字符长度
来源：http://hz.xuanzx.com/gtdctayryu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gtgsbuzdqi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtrnzvtlbm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtphqksfin.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtatoowebi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.316326.xyz/gtzimqvbzl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guowangkeji.top/gtogzfdwmu.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gtmauettfz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gtzbcqqejy.html

================================================================================
来源：http://hz.guowangkeji.top/gtvrjjzine.html

F. 文件与目录
来源：http://hz.jlsjyb.cn/gtjyribunc.html

================================================================================
来源：http://hz.c1oappe.top/gtgyxaioic.html

[F01] 读取整个文件
来源：http://hz.sxryk.cn/gtnzqllxpa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daria6918.cn/gtehybtbbt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydzc1.top/gtnsagvzfr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnqzz.top/gtpnyqnfoy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.bjfxy.top/gtwcxmaqbb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtzvlqvqdr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tianlin.xyz/gtcqifmdzf.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtatypckrd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258.top/gtmelihbsk.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangtech.top/gtmkhxfdpn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtoagcltfk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtjxaoigtc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtadbfuvyc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gtmgcmreee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtxdlzdjte.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtryiccvcl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtemczonuw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jiagoushi.top/gtnyawhvpc.html

[F03] 写入文件（覆盖）
来源：http://hz.cdnleiting.top/gtqfmkxyev.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtrobnxvmn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gtnpxyfizf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtplcvscxt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtsezsandl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.iojbl.cn/gthuyiyhec.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yanxiufei.cn/gtrpxgsrfb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sweek.top/gtpmjlovkk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cucudq.cn/gtffwlrryk.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gtjphrlnzw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pengpengdd.cyou/gtblgkdzcv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtftsvfkso.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtfdetckow.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtpggsxkoq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gtydxfkept.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sufxvd.cn/gtgzxtidkv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gtxnlakddq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtvospkeai.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtloqmkjbb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtahsoxiis.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtjmdnddqe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtmixwnffp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtyuqbjsgj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtzmznlgcq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtgsmuulsu.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydzc1.top/gtawlzdwll.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtcaxtdncg.html

[F06] 删除文件
来源：http://hz.c1oappe.top/gtkvuicnwg.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gtndknmbie.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtnxpseatz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtgzrezbod.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtzdljtydu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtihlcvzch.html

Go:   os.Remove("a.txt")
来源：http://hz.iojbl.cn/gtfvqowjkw.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtjwqxcyej.html

C#:   File.Delete("a.txt");
来源：http://hz.cdnleiting.top/gtqqmiumfi.html

[F07] 创建目录（含多级）
来源：http://hz.shuidangran.top/gtertanrkd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxinkj.top/gtvwzmylui.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtzjuxgpwc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtbnpqkodh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtbzaaqbfb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tanke756.top/gtzihefmdb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.kuanghao11.cn/gtknomxzrq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gogol.net.cn/gtuiixfosf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtddtpeuac.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtszuzytoi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.mhx1999.top/gtchzpudak.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtpdqdzzcc.html

JS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtabzlpdkk.html

TS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtruanfjcs.html


<!-- 参考信息 -->