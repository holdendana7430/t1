代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtogmdhyos.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhixingplan.top/gtgiglhjkg.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtyauknuha.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnxiangtu.top/gttonjspig.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtsdjfstev.html

[D24] 字典 / Map 基本操作
来源：http://hz.daria6918.cn/gtecxpsoeu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ppjwa.cn/gtjedtzxlk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtsfleroce.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gtqdhlvcws.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.aibaodan.cn/gtrtfksdmu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigufen.top/gtgocndjig.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jyoumei.cn/gtilcwgywe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtrfhwcfhm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtfxyagmoj.html

[D25] Set 集合去重与交并差
来源：http://hz.jiagoushi.top/gtagbxflqi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtwdayamnl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xinyue.icu/gtrvhgmnzw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.0kj1m.cn/gtjeacncvy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cheryme.top/gtghgebqdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinghuilouyu.cn/gtsmwsdlng.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtlxxzhipf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhoulong.xyz/gtuxktxdrd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhijiandao.cn/gtyhtlleam.html

[D26] 数组转字符串
来源：http://hz.yuanzhike.top/gtonubycxg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daria6918.cn/gtfcpuznoj.html

PHP:  implode(", ", $arr);
来源：http://hz.yanxiufei.cn/gtdoxkjzim.html

JS:   arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtwscsejxr.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtotvrjxeg.html

Java: String.join(", ", list)
来源：http://hz.tanke756.top/gtadkidjac.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gteajgbapy.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gtrugzluzn.html

C#:   string.Join(", ", list)
来源：http://hz.dianchejie.cn/gtzhigorwk.html

================================================================================
来源：http://hz.sufxvd.cn/gtiqwdriye.html

E. 字符串处理
来源：http://hz.316326.xyz/gtlazvmzyw.html

================================================================================
来源：http://hz.sufxvd.cn/gtwynsbsxn.html

[E01] 拼接字符串
来源：http://hz.bjfxy.top/gtpkdalmrt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.mhx1999.top/gtnuapdfji.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jianghu66.top/gtzefarfnn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtikineuju.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtijbaabwm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hfpthk.cn/gthhtnoiqh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhaomingkeji.xyz/gtlsnwyidw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sxryk.cn/gtuvltkhcn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fzhhl.top/gtumuvvzsd.html

[E02] 重复字符串
来源：http://hz.nwbrower.top/gtvndbszuv.html

Py:   "ab" * 3
来源：http://hz.andypj.xyz/gtfdsncblc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.svipenyu.cn/gtgbbldzru.html

JS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtdsmempxe.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtohdnacqs.html

Java: "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtoeymgrqh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhaomingkeji.xyz/gtyvakybom.html

Ruby: "ab" * 3
来源：http://hz.hnqzz.top/gtgaiqqrcl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258.top/gtxujcsulr.html

[E03] 截取子串
来源：http://hz.yvedp.cn/gtelxmnumg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.redwolf501.top/gtuikmstop.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.iojbl.cn/gtrriongdx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtjwnczhai.html

TS:   s.slice(1, 4)
来源：http://hz.nanxuanxn.top/gtzpfybtdf.html

Java: s.substring(1, 4)
来源：http://hz.xinyue.icu/gtoqegwzuk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnxiangtu.top/gtunxaqefd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.daria6918.cn/gtepppladv.html

C#:   s.Substring(1, 3)
来源：http://hz.yj202588.top/gtooxxeflo.html

[E04] 查找子串位置
来源：http://hz.aizwys.cn/gtaqjmnyrw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hywenlv.cn/gtytnayppw.html

PHP:  strpos($s, "x");
来源：http://hz.yj202588.top/gtwdkckvjq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hongshengwenyu.top/gtevvozcnn.html

TS:   s.indexOf("x")
来源：http://hz.nanxinkj.top/gtnvtabsyq.html

Java: s.indexOf("x")
来源：http://hz.ybcxt.top/gtbgmnixpy.html

Go:   strings.Index(s, "x")
来源：http://hz.hammf.cn/gtlraaicba.html

Ruby: s.index("x")
来源：http://hz.xziqi.cn/gtlejhhptz.html

C#:   s.IndexOf("x")
来源：http://hz.bjfxy.top/gtuzupnrvh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gtvdnjvvjw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.0kj1m.cn/gtumkmwcwd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.smart0.xyz/gtqapggyqk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtolpfipkp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ywan-chungtsiang.top/gtwdbddbtz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtxnypyxei.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xziqi.cn/gtvvuzdljj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sweek.top/gtwokpmqos.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cdnleiting.top/gtbsjcgadq.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtkgucuueu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.redwolf501.top/gtcaikmqkx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtmkrxmpdv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtoequcprw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtknsrtsgt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtonwawcwl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xylfe.cn/gtnheamaan.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtnlgdafeb.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgufenzy.top/gtuvxmwvqn.html

[E07] 按分隔符拆分
来源：http://hz.guowangkeji.top/gtivkrbygb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj202588.top/gtybbxdnmq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangshuangyany.cn/gtxctmicna.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtplryiyhb.html

TS:   s.split(",")
来源：http://hz.nanxinkj.top/gtegeoxjti.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gtbwjhtcct.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hnqzz.top/gtuzgqqffb.html

Ruby: s.split(",");  s.split
来源：http://hz.jqgfzy.top/gtoclqwofd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xuetiantiany.cn/gtuiucrduw.html

[E08] 数组按分隔符合并
来源：http://hz.pycfn.com/gthnstinhf.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtrswrfyqw.html

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gthtpglwsn.html

JS:   items.join(",")
来源：http://hz.zhengqikj.top/gtwltehtmh.html

TS:   items.join(",")
来源：http://hz.jianghu66.top/gtwqwwlgzo.html

Java: String.join(",", items)
来源：http://hz.yangfankeji.com/gtxlfywsra.html

Go:   strings.Join(items, ",")
来源：http://hz.xuanzx.com/gtlgqfwqeq.html

Ruby: items.join(",")
来源：http://hz.ywan-chungtsiang.top/gteqmziwxf.html

C#:   string.Join(",", items)
来源：http://hz.jqgfzy.top/gtejficerv.html

[E09] 去除所有空白字符
来源：http://hz.xuetiantiany.cn/gtkvmudaod.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtunuwgcyr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.quarkkingdee.top/gtmdxiokeh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtiefldsqn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtuytdnftn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtxnhfbjvh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shzxlz.cn/gthizoulht.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtzwisyyew.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhengqikj.top/gttutmbwee.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jyoumei.cn/gtqzdqlrcp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cucudq.cn/gtguuirmku.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtlkbjooxb.html

JS:   "7".padStart(3, "0")
来源：http://hz.svipenyu.cn/gtkwyigtmc.html

TS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtbtdjsyts.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtxhevngbz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtncnzuphl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtwearshmm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgfzy.top/gtlbpnaxbs.html

[E11] 反转字符串
来源：http://hz.ivvv.top/gtyqzhxyfx.html

Py:   s[::-1]
来源：http://hz.zhijiandao.cn/gtjdyxijmy.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gtqfwldeih.html

JS:   [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtwydowwkn.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtetodneiy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtsydlgntm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jyoumei.cn/gtnwahtbod.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtetnjmmrg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtqladuemz.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gtfqvunxvh.html

Py:   s.count("a")
来源：http://hz.nwbrower.top/gtcdahwjic.html

PHP:  substr_count($s, "a");
来源：http://hz.yuanzhike.top/gtaulmwtsp.html

JS:   s.split("a").length - 1
来源：http://hz.zdqjudy.top/gtfvnyqymq.html

TS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gtkuwmzced.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgfzy.top/gtuarbgfnc.html

Go:   strings.Count(s, "a")
来源：http://hz.haohaochexian.top/gtqrfoxhdz.html

Ruby: s.count("a")
来源：http://hz.ydjk.org.cn/gtudxoexwk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.smart0.xyz/gtfwapdfng.html

[E13] 逐字符遍历
来源：http://hz.yonumen.top/gtotuiqhni.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtnrwfgeyo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenlongwang.top/gttqmchycz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtolpnqals.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtpxdztkot.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sysykeji.top/gtjnljyzgq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhaomingkeji.xyz/gtuyeoshmh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shzxlz.cn/gtqdzzekes.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ywan-chungtsiang.top/gtbctyibao.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtmknovdyq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.bjfxy.top/gtwrrufsfb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.birdmap.top/gtdoylcudg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xylfe.cn/gtbqpnvjeg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gtusrdpolq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtnlidblez.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtkpuqldgc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangshuangyany.cn/gtfrljhjwy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtccfeithr.html

[E15] HTML 转义 / 反转义
来源：http://hz.ivvv.top/gtmnkglvvw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gaohongyu789.top/gtcccmhctt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cqqwz.cn/gtcxbfcvhh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.birdmap.top/gtloivppal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtuebybdhx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.meibo888.top/gtxkfojswq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnqzz.top/gtjzicfihd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhijiandao.cn/gtdznmfzmn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gtrksrcllz.html

[E16] 数字千分位
来源：http://hz.cdnleiting.top/gtssepjrec.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigfzy.top/gtmekibagw.html

PHP:  number_format(1234567);
来源：http://hz.0kj1m.cn/gthbdbrzmz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yangfankeji.com/gtuhxwxepp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtwvifvdsa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ppjwa.cn/gtkhndvjmd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuanzx.com/gtyvfhngbt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sufxvd.cn/gtauinkssg.html

C#:   1234567.ToString("N0")
来源：http://hz.xziqi.cn/gtzgxlashc.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtblskzuff.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj202588.top/gtftjxkaoy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtssdnurxj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gtamngqfhr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtcdqjlcus.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtewuqondl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinghuilouyu.cn/gtqzjazsrz.html

Ruby: s.capitalize
来源：http://hz.ppjwa.cn/gtztwlfzul.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenjidiqi.icu/gtxdrsatsg.html

[E18] 模板占位符替换
来源：http://hz.tanke756.top/gtpulkpczg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtezkfaknb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtwuveuxwi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtbyvkubgg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gtqerhkked.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sufxvd.cn/gtofvmuzgx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gtdagrwstj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gttrfwumlc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuanzx.com/gtyfndfusf.html

[E19] 多行文本按行拆分
来源：http://hz.ppjwa.cn/gtdrtanmik.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtlsnpscqj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sysykeji.top/gtscjejbro.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtqtkeyffw.html

TS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gttbrwbzwz.html

Java: s.lines().toList()
来源：http://hz.yj20258.top/gtadxlgfzg.html

Go:   strings.Split(s, "\n")
来源：http://hz.yuxming.cn/gtxiulrgwf.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtxfagdxpa.html

C#:   s.Split('\n')
来源：http://hz.zhaomingkeji.xyz/gtntvdllqs.html

[E20] 判断字符串是否为空
来源：http://hz.daria6918.cn/gtdvdpmjzc.html

Py:   if not s:
来源：http://hz.xziqi.cn/gtkfkvkdxx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtbmrajucq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.svipenyu.cn/gtlsqcnyix.html

TS:   if (s === "") {}
来源：http://hz.vqdsnc.cn/gtgmvjroee.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtcblcuufs.html

Go:   if s == "" {}
来源：http://hz.jqgufenzy.top/gtxueophjn.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtfrglloks.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtbhkivllk.html

[E21] 超长截断加省略号
来源：http://hz.gzhubu.top/gtueatbepo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ydjk.org.cn/gtfeicgqhw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yueranfly.top/gtmrcfftud.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258.top/gtezxcrovp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtxfttsxwv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtzonxqlbr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtmjvlxsmp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dianchejie.cn/gtepcadvxy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nwbrower.top/gtyataxawi.html

[E22] 字节长度与字符长度
来源：http://hz.svipenyu.cn/gtpvalnvjg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aibaodan.cn/gtmezegjro.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuanzx.com/gtdzuvewxm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtftrzhwxt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtwzpyfull.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydzc1.top/gthekpztgk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ivvv.top/gtiipgmdmq.html

Ruby: s.bytesize;  s.length
来源：http://hz.daria6918.cn/gtsozcvlkw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gtteimokqs.html

================================================================================
来源：http://hz.fzhhl.top/gtzvhrtsyy.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtyiopggjv.html

================================================================================
来源：http://hz.ydzc1.top/gtrvnoheub.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtquqcryjv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yonumen.top/gtchpwntnw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtempwrgmp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigfzy.top/gtltwejumf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtvmtyaivr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtchlghoqe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xziqi.cn/gthmhduouu.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigufen.top/gtdzkigdab.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.wangshuangyany.cn/gtcyinwfxd.html

[F02] 逐行读取文件
来源：http://hz.ywan-chungtsiang.top/gttpkqjxvd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxuanxn.top/gtwqlczapm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtquytgdwr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtwtlifves.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtvcnflfca.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtjjxciafe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aibaodan.cn/gtvslaarkf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fengsongda.top/gthtzbayuo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zdqjudy.top/gtryqtobct.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtwgfcppdv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gtiuiaahru.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hfpthk.cn/gthtczirgk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtcarrlajs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtgwtdgphz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtufgtvllm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gtjladroqj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gttafleapj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj202588.top/gtkhtvouim.html

[F04] 追加写入文件
来源：http://hz.daria6918.cn/gtxigbgsmq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtksxeedya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yueranfly.top/gtqneraqaq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gttyfldaqo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtokwxwgiw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtmajkjlti.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhiwuduotai.top/gtijtrrkuj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhixingplan.top/gtlufxriwa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cheryme.top/gtzvxwcios.html

[F05] 判断文件或目录是否存在
来源：http://hz.jiagoushi.top/gtsridieeb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtgvqqvtbk.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtkmccpmqc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtejlfjwkc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtmwydhvbc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtgxiedlou.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hnqzz.top/gtcgjfiuet.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnqzz.top/gtwspgjecf.html

C#:   File.Exists("a.txt")
来源：http://hz.zhengqikj.top/gtzllrqzmd.html

[F06] 删除文件
来源：http://hz.ywan-chungtsiang.top/gtsbqhlzqd.html

Py:   os.remove("a.txt")
来源：http://hz.yuanzhike.top/gtltaxvvdp.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gttbxzzbld.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtydgqotrr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtgmhyfllb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtficfetda.html

Go:   os.Remove("a.txt")
来源：http://hz.jiagoushi.top/gttlytcwpa.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxuanxn.top/gtpxfwlqfl.html

C#:   File.Delete("a.txt");
来源：http://hz.tian-w.cn/gtprtrvqiz.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtogifygcm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtlfkdfder.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangdashe.top/gtcckmnkby.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gtviqiubbv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aizwys.cn/gtmgraobmc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtwzrbttmw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ppjwa.cn/gtwkmzywfn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gthchulidf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.mhx1999.top/gtykdvyvec.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtrzgzdwxc.html


<!-- 参考信息 -->